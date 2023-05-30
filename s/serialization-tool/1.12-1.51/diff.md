# Comparing `tmp/serialization_tool-1.12.tar.gz` & `tmp/serialization_tool-1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialization_tool-1.12.tar", last modified: Tue May 23 18:31:16 2023, max compression
+gzip compressed data, was "serialization_tool-1.51.tar", last modified: Tue May 30 20:40:15 2023, max compression
```

## Comparing `serialization_tool-1.12.tar` & `serialization_tool-1.51.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 18:31:16.851911 serialization_tool-1.12/
--rw-rw-rw-   0        0        0    35823 2023-05-03 21:01:07.000000 serialization_tool-1.12/LICENSE.txt
--rw-rw-rw-   0        0        0      314 2023-05-23 18:31:16.852913 serialization_tool-1.12/PKG-INFO
--rw-rw-rw-   0        0        0       53 2023-05-03 20:59:54.000000 serialization_tool-1.12/README.md
--rw-rw-rw-   0        0        0      115 2023-05-23 18:31:16.853912 serialization_tool-1.12/setup.cfg
--rw-rw-rw-   0        0        0      427 2023-05-23 18:31:11.000000 serialization_tool-1.12/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 18:31:16.773697 serialization_tool-1.12/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 18:31:16.787784 serialization_tool-1.12/src/serialization_tool/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.12/src/serialization_tool/__init__.py
--rw-rw-rw-   0        0        0       44 2023-05-03 16:35:22.000000 serialization_tool-1.12/src/serialization_tool/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-23 18:31:16.837423 serialization_tool-1.12/src/serialization_tool/serialization/
--rw-rw-rw-   0        0        0        0 2023-05-01 04:12:05.000000 serialization_tool-1.12/src/serialization_tool/serialization/__init__.py
--rw-rw-rw-   0        0        0     1396 2023-05-03 17:44:51.000000 serialization_tool-1.12/src/serialization_tool/serialization/constants.py
--rw-rw-rw-   0        0        0     9770 2023-05-22 16:21:59.000000 serialization_tool-1.12/src/serialization_tool/serialization/serializer.py
--rw-rw-rw-   0        0        0      725 2023-05-18 09:47:32.000000 serialization_tool-1.12/src/serialization_tool/serialization_factory.py
-drwxrwxrwx   0        0        0        0 2023-05-23 18:31:16.840434 serialization_tool-1.12/src/serialization_tool/types/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.12/src/serialization_tool/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 18:31:16.845432 serialization_tool-1.12/src/serialization_tool/types/json/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.12/src/serialization_tool/types/json/__init__.py
--rw-rw-rw-   0        0        0      138 2023-04-28 13:23:00.000000 serialization_tool-1.12/src/serialization_tool/types/json/constants.py
--rw-rw-rw-   0        0        0      578 2023-05-17 19:50:20.000000 serialization_tool-1.12/src/serialization_tool/types/json/json.py
--rw-rw-rw-   0        0        0     6666 2023-05-22 16:21:59.000000 serialization_tool-1.12/src/serialization_tool/types/json/utilities.py
--rw-rw-rw-   0        0        0     1012 2023-05-18 09:50:41.000000 serialization_tool-1.12/src/serialization_tool/types/serialization.py
-drwxrwxrwx   0        0        0        0 2023-05-23 18:31:16.850914 serialization_tool-1.12/src/serialization_tool/types/xml/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.12/src/serialization_tool/types/xml/__init__.py
--rw-rw-rw-   0        0        0      132 2023-05-11 08:00:16.000000 serialization_tool-1.12/src/serialization_tool/types/xml/constants.py
--rw-rw-rw-   0        0        0     2246 2023-05-18 09:36:12.000000 serialization_tool-1.12/src/serialization_tool/types/xml/utilities.py
--rw-rw-rw-   0        0        0      857 2023-05-18 09:35:59.000000 serialization_tool-1.12/src/serialization_tool/types/xml/xml.py
-drwxrwxrwx   0        0        0        0 2023-05-23 18:31:16.832908 serialization_tool-1.12/src/serialization_tool.egg-info/
--rw-rw-rw-   0        0        0      314 2023-05-23 18:31:16.000000 serialization_tool-1.12/src/serialization_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      939 2023-05-23 18:31:16.000000 serialization_tool-1.12/src/serialization_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 18:31:16.000000 serialization_tool-1.12/src/serialization_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-23 18:31:16.000000 serialization_tool-1.12/src/serialization_tool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 20:40:15.806386 serialization_tool-1.51/
+-rw-rw-rw-   0        0        0    35823 2023-05-03 21:01:07.000000 serialization_tool-1.51/LICENSE.txt
+-rw-rw-rw-   0        0        0      314 2023-05-30 20:40:15.807387 serialization_tool-1.51/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2023-05-03 20:59:54.000000 serialization_tool-1.51/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-30 20:40:15.821301 serialization_tool-1.51/setup.cfg
+-rw-rw-rw-   0        0        0      490 2023-05-30 20:40:12.000000 serialization_tool-1.51/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:40:15.705177 serialization_tool-1.51/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 20:40:15.718501 serialization_tool-1.51/src/serialization_tool/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.51/src/serialization_tool/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-05-03 16:35:22.000000 serialization_tool-1.51/src/serialization_tool/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:40:15.783801 serialization_tool-1.51/src/serialization_tool/serialization/
+-rw-rw-rw-   0        0        0        0 2023-05-01 04:12:05.000000 serialization_tool-1.51/src/serialization_tool/serialization/__init__.py
+-rw-rw-rw-   0        0        0     2240 2023-05-30 17:28:57.000000 serialization_tool-1.51/src/serialization_tool/serialization/constants.py
+-rw-rw-rw-   0        0        0    11717 2023-05-30 20:39:01.000000 serialization_tool-1.51/src/serialization_tool/serialization/serializer.py
+-rw-rw-rw-   0        0        0      725 2023-05-18 09:47:32.000000 serialization_tool-1.51/src/serialization_tool/serialization_factory.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:40:15.787309 serialization_tool-1.51/src/serialization_tool/types/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.51/src/serialization_tool/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:40:15.797368 serialization_tool-1.51/src/serialization_tool/types/json/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.51/src/serialization_tool/types/json/__init__.py
+-rw-rw-rw-   0        0        0      850 2023-05-30 16:17:26.000000 serialization_tool-1.51/src/serialization_tool/types/json/constants.py
+-rw-rw-rw-   0        0        0      536 2023-05-30 18:02:49.000000 serialization_tool-1.51/src/serialization_tool/types/json/json.py
+-rw-rw-rw-   0        0        0     2032 2023-05-30 20:38:34.000000 serialization_tool-1.51/src/serialization_tool/types/json/utilities.py
+-rw-rw-rw-   0        0        0     1012 2023-05-18 09:50:41.000000 serialization_tool-1.51/src/serialization_tool/types/serialization.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:40:15.805385 serialization_tool-1.51/src/serialization_tool/types/xml/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.51/src/serialization_tool/types/xml/__init__.py
+-rw-rw-rw-   0        0        0      371 2023-05-30 17:50:19.000000 serialization_tool-1.51/src/serialization_tool/types/xml/constants.py
+-rw-rw-rw-   0        0        0     2264 2023-05-30 20:38:44.000000 serialization_tool-1.51/src/serialization_tool/types/xml/utilities.py
+-rw-rw-rw-   0        0        0     1038 2023-05-30 18:00:48.000000 serialization_tool-1.51/src/serialization_tool/types/xml/xml.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:40:15.778793 serialization_tool-1.51/src/serialization_tool.egg-info/
+-rw-rw-rw-   0        0        0      314 2023-05-30 20:40:15.000000 serialization_tool-1.51/src/serialization_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      984 2023-05-30 20:40:15.000000 serialization_tool-1.51/src/serialization_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 20:40:15.000000 serialization_tool-1.51/src/serialization_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 20:40:15.000000 serialization_tool-1.51/src/serialization_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-30 20:40:15.000000 serialization_tool-1.51/src/serialization_tool.egg-info/top_level.txt
```

### Comparing `serialization_tool-1.12/LICENSE.txt` & `serialization_tool-1.51/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.12/src/serialization_tool/serialization/constants.py` & `serialization_tool-1.51/src/serialization_tool/serialization/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import types
 
