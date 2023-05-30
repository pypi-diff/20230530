# Comparing `tmp/arrayclasses-0.1.3.tar.gz` & `tmp/arrayclasses-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrayclasses-0.1.3.tar", max compression
+gzip compressed data, was "arrayclasses-0.1.4.tar", max compression
```

## Comparing `arrayclasses-0.1.3.tar` & `arrayclasses-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-05-26 18:48:49.288191 arrayclasses-0.1.3/LICENSE
--rw-r--r--   0        0        0      731 2023-05-26 18:39:05.635839 arrayclasses-0.1.3/README.md
--rw-r--r--   0        0        0      685 2023-05-26 19:45:38.991969 arrayclasses-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      121 2023-05-26 18:28:15.092746 arrayclasses-0.1.3/src/arrayclasses/__init__.py
--rw-r--r--   0        0        0     3508 2023-05-26 19:44:05.265345 arrayclasses-0.1.3/src/arrayclasses/wrapper.py
--rw-r--r--   0        0        0     1533 2023-05-26 19:45:43.327612 arrayclasses-0.1.3/setup.py
--rw-r--r--   0        0        0     1355 2023-05-26 19:45:43.327820 arrayclasses-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-26 18:48:49.288191 arrayclasses-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1866 2023-05-30 15:01:46.280111 arrayclasses-0.1.4/README.md
+-rw-r--r--   0        0        0      685 2023-05-30 15:02:00.893665 arrayclasses-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      121 2023-05-26 18:28:15.092746 arrayclasses-0.1.4/src/arrayclasses/__init__.py
+-rw-r--r--   0        0        0     3735 2023-05-30 14:56:26.025139 arrayclasses-0.1.4/src/arrayclasses/wrapper.py
+-rw-r--r--   0        0        0     2698 2023-05-30 15:05:26.655300 arrayclasses-0.1.4/setup.py
+-rw-r--r--   0        0        0     2490 2023-05-30 15:05:26.655533 arrayclasses-0.1.4/PKG-INFO
```

### Comparing `arrayclasses-0.1.3/LICENSE` & `arrayclasses-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arrayclasses-0.1.3/pyproject.toml` & `arrayclasses-0.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arrayclasses"
-version = "0.1.3"
+version = "0.1.4"
 description = "Analogue to dataclass that uses a numpy-backed array to store values."
 authors = ["Lukas Tenbrink <lukas.tenbrink@gmail.com>"]
 keywords = ["numpy", "dataclass"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/Ivorforce/python-arrayclass"
 repository = "https://github.com/Ivorforce/python-arrayclass"
```

### Comparing `arrayclasses-0.1.3/src/arrayclasses/wrapper.py` & `arrayclasses-0.1.4/src/arrayclasses/wrapper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import dataclasses
 import functools
 import typing
 import numpy as np
 
 
 def from_array(cls, array):
+    array = np.asarray(array, dtype=cls.__VALUES_TYPE__)
     if cls.__VALUES_LEN__ != len(array):
         raise RuntimeError(
             f"cannot construct arrayclass '{cls}' of length {cls.__VALUES_LEN__} from array of length {len(array)}"
         )
 
     return cls(*np.split(array, cls.__VALUES_OFFSETS__[1:]))
 
@@ -29,100 +30,106 @@
     object.values[item] = value
 
 
 @functools.wraps(dataclasses.dataclass)
 def arrayclass(
     cls=None,
     /,
+    dtype=None,
     **kwargs
 ):
     """Calls dataclasses.dataclass. Also adds the following:
     object.values
     object.__array__
     object.__len__
     object.__getitem__
     object.__setitem__
 
     class.__VALUES_OFFSETS__
     class.__VALUES_LEN__
     """
 
     def wrap(cls):
-        return _process_class(cls, **kwargs)
+        return _process_class(cls, dtype=dtype, **kwargs)
 
     # See if we're being called as @arrayclass or @arrayclass().
     if cls is None:
         # We're called with parens.
         return wrap
 
     # We're called without parens.
     return wrap(cls)
 
 
-def _process_class(cls, **kwargs):
+def _process_class(cls, dtype=None, **kwargs):
     # Copied from dataclasses._process_class, it's not that bad to redo this
     cls_annotations = cls.__dict__.get("__annotations__", {})
     cls_fields = [
         dataclasses._get_field(cls, name, type)
         for name, type in cls_annotations.items()
     ]
 
+    # Go through all the fields and prepare getters / setters.
     value_count = 0
     properties = dict()
     values_offsets = []
     types = []
 
-    # This will be called when the first setter is called in __init__.
-    def create_values_field(self):
-        self.values = np.empty(value_count, dtype=common_type)
-
-    # Go through all the fields and prepare getters / setters.
     for f in cls_fields:
         type_args = typing.get_args(f.type)
         field_length = len(type_args)
         if field_length == 0:
             # Single value
             index = value_count
             field_length = 1
             types.append(f.type)
         else:
             # Multi-Value
             index = slice(value_count, value_count + field_length)
             types.extend(type_args)
 
-        # index=index is a dirty hack; it would be better to construct the function from code
+        # TODO index=index is a dirty hack; it would be better to construct the function from code
         # but eh, that takes effort, right?
         def get(self, *, index=index):
             return self.values[index]
 
         def set(self, value, *, index=index):
-            if not hasattr(self, "values"):
-                create_values_field(self)
             self.values[index] = value
 
         properties[f.name] = property(fget=get, fset=set)
 
         values_offsets.append(value_count)
         value_count += field_length
 
-    common_type = np.find_common_type([], types)
+    if dtype is None:
+        dtype = np.find_common_type([], types)
 
-    # cls.values will be treated as if added by the user, resolving to a field
+    # Make it a dataclass!
     cls = dataclasses.dataclass(cls, **kwargs)
 
+    # Override the init
+    @functools.wraps(cls.__init__)
+    def init(self, *args, **kwargs):
+        self.values = np.empty(value_count, dtype=dtype)
+        self.__dataclass_init__(*args, **kwargs)
+
+    cls.__dataclass_init__ = cls.__init__
+    cls.__init__ = init
+
     # Add the created properties.
-    # Needs to happen after dataclasses.dataclass() because that one queries the assignments (field() or defaults)
+    # There's no references besides __init__ that values should be in __dict__ - so we can just make them properties.
+    # This needs to happen after dataclasses.dataclass() because that one queries the assignments (field() or defaults)
     for name, prop in properties.items():
         setattr(cls, name, prop)
-        pass
 
     # Make us accessible like an array, so things like tuple(obj) and np.array(obj) work.
     cls.__array__ = to_array
     cls.__len__ = get_len
     cls.__getitem__ = getitem
     cls.__setitem__ = setitem
 
     # Used in from_array()
+    cls.__VALUES_TYPE__ = dtype
     cls.__VALUES_OFFSETS__ = values_offsets
     cls.__VALUES_LEN__ = value_count
 
     return cls
```

