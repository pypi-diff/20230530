# Comparing `tmp/servir-0.0.6.tar.gz` & `tmp/servir-0.1.0.tar.gz`

## Comparing `servir-0.0.6.tar` & `servir-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 servir-0.0.6/.github/workflows/ci.yml
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 servir-0.0.6/.github/workflows/release.yml
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 servir-0.0.6/src/servir/__init__.py
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 servir-0.0.6/src/servir/_background_server.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 servir-0.0.6/src/servir/_protocols.py
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 servir-0.0.6/src/servir/_provide.py
--rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 servir-0.0.6/src/servir/_resources.py
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 servir-0.0.6/src/servir/_tilesets.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 servir-0.0.6/src/servir/_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 servir-0.0.6/src/servir/py.typed
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 servir-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 servir-0.0.6/tests/test_provider.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 servir-0.0.6/tests/test_servir.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 servir-0.0.6/tests/test_tilesets.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 servir-0.0.6/tests/test_util.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 servir-0.0.6/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 servir-0.0.6/LICENSE
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 servir-0.0.6/README.md
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 servir-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 servir-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 servir-0.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 servir-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 servir-0.1.0/src/servir/__init__.py
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 servir-0.1.0/src/servir/_background_server.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 servir-0.1.0/src/servir/_protocols.py
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 servir-0.1.0/src/servir/_provide.py
+-rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 servir-0.1.0/src/servir/_resources.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 servir-0.1.0/src/servir/_tilesets.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 servir-0.1.0/src/servir/_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 servir-0.1.0/src/servir/py.typed
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 servir-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 servir-0.1.0/tests/test_provider.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 servir-0.1.0/tests/test_servir.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 servir-0.1.0/tests/test_tilesets.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 servir-0.1.0/tests/test_util.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 servir-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 servir-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 servir-0.1.0/README.md
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 servir-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 servir-0.1.0/PKG-INFO
```

### Comparing `servir-0.0.6/.github/workflows/ci.yml` & `servir-0.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `servir-0.0.6/src/servir/_background_server.py` & `servir-0.1.0/src/servir/_background_server.py`

 * *Files identical despite different names*

### Comparing `servir-0.0.6/src/servir/_protocols.py` & `servir-0.1.0/src/servir/_protocols.py`

 * *Files identical despite different names*

### Comparing `servir-0.0.6/src/servir/_provide.py` & `servir-0.1.0/src/servir/_provide.py`

 * *Files identical despite different names*

### Comparing `servir-0.0.6/src/servir/_resources.py` & `servir-0.1.0/src/servir/_resources.py`

 * *Files identical despite different names*

### Comparing `servir-0.0.6/src/servir/_tilesets.py` & `servir-0.1.0/src/servir/_tilesets.py`

 * *Files identical despite different names*

### Comparing `servir-0.0.6/src/servir/_util.py` & `servir-0.1.0/src/servir/_util.py`

 * *Files identical despite different names*

### Comparing `servir-0.0.6/tests/test_provider.py` & `servir-0.1.0/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `servir-0.0.6/tests/test_util.py` & `servir-0.1.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `servir-0.0.6/LICENSE` & `servir-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `servir-0.0.6/README.md` & `servir-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # servir
 
 [![PyPI - Version](https://img.shields.io/pypi/v/servir.svg)](https://pypi.org/project/servir)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/servir.svg)](https://pypi.org/project/servir)
 
 an extensible async background server for python
 
------
+---
 
 **table of contents**
 
 - [installation](#installation)
 - [usage](#usage)
 - [license](#license)
 
@@ -35,39 +35,40 @@
 
 path = pathlib.Path("hello.txt")
 path.write_text("hello, world")
 
 file_resource = provider.create(path)
 response = requests.get(file_resource.url)
 assert response.text == "hello, world"
-assert "text/plain" in response.headers["Content-Type"] 
+assert "text/plain" in response.headers["Content-Type"]
 
 ### Directory (supports range requests)
 
 root = pathlib.Path("data_dir")
 root.mkdir()
 (root / "hello.txt").write_text("hello, world")
 
 dir_resource = provider.create(root)
 response = requests.get(file_resource.url + "/hello.txt")
 assert response.text == "hello, world"
 assert "text/plain" in response.headers["Content-Type"]
 
 
-### In-memory
+### In-Memory
 
 data = "a,b,c,\n1,2,3,\n4,5,6"
 
 content_resource = provider.create(data, extension=".csv")
 response = requests.get(content_resource.url)
 assert response.text == data
 assert "text/csv" in response.headers["Content-Type"]
 ```
 
 > **Note**: the `Provider` holds a _weak reference_ to each resource it creates.
 > This allows the provider to cleanup unused resources and prevent memory leaks.
-> As an end user, you must hold a **strong** reference each resource returned
-> by the provider so long as you'd like that endpoint to remain avaiable.
+> As an end user, you must hold a **strong** reference each resource returned by
+> the provider so long as you'd like that endpoint to remain avaiable.
 
 ## license
 
-`servir` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`servir` is distributed under the terms of the
+[MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `servir-0.0.6/pyproject.toml` & `servir-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `servir-0.0.6/PKG-INFO` & `servir-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servir
-Version: 0.0.6
+Version: 0.1.0
 Summary: an extensible async background server
 Project-URL: Documentation, https://github.com/unknown/servir#readme
 Project-URL: Issues, https://github.com/unknown/servir/issues
 Project-URL: Source, https://github.com/unknown/servir
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
@@ -26,15 +26,15 @@
 # servir
 
 [![PyPI - Version](https://img.shields.io/pypi/v/servir.svg)](https://pypi.org/project/servir)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/servir.svg)](https://pypi.org/project/servir)
 
 an extensible async background server for python
 
------
+---
 
 **table of contents**
 
 - [installation](#installation)
 - [usage](#usage)
 - [license](#license)
 
@@ -60,39 +60,40 @@
 
 path = pathlib.Path("hello.txt")
 path.write_text("hello, world")
 
 file_resource = provider.create(path)
 response = requests.get(file_resource.url)
 assert response.text == "hello, world"
-assert "text/plain" in response.headers["Content-Type"] 
+assert "text/plain" in response.headers["Content-Type"]
 
 ### Directory (supports range requests)
 
 root = pathlib.Path("data_dir")
 root.mkdir()
 (root / "hello.txt").write_text("hello, world")
 
 dir_resource = provider.create(root)
 response = requests.get(file_resource.url + "/hello.txt")
 assert response.text == "hello, world"
 assert "text/plain" in response.headers["Content-Type"]
 
 
-### In-memory
+### In-Memory
 
 data = "a,b,c,\n1,2,3,\n4,5,6"
 
 content_resource = provider.create(data, extension=".csv")
 response = requests.get(content_resource.url)
 assert response.text == data
 assert "text/csv" in response.headers["Content-Type"]
 ```
 
 > **Note**: the `Provider` holds a _weak reference_ to each resource it creates.
 > This allows the provider to cleanup unused resources and prevent memory leaks.
-> As an end user, you must hold a **strong** reference each resource returned
-> by the provider so long as you'd like that endpoint to remain avaiable.
+> As an end user, you must hold a **strong** reference each resource returned by
+> the provider so long as you'd like that endpoint to remain avaiable.
 
 ## license
 
-`servir` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`servir` is distributed under the terms of the
+[MIT](https://spdx.org/licenses/MIT.html) license.
```

