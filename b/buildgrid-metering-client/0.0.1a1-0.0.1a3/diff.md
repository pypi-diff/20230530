# Comparing `tmp/buildgrid-metering-client-0.0.1a1.tar.gz` & `tmp/buildgrid-metering-client-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildgrid-metering-client-0.0.1a1.tar", last modified: Mon May  1 18:24:25 2023, max compression
+gzip compressed data, was "buildgrid-metering-client-0.0.1a3.tar", last modified: Tue May 30 16:41:05 2023, max compression
```

## Comparing `buildgrid-metering-client-0.0.1a1.tar` & `buildgrid-metering-client-0.0.1a3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 zchen723  (1000) zchen723  (1000)        0 2023-05-01 18:24:25.529417 buildgrid-metering-client-0.0.1a1/
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)    11358 2023-05-01 18:19:54.000000 buildgrid-metering-client-0.0.1a1/LICENSE
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)    15124 2023-05-01 18:24:25.529417 buildgrid-metering-client-0.0.1a1/PKG-INFO
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)     1572 2023-05-01 18:19:54.000000 buildgrid-metering-client-0.0.1a1/README.md
-drwxr-xr-x   0 zchen723  (1000) zchen723  (1000)        0 2023-05-01 18:24:25.529417 buildgrid-metering-client-0.0.1a1/buildgrid_metering/
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)        0 2023-04-27 20:36:28.000000 buildgrid-metering-client-0.0.1a1/buildgrid_metering/__init__.py
-drwxr-xr-x   0 zchen723  (1000) zchen723  (1000)        0 2023-05-01 18:24:25.529417 buildgrid-metering-client-0.0.1a1/buildgrid_metering/client/
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)       79 2023-04-27 20:36:28.000000 buildgrid-metering-client-0.0.1a1/buildgrid_metering/client/__init__.py
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)     2369 2023-04-27 20:36:28.000000 buildgrid-metering-client-0.0.1a1/buildgrid_metering/client/auth.py
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)     4889 2023-04-27 20:36:28.000000 buildgrid-metering-client-0.0.1a1/buildgrid_metering/client/client.py
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)     1253 2023-04-27 20:36:28.000000 buildgrid-metering-client-0.0.1a1/buildgrid_metering/client/exceptions.py
-drwxr-xr-x   0 zchen723  (1000) zchen723  (1000)        0 2023-05-01 18:24:25.529417 buildgrid-metering-client-0.0.1a1/buildgrid_metering/models/
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)        0 2023-04-27 20:36:28.000000 buildgrid-metering-client-0.0.1a1/buildgrid_metering/models/__init__.py
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)     1639 2023-04-27 20:36:28.000000 buildgrid-metering-client-0.0.1a1/buildgrid_metering/models/api.py
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)     3621 2023-04-27 20:36:28.000000 buildgrid-metering-client-0.0.1a1/buildgrid_metering/models/dataclasses.py
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)        0 2023-04-27 20:36:28.000000 buildgrid-metering-client-0.0.1a1/buildgrid_metering/py.typed
-drwxr-xr-x   0 zchen723  (1000) zchen723  (1000)        0 2023-05-01 18:24:25.529417 buildgrid-metering-client-0.0.1a1/buildgrid_metering_client.egg-info/
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)    15124 2023-05-01 18:24:25.000000 buildgrid-metering-client-0.0.1a1/buildgrid_metering_client.egg-info/PKG-INFO
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)      635 2023-05-01 18:24:25.000000 buildgrid-metering-client-0.0.1a1/buildgrid_metering_client.egg-info/SOURCES.txt
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)        1 2023-05-01 18:24:25.000000 buildgrid-metering-client-0.0.1a1/buildgrid_metering_client.egg-info/dependency_links.txt
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)      143 2023-05-01 18:24:25.000000 buildgrid-metering-client-0.0.1a1/buildgrid_metering_client.egg-info/requires.txt
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)       19 2023-05-01 18:24:25.000000 buildgrid-metering-client-0.0.1a1/buildgrid_metering_client.egg-info/top_level.txt
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)     1573 2023-04-27 20:36:28.000000 buildgrid-metering-client-0.0.1a1/pyproject.toml
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)       38 2023-05-01 18:24:25.529417 buildgrid-metering-client-0.0.1a1/setup.cfg
-drwxr-xr-x   0 zchen723  (1000) zchen723  (1000)        0 2023-05-01 18:24:25.529417 buildgrid-metering-client-0.0.1a1/tests/
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)     2284 2023-04-27 20:36:28.000000 buildgrid-metering-client-0.0.1a1/tests/test_auth.py
--rw-r--r--   0 zchen723  (1000) zchen723  (1000)     4019 2023-04-27 20:36:28.000000 buildgrid-metering-client-0.0.1a1/tests/test_client.py
+drwxr-xr-x   0 zchen723  (1000) zchen723  (1000)        0 2023-05-30 16:41:05.502536 buildgrid-metering-client-0.0.1a3/
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)    11358 2023-05-01 18:19:54.000000 buildgrid-metering-client-0.0.1a3/LICENSE
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)    15124 2023-05-30 16:41:05.502536 buildgrid-metering-client-0.0.1a3/PKG-INFO
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)     1572 2023-05-01 18:19:54.000000 buildgrid-metering-client-0.0.1a3/README.md
+drwxr-xr-x   0 zchen723  (1000) zchen723  (1000)        0 2023-05-30 16:41:05.492536 buildgrid-metering-client-0.0.1a3/buildgrid_metering/
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)        0 2023-04-27 20:36:28.000000 buildgrid-metering-client-0.0.1a3/buildgrid_metering/__init__.py
+drwxr-xr-x   0 zchen723  (1000) zchen723  (1000)        0 2023-05-30 16:41:05.492536 buildgrid-metering-client-0.0.1a3/buildgrid_metering/client/
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)      269 2023-05-30 15:06:53.000000 buildgrid-metering-client-0.0.1a3/buildgrid_metering/client/__init__.py
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)     2369 2023-05-30 16:36:33.000000 buildgrid-metering-client-0.0.1a3/buildgrid_metering/client/auth.py
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)     6233 2023-05-30 16:36:33.000000 buildgrid-metering-client-0.0.1a3/buildgrid_metering/client/client.py
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)     1253 2023-04-27 20:36:28.000000 buildgrid-metering-client-0.0.1a3/buildgrid_metering/client/exceptions.py
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)     1446 2023-05-30 15:06:53.000000 buildgrid-metering-client-0.0.1a3/buildgrid_metering/client/retry.py
+drwxr-xr-x   0 zchen723  (1000) zchen723  (1000)        0 2023-05-30 16:41:05.492536 buildgrid-metering-client-0.0.1a3/buildgrid_metering/models/
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)        0 2023-04-27 20:36:28.000000 buildgrid-metering-client-0.0.1a3/buildgrid_metering/models/__init__.py
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)     1639 2023-05-30 16:36:33.000000 buildgrid-metering-client-0.0.1a3/buildgrid_metering/models/api.py
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)     3621 2023-05-30 16:36:33.000000 buildgrid-metering-client-0.0.1a3/buildgrid_metering/models/dataclasses.py
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)        0 2023-04-27 20:36:28.000000 buildgrid-metering-client-0.0.1a3/buildgrid_metering/py.typed
+drwxr-xr-x   0 zchen723  (1000) zchen723  (1000)        0 2023-05-30 16:41:05.502536 buildgrid-metering-client-0.0.1a3/buildgrid_metering_client.egg-info/
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)    15124 2023-05-30 16:41:05.000000 buildgrid-metering-client-0.0.1a3/buildgrid_metering_client.egg-info/PKG-INFO
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)      670 2023-05-30 16:41:05.000000 buildgrid-metering-client-0.0.1a3/buildgrid_metering_client.egg-info/SOURCES.txt
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)        1 2023-05-30 16:41:05.000000 buildgrid-metering-client-0.0.1a3/buildgrid_metering_client.egg-info/dependency_links.txt
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)      157 2023-05-30 16:41:05.000000 buildgrid-metering-client-0.0.1a3/buildgrid_metering_client.egg-info/requires.txt
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)       19 2023-05-30 16:41:05.000000 buildgrid-metering-client-0.0.1a3/buildgrid_metering_client.egg-info/top_level.txt
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)     1723 2023-05-30 16:36:33.000000 buildgrid-metering-client-0.0.1a3/pyproject.toml
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)       38 2023-05-30 16:41:05.502536 buildgrid-metering-client-0.0.1a3/setup.cfg
+drwxr-xr-x   0 zchen723  (1000) zchen723  (1000)        0 2023-05-30 16:41:05.502536 buildgrid-metering-client-0.0.1a3/tests/
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)     2284 2023-05-30 16:36:33.000000 buildgrid-metering-client-0.0.1a3/tests/test_auth.py
+-rw-r--r--   0 zchen723  (1000) zchen723  (1000)     6920 2023-05-30 16:36:33.000000 buildgrid-metering-client-0.0.1a3/tests/test_client.py
```

### Comparing `buildgrid-metering-client-0.0.1a1/LICENSE` & `buildgrid-metering-client-0.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `buildgrid-metering-client-0.0.1a1/PKG-INFO` & `buildgrid-metering-client-0.0.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildgrid-metering-client
-Version: 0.0.1a1
+Version: 0.0.1a3
 Summary: Client library of buildgrid-metering service
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `buildgrid-metering-client-0.0.1a1/README.md` & `buildgrid-metering-client-0.0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `buildgrid-metering-client-0.0.1a1/buildgrid_metering/client/auth.py` & `buildgrid-metering-client-0.0.1a3/buildgrid_metering/client/auth.py`

 * *Files identical despite different names*

