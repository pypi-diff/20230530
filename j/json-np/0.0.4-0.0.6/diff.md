# Comparing `tmp/json_np-0.0.4.tar.gz` & `tmp/json_np-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/luca/work/json_np/dist/.tmp-fwtmjtui/json_np-0.0.4.tar", last modified: Tue May 30 02:09:34 2023, max compression
+gzip compressed data, was "/Users/luca/work/json_np/dist/.tmp-0u93b4yk/json_np-0.0.6.tar", last modified: Tue May 30 02:33:00 2023, max compression
```

## Comparing `json_np-0.0.4.tar` & `json_np-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-05-30 02:09:34.000000 json_np-0.0.4/
--rw-r--r--   0 luca       (501) staff       (20)     1086 2023-05-29 20:09:17.000000 json_np-0.0.4/LICENSE
--rw-r--r--   0 luca       (501) staff       (20)     3758 2023-05-30 02:09:34.000000 json_np-0.0.4/PKG-INFO
--rw-r--r--   0 luca       (501) staff       (20)     1502 2023-05-29 23:04:27.000000 json_np-0.0.4/README.md
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-05-30 02:09:34.000000 json_np-0.0.4/json_np/
--rw-r--r--   0 luca       (501) staff       (20)       48 2023-05-29 20:27:51.000000 json_np-0.0.4/json_np/__init__.py
--rw-r--r--   0 luca       (501) staff       (20)     9779 2023-05-30 02:09:02.000000 json_np-0.0.4/json_np/json_np.py
-drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-05-30 02:09:34.000000 json_np-0.0.4/json_np.egg-info/
--rw-r--r--   0 luca       (501) staff       (20)     3758 2023-05-30 02:09:34.000000 json_np-0.0.4/json_np.egg-info/PKG-INFO
--rw-r--r--   0 luca       (501) staff       (20)      281 2023-05-30 02:09:34.000000 json_np-0.0.4/json_np.egg-info/SOURCES.txt
--rw-r--r--   0 luca       (501) staff       (20)        1 2023-05-30 02:09:34.000000 json_np-0.0.4/json_np.egg-info/dependency_links.txt
--rw-r--r--   0 luca       (501) staff       (20)        1 2023-05-29 22:17:27.000000 json_np-0.0.4/json_np.egg-info/not-zip-safe
--rw-r--r--   0 luca       (501) staff       (20)        6 2023-05-30 02:09:34.000000 json_np-0.0.4/json_np.egg-info/requires.txt
--rw-r--r--   0 luca       (501) staff       (20)        8 2023-05-30 02:09:34.000000 json_np-0.0.4/json_np.egg-info/top_level.txt
--rw-r--r--   0 luca       (501) staff       (20)      994 2023-05-30 02:09:11.000000 json_np-0.0.4/pyproject.toml
--rw-r--r--   0 luca       (501) staff       (20)        7 2023-05-29 20:22:57.000000 json_np-0.0.4/requirements.txt
--rw-r--r--   0 luca       (501) staff       (20)       38 2023-05-30 02:09:34.000000 json_np-0.0.4/setup.cfg
--rw-r--r--   0 luca       (501) staff       (20)     1156 2023-05-29 23:35:49.000000 json_np-0.0.4/setup.py
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-05-30 02:33:00.000000 json_np-0.0.6/
+-rw-r--r--   0 luca       (501) staff       (20)     1086 2023-05-29 20:09:17.000000 json_np-0.0.6/LICENSE
+-rw-r--r--   0 luca       (501) staff       (20)     3810 2023-05-30 02:33:00.000000 json_np-0.0.6/PKG-INFO
+-rw-r--r--   0 luca       (501) staff       (20)     1727 2023-05-30 02:29:47.000000 json_np-0.0.6/README.md
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-05-30 02:33:00.000000 json_np-0.0.6/json_np/
+-rw-r--r--   0 luca       (501) staff       (20)       48 2023-05-29 20:27:51.000000 json_np-0.0.6/json_np/__init__.py
+-rw-r--r--   0 luca       (501) staff       (20)     9956 2023-05-30 02:25:57.000000 json_np-0.0.6/json_np/json_np.py
+drwxr-xr-x   0 luca       (501) staff       (20)        0 2023-05-30 02:33:00.000000 json_np-0.0.6/json_np.egg-info/
+-rw-r--r--   0 luca       (501) staff       (20)     3810 2023-05-30 02:33:00.000000 json_np-0.0.6/json_np.egg-info/PKG-INFO
+-rw-r--r--   0 luca       (501) staff       (20)      242 2023-05-30 02:33:00.000000 json_np-0.0.6/json_np.egg-info/SOURCES.txt
+-rw-r--r--   0 luca       (501) staff       (20)        1 2023-05-30 02:33:00.000000 json_np-0.0.6/json_np.egg-info/dependency_links.txt
+-rw-r--r--   0 luca       (501) staff       (20)        6 2023-05-30 02:33:00.000000 json_np-0.0.6/json_np.egg-info/requires.txt
+-rw-r--r--   0 luca       (501) staff       (20)        8 2023-05-30 02:33:00.000000 json_np-0.0.6/json_np.egg-info/top_level.txt
+-rw-r--r--   0 luca       (501) staff       (20)      994 2023-05-30 02:32:46.000000 json_np-0.0.6/pyproject.toml
+-rw-r--r--   0 luca       (501) staff       (20)        7 2023-05-29 20:22:57.000000 json_np-0.0.6/requirements.txt
+-rw-r--r--   0 luca       (501) staff       (20)       38 2023-05-30 02:33:00.000000 json_np-0.0.6/setup.cfg
```

### Comparing `json_np-0.0.4/LICENSE` & `json_np-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `json_np-0.0.4/PKG-INFO` & `json_np-0.0.6/json_np.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 Metadata-Version: 2.1
-Name: json_np
-Version: 0.0.4
+Name: json-np
+Version: 0.0.6
 Summary: Json serialization extended to dates, numpy arrays, and more
-Home-page: https://github.com/lucadealfaro/json_np
-Author: Luca de Alfaro and Massimo Di Pierro
 Author-email: Luca de Alfaro <luca@dealfaro.com>, Massimo Di Pierro <massimo.dipierro@gmail.com>
-Maintainer: Luca de Alfaro
-Maintainer-email: luca@dealfaro.com
 License: MIT License
         
         Copyright (c) 2017 Camio and 2023 Luca de Alfaro
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -27,15 +23,14 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/lucadealfaro/json_np
 Project-URL: Bug Tracker, https://github.com/lucadealfaro/json_np/issues
-Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -72,32 +67,41 @@
 
 Here, we have applied `json_np.dumps` to a numpy array, but we could equally 
 well have used a datetime, a dictionary, a list, etc (nesting of such types is 
 allowed).
 
 ## Class-Based Usage
 
-In class-based usage, you can declare a class to be a subclass of `json_np.
-Serializable`.  Then, calling the `to_json` method of an object causes the 
-complete object to be serialized, including recursively all object 
-attributes, except for the attributes that start with underscore (`_`). 
+You can also dump any object.
+All object attributes, except those whose name begins with underscore (`_`), 
+will be serialized. 
+Optionally, if `serializable_only` is True, only objects that are 
+instances of `Serializable`, or that are dates, numpy arrays,  will be 
+serialized. 
+
+The deserialization happens in the same class, if:
+* the class can be loaded
+* the class initializer has no required arguments.
+
+If any of these two conditions is not met, the deserialization happens
+using the `Serializable` class. 
 
 ```
 from json_np import Serializable
 
