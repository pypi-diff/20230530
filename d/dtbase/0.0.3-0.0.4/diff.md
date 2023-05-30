# Comparing `tmp/dtbase-0.0.3.tar.gz` & `tmp/dtbase-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtbase-0.0.3.tar", max compression
+gzip compressed data, was "dtbase-0.0.4.tar", max compression
```

## Comparing `dtbase-0.0.3.tar` & `dtbase-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       43 2023-05-26 23:58:37.938978 dtbase-0.0.3/dtbase/__init__.py
--rw-r--r--   0        0        0     5281 2023-05-26 23:45:18.887306 dtbase-0.0.3/dtbase/config.py
--rw-r--r--   0        0        0     5718 2023-05-26 23:58:37.934512 dtbase-0.0.3/dtbase/engine.py
--rw-r--r--   0        0        0      369 2023-05-28 21:57:12.156664 dtbase-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      632 2023-05-28 21:57:24.397059 dtbase-0.0.3/setup.py
--rw-r--r--   0        0        0      412 2023-05-28 21:57:24.397279 dtbase-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-05-26 23:58:37.938978 dtbase-0.0.4/dtbase/__init__.py
+-rw-r--r--   0        0        0     5281 2023-05-26 23:45:18.887306 dtbase-0.0.4/dtbase/config.py
+-rw-r--r--   0        0        0     6359 2023-05-30 02:16:18.130747 dtbase-0.0.4/dtbase/engine.py
+-rw-r--r--   0        0        0      352 2023-05-30 02:20:57.830457 dtbase-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      609 2023-05-30 02:21:13.006971 dtbase-0.0.4/setup.py
+-rw-r--r--   0        0        0      374 2023-05-30 02:21:13.007151 dtbase-0.0.4/PKG-INFO
```

### Comparing `dtbase-0.0.3/dtbase/config.py` & `dtbase-0.0.4/dtbase/config.py`

 * *Files identical despite different names*

### Comparing `dtbase-0.0.3/dtbase/engine.py` & `dtbase-0.0.4/dtbase/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,41 @@
-__all__ = ['DetaBase']
+__all__ = [
+		'DetaBase',
+		'JsonPrimitive',
+		'DetaData',
+		'DetaKey',
+		'ExpireAt',
+		'ExpireIn',
+		'Jsonable',
+		'JsonSequence',
+		'DetaQuery',
+		'ExistParams',
+		'SearchParam',
+]
 
+import datetime
 from typing import Union, Optional
 from deta import Deta
-from dhint.hints import *
 from .config import DetaConfig
 
 
 config = DetaConfig('.env')
 
+JsonPrimitive = Union[str, float, int, bool, None]
+DetaData = Union[dict, list, str, float, int, bool]
+DetaKey = Union[str, None]
+ExpireIn = Union[str, None]
+ExpireAt = Union[datetime.datetime, int, float, None]
+JsonSequence = list[JsonPrimitive]
+JsonDict = dict[str, Union[JsonSequence, JsonPrimitive]]
+Jsonable = Union[JsonDict, JsonSequence, JsonPrimitive]
+DetaQuery = Union[dict[str, JsonPrimitive], list[dict[str, JsonPrimitive]]]
+ExistParams = Union[list[str], str]
+SearchParam = str
+
 
 class DetaBase:
 	
 	def __init__(self, table: str, project_key: str = None):
 		self.table = table
 		self.project_key = project_key
```

### Comparing `dtbase-0.0.3/setup.py` & `dtbase-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['dtbase']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['deta[async]==1.1.0a2', 'dhint>=0.0.6,<0.0.7', 'starlette>=0.27.0,<0.28.0']
+['deta[async]==1.1.0a2', 'starlette>=0.27.0,<0.28.0']
 
 setup_kwargs = {
     'name': 'dtbase',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

