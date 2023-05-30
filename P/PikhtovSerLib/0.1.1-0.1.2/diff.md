# Comparing `tmp/PikhtovSerLib-0.1.1.tar.gz` & `tmp/PikhtovSerLib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PikhtovSerLib-0.1.1.tar", last modified: Mon May 29 22:00:27 2023, max compression
+gzip compressed data, was "PikhtovSerLib-0.1.2.tar", last modified: Tue May 30 19:14:00 2023, max compression
```

## Comparing `PikhtovSerLib-0.1.1.tar` & `PikhtovSerLib-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2023-05-29 22:00:27.578238 PikhtovSerLib-0.1.1/
--rw-rw-r--   0 maria     (1000) maria     (1000)      706 2023-05-29 22:00:27.578238 PikhtovSerLib-0.1.1/PKG-INFO
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2023-05-29 22:00:27.578238 PikhtovSerLib-0.1.1/PikhtovSerLib/
--rw-rw-r--   0 maria     (1000) maria     (1000)      242 2023-05-29 21:56:08.000000 PikhtovSerLib-0.1.1/PikhtovSerLib/__init__.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     2021 2023-05-28 13:03:52.000000 PikhtovSerLib-0.1.1/PikhtovSerLib/constants.py
--rw-rw-r--   0 maria     (1000) maria     (1000)      418 2023-05-29 19:59:55.000000 PikhtovSerLib-0.1.1/PikhtovSerLib/create_ser.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     2569 2023-05-29 20:50:44.000000 PikhtovSerLib-0.1.1/PikhtovSerLib/json_serealazer.py
--rw-rw-r--   0 maria     (1000) maria     (1000)    12442 2023-05-29 19:59:55.000000 PikhtovSerLib-0.1.1/PikhtovSerLib/my_serelizator.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     3113 2023-05-29 20:55:05.000000 PikhtovSerLib-0.1.1/PikhtovSerLib/xml_serealazer.py
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2023-05-29 22:00:27.578238 PikhtovSerLib-0.1.1/PikhtovSerLib.egg-info/
--rw-rw-r--   0 maria     (1000) maria     (1000)      706 2023-05-29 22:00:27.000000 PikhtovSerLib-0.1.1/PikhtovSerLib.egg-info/PKG-INFO
--rw-rw-r--   0 maria     (1000) maria     (1000)      380 2023-05-29 22:00:27.000000 PikhtovSerLib-0.1.1/PikhtovSerLib.egg-info/SOURCES.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)        1 2023-05-29 22:00:27.000000 PikhtovSerLib-0.1.1/PikhtovSerLib.egg-info/dependency_links.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)        6 2023-05-29 22:00:27.000000 PikhtovSerLib-0.1.1/PikhtovSerLib.egg-info/requires.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)       14 2023-05-29 22:00:27.000000 PikhtovSerLib-0.1.1/PikhtovSerLib.egg-info/top_level.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)       18 2023-05-29 21:00:06.000000 PikhtovSerLib-0.1.1/README.md
--rw-rw-r--   0 maria     (1000) maria     (1000)       38 2023-05-29 22:00:27.582239 PikhtovSerLib-0.1.1/setup.cfg
--rw-rw-r--   0 maria     (1000) maria     (1000)     1302 2023-05-29 21:46:22.000000 PikhtovSerLib-0.1.1/setup.py
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2023-05-30 19:14:00.593127 PikhtovSerLib-0.1.2/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      706 2023-05-30 19:14:00.593127 PikhtovSerLib-0.1.2/PKG-INFO
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2023-05-30 19:14:00.593127 PikhtovSerLib-0.1.2/PikhtovSerLib/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      242 2023-05-29 21:56:08.000000 PikhtovSerLib-0.1.2/PikhtovSerLib/__init__.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     2021 2023-05-28 13:03:52.000000 PikhtovSerLib-0.1.2/PikhtovSerLib/constants.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      418 2023-05-29 19:59:55.000000 PikhtovSerLib-0.1.2/PikhtovSerLib/create_ser.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     2569 2023-05-30 12:24:50.000000 PikhtovSerLib-0.1.2/PikhtovSerLib/json_serealazer.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)    12735 2023-05-30 19:02:53.000000 PikhtovSerLib-0.1.2/PikhtovSerLib/my_serelizator.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     3113 2023-05-29 20:55:05.000000 PikhtovSerLib-0.1.2/PikhtovSerLib/xml_serealazer.py
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2023-05-30 19:14:00.593127 PikhtovSerLib-0.1.2/PikhtovSerLib.egg-info/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      706 2023-05-30 19:14:00.000000 PikhtovSerLib-0.1.2/PikhtovSerLib.egg-info/PKG-INFO
+-rw-rw-r--   0 maria     (1000) maria     (1000)      380 2023-05-30 19:14:00.000000 PikhtovSerLib-0.1.2/PikhtovSerLib.egg-info/SOURCES.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)        1 2023-05-30 19:14:00.000000 PikhtovSerLib-0.1.2/PikhtovSerLib.egg-info/dependency_links.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)        6 2023-05-30 19:14:00.000000 PikhtovSerLib-0.1.2/PikhtovSerLib.egg-info/requires.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)       14 2023-05-30 19:14:00.000000 PikhtovSerLib-0.1.2/PikhtovSerLib.egg-info/top_level.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)       18 2023-05-29 21:00:06.000000 PikhtovSerLib-0.1.2/README.md
+-rw-rw-r--   0 maria     (1000) maria     (1000)       38 2023-05-30 19:14:00.593127 PikhtovSerLib-0.1.2/setup.cfg
+-rw-rw-r--   0 maria     (1000) maria     (1000)     1302 2023-05-30 19:11:04.000000 PikhtovSerLib-0.1.2/setup.py
```

### Comparing `PikhtovSerLib-0.1.1/PKG-INFO` & `PikhtovSerLib-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PikhtovSerLib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Demo library
 Home-page: https://pikhtovserlib.readthedocs.io/
 Author: Pikhtovnikava Maria
 Author-email: pikhtovnikava_maria@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PikhtovSerLib-0.1.1/PikhtovSerLib/constants.py` & `PikhtovSerLib-0.1.2/PikhtovSerLib/constants.py`

 * *Files identical despite different names*

### Comparing `PikhtovSerLib-0.1.1/PikhtovSerLib/json_serealazer.py` & `PikhtovSerLib-0.1.2/PikhtovSerLib/json_serealazer.py`

 * *Files identical despite different names*

### Comparing `PikhtovSerLib-0.1.1/PikhtovSerLib/my_serelizator.py` & `PikhtovSerLib-0.1.2/PikhtovSerLib/my_serelizator.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,30 +32,31 @@
             inf['value'] = selff.dumpss(obj.__name__)
             return inf
         elif isinstance(obj, types.CellType):
             inf['type'] = 'cell'
             inf['value'] = selff.dumpss(obj.cell_contents)
             return inf
 