-class C(Serializable):
+class C(object):
 
-    def __init__(self, a):
+    def __init__(self, a=8):
         super().__init__()
         self.a = a # Serialized
         self._b = 32 # Not serialized
 
 c = C("hello")
-s = c.to_json()
-cc = C.from_json(s)
+s = json_np.dumps(c)
+cc = json_np.loads(s)
 ```
 
 Obviously, you should ensure that C contains compatible fields when it is 
 deserialized, in case the code changed in the meantime. 
 
 ## History
```

### Comparing `json_np-0.0.4/README.md` & `json_np-0.0.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -27,32 +27,41 @@
 
 Here, we have applied `json_np.dumps` to a numpy array, but we could equally 
 well have used a datetime, a dictionary, a list, etc (nesting of such types is 
 allowed).
 
 ## Class-Based Usage
 
-In class-based usage, you can declare a class to be a subclass of `json_np.
-Serializable`.  Then, calling the `to_json` method of an object causes the 
-complete object to be serialized, including recursively all object 
-attributes, except for the attributes that start with underscore (`_`). 
+You can also dump any object.
+All object attributes, except those whose name begins with underscore (`_`), 
+will be serialized. 
+Optionally, if `serializable_only` is True, only objects that are 
+instances of `Serializable`, or that are dates, numpy arrays,  will be 
+serialized. 
+
+The deserialization happens in the same class, if:
+* the class can be loaded
+* the class initializer has no required arguments.
+
+If any of these two conditions is not met, the deserialization happens
+using the `Serializable` class. 
 
 ```
 from json_np import Serializable
 
-class C(Serializable):
+class C(object):
 
-    def __init__(self, a):
+    def __init__(self, a=8):
         super().__init__()
         self.a = a # Serialized
         self._b = 32 # Not serialized
 
 c = C("hello")
-s = c.to_json()
-cc = C.from_json(s)
+s = json_np.dumps(c)
+cc = json_np.loads(s)
 ```
 
 Obviously, you should ensure that C contains compatible fields when it is 
 deserialized, in case the code changed in the meantime. 
 
 ## History
