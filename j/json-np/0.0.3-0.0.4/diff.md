# Comparing `tmp/json_np-0.0.3.tar.gz` & `tmp/json_np-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/luca/work/json_np/dist/.tmp-qrzsxqmq/json_np-0.0.3.tar", last modified: Mon May 29 23:36:30 2023, max compression
+gzip compressed data, was "/Users/luca/work/json_np/dist/.tmp-fwtmjtui/json_np-0.0.4.tar", last modified: Tue May 30 02:09:34 2023, max compression
```

## Comparing `json_np-0.0.3.tar` & `json_np-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-05-29 23:36:30.000000 json_np-0.0.3/
--rw-r--r--   0 luca       (501) staff       (20)     1086 2023-05-29 20:09:17.000000 json_np-0.0.3/LICENSE
--rw-r--r--   0 luca       (501) staff       (20)     2322 2023-05-29 23:36:30.000000 json_np-0.0.3/PKG-INFO
--rw-r--r--   0 luca       (501) staff       (20)     1502 2023-05-29 23:04:27.000000 json_np-0.0.3/README.md
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-05-29 23:36:30.000000 json_np-0.0.3/json_np/
--rw-r--r--   0 luca       (501) staff       (20)       48 2023-05-29 20:27:51.000000 json_np-0.0.3/json_np/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)     8435 2023-05-29 23:32:42.000000 json_np-0.0.3/json_np/json_np.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-05-29 23:36:30.000000 json_np-0.0.3/json_np.egg-info/
--rw-r--r--   0 luca       (501) staff       (20)     2322 2023-05-29 23:36:30.000000 json_np-0.0.3/json_np.egg-info/PKG-INFO
--rw-r--r--   0 luca       (501) staff       (20)      264 2023-05-29 23:36:30.000000 json_np-0.0.3/json_np.egg-info/SOURCES.txt
--rw-r--r--   0 luca       (501) staff       (20)        1 2023-05-29 23:36:30.000000 json_np-0.0.3/json_np.egg-info/dependency_links.txt
--rw-r--r--   0 luca       (501) staff       (20)        1 2023-05-29 22:17:27.000000 json_np-0.0.3/json_np.egg-info/not-zip-safe
--rw-r--r--   0 luca       (501) staff       (20)        6 2023-05-29 23:36:30.000000 json_np-0.0.3/json_np.egg-info/requires.txt
--rw-r--r--   0 luca       (501) staff       (20)        8 2023-05-29 23:36:30.000000 json_np-0.0.3/json_np.egg-info/top_level.txt
--rw-r--r--   0 luca       (501) staff       (20)      104 2023-05-29 20:15:57.000000 json_np-0.0.3/pyproject.toml
--rw-r--r--   0 luca       (501) staff       (20)       38 2023-05-29 23:36:30.000000 json_np-0.0.3/setup.cfg
--rw-r--r--   0 luca       (501) staff       (20)     1156 2023-05-29 23:35:49.000000 json_np-0.0.3/setup.py
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-05-30 02:09:34.000000 json_np-0.0.4/
+-rw-r--r--   0 luca       (501) staff       (20)     1086 2023-05-29 20:09:17.000000 json_np-0.0.4/LICENSE
+-rw-r--r--   0 luca       (501) staff       (20)     3758 2023-05-30 02:09:34.000000 json_np-0.0.4/PKG-INFO
+-rw-r--r--   0 luca       (501) staff       (20)     1502 2023-05-29 23:04:27.000000 json_np-0.0.4/README.md
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-05-30 02:09:34.000000 json_np-0.0.4/json_np/
+-rw-r--r--   0 luca       (501) staff       (20)       48 2023-05-29 20:27:51.000000 json_np-0.0.4/json_np/__init__.py
+-rw-r--r--   0 luca       (501) staff       (20)     9779 2023-05-30 02:09:02.000000 json_np-0.0.4/json_np/json_np.py
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-05-30 02:09:34.000000 json_np-0.0.4/json_np.egg-info/
+-rw-r--r--   0 luca       (501) staff       (20)     3758 2023-05-30 02:09:34.000000 json_np-0.0.4/json_np.egg-info/PKG-INFO
+-rw-r--r--   0 luca       (501) staff       (20)      281 2023-05-30 02:09:34.000000 json_np-0.0.4/json_np.egg-info/SOURCES.txt
+-rw-r--r--   0 luca       (501) staff       (20)        1 2023-05-30 02:09:34.000000 json_np-0.0.4/json_np.egg-info/dependency_links.txt
+-rw-r--r--   0 luca       (501) staff       (20)        1 2023-05-29 22:17:27.000000 json_np-0.0.4/json_np.egg-info/not-zip-safe
+-rw-r--r--   0 luca       (501) staff       (20)        6 2023-05-30 02:09:34.000000 json_np-0.0.4/json_np.egg-info/requires.txt
+-rw-r--r--   0 luca       (501) staff       (20)        8 2023-05-30 02:09:34.000000 json_np-0.0.4/json_np.egg-info/top_level.txt
+-rw-r--r--   0 luca       (501) staff       (20)      994 2023-05-30 02:09:11.000000 json_np-0.0.4/pyproject.toml
+-rw-r--r--   0 luca       (501) staff       (20)        7 2023-05-29 20:22:57.000000 json_np-0.0.4/requirements.txt
+-rw-r--r--   0 luca       (501) staff       (20)       38 2023-05-30 02:09:34.000000 json_np-0.0.4/setup.cfg
+-rw-r--r--   0 luca       (501) staff       (20)     1156 2023-05-29 23:35:49.000000 json_np-0.0.4/setup.py
```

### Comparing `json_np-0.0.3/LICENSE` & `json_np-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `json_np-0.0.3/PKG-INFO` & `json_np-0.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: json_np
-Version: 0.0.3
-Summary: Json serialization extended to dates, numpy arrays, and more
-Home-page: https://github.com/lucadealfaro/json_np
-Author: Luca de Alfaro and Massimo Di Pierro
-Author-email: luca@dealfaro.com, mdipierro@gmail.com
-Maintainer: Luca de Alfaro
-Maintainer-email: luca@dealfaro.com
-License: BSD
-Platform: any
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # json_np
 
 Json for numpy, or if you prefer, json no problems! 
 
 **Authors:** Luca de Alfaro (luca@dealfaro.com) and Massimo Di Pierro 
 (mdipierro@gmail.com)
```

