# Comparing `tmp/Shchirov_serializer-1.1.3.tar.gz` & `tmp/Shchirov_serializer-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shchirov_serializer-1.1.3.tar", last modified: Tue May 30 21:04:28 2023, max compression
+gzip compressed data, was "Shchirov_serializer-1.1.4.tar", last modified: Tue May 30 21:19:22 2023, max compression
```

## Comparing `Shchirov_serializer-1.1.3.tar` & `Shchirov_serializer-1.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:04:28.024458 Shchirov_serializer-1.1.3/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      320 2023-05-30 21:04:28.024458 Shchirov_serializer-1.1.3/PKG-INFO
--rw-r--r--   0 pavel     (1000) pavel     (1000)       66 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.3/README.md
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:04:28.020458 Shchirov_serializer-1.1.3/Shchirov_serializer.egg-info/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      320 2023-05-30 21:04:27.000000 Shchirov_serializer-1.1.3/Shchirov_serializer.egg-info/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      651 2023-05-30 21:04:28.000000 Shchirov_serializer-1.1.3/Shchirov_serializer.egg-info/SOURCES.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-05-30 21:04:27.000000 Shchirov_serializer-1.1.3/Shchirov_serializer.egg-info/dependency_links.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       84 2023-05-30 21:04:27.000000 Shchirov_serializer-1.1.3/Shchirov_serializer.egg-info/top_level.txt
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:04:28.020458 Shchirov_serializer-1.1.3/serializers/
--rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.3/serializers/__init__.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:04:28.024458 Shchirov_serializer-1.1.3/serializers/base/
--rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.3/serializers/base/__init__.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     2780 2023-05-30 17:50:06.000000 Shchirov_serializer-1.1.3/serializers/base/constants.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     5479 2023-05-30 19:38:26.000000 Shchirov_serializer-1.1.3/serializers/base/deserialization.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     5488 2023-05-30 20:58:37.000000 Shchirov_serializer-1.1.3/serializers/base/serialization.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)      455 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.3/serializers/factory.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:04:28.024458 Shchirov_serializer-1.1.3/serializers/json_serializer/
--rw-r--r--   0 pavel     (1000) pavel     (1000)     3409 2023-05-30 21:04:20.000000 Shchirov_serializer-1.1.3/serializers/json_serializer/JsonSerializer.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.3/serializers/json_serializer/__init__.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     1313 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.3/serializers/json_serializer/serialization_logic.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:04:28.024458 Shchirov_serializer-1.1.3/serializers/xml_serializer/
--rw-r--r--   0 pavel     (1000) pavel     (1000)     3748 2023-05-30 19:42:12.000000 Shchirov_serializer-1.1.3/serializers/xml_serializer/XmlSerializer.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.3/serializers/xml_serializer/__init__.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     1430 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.3/serializers/xml_serializer/serialization_logic.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       38 2023-05-30 21:04:28.024458 Shchirov_serializer-1.1.3/setup.cfg
--rw-r--r--   0 pavel     (1000) pavel     (1000)      549 2023-05-30 21:04:25.000000 Shchirov_serializer-1.1.3/setup.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:04:28.024458 Shchirov_serializer-1.1.3/tests/
--rw-r--r--   0 pavel     (1000) pavel     (1000)     7933 2023-05-30 19:59:33.000000 Shchirov_serializer-1.1.3/tests/tests.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:19:22.884149 Shchirov_serializer-1.1.4/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      320 2023-05-30 21:19:22.884149 Shchirov_serializer-1.1.4/PKG-INFO
+-rw-r--r--   0 pavel     (1000) pavel     (1000)       66 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.4/README.md
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:19:22.884149 Shchirov_serializer-1.1.4/Shchirov_serializer.egg-info/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      320 2023-05-30 21:19:22.000000 Shchirov_serializer-1.1.4/Shchirov_serializer.egg-info/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      651 2023-05-30 21:19:22.000000 Shchirov_serializer-1.1.4/Shchirov_serializer.egg-info/SOURCES.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-05-30 21:19:22.000000 Shchirov_serializer-1.1.4/Shchirov_serializer.egg-info/dependency_links.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       84 2023-05-30 21:19:22.000000 Shchirov_serializer-1.1.4/Shchirov_serializer.egg-info/top_level.txt
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:19:22.884149 Shchirov_serializer-1.1.4/serializers/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.4/serializers/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:19:22.884149 Shchirov_serializer-1.1.4/serializers/base/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.4/serializers/base/__init__.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     2780 2023-05-30 17:50:06.000000 Shchirov_serializer-1.1.4/serializers/base/constants.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     5479 2023-05-30 19:38:26.000000 Shchirov_serializer-1.1.4/serializers/base/deserialization.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     5488 2023-05-30 20:58:37.000000 Shchirov_serializer-1.1.4/serializers/base/serialization.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)      455 2023-05-30 21:08:16.000000 Shchirov_serializer-1.1.4/serializers/factory.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:19:22.884149 Shchirov_serializer-1.1.4/serializers/json_serializer/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     3210 2023-05-30 21:13:36.000000 Shchirov_serializer-1.1.4/serializers/json_serializer/JsonSerializer.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.4/serializers/json_serializer/__init__.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     1313 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.4/serializers/json_serializer/serialization_logic.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:19:22.884149 Shchirov_serializer-1.1.4/serializers/xml_serializer/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     3748 2023-05-30 19:42:12.000000 Shchirov_serializer-1.1.4/serializers/xml_serializer/XmlSerializer.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.4/serializers/xml_serializer/__init__.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     1430 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.4/serializers/xml_serializer/serialization_logic.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       38 2023-05-30 21:19:22.884149 Shchirov_serializer-1.1.4/setup.cfg
+-rw-r--r--   0 pavel     (1000) pavel     (1000)      549 2023-05-30 21:19:21.000000 Shchirov_serializer-1.1.4/setup.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:19:22.884149 Shchirov_serializer-1.1.4/tests/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     8041 2023-05-30 21:18:45.000000 Shchirov_serializer-1.1.4/tests/tests.py
```

### Comparing `Shchirov_serializer-1.1.3/Shchirov_serializer.egg-info/SOURCES.txt` & `Shchirov_serializer-1.1.4/Shchirov_serializer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.3/serializers/base/constants.py` & `Shchirov_serializer-1.1.4/serializers/base/constants.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.3/serializers/base/deserialization.py` & `Shchirov_serializer-1.1.4/serializers/base/deserialization.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.3/serializers/base/serialization.py` & `Shchirov_serializer-1.1.4/serializers/base/serialization.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.3/serializers/json_serializer/JsonSerializer.py` & `Shchirov_serializer-1.1.4/serializers/json_serializer/JsonSerializer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-# from ..base.serialization import get_serializer_function
-# from ..base.deserialization import create_deserializer
-# from .serialization_logic import serialize_to_json
-# from .serialization_logic import deserialize_json
-
 from typing import Any
 from serializers.base.deserialization import Deserializer
 from serializers.base.serialization import Serializer
 from ..base.constants import (PRIMITIVES,
                          JsonRegularExpression as Expression)
