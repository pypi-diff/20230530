# Comparing `tmp/vessel-4.0.0.tar.gz` & `tmp/vessel-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vessel-4.0.0.tar", last modified: Sat May 27 16:07:55 2023, max compression
+gzip compressed data, was "vessel-4.1.0.tar", last modified: Mon May 29 22:05:32 2023, max compression
```

## Comparing `vessel-4.0.0.tar` & `vessel-4.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:07:55.548474 vessel-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-27 16:07:55.548474 vessel-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-27 16:07:42.000000 vessel-4.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 16:07:55.548474 vessel-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-27 16:07:42.000000 vessel-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:07:55.548474 vessel-4.0.0/vessel/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-27 16:07:42.000000 vessel-4.0.0/vessel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-27 16:07:42.000000 vessel-4.0.0/vessel/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16924 2023-05-27 16:07:42.000000 vessel-4.0.0/vessel/_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-27 16:07:42.000000 vessel-4.0.0/vessel/_manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:07:55.548474 vessel-4.0.0/vessel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-27 16:07:55.000000 vessel-4.0.0/vessel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-27 16:07:55.000000 vessel-4.0.0/vessel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 16:07:55.000000 vessel-4.0.0/vessel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-27 16:07:55.000000 vessel-4.0.0/vessel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 16:07:55.000000 vessel-4.0.0/vessel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:05:32.009321 vessel-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-29 22:05:32.009321 vessel-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-29 22:05:20.000000 vessel-4.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 22:05:32.009321 vessel-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-29 22:05:20.000000 vessel-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:05:32.009321 vessel-4.1.0/vessel/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-29 22:05:20.000000 vessel-4.1.0/vessel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-29 22:05:20.000000 vessel-4.1.0/vessel/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17421 2023-05-29 22:05:20.000000 vessel-4.1.0/vessel/_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-29 22:05:20.000000 vessel-4.1.0/vessel/_manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:05:32.009321 vessel-4.1.0/vessel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-29 22:05:31.000000 vessel-4.1.0/vessel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-29 22:05:31.000000 vessel-4.1.0/vessel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 22:05:31.000000 vessel-4.1.0/vessel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-29 22:05:31.000000 vessel-4.1.0/vessel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 22:05:31.000000 vessel-4.1.0/vessel.egg-info/top_level.txt
```

### Comparing `vessel-4.0.0/setup.py` & `vessel-4.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
-with open('README.rst') as file:
+with open('README.rst', encoding = 'utf-8') as file:
     readme = file.read()
 
 author = 'Exahilosys'
 project = 'vessel'
