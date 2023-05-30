# Comparing `tmp/betterdataclass-3.3.tar.gz` & `tmp/betterdataclass-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterdataclass-3.3.tar", last modified: Sat May 27 12:48:23 2023, max compression
+gzip compressed data, was "betterdataclass-4.0.tar", last modified: Tue May 30 18:48:54 2023, max compression
```

## Comparing `betterdataclass-3.3.tar` & `betterdataclass-4.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:48:23.268362 betterdataclass-3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-27 12:48:10.000000 betterdataclass-3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-05-27 12:48:23.268362 betterdataclass-3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-05-27 12:48:10.000000 betterdataclass-3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:48:23.268362 betterdataclass-3.3/betterdataclass/
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-27 12:48:10.000000 betterdataclass-3.3/betterdataclass/StrictDictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-27 12:48:10.000000 betterdataclass-3.3/betterdataclass/StrictList.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 12:48:10.000000 betterdataclass-3.3/betterdataclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:48:23.268362 betterdataclass-3.3/betterdataclass/helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 12:48:10.000000 betterdataclass-3.3/betterdataclass/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-27 12:48:10.000000 betterdataclass-3.3/betterdataclass/helper/initiate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-27 12:48:10.000000 betterdataclass-3.3/betterdataclass/helper/to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-27 12:48:10.000000 betterdataclass-3.3/betterdataclass/helper/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-27 12:48:10.000000 betterdataclass-3.3/betterdataclass/strictEnum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:48:23.268362 betterdataclass-3.3/betterdataclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-05-27 12:48:23.000000 betterdataclass-3.3/betterdataclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-27 12:48:23.000000 betterdataclass-3.3/betterdataclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 12:48:23.000000 betterdataclass-3.3/betterdataclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 12:48:23.000000 betterdataclass-3.3/betterdataclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 12:48:23.268362 betterdataclass-3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-27 12:48:10.000000 betterdataclass-3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:48:54.475247 betterdataclass-4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-30 18:48:41.000000 betterdataclass-4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-05-30 18:48:54.475247 betterdataclass-4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-05-30 18:48:41.000000 betterdataclass-4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:48:54.475247 betterdataclass-4.0/betterdataclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-30 18:48:41.000000 betterdataclass-4.0/betterdataclass/StrictDictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-30 18:48:41.000000 betterdataclass-4.0/betterdataclass/StrictList.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:48:41.000000 betterdataclass-4.0/betterdataclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:48:54.475247 betterdataclass-4.0/betterdataclass/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:48:41.000000 betterdataclass-4.0/betterdataclass/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 18:48:41.000000 betterdataclass-4.0/betterdataclass/helper/filterObjectDict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-30 18:48:41.000000 betterdataclass-4.0/betterdataclass/helper/initiate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-30 18:48:41.000000 betterdataclass-4.0/betterdataclass/helper/to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-30 18:48:41.000000 betterdataclass-4.0/betterdataclass/helper/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-30 18:48:41.000000 betterdataclass-4.0/betterdataclass/strictEnum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:48:54.475247 betterdataclass-4.0/betterdataclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-05-30 18:48:54.000000 betterdataclass-4.0/betterdataclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-30 18:48:54.000000 betterdataclass-4.0/betterdataclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:48:54.000000 betterdataclass-4.0/betterdataclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 18:48:54.000000 betterdataclass-4.0/betterdataclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 18:48:54.475247 betterdataclass-4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-30 18:48:41.000000 betterdataclass-4.0/setup.py
```

### Comparing `betterdataclass-3.3/LICENSE` & `betterdataclass-4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `betterdataclass-3.3/PKG-INFO` & `betterdataclass-4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterdataclass
-Version: 3.3
+Version: 4.0
 Summary: A multipurpose dataclass libarary used for validation and data structuring.
 Home-page: https://github.com/dvnasutosh/betterdataclasses
 Author: Asutosh Rath
 Author-email: dvnasutosh@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `betterdataclass-3.3/README.rst` & `betterdataclass-4.0/README.rst`

 * *Files identical despite different names*

### Comparing `betterdataclass-3.3/betterdataclass/StrictDictionary.py` & `betterdataclass-4.0/betterdataclass/StrictDictionary.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,61 +18,70 @@
         """
         # Iterate over the class annotations and set the attributes
         # based on the given keyword arguments
         for i,j in self.__annotations__.items():
             try:
                 self.__data__= getattr(self,i)
             except AttributeError:
-                self.__data__[i]=None
+                self.__setattr__(i,None)
         kwargs = kwargs or {}
 
         for i, j in kwargs.items():
-            self.__data__[i] = j
+            self.__setattr__(i,j)
         
     def __repr__(self) -> str:
         """
         Returns a string representation of the object's dictionary.
         """
         return str(self.__raw__())
     
     def __call__(self,raw:bool=False) -> dict:
-        return self.__raw__() if raw else self.__data__
+        return self.__raw__() if raw else {
+            k: self.__dict__[k]
+            for k in self.__dict__
+            if not (len(k) > 1 and k[0] == k[1] == '_')
+        }
     
     def __str__(self):
         return str(self.__raw__())
 
     def __json__(self)->str:
         return json.dumps(self.__raw__())
     
     def __raw__(self):
         # print(type(self.__data__['nested']))
         from .helper.to_dict import to_raw_dict
-        return to_raw_dict(self.__data__)
+        _data = {
+            k: self.__dict__[k]
+            for k in self.__dict__
+            if not (len(k) > 1 and k[0] == k[1] == '_')
+        }
+        return to_raw_dict(_data)
 
     def __setitem__(self, name, value) -> None:
         """
         Provides indexing and assignment functionality to the object.
         """
-        self.__data__[name]=value
+        self.__setattr__(name,value)
         
 
-    def __setattr__(self, __name: str, __value: Any) -> None:
-        self.__data__[__name]=__value
+    # def __setattr__(self, __name: str, __value: Any) -> None:
+    #     self.__data__[__name]=__value
     
-    def __getattribute__(self, __name: str) -> Any:
-        if __name in super().__getattribute__("__data__").keys():
-            return super().__getattribute__('__data__')[__name]
-        else:
-            return super().__getattribute__(__name)
+    # def __getattribute__(self, __name: str) -> Any:
+    #     if __name in super().__getattribute__("__data__").keys():
+    #         return super().__getattribute__('__data__')[__name]
+    #     else:
+    #         return super().__getattribute__(__name)
     
     def __getitem__(self, name) -> Any:
         """
         Provides indexing and retrieval functionality to the object.
         """
-        return self.__data__[name]
+        return self.__getattribute__(name)
 
 class StrictDictionary(Dictionary):
     """
     A subclass of `Dictionary` that enforces strict typing of the values based on the annotations of the class attributes.
     precaution: dont use Enum. Cant be converted into JSON 
     """
     def __init__(self, **kwargs) -> None:
@@ -89,27 +98,27 @@
                 
                 #SECTION: validation logic 
                 if not validate(self.__annotations__[i],j):
                     raise TypeError(
                         f'{i} key has a value {j} which is of type {type(j)}. {self.__annotations__[i]} expected.')
                 #!SECTION
                 
-                super().__setitem__(i,j)
+                super().__setattr__(i,j)
 
     
     def __init_subclass__(cls) -> None:
         cls.__data__= {}
         
         for k,v in cls.__dict__.items():
             if len(k)>=2 and k[0]!='_' and k[1]!='_':
                 # Handling when it is present in dict but not in annot.(It will default to What is provided)
                 if k not in cls.__annotations__:
                     pass
                 elif Final == cls.__annotations__[k]:
-                    pass         
+                    pass
                 elif Final == get_origin(cls.__annotations__[k]):
                     if not validate(get_args(cls.__annotations__[k])[0],v):
                         raise ValueError(f"{v} is not of type {get_args(cls.__annotations__[k])[0]}")
                 cls.__data__[k] = v
 
         for k,v in cls.__annotations__.items():
             if k not in cls.__data__:
@@ -125,15 +134,15 @@
         # Raise error if the given value is not of the expected type
         if name in self.__data__ and name not in self.__annotations__:
             pass
         elif not validate(self.__annotations__[name],value):
             raise TypeError(
                 f'{name} key has a value {value} which is of type {type(value)}. {self.__annotations__[name]} expected.')
 
-        super().__setitem__(name, value)
+        super().__setattr__(name, value)
 
     def __setitem__(self, name, value) -> None:
         """
         Overrides the superclass `__setitem__` method to perform type checking before assignment.
         If the value to be assigned is not of the expected type, a `TypeError` is raised.
         """
         if name in self.__data__ and name not in self.__annotations__:
```

### Comparing `betterdataclass-3.3/betterdataclass/StrictList.py` & `betterdataclass-4.0/betterdataclass/StrictList.py`

 * *Files identical despite different names*

### Comparing `betterdataclass-3.3/betterdataclass/helper/initiate.py` & `betterdataclass-4.0/betterdataclass/helper/initiate.py`

 * *Files identical despite different names*

### Comparing `betterdataclass-3.3/betterdataclass/helper/to_dict.py` & `betterdataclass-4.0/betterdataclass/helper/to_dict.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 from enum import Enum
 
+from betterdataclass.helper.filterObjectDict import filterDict
+
 
 from ..StrictDictionary import StrictDictionary
 
 
-def to_raw_dict(obj: object, processed=None):
-    if processed is None:
-        processed = set()
-    if id(obj) in processed:
-        return "<circular reference>"
-    processed.add(id(obj))
+def to_raw_dict(obj: object):
     if isinstance(obj, dict):
         out = {}
         for key, value in obj.items():
             if value is None:
                 out[key] = value
             elif isinstance(value, dict):
-                out[key] = to_raw_dict(value, processed)
+                out[key] = to_raw_dict(value)
             elif isinstance(value, Enum):
                 out[key] = [str(value), value.value]
             elif isinstance(value, (list, tuple, set)):
-                out[key] = to_raw_dict(value, processed)
+                out[key] = to_raw_dict(value)
             elif isinstance(value, (int, float, bool, complex, str)):
                 out[key] = value
-            elif isinstance(value,StrictDictionary):
-                out[key] = to_raw_dict(value.__data__, processed)
+            # elif isinstance(value,StrictDictionary):
+            #     out[key] = to_raw_dict(value.__dict__, processed)
             elif isinstance(value, object):
-                out[key] = to_raw_dict(value.__dict__, processed)
+                out[key] = to_raw_dict(filterDict(value.__dict__))
             else:
                 out[key] = str(value)
         return out
     elif obj is None:
         return obj
     elif isinstance(obj, (list, tuple, set)):
-        return [to_raw_dict(item, processed) for item in obj]
+        return [to_raw_dict(item) for item in obj]
     elif isinstance(obj, (int, float, bool, complex, str)):
         return obj
     elif isinstance(obj, Enum):
         return [str(obj), obj.value]
-    elif isinstance(obj,StrictDictionary.StrictDictionary):
-        return to_raw_dict(obj.__data__, processed)
+
     elif isinstance(obj, object):
-        return to_raw_dict(obj.__dict__, processed)
+        return to_raw_dict(filterDict(obj.__dict__))
     else:
         return str(obj)
```

### Comparing `betterdataclass-3.3/betterdataclass/helper/validate.py` & `betterdataclass-4.0/betterdataclass/helper/validate.py`

 * *Files identical despite different names*

### Comparing `betterdataclass-3.3/betterdataclass.egg-info/PKG-INFO` & `betterdataclass-4.0/betterdataclass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterdataclass
-Version: 3.3
+Version: 4.0
 Summary: A multipurpose dataclass libarary used for validation and data structuring.
 Home-page: https://github.com/dvnasutosh/betterdataclasses
 Author: Asutosh Rath
 Author-email: dvnasutosh@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `betterdataclass-3.3/setup.py` & `betterdataclass-4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 import setuptools
 
 
 setup(
     name="betterdataclass",
-    version="3.03",
+    version="4.0",
     description="A multipurpose dataclass libarary used for validation and data structuring.",
     long_description=open('./README.rst').read(),
     url='https://github.com/dvnasutosh/betterdataclasses',
     
     author="Asutosh Rath",
     author_email="dvnasutosh@gmail.com",
     packages=find_packages(),
```

