# Comparing `tmp/proton-db-0.1.3.tar.gz` & `tmp/proton-db-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proton-db-0.1.3.tar", max compression
+gzip compressed data, was "proton-db-0.1.4.tar", max compression
```

## Comparing `proton-db-0.1.3.tar` & `proton-db-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      577 2023-05-30 20:03:17.025198 proton-db-0.1.3/README.rst
--rw-r--r--   0        0        0     1593 2023-05-30 20:08:14.248782 proton-db-0.1.3/proton_db/__init__.py
--rw-r--r--   0        0        0      347 2023-05-30 20:08:10.904787 proton-db-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1127 2023-05-30 20:08:21.285067 proton-db-0.1.3/setup.py
--rw-r--r--   0        0        0      873 2023-05-30 20:08:21.285457 proton-db-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      580 2023-05-30 20:15:17.164191 proton-db-0.1.4/README.rst
+-rw-r--r--   0        0        0     1593 2023-05-30 20:10:09.720621 proton-db-0.1.4/proton_db/__init__.py
+-rw-r--r--   0        0        0      347 2023-05-30 20:10:07.956623 proton-db-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1133 2023-05-30 20:15:25.956476 proton-db-0.1.4/setup.py
+-rw-r--r--   0        0        0      876 2023-05-30 20:15:25.956872 proton-db-0.1.4/PKG-INFO
```

### Comparing `proton-db-0.1.3/README.rst` & `proton-db-0.1.4/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -19,8 +19,10 @@
 appId - The game ID for this report. Redundant for uniformity's sake.
 timestamp
 rating
 notes
 os
 gpuDriver
 specs
-protonVersion
+protonVersion
+
+
```

### Comparing `proton-db-0.1.3/proton_db/__init__.py` & `proton-db-0.1.4/proton_db/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 
 import requests, json
 #Api provided by https://protondb.max-p.me/
 class protonDB():
   def __init__(self,cache=True):
     self.api = "https://protondb.max-p.me/"
     self.cachingEnabled = cache
```

### Comparing `proton-db-0.1.3/setup.py` & `proton-db-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['proton_db']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'proton-db',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'A simple wrapper for the unofficial Proton-DB API.',
-    'long_description': "Lightweight wrapper for the unofficial Proton-DB API (https://protondb.max-p.me/)\n\nUsage:\nimport proton_db as proton\n\nprotonDB = proton.protonDB()\n\n\ngetGames()\nLists all the games we have discovered so far. Returns an array of objects with these fields in it:\n\nappId\ntitle\n\ngetReports(appId)\nLists all reports for a given game (by Valve's appId), in reverse timestamp order. Returns an array of objects with these fields in it:\n\nid - Server's local id\nappId - The game ID for this report. Redundant for uniformity's sake.\ntimestamp\nrating\nnotes\nos\ngpuDriver\nspecs\nprotonVersion",
+    'long_description': "Lightweight wrapper for the unofficial Proton-DB API (https://protondb.max-p.me/)\n\nUsage:\nimport proton_db as proton\n\nprotonDB = proton.protonDB()\n\n\ngetGames()\nLists all the games we have discovered so far. Returns an array of objects with these fields in it:\n\nappId\ntitle\n\ngetReports(appId)\nLists all reports for a given game (by Valve's appId), in reverse timestamp order. Returns an array of objects with these fields in it:\n\nid - Server's local id\nappId - The game ID for this report. Redundant for uniformity's sake.\ntimestamp\nrating\nnotes\nos\ngpuDriver\nspecs\nprotonVersion\n\n\n",
     'author': 'BiFr0st',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `proton-db-0.1.3/PKG-INFO` & `proton-db-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proton-db
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple wrapper for the unofficial Proton-DB API.
 Author: BiFr0st
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 
@@ -30,7 +30,10 @@
 timestamp
 rating
 notes
 os
 gpuDriver
 specs
 protonVersion
+
+
+
```