-version = '4.0.0'
+version = '4.1.0'
 
 url = 'https://github.com/{0}/{1}'.format(author, project)
 
 setuptools.setup(
     name = project,
     python_requires = '>=3.11',
     version = version,
```

### Comparing `vessel-4.0.0/vessel/_helpers.py` & `vessel-4.1.0/vessel/_helpers.py`

 * *Files identical despite different names*

### Comparing `vessel-4.0.0/vessel/_instance.py` & `vessel-4.1.0/vessel/_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import typing
 import weakref
 import collections.abc
 import functools
 import copy
+import contextlib
 
 from . import _helpers
 from . import _manage
 
 
 __all__ = (
-    'Tool', 'theme', 'Unit', 'update', 
+    'Tool', 'resolve', 'theme', 'Unit', 'update', 
     'Object', 'keyify', 
     'List', 'Dict', 'add', 'pop', 
     'collect', 'Collection',
     'strip'
 )
 
 
@@ -71,14 +72,25 @@
 
     info = _Unit_infos[cls]
     root = info.cache_unit_to_root[unit]
 
     return info, root
 
 
+def resolve(unit):
+
+    """
+    Get the root data for a unit.
+    """
+
+    info, root = _analyze(unit)
+
+    return root
+
+
 def _Unit_expose(name):
 
     def method(self, *args, **kwargs):
         info, root = _analyze(self)
         return getattr(root, name)(*args, **kwargs)
     
     method.__name__ = name
@@ -91,14 +103,16 @@
     def __new__(cls, name, bases, space, tool = None, expose = ()):
         
         space = dict(space)
 
         space.setdefault('__slots__', ())
 
         for attr_name in expose:
+            if attr_name in space:
+                continue
             space[attr_name] = _Unit_expose(attr_name)
 
         self = super().__new__(cls, name, bases, space)
 
         if not tool is None:
             cache_unit_to_root = weakref.WeakKeyDictionary()
             cache_name_to_unit = weakref.WeakValueDictionary()
@@ -290,18 +304,19 @@
 
 class ObjectType(UnitType):
 
     @classmethod
     def _get_fields(cls, space):
         
         fields = {}
-        for field_name, field in space.items():
+        for field_name, field in tuple(space.items()):
             if not isinstance(field, GetField):
                 continue
             fields[field_name] = field
+            del space[field_name]
 
         return fields
 
     def __new__(cls, 
                 name, bases, space, 
                 fields  : dict[str, SetField]                                               = None, 
                 identify: typing.Callable[[list[_PathV], _DataV], collections.abc.Hashable] = None,
@@ -321,19 +336,38 @@
 
         if not tool is None:
             _Object_metas[self] = ObjectMeta(set_fields, get_fields, keyify)
 
         return self
     
 
-def _Object_select(root, field):
+_unsafes = set()
+
+
+@contextlib.contextmanager
+def unsafe(cls):
+
+    """
+    Context managers for raising :exc:`AttributeError` instead of returning :var:`.missing`.
+    """
+
+    _unsafes.add(cls)
+
+    yield
+
+    _unsafes.discard(cls)
+    
+
+def _Object_select(name, cls, root, field):
 
     try:
         value = field.select(root)
     except KeyError:
+        if cls in _unsafes:
+            raise AttributeError(name)
         value = _manage.missing
 
     return value
 
 
 class Object(Unit[_DataV], metaclass = ObjectType):
 
@@ -368,45 +402,42 @@
 
         data1 = {'id': 0, 'name': 'One'}
         user1 = User(data1) # <User(id=0, name='One')>
 
         user0 is user1 # True (identify matches)
     """
 
-    def __getattribute__(self, name):
-
-        if name.startswith('__'):
-            return object.__getattribute__(self, name)
+    def __getattr__(self, name):
 
         cls = self.__class__
 
         meta = _Object_metas[cls]
 
         try:
             field = meta.get_fields[name]
         except KeyError as error:
             raise AttributeError(*error.args)
 
         info = _Unit_infos[cls]
 
         root = info.cache_unit_to_root[self]
 
-        value = _Object_select(root, field)
+        value = _Object_select(name, cls, root, field)
         
         return value
     
     def __repr__(self):
 
         cls = self.__class__
 
         info, root, meta = _analyze_object(self, cls)
 
         pairs = []
         for name, field in meta.get_fields.items():
-            value = _Object_select(root, field)
+            value = _Object_select(name, cls, root, field)
             if value is _manage.missing:
                 continue
             pairs.append(f'{name}={repr(value)}')
         
         description = ', '.join(pairs)
 
         return f'<{cls.__name__}({description})>'
```

### Comparing `vessel-4.0.0/vessel/_manage.py` & `vessel-4.1.0/vessel/_manage.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,27 +24,49 @@
     def __getitem__(self, name):
         raise KeyError(name)
     
     def __len__(self):
         return 0
     
     def __getattr__(self, name):
-        return _missing
+        return self
 
     def __delattr__(self, name):
         pass
     
     def __eq__(self, other):
         return False
     
     def __ne__(self, other):
         return True
     
+    def __lt__(self, other):
+        return False
+    
+    def __le__(self, other):
+        return False
+    
+    def __gt__(segf, other):
+        return False
+    
+    def __ge__(self, other):
+        return False
+    
     def __hash__(self):
         return id(self)
+    
+    def __add__(self, other):
+        return self
+    
+    def __sub__(self, other):
+        return self
+    
+    def __mod__(self, other):
+        return self
+        
 
 
 _missing = Missing()
 
 
 missing = _missing
 """
```