### Comparing `buildgrid-metering-client-0.0.1a1/buildgrid_metering/client/exceptions.py` & `buildgrid-metering-client-0.0.1a3/buildgrid_metering/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildgrid-metering-client-0.0.1a1/buildgrid_metering/models/api.py` & `buildgrid-metering-client-0.0.1a3/buildgrid_metering/models/api.py`

 * *Files identical despite different names*

### Comparing `buildgrid-metering-client-0.0.1a1/buildgrid_metering/models/dataclasses.py` & `buildgrid-metering-client-0.0.1a3/buildgrid_metering/models/dataclasses.py`

 * *Files identical despite different names*

### Comparing `buildgrid-metering-client-0.0.1a1/buildgrid_metering_client.egg-info/PKG-INFO` & `buildgrid-metering-client-0.0.1a3/buildgrid_metering_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildgrid-metering-client
-Version: 0.0.1a1
+Version: 0.0.1a3
 Summary: Client library of buildgrid-metering service
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `buildgrid-metering-client-0.0.1a1/buildgrid_metering_client.egg-info/SOURCES.txt` & `buildgrid-metering-client-0.0.1a3/buildgrid_metering_client.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 buildgrid_metering/__init__.py
 buildgrid_metering/py.typed
 buildgrid_metering/client/__init__.py
 buildgrid_metering/client/auth.py
 buildgrid_metering/client/client.py
 buildgrid_metering/client/exceptions.py
+buildgrid_metering/client/retry.py
 buildgrid_metering/models/__init__.py
 buildgrid_metering/models/api.py
 buildgrid_metering/models/dataclasses.py
 buildgrid_metering_client.egg-info/PKG-INFO
 buildgrid_metering_client.egg-info/SOURCES.txt
 buildgrid_metering_client.egg-info/dependency_links.txt
 buildgrid_metering_client.egg-info/requires.txt
```