-        # elif isinstance(obj, types.GeneratorType):
-        #     inf['type'] = 'generator'
-        #     inf['value'] =
-
         elif isclass(obj):
             inf['type'] = 'class'
             inf['value'] = selff.serealize_Class(obj)
             return inf
         elif not obj:
             inf["type"] = "NoneType"
             inf["value"] = 'Null'
             return inf
         elif isinstance(obj, property):
             inf["type"] = "property"
             inf["value"] = selff.serialize_property(obj)
             return inf
+        elif hasattr(obj, "__next__") and hasattr(obj, "__iter__") and callable(obj.__iter__):
+            inf['type'] = 'iterator'
+            inf['value'] = list(map(selff.dumpss, obj))
+            return inf
+
         else:
             inf['type'] = 'object'
             inf['value'] = selff.serelization_Obj(obj)
             return inf
 
     def serialize_property(self, obj):
         val = dict()
@@ -222,14 +223,21 @@
 
         elif obj["type"] == "object":
             return selff.deser_obj(obj["value"])
 
         elif obj["type"] == "property":
             return selff.deser_property(obj)
 
+        elif obj["type"] == "iterator":
+            return selff.deser_iterator(obj)
+
+    def deser_iterator(self, obj):
+        data = obj["value"]
+        return iter(self.loadss(val) for val in data)
+
     def deser_property(self, obj):
         return property(fget=self.loadss(obj["value"]["fget"]),
                         fset=self.loadss(obj["value"]["fset"]),
                         fdel=self.loadss(obj["value"]["fdel"]))
 
     def deser_obj(self, obj):
         clas = self.loadss(obj['__class__'])
```

### Comparing `PikhtovSerLib-0.1.1/PikhtovSerLib/xml_serealazer.py` & `PikhtovSerLib-0.1.2/PikhtovSerLib/xml_serealazer.py`

 * *Files identical despite different names*

### Comparing `PikhtovSerLib-0.1.1/PikhtovSerLib.egg-info/PKG-INFO` & `PikhtovSerLib-0.1.2/PikhtovSerLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PikhtovSerLib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Demo library
 Home-page: https://pikhtovserlib.readthedocs.io/
 Author: Pikhtovnikava Maria
 Author-email: pikhtovnikava_maria@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PikhtovSerLib-0.1.1/setup.py` & `PikhtovSerLib-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="PikhtovSerLib",
-    version="0.1.1",
+    version="0.1.2",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pikhtovserlib.readthedocs.io/",
     author="Pikhtovnikava Maria",
     author_email="pikhtovnikava_maria@email.com",
     license="MIT",
```