```

### Comparing `json_np-0.0.4/json_np/json_np.py` & `json_np-0.0.6/json_np/json_np.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,22 +124,25 @@
                 tolerant=tolerant,
                 indent=indent,
                 encoding=encoding,
             )
         )
 
     @staticmethod
-    def dumps(obj, pack_ndarray=True, tolerant=True, indent=2, encoding="utf-8"):
+    def dumps(obj, pack_ndarray=True, tolerant=True, indent=2, encoding="utf-8",
+              serializable_only=False):
         """
         Dumps an object to a string.
         :param obj: The object to serialize.
         :param pack_ndarray: Whether to serialize numpy arrays.  Default is yes.
         :param tolerant: Ignore attributes that cannot be serialized.
         :param indent: Indentation of resulting json.
         :param encoding: encoding used for bytes
+        :param serializable_only: if True, only classes of Serializable subclass
+            will be serialized.
         :return: The serialized object.
         """
 
         def custom(o):
             if isinstance(o, Serializable):
                 module = o.__class__.__module__.split(".")[-1]
                 d = collections.OrderedDict()
@@ -183,25 +186,24 @@
 
             if isinstance(o, numbers.Real):
                 return float(o)
 
             if isinstance(o, bool):
                 return bool(o)
 
-            if isinstance(o, object):
+            if isinstance(o, object) and not serializable_only:
                 # This takes care of arbitrary objects.
                 module = o.__class__.__module__.split(".")[-1]
                 d = collections.OrderedDict()
                 d["meta_class"] = "%s.%s" % (module, o.__class__.__name__)
                 d.update(
                     item for item in o.__dict__.items() if not item[0].startswith("_")
                 )
                 return d
 
-
             if tolerant:
                 return None
 
             raise ValueError("Cannot encode in json object %r" % o)
 
         return json.dumps(obj, default=custom, indent=indent)
```

### Comparing `json_np-0.0.4/json_np.egg-info/PKG-INFO` & `json_np-0.0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 Metadata-Version: 2.1
-Name: json-np
-Version: 0.0.4
+Name: json_np
+Version: 0.0.6
 Summary: Json serialization extended to dates, numpy arrays, and more
-Home-page: https://github.com/lucadealfaro/json_np
-Author: Luca de Alfaro and Massimo Di Pierro
 Author-email: Luca de Alfaro <luca@dealfaro.com>, Massimo Di Pierro <massimo.dipierro@gmail.com>
-Maintainer: Luca de Alfaro
-Maintainer-email: luca@dealfaro.com
 License: MIT License
         
         Copyright (c) 2017 Camio and 2023 Luca de Alfaro
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -27,15 +23,14 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/lucadealfaro/json_np
 Project-URL: Bug Tracker, https://github.com/lucadealfaro/json_np/issues
-Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -72,32 +67,41 @@
 
 Here, we have applied `json_np.dumps` to a numpy array, but we could equally 
 well have used a datetime, a dictionary, a list, etc (nesting of such types is 
 allowed).
 
 ## Class-Based Usage
 
-In class-based usage, you can declare a class to be a subclass of `json_np.
-Serializable`.  Then, calling the `to_json` method of an object causes the 
-complete object to be serialized, including recursively all object 
-attributes, except for the attributes that start with underscore (`_`). 
+You can also dump any object.
+All object attributes, except those whose name begins with underscore (`_`), 
+will be serialized. 
+Optionally, if `serializable_only` is True, only objects that are 
+instances of `Serializable`, or that are dates, numpy arrays,  will be 
+serialized. 
+
+The deserialization happens in the same class, if:
+* the class can be loaded
+* the class initializer has no required arguments.
+
+If any of these two conditions is not met, the deserialization happens
+using the `Serializable` class. 
 
 ```
 from json_np import Serializable
 
-class C(Serializable):
+class C(object):
 
-    def __init__(self, a):
+    def __init__(self, a=8):
         super().__init__()
         self.a = a # Serialized
         self._b = 32 # Not serialized
 
 c = C("hello")
-s = c.to_json()
-cc = C.from_json(s)
+s = json_np.dumps(c)
+cc = json_np.loads(s)
 ```
 
 Obviously, you should ensure that C contains compatible fields when it is 
 deserialized, in case the code changed in the meantime. 
 
 ## History
```

### Comparing `json_np-0.0.4/pyproject.toml` & `json_np-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "json_np"
-version = "0.0.4"
+version = "0.0.6"
 authors = [{name="Luca de Alfaro", email="luca@dealfaro.com"}, {name="Massimo Di Pierro", email="massimo.dipierro@gmail.com" },]
 description = "Json serialization extended to dates, numpy arrays, and more"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file="LICENSE"}
 classifiers = [
         "Development Status :: 3 - Alpha",
```