### Comparing `json_np-0.0.3/json_np/json_np.py` & `json_np-0.0.4/json_np/json_np.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,227 +1,291 @@
 #!/usr/bin/env python
+"""
+Copyright 2014 Camiolog Inc.
+Authors: Luca de Alfaro and Massimo Di Pierro
+"""
 
-# Copyright 2014 Camiolog Inc.
-# Authors: Luca de Alfaro and Massimo Di Pierro
+# pylint: disable=invalid-name,too-many-return-statements
 
 import base64
 import collections
 import datetime
 import importlib
 import io
 import json
 import numbers
-import traceback
 
 import numpy
 
 
 class Storage(dict):
+    """
+    Like a dict but attributes can be accessed
+    with obj.name instead obj[name]
+    """
+
     __getattr__ = dict.__getitem__
     __setattr__ = dict.__setitem__
+    __delattr__ = dict.__delitem__
 
 
-class Serializable(object):
+class Serializable:
     """
     If a class subclasses Serializable, then json_plus
     will serialize its objects.
     In a composite object Obj, json_plus will traverse and serialize:
     - primitive types that are json-serializable
     - all lists, dictionaries, sets, numpy arrays, dates.
     - all attributes that are of a Serializable class.
     """
 
-    # We mimick a dict.
+    # We mimic a dict.
     def __getitem__(self, key):
+        """Get a value given a corresponding key."""
         return getattr(self, key)
+
     def __setitem__(self, key, value):
+        """Set a value for the correspoding key."""
         setattr(self, key, value)
+
     def __delitem__(self, key):
