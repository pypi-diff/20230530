# Comparing `tmp/firestone_lib-0.1.6.tar.gz` & `tmp/firestone_lib-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firestone_lib-0.1.6.tar", max compression
+gzip compressed data, was "firestone_lib-0.1.7.tar", max compression
```

## Comparing `firestone_lib-0.1.6.tar` & `firestone_lib-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/LICENSE
--rw-r--r--   0        0        0      311 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/firestone_lib/__init__.py
--rw-r--r--   0        0        0     4917 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/firestone_lib/cli.py
--rw-r--r--   0        0        0     1419 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/firestone_lib/resource.py
--rw-r--r--   0        0        0        0 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/firestone_lib/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/firestone_lib/resources/logging/__init__.py
--rw-r--r--   0        0        0      396 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/firestone_lib/resources/logging/cli.conf
--rw-r--r--   0        0        0      319 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/firestone_lib/utils.py
--rw-r--r--   0        0        0      970 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 firestone_lib-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/LICENSE
+-rw-r--r--   0        0        0      311 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/firestone_lib/__init__.py
+-rw-r--r--   0        0        0     4736 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/firestone_lib/cli.py
+-rw-r--r--   0        0        0     1419 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/firestone_lib/resource.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/firestone_lib/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/firestone_lib/resources/logging/__init__.py
+-rw-r--r--   0        0        0      396 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/firestone_lib/resources/logging/cli.conf
+-rw-r--r--   0        0        0      319 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/firestone_lib/utils.py
+-rw-r--r--   0        0        0      970 2023-05-30 09:36:17.962184 firestone_lib-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 firestone_lib-0.1.7/PKG-INFO
```

### Comparing `firestone_lib-0.1.6/LICENSE` & `firestone_lib-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `firestone_lib-0.1.6/firestone_lib/cli.py` & `firestone_lib-0.1.7/firestone_lib/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 Common CLI utility functions for firestone and firestone apps.
 """
 import configparser
 import io
 import json
 import logging
 import logging.config
+import os
 import re
 import time
 
 import click
+import jinja2
 import pkg_resources
 import yaml
 
 try:
     from yaml import CLoader as Loader
 except ImportError:
     from yaml import Loader
@@ -62,49 +64,46 @@
 
 
 class FromJsonOrYaml(click.ParamType):
     """Converts a string from the CLI as a parameter to JSON or YAML object."""
 
     name = "String to JSON or YAML object, optionally via a file, using @file.json"
 
-    def __init__(self, decoder=None):
-        self.decoder = decoder or json.JSONDecoder()
-
     def convert(self, value, param, ctx):
         """Convert a string from the CLI as a parameter to JSON object."""
         if value == "-":
             return "-"
         if not isinstance(value, str):
             return value
 
+        raw_str = value
         if value.startswith("@"):
             filename = value[1:]
             _LOGGER.debug(f"Reading data from file {filename}...")
             with io.open(filename, "r", encoding="utf-8") as fh:
-                try:
-                    _LOGGER.debug("Trying json.load")
-                    print("trying json")
-                    return json.load(fh)
-                # pylint: disable=broad-exception-caught
-                except Exception:
-                    pass
-                try:
-                    _LOGGER.debug("Trying yaml.load")
-                    return yaml.load(fh, Loader=Loader)
-                # pylint: disable=broad-exception-caught
-                except Exception:
-                    self.fail(f"{value} is not in JSON or YAML format", param, ctx)
+                raw_str = fh.readlines()
+
+        template = jinja2.Environment(loader=jinja2.BaseLoader()).from_string(raw_str)
+        data = template.render(**os.environ)
 
-        raw_str = rf"{value}"
         try:
-            return self.decoder.decode(raw_str)
-        except json.decoder.JSONDecodeError:
+            _LOGGER.debug("Trying json.load")
+            return json.loads(data)
+        # pylint: disable=broad-exception-caught
+        except Exception:
             pass
 
-        return yaml.load(value, Loader=Loader)
+        try:
+            _LOGGER.debug("Trying yaml.load")
+            return yaml.load(data, Loader=Loader)
+        # pylint: disable=broad-exception-caught
+        except Exception:
+            self.fail(f"{value} is not in JSON or YAML format", param, ctx)
+
+        return data
 
 
 class KeyValue(click.ParamType):
     """A custom click parameter type tha takes key/value items."""
 
     name = "Key and value click type" ""
```

### Comparing `firestone_lib-0.1.6/firestone_lib/resource.py` & `firestone_lib-0.1.7/firestone_lib/resource.py`

 * *Files identical despite different names*

### Comparing `firestone_lib-0.1.6/pyproject.toml` & `firestone_lib-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "firestone-lib"
-version = "0.1.6"
+version = "0.1.7"
 description = "Library to help build OpenAPI, AsyncAPI and gRPC specs based off one or more resource json schema files"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [
     { include = "firestone_lib" }
 ]
```

### Comparing `firestone_lib-0.1.6/PKG-INFO` & `firestone_lib-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firestone-lib
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library to help build OpenAPI, AsyncAPI and gRPC specs based off one or more resource json schema files
 License: Apache 2.0
 Author: Erick Bourgeois
 Author-email: erick@jeb.ca
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