-OBJECT_TYPE_REGEX = "\'([\w\W]+)\'"
+OBJECT_TYPE_REGEX = "'([\w\W]+)'"
 REGEX_TYPE = r"\'(\w+)\'"
 
 TYPE = "TYPE"
 VALUE = "VALUE"
 CLASS = "class"
 OBJECT = "object"
 DICTIONARY = "dict"
@@ -15,66 +16,102 @@
 BUILTINS = "__builtins__"
 CLOSURE = "__closure__"
 DOC = "__doc__"
 GLOBALS = "__globals__"
 OBJECT_NAME = "__object_type__"
 FIELDS_NAME = "__fields__"
 MODULE_NAME = "__module__name__"
+ITERATOR = "iterator"
+
 
 CODE = "__code__"
 MODULE = "module"
 
-TYPES = [
-    "int",
-    "float",
-    "bool",
-    "str",
-    "complex",
-    "NoneType"
-]
+TYPES = ["int", "float", "bool", "str", "complex", "NoneType"]
+PRIMITIVES = (int, float, bool, str, types.NoneType, complex)
 
-ITERABLE_TYPES = [
-    "list",
-    "tuple",
-    "set",
-    "bytes"
-]
+COLLECTIONS = (set, list, tuple, bytes, bytearray)
+
+
+ITERABLE_TYPES = ["list", "tuple", "set", "bytes"]
+
+METHOD_DECORATORS = (classmethod, staticmethod)
 
 FUNCTION_ATTRIBUTES = [
-    "__code__",
     "__name__",
+    "__globals__",
+    "__closure__",
     "__defaults__",
-    "__closure__"
+    "__kwdefaults__",
+    "__code__",
 ]
 