+        """Delete a value given a corresponding key."""
         del self.__dict__[key]
+
     def keys(self):
+        """Returns an iterator over keys."""
         return self.__dict__.keys()
+
     def items(self):
+        """Returns an iterator over items."""
         return self.__dict__.items()
+
     def values(self):
+        """Returns an interator over values."""
         return self.__dict__.values()
-    def update(self, d):
-        self.__dict__.update(d)
+
+    def update(self, data):
+        """Update values from provided data dict."""
+        self.__dict__.update(data)
+
     def __len__(self):
+        """Returns the number of items stored."""
         return len(self.__dict__)
+
     def __contains__(self, item):
+        """Returns True if the item is stored, else otherwise."""
         return item in self.__dict__
+
     def __repr__(self):
+        """Returns a string representation for the object."""
         return repr(self.__dict__)
 
-    def get(self, k, d=None):
-        try:
-            return getattr(self, k)
-        except AttributeError:
-            return d
+    def get(self, key, default=None):
+        """Returns the value corresponding to the key or default value."""
+        return getattr(self, key, default)
 
     def __eq__(self, other):
-        return hasattr(other, '__dict__') and self.__dict__ == other.__dict__
+        return hasattr(other, "__dict__") and self.__dict__ == other.__dict__
 
-    def to_json(self, pack_ndarray=True, tolerant=True, indent=2, encoding='utf-8'):
+    def to_json(self, pack_ndarray=True, tolerant=True, indent=2, encoding="utf-8"):
         """
         Dumps itself to a string.
         :param pack_ndarray: Whether to serialize numpy arrays.  Default is yes.
         :param tolerant: Ignore attributes that cannot be serialized.
         :param indent: Indentation of resulting json.
         :param encoding: encoding used for bytes
         :return: The serialized object.
         """
-        return Serializable.dumps(self, pack_ndarray=pack_ndarray, tolerant=tolerant, indent=indent, encoding=encoding)
+        return Serializable.dumps(
+            self,
+            pack_ndarray=pack_ndarray,
+            tolerant=tolerant,
+            indent=indent,
+            encoding=encoding,
+        )
 
     @staticmethod
-    def dump(obj, fp, pack_ndarray=True, tolerant=True, indent=2, encoding='utf-8'):
+    def dump(
+        obj, stream, pack_ndarray=True, tolerant=True, indent=2, encoding="utf-8"
+    ):  # pylint: disable=too-many-arguments
         """
         Dumps an object to a string.
-        :param fp: file where to dump the result.
+        :param stream: file where to dump the result.
         :param obj: The object to serialize.
         :param pack_ndarray: Whether to serialize numpy arrays.  Default is yes.
         :param tolerant: Ignore attributes that cannot be serialized.
         :param indent: Indentation of resulting json.
         :param encoding: encoding used for bytes
         :return: The serialized object.
         """
-        return fp.write(Serializable.dumps(obj, pack_ndarray=pack_ndarray, tolerant=tolerant, indent=indent, encoding=encoding))
+        return stream.write(
+            Serializable.dumps(
+                obj,
+                pack_ndarray=pack_ndarray,
+                tolerant=tolerant,
+                indent=indent,
+                encoding=encoding,
+            )
+        )
 
     @staticmethod
-    def dumps(obj, pack_ndarray=True, tolerant=True, indent=2, encoding='utf-8'):
+    def dumps(obj, pack_ndarray=True, tolerant=True, indent=2, encoding="utf-8"):
         """
         Dumps an object to a string.
         :param obj: The object to serialize.
         :param pack_ndarray: Whether to serialize numpy arrays.  Default is yes.
         :param tolerant: Ignore attributes that cannot be serialized.
         :param indent: Indentation of resulting json.
         :param encoding: encoding used for bytes
         :return: The serialized object.
         """
+
         def custom(o):
             if isinstance(o, Serializable):
                 module = o.__class__.__module__.split(".")[-1]
-                # make sure keys are sorted
                 d = collections.OrderedDict()
