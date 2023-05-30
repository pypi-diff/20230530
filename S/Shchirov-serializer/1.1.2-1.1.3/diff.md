# Comparing `tmp/Shchirov_serializer-1.1.2.tar.gz` & `tmp/Shchirov_serializer-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shchirov_serializer-1.1.2.tar", last modified: Tue May 30 20:58:59 2023, max compression
+gzip compressed data, was "Shchirov_serializer-1.1.3.tar", last modified: Tue May 30 21:04:28 2023, max compression
```

## Comparing `Shchirov_serializer-1.1.2.tar` & `Shchirov_serializer-1.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 20:58:59.005830 Shchirov_serializer-1.1.2/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      320 2023-05-30 20:58:59.005830 Shchirov_serializer-1.1.2/PKG-INFO
--rw-r--r--   0 pavel     (1000) pavel     (1000)       66 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.2/README.md
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 20:58:59.001831 Shchirov_serializer-1.1.2/Shchirov_serializer.egg-info/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      320 2023-05-30 20:58:58.000000 Shchirov_serializer-1.1.2/Shchirov_serializer.egg-info/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      651 2023-05-30 20:58:58.000000 Shchirov_serializer-1.1.2/Shchirov_serializer.egg-info/SOURCES.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-05-30 20:58:58.000000 Shchirov_serializer-1.1.2/Shchirov_serializer.egg-info/dependency_links.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       84 2023-05-30 20:58:58.000000 Shchirov_serializer-1.1.2/Shchirov_serializer.egg-info/top_level.txt
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 20:58:59.001831 Shchirov_serializer-1.1.2/serializers/
--rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.2/serializers/__init__.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 20:58:59.001831 Shchirov_serializer-1.1.2/serializers/base/
--rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.2/serializers/base/__init__.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     2780 2023-05-30 17:50:06.000000 Shchirov_serializer-1.1.2/serializers/base/constants.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     5479 2023-05-30 19:38:26.000000 Shchirov_serializer-1.1.2/serializers/base/deserialization.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     5488 2023-05-30 20:58:37.000000 Shchirov_serializer-1.1.2/serializers/base/serialization.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)      455 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.2/serializers/factory.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 20:58:59.001831 Shchirov_serializer-1.1.2/serializers/json_serializer/
--rw-r--r--   0 pavel     (1000) pavel     (1000)     3433 2023-05-30 20:58:23.000000 Shchirov_serializer-1.1.2/serializers/json_serializer/JsonSerializer.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.2/serializers/json_serializer/__init__.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     1313 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.2/serializers/json_serializer/serialization_logic.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 20:58:59.005830 Shchirov_serializer-1.1.2/serializers/xml_serializer/
--rw-r--r--   0 pavel     (1000) pavel     (1000)     3748 2023-05-30 19:42:12.000000 Shchirov_serializer-1.1.2/serializers/xml_serializer/XmlSerializer.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.2/serializers/xml_serializer/__init__.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     1430 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.2/serializers/xml_serializer/serialization_logic.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       38 2023-05-30 20:58:59.005830 Shchirov_serializer-1.1.2/setup.cfg
--rw-r--r--   0 pavel     (1000) pavel     (1000)      549 2023-05-30 20:58:51.000000 Shchirov_serializer-1.1.2/setup.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 20:58:59.005830 Shchirov_serializer-1.1.2/tests/
--rw-r--r--   0 pavel     (1000) pavel     (1000)     7933 2023-05-30 19:59:33.000000 Shchirov_serializer-1.1.2/tests/tests.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:04:28.024458 Shchirov_serializer-1.1.3/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      320 2023-05-30 21:04:28.024458 Shchirov_serializer-1.1.3/PKG-INFO
+-rw-r--r--   0 pavel     (1000) pavel     (1000)       66 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.3/README.md
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:04:28.020458 Shchirov_serializer-1.1.3/Shchirov_serializer.egg-info/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      320 2023-05-30 21:04:27.000000 Shchirov_serializer-1.1.3/Shchirov_serializer.egg-info/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      651 2023-05-30 21:04:28.000000 Shchirov_serializer-1.1.3/Shchirov_serializer.egg-info/SOURCES.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-05-30 21:04:27.000000 Shchirov_serializer-1.1.3/Shchirov_serializer.egg-info/dependency_links.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       84 2023-05-30 21:04:27.000000 Shchirov_serializer-1.1.3/Shchirov_serializer.egg-info/top_level.txt
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:04:28.020458 Shchirov_serializer-1.1.3/serializers/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.3/serializers/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:04:28.024458 Shchirov_serializer-1.1.3/serializers/base/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.3/serializers/base/__init__.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     2780 2023-05-30 17:50:06.000000 Shchirov_serializer-1.1.3/serializers/base/constants.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     5479 2023-05-30 19:38:26.000000 Shchirov_serializer-1.1.3/serializers/base/deserialization.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     5488 2023-05-30 20:58:37.000000 Shchirov_serializer-1.1.3/serializers/base/serialization.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)      455 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.3/serializers/factory.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:04:28.024458 Shchirov_serializer-1.1.3/serializers/json_serializer/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     3409 2023-05-30 21:04:20.000000 Shchirov_serializer-1.1.3/serializers/json_serializer/JsonSerializer.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.3/serializers/json_serializer/__init__.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     1313 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.3/serializers/json_serializer/serialization_logic.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:04:28.024458 Shchirov_serializer-1.1.3/serializers/xml_serializer/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     3748 2023-05-30 19:42:12.000000 Shchirov_serializer-1.1.3/serializers/xml_serializer/XmlSerializer.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.3/serializers/xml_serializer/__init__.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     1430 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.3/serializers/xml_serializer/serialization_logic.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       38 2023-05-30 21:04:28.024458 Shchirov_serializer-1.1.3/setup.cfg
+-rw-r--r--   0 pavel     (1000) pavel     (1000)      549 2023-05-30 21:04:25.000000 Shchirov_serializer-1.1.3/setup.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:04:28.024458 Shchirov_serializer-1.1.3/tests/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     7933 2023-05-30 19:59:33.000000 Shchirov_serializer-1.1.3/tests/tests.py
```

### Comparing `Shchirov_serializer-1.1.2/Shchirov_serializer.egg-info/SOURCES.txt` & `Shchirov_serializer-1.1.3/Shchirov_serializer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.2/serializers/base/constants.py` & `Shchirov_serializer-1.1.3/serializers/base/constants.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.2/serializers/base/deserialization.py` & `Shchirov_serializer-1.1.3/serializers/base/deserialization.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.2/serializers/base/serialization.py` & `Shchirov_serializer-1.1.3/serializers/base/serialization.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.2/serializers/json_serializer/JsonSerializer.py` & `Shchirov_serializer-1.1.3/serializers/json_serializer/JsonSerializer.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # from .serialization_logic import deserialize_json
 
 from typing import Any
 from serializers.base.deserialization import Deserializer
 from serializers.base.serialization import Serializer
 from ..base.constants import (PRIMITIVES,
                          JsonRegularExpression as Expression)
