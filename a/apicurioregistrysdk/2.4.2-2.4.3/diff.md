# Comparing `tmp/apicurioregistrysdk-2.4.2.tar.gz` & `tmp/apicurioregistrysdk-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apicurioregistrysdk-2.4.2.tar", max compression
+gzip compressed data, was "apicurioregistrysdk-2.4.3.tar", max compression
```

## Comparing `apicurioregistrysdk-2.4.2.tar` & `apicurioregistrysdk-2.4.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      368 2023-05-16 11:09:16.401927 apicurioregistrysdk-2.4.2/README.md
--rw-r--r--   0        0        0     2207 2023-05-16 11:09:16.402810 apicurioregistrysdk-2.4.2/kiota-gen.py
--rw-r--r--   0        0        0     1024 2023-05-16 11:36:02.634387 apicurioregistrysdk-2.4.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 11:09:16.404377 apicurioregistrysdk-2.4.2/python_sdk/__init__.py
--rw-r--r--   0        0        0     1150 1970-01-01 00:00:00.000000 apicurioregistrysdk-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0      368 2023-05-30 19:31:39.754700 apicurioregistrysdk-2.4.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 19:31:39.754700 apicurioregistrysdk-2.4.3/apicurioregistrysdk/__init__.py
+-rw-r--r--   0        0        0     2604 2023-05-30 19:31:39.754700 apicurioregistrysdk-2.4.3/kiota-gen.py
+-rw-r--r--   0        0        0     1281 2023-05-30 19:31:57.327038 apicurioregistrysdk-2.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1250 1970-01-01 00:00:00.000000 apicurioregistrysdk-2.4.3/PKG-INFO
```

### Comparing `apicurioregistrysdk-2.4.2/kiota-gen.py` & `apicurioregistrysdk-2.4.3/kiota-gen.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import requests
 import zipfile
 import io
 import os
-import shutil
 import stat
 import sys
+import shutil
 import platform
+from pathlib import Path
 
 KIOTA_VERSION = "1.1.3"
 
 KIOTA_OS_NAMES = {"Windows": "win", "Darwin": "osx", "Linux": "linux"}
 KIOTA_ARCH_NAMES = {"32bit": "x86", "64bit": "x64"}
 
 
@@ -43,28 +44,38 @@
             f"Using kiota already available on path if something goes wrong, please clean the local 'kiota_tmp' folder."
         )
 
     kiota_bin = os.path.join(tmpdir, "kiota")
     st = os.stat(kiota_bin)
     os.chmod(kiota_bin, st.st_mode | stat.S_IEXEC)
 
-    openapi_doc = os.path.join(
-        sys.path[0],
-        "..",
-        "common",
-        "src",
-        "main",
-        "resources",
-        "META-INF",
-        "openapi.json",
-    )
-    output = os.path.join(sys.path[0], "python_sdk", "client")
+    openapi_doc = Path(__file__).parent.joinpath("openapi.json")
+    if not os.path.exists(openapi_doc):
+        shutil.copyfile(
+            os.path.join(
+                sys.path[0],
+                "..",
+                "common",
+                "src",
+                "main",
+                "resources",
+                "META-INF",
+                "openapi.json",
+            ),
+            openapi_doc,
+        )
+
+    output = Path(__file__).parent.joinpath("apicurioregistrysdk", "client")
+
     command = f'{kiota_bin} generate --language=python --openapi="{openapi_doc}" --output="{output}" --class-name=RegistryClient --namespace-name=client --clean-output --clear-cache'
     print(f"Executing kiota command: {command}")
 
     os.system(command)
     print("Kiota client generation has been successful")
     return setup_kwargs
 
 
 if __name__ == "__main__":
-    generate_kiota_client_files({})
+    if not os.path.exists(
+        os.path.join(sys.path[0], "apicurioregistrysdk", "client", "kiota-lock.json")
+    ):
+        generate_kiota_client_files({})
```

### Comparing `apicurioregistrysdk-2.4.2/pyproject.toml` & `apicurioregistrysdk-2.4.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 [tool.poetry]
 name = "apicurioregistrysdk"
-version = "2.4.2"
+version = "2.4.3"
 description = ""
 authors = ["Andrea Peruffo <andrea.peruffo1982@gmail.com>"]
 readme = "README.md"
-packages = [{include = "python_sdk"}]
+packages = [{include = "apicurioregistrysdk"}]
+include = [
+    { path = "openapi.json", format=["sdist", "wheel"] },
+    { path = "apicurioregistrysdk/client/**/*", format=["sdist", "wheel"] },
+]
+exclude = [
+    { path = "apicurioregistrysdk/__pycache__", format=["sdist", "wheel"] },
+]
 license = "Apache 2.0"
 homepage = "https://github.com/apicurio/apicurio-registry"
 repository = "https://github.com/apicurio/apicurio-registry"
 keywords = ["apicurio", "registry"]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.9"
 microsoft-kiota-abstractions = "^0.5.1"
 microsoft-kiota-http = "^0.4.1"
 microsoft-kiota-serialization-json = "^0.3.2"
 microsoft-kiota-serialization-text = "^0.2.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
-requests = "2.29.0"
+requests = "2.31.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core", "requests", "shutils"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.build]
 generate-setup-file = false
 script = "kiota-gen.py"
 
 [tool.pytest.ini_options]
-pythonpath = [ "python_sdk" ]
+pythonpath = [ "apicurioregistrysdk" ]
 
 [tool.black]
 extend-exclude = 'client'
```

### Comparing `apicurioregistrysdk-2.4.2/PKG-INFO` & `apicurioregistrysdk-2.4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: apicurioregistrysdk
-Version: 2.4.2
+Version: 2.4.3
 Summary: 
 Home-page: https://github.com/apicurio/apicurio-registry
 License: Apache 2.0
 Keywords: apicurio,registry
 Author: Andrea Peruffo
 Author-email: andrea.peruffo1982@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: microsoft-kiota-abstractions (>=0.5.1,<0.6.0)
 Requires-Dist: microsoft-kiota-http (>=0.4.1,<0.5.0)
 Requires-Dist: microsoft-kiota-serialization-json (>=0.3.2,<0.4.0)
 Requires-Dist: microsoft-kiota-serialization-text (>=0.2.0,<0.3.0)
 Project-URL: Repository, https://github.com/apicurio/apicurio-registry
 Description-Content-Type: text/markdown
```

