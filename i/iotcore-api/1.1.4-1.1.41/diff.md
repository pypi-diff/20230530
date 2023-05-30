# Comparing `tmp/iotcore_api-1.1.4.tar.gz` & `tmp/iotcore_api-1.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iotcore_api-1.1.4.tar", max compression
+gzip compressed data, was "iotcore_api-1.1.41.tar", max compression
```

## Comparing `iotcore_api-1.1.4.tar` & `iotcore_api-1.1.41.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      483 2023-03-15 03:19:14.000000 iotcore_api-1.1.4/iotcoreapi/__init__.py
--rw-r--r--   0        0        0      963 2023-03-13 08:36:48.000000 iotcore_api-1.1.4/iotcoreapi/exceptions.py
--rw-r--r--   0        0        0    56452 2023-05-30 15:26:21.704664 iotcore_api-1.1.4/iotcoreapi/iotcoreapi.py
--rw-r--r--   0        0        0     1734 2023-05-16 07:36:12.815682 iotcore_api-1.1.4/iotcoreapi/nan_treatment.py
--rw-r--r--   0        0        0      967 2023-05-30 15:40:52.758521 iotcore_api-1.1.4/pyproject.toml
--rw-r--r--   0        0        0    34548 2023-05-30 15:40:36.063059 iotcore_api-1.1.4/README.md
--rw-r--r--   0        0        0    34183 1970-01-01 00:00:00.000000 iotcore_api-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      483 2023-03-15 03:19:14.000000 iotcore_api-1.1.41/iotcoreapi/__init__.py
+-rw-r--r--   0        0        0      963 2023-03-13 08:36:48.000000 iotcore_api-1.1.41/iotcoreapi/exceptions.py
+-rw-r--r--   0        0        0    56452 2023-05-30 15:26:21.704664 iotcore_api-1.1.41/iotcoreapi/iotcoreapi.py
+-rw-r--r--   0        0        0     1734 2023-05-16 07:36:12.815682 iotcore_api-1.1.41/iotcoreapi/nan_treatment.py
+-rw-r--r--   0        0        0      744 2023-05-30 15:42:45.508297 iotcore_api-1.1.41/pyproject.toml
+-rw-r--r--   0        0        0    34548 2023-05-30 15:40:36.063059 iotcore_api-1.1.41/README.md
+-rw-r--r--   0        0        0    34051 1970-01-01 00:00:00.000000 iotcore_api-1.1.41/PKG-INFO
```

### Comparing `iotcore_api-1.1.4/iotcoreapi/exceptions.py` & `iotcore_api-1.1.41/iotcoreapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `iotcore_api-1.1.4/iotcoreapi/iotcoreapi.py` & `iotcore_api-1.1.41/iotcoreapi/iotcoreapi.py`

 * *Files identical despite different names*

### Comparing `iotcore_api-1.1.4/iotcoreapi/nan_treatment.py` & `iotcore_api-1.1.41/iotcoreapi/nan_treatment.py`

 * *Files identical despite different names*

### Comparing `iotcore_api-1.1.4/pyproject.toml` & `iotcore_api-1.1.41/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,16 @@
 [tool.poetry]
 name = "iotcore-api"
-version = "1.1.4"
+version = "1.1.41"
 description ="IoT core connection methods and utilities"
 readme = "README.md"
 packages = [
     {include = 'iotcoreapi/*.py'}
 ]
-authors = [
-    "Ricardo Gomez <ricardo.gomez.aldaravi@idrica.com>",
-    "Laura Moreno <laura.moreno@idrica.com>"
-]
-
-maintainers = [
-    "Ricardo Gomez <ricardo.gomez.aldaravi@idrica.com>",
-    "Laura Moreno <laura.moreno@idrica.com>"
-]
+authors = ["Idrica"]
 keywords = ["iotcoreapi", "goaigua"]
 
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = "^2.0.1"
```

### Comparing `iotcore_api-1.1.4/README.md` & `iotcore_api-1.1.41/README.md`

 * *Files identical despite different names*

### Comparing `iotcore_api-1.1.4/PKG-INFO` & `iotcore_api-1.1.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: iotcore-api
-Version: 1.1.4
+Version: 1.1.41
 Summary: IoT core connection methods and utilities
 Keywords: iotcoreapi,goaigua
-Author: Ricardo Gomez
-Author-email: ricardo.gomez.aldaravi@idrica.com
-Maintainer: Ricardo Gomez
-Maintainer-email: ricardo.gomez.aldaravi@idrica.com
+Author: Idrica
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
```