-import regex
+import re
 
 
 class _JsonSerializer:
     def dumps(self, obj: Any) -> str:
         """
         Convert an object to string of 'JSON' format.
 
@@ -75,33 +75,33 @@
 
         :return: Dictionary that represents object.
         :rtype: dict
         """
 
         string = string.strip()
 
-        if regex.fullmatch(Expression.INT.value, string):
+        if re.fullmatch(Expression.INT.value, string):
             return int(string)
 
-        if regex.fullmatch(Expression.STR.value, string):
+        if re.fullmatch(Expression.STR.value, string):
             string = string.replace("\\\\", "\\").replace(r"\"", '"').replace(r"\'", "'")
             return string[1:-1]
 
-        if regex.fullmatch(Expression.FLOAT.value, string):
+        if re.fullmatch(Expression.FLOAT.value, string):
             return float(string)
 
-        if regex.fullmatch(Expression.BOOL.value, string):
+        if re.fullmatch(Expression.BOOL.value, string):
             return True if string == 'True' else False
 
-        if regex.fullmatch(Expression.NONE.value, string):
+        if re.fullmatch(Expression.NONE.value, string):
             return None
 
         if string.startswith("[") and string.endswith("]"):
             string = string[1:-1]
-            matches = regex.findall(Expression.ANY_VALUE.value, string)
+            matches = re.findall(Expression.ANY_VALUE.value, string)
             return [self._deconvert(match[0]) for match in matches]
 
         if string.startswith("{") and string.endswith("}"):
             string = string[1:-1]
-            matches = regex.findall(Expression.ANY_VALUE.value, string)
+            matches = re.findall(Expression.ANY_VALUE.value, string)
             return {self._deconvert(matches[i][0]): self._deconvert(matches[i + 1][0])
                     for i in range(0, len(matches), 2)}
```

### Comparing `Shchirov_serializer-1.1.2/serializers/json_serializer/serialization_logic.py` & `Shchirov_serializer-1.1.3/serializers/json_serializer/serialization_logic.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.2/serializers/xml_serializer/XmlSerializer.py` & `Shchirov_serializer-1.1.3/serializers/xml_serializer/XmlSerializer.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.2/serializers/xml_serializer/serialization_logic.py` & `Shchirov_serializer-1.1.3/serializers/xml_serializer/serialization_logic.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.2/setup.py` & `Shchirov_serializer-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="Shchirov_serializer",
-    version="1.1.2",
+    version="1.1.3",
     description="python library for serialization",
     url="https://github.com/PaShampusik/PythonLabs/Lab_3",
     author="PaShampusik",
     author_email="shchirovpavel@gmail.com",
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent"
```

### Comparing `Shchirov_serializer-1.1.2/tests/tests.py` & `Shchirov_serializer-1.1.3/tests/tests.py`

 * *Files identical despite different names*