-CLASS_ATTRIBUTE_NAMES = ["__class__",
-                         "__doc__",
-                         "__getattribute__",
-                         "__new__",
-                         "__setattr__"
+CLASS_ATTRIBUTE_NAMES = [
+    "__class__",
+    "__doc__",
+    "__getattribute__",
+    "__new__",
+    "__setattr__",
 ]
 
+NOT_SERIALIZING_CLASS_ATTRIBUTES = [
+    "__name__",
+    "__base__",
+    "__basicsize__",
+    "__dictoffset__",
+    "__class__",
+]
+
+NOT_SERIALIZING_TYPES = (
+    types.WrapperDescriptorType,
+    types.MethodDescriptorType,
+    types.BuiltinFunctionType,
+    types.GetSetDescriptorType,
+    types.MappingProxyType,
+)
+
 NOT_CLASS_ATTRIBUTES = [
     "__class__",
     "__getattribute__",
     "__new__",
     "__setattr__",
 ]
 
+CODE_ATTRIBUTES = (
+    "co_argcount",
+    "co_posonlyargcount",
+    "co_kwonlyargcount",
+    "co_nlocals",
+    "co_stacksize",
+    "co_flags",
+    "co_code",
+    "co_consts",
+    "co_names",
+    "co_varnames",
+    "co_filename",
+    "co_name",
+    "co_qualname",
+    "co_firstlineno",
+    "co_lnotab",
+    "co_exceptiontable",
+    "co_freevars",
+    "co_cellvars",
+)
+
 CODE_OBJECT_ARGS = [
-    'co_argcount',
-    'co_posonlyargcount',
-    'co_kwonlyargcount',
-    'co_nlocals',
-    'co_stacksize',
-    'co_flags',
-    'co_code',
-    'co_consts',
-    'co_names',
-    'co_varnames',
-    'co_filename',
-    'co_name',
-    'co_firstlineno',
-    'co_lnotab',
-    'co_freevars',
-    'co_cellvars'
-]
+    "co_argcount",
+    "co_posonlyargcount",
+    "co_kwonlyargcount",
+    "co_nlocals",
+    "co_stacksize",
+    "co_flags",
+    "co_code",
+    "co_consts",
+    "co_names",
+    "co_varnames",
+    "co_filename",
+    "co_name",
+    "co_firstlineno",
+    "co_lnotab",
+    "co_freevars",
+    "co_cellvars",
+]
```

### Comparing `serialization_tool-1.12/src/serialization_tool/serialization_factory.py` & `serialization_tool-1.51/src/serialization_tool/serialization_factory.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.12/src/serialization_tool/types/serialization.py` & `serialization_tool-1.51/src/serialization_tool/types/serialization.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-1.12/src/serialization_tool/types/xml/xml.py` & `serialization_tool-1.51/src/serialization_tool/types/xml/xml.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,21 +5,25 @@
 
 class XmlSerialization(Serialization):
     def dump(self, obj, file):
         with open(file, "w") as f:
             f.write(self.dumps(obj))
 
     def dumps(self, obj):
-        res = to_xml(self.serializer.serialize(obj)).replace('\n', '\n\t')
-        res = "\n<tuple>" + res + "\n</tuple>"
-        return res.replace(
-            "\n", '<?xml version="1.0" encoding="utf-8"?>\n', 1
-        )
+        # res = to_xml(self.serializer.serialize(obj)).replace('\n', '\n\t')
+        # res = "\n<tuple>" + res + "\n</tuple>"
+        # return res.replace(
+        #     "\n", '<?xml version="1.0" encoding="utf-8"?>\n', 1
+        # )
+        result = self.serializer.serialize(obj)
+        return to_xml(result)
 
     def load(self, file):
         with open(file, "r") as f:
             return self.loads(f.read())
 
     def loads(self, data: str):
-        data = data.replace('<?xml version="1.0" encoding="utf-8"?>\n', '')
-        data = data.replace('\n', '').replace('\t', '')
-        return self.serializer.deserialize(from_xml(data))
+        # data = data.replace('<?xml version="1.0" encoding="utf-8"?>\n', '')
+        # data = data.replace('\n', '').replace('\t', '')
+        # return self.serializer.deserialize(from_xml(data))
+        result = self.serializer.deserialize(from_xml(data))
+        return result
```

### Comparing `serialization_tool-1.12/src/serialization_tool.egg-info/SOURCES.txt` & `serialization_tool-1.51/src/serialization_tool.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 src/serialization_tool/__init__.py
 src/serialization_tool/constants.py
 src/serialization_tool/serialization_factory.py
 src/serialization_tool.egg-info/PKG-INFO
 src/serialization_tool.egg-info/SOURCES.txt
 src/serialization_tool.egg-info/dependency_links.txt
+src/serialization_tool.egg-info/requires.txt
 src/serialization_tool.egg-info/top_level.txt
 src/serialization_tool/serialization/__init__.py
 src/serialization_tool/serialization/constants.py
 src/serialization_tool/serialization/serializer.py
 src/serialization_tool/types/__init__.py
 src/serialization_tool/types/serialization.py
 src/serialization_tool/types/json/__init__.py
```