-                d['meta_class'] = '%s.%s' % (module, o.__class__.__name__)
-                d.update(item for item in o.__dict__.items()
-                                 if not item[0].startswith('_'))
+                d["meta_class"] = "%s.%s" % (module, o.__class__.__name__)
+                d.update(
+                    item for item in o.__dict__.items() if not item[0].startswith("_")
+                )
                 return d
-            elif isinstance(o, bytes):
+
+            if isinstance(o, bytes):
                 # Bytes are encoded.
-                d = {'meta_class': 'bytes',
-                    'bytes': o.decode(encoding)}
+                d = {"meta_class": "bytes", "bytes": o.decode(encoding)}
                 return d
-            elif isinstance(o, datetime.datetime):
-                d = {'meta_class': 'datetime.datetime',
-                     'date': o.isoformat()}
-                return d
-            elif isinstance(o, set):
-                d = {'meta_class': 'set',
-                     'set': list(o)}
-                return d
-            elif isinstance(o, io.FileIO):
-                return '<file %r>' % o.name
-
-            elif pack_ndarray and isinstance(o, numpy.ndarray):
-                d = {'meta_class': 'numpy.ndarray',
-                     'dtype': str(o.dtype),
-                     'shape': o.shape,
-                     'data': base64.b64encode(o.tobytes())}
+
+            if isinstance(o, datetime.datetime):
+                d = {"meta_class": "datetime.datetime", "date": o.isoformat()}
+                return d
+
+            if isinstance(o, set):
+                d = {"meta_class": "set", "set": list(o)}
+                return d
+
+            if isinstance(o, io.FileIO):
+                return "<file %r>" % o.name
+
+            if pack_ndarray and isinstance(o, numpy.ndarray):
+                d = {
+                    "meta_class": "numpy.ndarray",
+                    "dtype": str(o.dtype),
+                    "shape": o.shape,
+                    "data": base64.b64encode(o.tobytes()),
+                }
                 return d
 
             # Normal Python types are unchanged
-            elif isinstance(o, (int, str, float, bool, list, dict, tuple)):
+            if isinstance(o, (int, str, float, bool, list, dict, tuple)):
                 return o
-            elif isinstance(o, numbers.Integral):
+
+            if isinstance(o, numbers.Integral):
                 return int(o)
-            elif isinstance(o, numbers.Real):
+
+            if isinstance(o, numbers.Real):
                 return float(o)
-            elif isinstance(o, bool):
+
+            if isinstance(o, bool):
                 return bool(o)
-            elif tolerant:
+
+            if isinstance(o, object):
+                # This takes care of arbitrary objects.
+                module = o.__class__.__module__.split(".")[-1]
+                d = collections.OrderedDict()
+                d["meta_class"] = "%s.%s" % (module, o.__class__.__name__)
+                d.update(
+                    item for item in o.__dict__.items() if not item[0].startswith("_")
+                )
+                return d
+
+
+            if tolerant:
                 return None
-            else:
-                raise ValueError("Cannot encode in json object %r" % o)
+
+            raise ValueError("Cannot encode in json object %r" % o)
+
         return json.dumps(obj, default=custom, indent=indent)
 
     @staticmethod
     def from_json(s, mapper=None, encoding="utf-8"):
         """Decodes json_plus.
          :param s : the string to decode
          :param mapper : A dictionary. key classes are replaced by the value classes in the
                 decoding. Classes not found are replaced by Serializable.
         :param encoding: encoding used for bytes
         :return: the decoded object.
         """
         mapper = mapper or {}
+
         def hook(o):
-            meta_module, meta_class = None, o.get('meta_class')
-            if meta_class in ('Datetime', 'datetime.datetime'):
+            meta_module, meta_class = None, o.get("meta_class")
+            if meta_class in ("Datetime", "datetime.datetime"):
                 # 'Datetime' included for backward compatibility
