# Comparing `tmp/firestone_lib-0.1.7.tar.gz` & `tmp/firestone_lib-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firestone_lib-0.1.7.tar", max compression
+gzip compressed data, was "firestone_lib-0.1.8.tar", max compression
```

## Comparing `firestone_lib-0.1.7.tar` & `firestone_lib-0.1.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/LICENSE
--rw-r--r--   0        0        0      311 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/firestone_lib/__init__.py
--rw-r--r--   0        0        0     4736 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/firestone_lib/cli.py
--rw-r--r--   0        0        0     1419 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/firestone_lib/resource.py
--rw-r--r--   0        0        0        0 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/firestone_lib/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/firestone_lib/resources/logging/__init__.py
--rw-r--r--   0        0        0      396 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/firestone_lib/resources/logging/cli.conf
--rw-r--r--   0        0        0      319 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/firestone_lib/utils.py
--rw-r--r--   0        0        0      970 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 firestone_lib-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 10:47:21.709603 firestone_lib-0.1.8/LICENSE
+-rw-r--r--   0        0        0      311 2023-05-30 10:47:21.709603 firestone_lib-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 10:47:21.709603 firestone_lib-0.1.8/firestone_lib/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-30 10:47:21.709603 firestone_lib-0.1.8/firestone_lib/cli.py
+-rw-r--r--   0        0        0     1419 2023-05-30 10:47:21.709603 firestone_lib-0.1.8/firestone_lib/resource.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:47:21.709603 firestone_lib-0.1.8/firestone_lib/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:47:21.709603 firestone_lib-0.1.8/firestone_lib/resources/logging/__init__.py
+-rw-r--r--   0        0        0      396 2023-05-30 10:47:21.709603 firestone_lib-0.1.8/firestone_lib/resources/logging/cli.conf
+-rw-r--r--   0        0        0      319 2023-05-30 10:47:21.709603 firestone_lib-0.1.8/firestone_lib/utils.py
+-rw-r--r--   0        0        0      970 2023-05-30 10:47:21.713603 firestone_lib-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 firestone_lib-0.1.8/PKG-INFO
```

### Comparing `firestone_lib-0.1.7/LICENSE` & `firestone_lib-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `firestone_lib-0.1.7/firestone_lib/cli.py` & `firestone_lib-0.1.8/firestone_lib/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             return value
 
         raw_str = value
         if value.startswith("@"):
             filename = value[1:]
             _LOGGER.debug(f"Reading data from file {filename}...")
             with io.open(filename, "r", encoding="utf-8") as fh:
-                raw_str = fh.readlines()
+                raw_str = fh.read()
 
         template = jinja2.Environment(loader=jinja2.BaseLoader()).from_string(raw_str)
         data = template.render(**os.environ)
 
         try:
             _LOGGER.debug("Trying json.load")
             return json.loads(data)
```

### Comparing `firestone_lib-0.1.7/firestone_lib/resource.py` & `firestone_lib-0.1.8/firestone_lib/resource.py`

 * *Files identical despite different names*

### Comparing `firestone_lib-0.1.7/pyproject.toml` & `firestone_lib-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "firestone-lib"
-version = "0.1.7"
+version = "0.1.8"
 description = "Library to help build OpenAPI, AsyncAPI and gRPC specs based off one or more resource json schema files"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [
     { include = "firestone_lib" }
 ]
```

### Comparing `firestone_lib-0.1.7/PKG-INFO` & `firestone_lib-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firestone-lib
-Version: 0.1.7
+Version: 0.1.8
 Summary: Library to help build OpenAPI, AsyncAPI and gRPC specs based off one or more resource json schema files
 License: Apache 2.0
 Author: Erick Bourgeois
 Author-email: erick@jeb.ca
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

