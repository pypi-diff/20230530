# Comparing `tmp/vessel-4.1.0.tar.gz` & `tmp/vessel-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vessel-4.1.0.tar", last modified: Mon May 29 22:05:32 2023, max compression
+gzip compressed data, was "vessel-4.1.1.tar", last modified: Mon May 29 22:12:26 2023, max compression
```

## Comparing `vessel-4.1.0.tar` & `vessel-4.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:05:32.009321 vessel-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-29 22:05:32.009321 vessel-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-29 22:05:20.000000 vessel-4.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 22:05:32.009321 vessel-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-29 22:05:20.000000 vessel-4.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:05:32.009321 vessel-4.1.0/vessel/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-29 22:05:20.000000 vessel-4.1.0/vessel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-29 22:05:20.000000 vessel-4.1.0/vessel/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17421 2023-05-29 22:05:20.000000 vessel-4.1.0/vessel/_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-29 22:05:20.000000 vessel-4.1.0/vessel/_manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:05:32.009321 vessel-4.1.0/vessel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-29 22:05:31.000000 vessel-4.1.0/vessel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-29 22:05:31.000000 vessel-4.1.0/vessel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 22:05:31.000000 vessel-4.1.0/vessel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-29 22:05:31.000000 vessel-4.1.0/vessel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 22:05:31.000000 vessel-4.1.0/vessel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:12:26.131142 vessel-4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-29 22:12:26.131142 vessel-4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-29 22:12:17.000000 vessel-4.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 22:12:26.131142 vessel-4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-29 22:12:17.000000 vessel-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:12:26.131142 vessel-4.1.1/vessel/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-29 22:12:17.000000 vessel-4.1.1/vessel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-29 22:12:17.000000 vessel-4.1.1/vessel/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17470 2023-05-29 22:12:17.000000 vessel-4.1.1/vessel/_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-29 22:12:17.000000 vessel-4.1.1/vessel/_manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:12:26.131142 vessel-4.1.1/vessel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-29 22:12:26.000000 vessel-4.1.1/vessel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-29 22:12:26.000000 vessel-4.1.1/vessel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 22:12:26.000000 vessel-4.1.1/vessel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-29 22:12:26.000000 vessel-4.1.1/vessel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 22:12:26.000000 vessel-4.1.1/vessel.egg-info/top_level.txt
```

### Comparing `vessel-4.1.0/setup.py` & `vessel-4.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.rst', encoding = 'utf-8') as file:
     readme = file.read()
 
 author = 'Exahilosys'
 project = 'vessel'
-version = '4.1.0'
+version = '4.1.1'
 
 url = 'https://github.com/{0}/{1}'.format(author, project)
 
 setuptools.setup(
     name = project,
     python_requires = '>=3.11',
     version = version,
```

### Comparing `vessel-4.1.0/vessel/_helpers.py` & `vessel-4.1.1/vessel/_helpers.py`

 * *Files identical despite different names*

### Comparing `vessel-4.1.0/vessel/_instance.py` & `vessel-4.1.1/vessel/_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     def __new__(cls, name, bases, space, tool = None, expose = ()):
         
         space = dict(space)
 
         space.setdefault('__slots__', ())
 
         for attr_name in expose:
-            if attr_name in space:
+            if attr_name in space or any(hasattr(cls, attr_name) for cls in bases):
                 continue
             space[attr_name] = _Unit_expose(attr_name)
 
         self = super().__new__(cls, name, bases, space)
 
         if not tool is None:
             cache_unit_to_root = weakref.WeakKeyDictionary()
```

### Comparing `vessel-4.1.0/vessel/_manage.py` & `vessel-4.1.1/vessel/_manage.py`

 * *Files identical despite different names*