-                try:
-                    tmp = datetime.datetime.strptime(
-                        o['date'], '%Y-%m-%dT%H:%M:%S.%f')
-                except Exception:
-                    tmp = datetime.datetime.strptime(
-                        o['date'], '%Y-%m-%dT%H:%M:%S')
-                return tmp
-            elif meta_class == 'set':
-                return set(o['set'])
-            elif meta_class == 'bytes':
-                return o['bytes'].encode(encoding)
+                fmt = "%Y-%m-%dT%H:%M:%S"
+                if len(o["date"]) > 19:
+                    fmt += ".%f"
+                return datetime.datetime.strptime(o["date"], fmt)
+
+            if meta_class == "set":
+                return set(o["set"])
+
+            if meta_class == "bytes":
+                return o["bytes"].encode(encoding)
+
             # Numpy arrays.
-            elif meta_class == 'numpy.ndarray':
-                data = base64.b64decode(o['data'])
-                dtype = o['dtype']
-                shape = o['shape']
+            if meta_class == "numpy.ndarray":
+                data = base64.b64decode(o["data"])
+                dtype = o["dtype"]
+                shape = o["shape"]
                 v = numpy.frombuffer(data, dtype=dtype)
                 v = v.reshape(shape)
                 obj = v.copy()
                 obj.flags.writeable = True
                 return obj
 
-            elif meta_class and '.' in meta_class:
+            if meta_class and "." in meta_class:
                 # correct for classes that have migrated from one module to another
                 meta_class = mapper.get(meta_class, meta_class)
                 # separate the module name from the actual class name
-                meta_module, meta_class = meta_class.rsplit('.', 1)
+                meta_module, meta_class = meta_class.rsplit(".", 1)
 
             if meta_class is not None:
-                del o['meta_class']
+                del o["meta_class"]
                 if meta_module is not None:
                     meta_class = mapper.get(meta_class, meta_class)
                     try:
                         module = importlib.import_module(meta_module)
                         cls = getattr(module, meta_class)
                         obj = cls()
                         obj.__dict__.update(o)
                         o = obj
-                    except Exception:
+                    except Exception:  # pylint: disable=broad-except
                         # If an object is unknown, restores it as a member
                         # of this same class.
                         obj = Serializable()
                         obj.__dict__.update(o)
                         o = obj
                 else:
                     # Map all to Serializable.
                     obj = Serializable()
                     obj.__dict__.update(o)
                     o = obj
-            elif type(o).__name__ == 'dict':
+            elif type(o).__name__ == "dict":
                 # For convenience we deserialize dict into Storage.
                 o = Storage(o)
             return o
 
         return json.loads(s, object_hook=hook)
 
     @staticmethod
-    def loads(s):
-        return Serializable.from_json(s)
+    def loads(string):
+        """Loads json from input string."""
+        return Serializable.from_json(string)
 
     @staticmethod
-    def load(fp):
-        return Serializable.loads(fp.read())
+    def load(stream):
+        """Loads json from input stream."""
+        return Serializable.loads(stream.read())
 
 
 loads = Serializable.loads
 dumps = Serializable.dumps
```

### Comparing `json_np-0.0.3/json_np.egg-info/PKG-INFO` & `json_np-0.0.4/json_np.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,46 @@
 Metadata-Version: 2.1
 Name: json-np
-Version: 0.0.3
+Version: 0.0.4
 Summary: Json serialization extended to dates, numpy arrays, and more
 Home-page: https://github.com/lucadealfaro/json_np
 Author: Luca de Alfaro and Massimo Di Pierro
-Author-email: luca@dealfaro.com, mdipierro@gmail.com
+Author-email: Luca de Alfaro <luca@dealfaro.com>, Massimo Di Pierro <massimo.dipierro@gmail.com>
 Maintainer: Luca de Alfaro
 Maintainer-email: luca@dealfaro.com
-License: BSD
+License: MIT License
+        
+        Copyright (c) 2017 Camio and 2023 Luca de Alfaro
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/lucadealfaro/json_np
+Project-URL: Bug Tracker, https://github.com/lucadealfaro/json_np/issues
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # json_np
```

### Comparing `json_np-0.0.3/setup.py` & `json_np-0.0.4/setup.py`

 * *Files identical despite different names*