### Comparing `buildgrid-metering-client-0.0.1a1/pyproject.toml` & `buildgrid-metering-client-0.0.1a3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "buildgrid-metering-client"
-version = "0.0.1-alpha.1"
+version = "0.0.1-alpha.3"
 requires-python = ">=3.8"
 description = "Client library of buildgrid-metering service"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["buildgrid"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License"
 ]
 dependencies = [
     "pydantic >= 1.10",
     "aiohttp >= 3.8",
     "aiofiles >= 23.1",
-    "async_lru >= 2.0"
+    "async_lru >= 2.0",
+    "tenacity >= 8.2"
 ]
 
 [project.optional-dependencies]
 dev = [
     # Testing
     "pytest",
     "pytest-cov",
@@ -46,15 +47,21 @@
 include = ["buildgrid_metering*"]
 
 [tool.setuptools.package-data]
 "*" = ["py.typed"]
 
 [tool.mypy]
 strict = true
-ignore_missing_imports = true
+plugins = ["pydantic.mypy"]
+
+[tool.pydantic-mypy]
+init_forbid_extra = true
+init_typed = true
+warn_required_dynamic_aliases = true
+warn_untyped_fields = true
 
 [tool.pylint.basic]
 good-names = '''e'''
 
 [tool.pylint.messages_control]
 extension-pkg-whitelist = "pydantic"
 disable = [
```

### Comparing `buildgrid-metering-client-0.0.1a1/tests/test_auth.py` & `buildgrid-metering-client-0.0.1a3/tests/test_auth.py`

 * *Files identical despite different names*