-import re
+import regex
 
 
-class _JsonSerializer:
+class JsonSerializer:
     def dumps(self, obj: Any) -> str:
         """
         Convert an object to string of 'JSON' format.
 
         :param obj: Any python object.
         :type obj: Any
 
@@ -75,33 +70,33 @@
 
         :return: Dictionary that represents object.
         :rtype: dict
         """
 
         string = string.strip()
 
-        if re.fullmatch(Expression.INT.value, string):
+        if regex.fullmatch(Expression.INT.value, string):
             return int(string)
 
-        if re.fullmatch(Expression.STR.value, string):
+        if regex.fullmatch(Expression.STR.value, string):
             string = string.replace("\\\\", "\\").replace(r"\"", '"').replace(r"\'", "'")
             return string[1:-1]
 
-        if re.fullmatch(Expression.FLOAT.value, string):
+        if regex.fullmatch(Expression.FLOAT.value, string):
             return float(string)
 
-        if re.fullmatch(Expression.BOOL.value, string):
+        if regex.fullmatch(Expression.BOOL.value, string):
             return True if string == 'True' else False
 
-        if re.fullmatch(Expression.NONE.value, string):
+        if regex.fullmatch(Expression.NONE.value, string):
             return None
 
         if string.startswith("[") and string.endswith("]"):
             string = string[1:-1]
-            matches = re.findall(Expression.ANY_VALUE.value, string)
+            matches = regex.findall(Expression.ANY_VALUE.value, string)
             return [self._deconvert(match[0]) for match in matches]
 
         if string.startswith("{") and string.endswith("}"):
             string = string[1:-1]
-            matches = re.findall(Expression.ANY_VALUE.value, string)
+            matches = regex.findall(Expression.ANY_VALUE.value, string)
             return {self._deconvert(matches[i][0]): self._deconvert(matches[i + 1][0])
                     for i in range(0, len(matches), 2)}
```

### Comparing `Shchirov_serializer-1.1.3/serializers/json_serializer/serialization_logic.py` & `Shchirov_serializer-1.1.4/serializers/json_serializer/serialization_logic.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.3/serializers/xml_serializer/XmlSerializer.py` & `Shchirov_serializer-1.1.4/serializers/xml_serializer/XmlSerializer.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.3/serializers/xml_serializer/serialization_logic.py` & `Shchirov_serializer-1.1.4/serializers/xml_serializer/serialization_logic.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.3/setup.py` & `Shchirov_serializer-1.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="Shchirov_serializer",
-    version="1.1.3",
+    version="1.1.4",
     description="python library for serialization",
     url="https://github.com/PaShampusik/PythonLabs/Lab_3",
     author="PaShampusik",
     author_email="shchirovpavel@gmail.com",
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent"
```

### Comparing `Shchirov_serializer-1.1.3/tests/tests.py` & `Shchirov_serializer-1.1.4/tests/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import unittest
-from serializers.json_serializer.JsonSerializer import _JsonSerializer
+from serializers.json_serializer.JsonSerializer import JsonSerializer
+from serializers.xml_serializer.XmlSerializer import XmlSerializer
 from tests.constants_for_testing import (circle_area, square_area, generator, bts, bts_arr, sum_func,
                         generator_expression, closure, factorial, Profile,
                         sum_args, sum_kwargs, sum_args_kwargs, subgenerator,
                         lambda_pow, C, E, Human, func1, func2, func3, it)
 
 
 
 class BaseJsonTestCase(unittest.TestCase):
     def setUp(self) -> None:
-        self.serializer = _JsonSerializer()
+        self.serializer = JsonSerializer()
+        #self.serializer = XmlSerializer()
         self.alias = lambda x: self.serializer.loads(self.serializer.dumps(x))
 
 
 class PrimitivesTestCase(BaseJsonTestCase):
     def test_int(self):
         self.assertEqual(10, self.alias(10))
         self.assertEqual(0, 0)
```

