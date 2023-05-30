# Comparing `tmp/proton-db-0.1.4.tar.gz` & `tmp/proton-db-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proton-db-0.1.4.tar", max compression
+gzip compressed data, was "proton-db-0.1.5.tar", max compression
```

## Comparing `proton-db-0.1.4.tar` & `proton-db-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      580 2023-05-30 20:15:17.164191 proton-db-0.1.4/README.rst
--rw-r--r--   0        0        0     1593 2023-05-30 20:10:09.720621 proton-db-0.1.4/proton_db/__init__.py
--rw-r--r--   0        0        0      347 2023-05-30 20:10:07.956623 proton-db-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1133 2023-05-30 20:15:25.956476 proton-db-0.1.4/setup.py
--rw-r--r--   0        0        0      876 2023-05-30 20:15:25.956872 proton-db-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      597 2023-05-30 20:16:25.420095 proton-db-0.1.5/README.rst
+-rw-r--r--   0        0        0     1593 2023-05-30 20:16:46.336066 proton-db-0.1.5/proton_db/__init__.py
+-rw-r--r--   0        0        0      347 2023-05-30 20:16:35.168081 proton-db-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1167 2023-05-30 20:16:51.451901 proton-db-0.1.5/setup.py
+-rw-r--r--   0        0        0      893 2023-05-30 20:16:51.452253 proton-db-0.1.5/PKG-INFO
```

### Comparing `proton-db-0.1.4/README.rst` & `proton-db-0.1.5/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,45 @@
 Lightweight wrapper for the unofficial Proton-DB API (https://protondb.max-p.me/)
 
+
 Usage:
+
 import proton_db as proton
 
+
 protonDB = proton.protonDB()
 
 
+
 getGames()
 Lists all the games we have discovered so far. Returns an array of objects with these fields in it:
 
+
 appId
+
 title
 
+
+
 getReports(appId)
 Lists all reports for a given game (by Valve's appId), in reverse timestamp order. Returns an array of objects with these fields in it:
 
+
 id - Server's local id
+
 appId - The game ID for this report. Redundant for uniformity's sake.
+
 timestamp
+
 rating
+
 notes
+
 os
+
 gpuDriver
+
 specs
+
 protonVersion
```

### Comparing `proton-db-0.1.4/proton_db/__init__.py` & `proton-db-0.1.5/proton_db/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 
 import requests, json
 #Api provided by https://protondb.max-p.me/
 class protonDB():
   def __init__(self,cache=True):
     self.api = "https://protondb.max-p.me/"
     self.cachingEnabled = cache
```

### Comparing `proton-db-0.1.4/setup.py` & `proton-db-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['proton_db']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'proton-db',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'A simple wrapper for the unofficial Proton-DB API.',
-    'long_description': "Lightweight wrapper for the unofficial Proton-DB API (https://protondb.max-p.me/)\n\nUsage:\nimport proton_db as proton\n\nprotonDB = proton.protonDB()\n\n\ngetGames()\nLists all the games we have discovered so far. Returns an array of objects with these fields in it:\n\nappId\ntitle\n\ngetReports(appId)\nLists all reports for a given game (by Valve's appId), in reverse timestamp order. Returns an array of objects with these fields in it:\n\nid - Server's local id\nappId - The game ID for this report. Redundant for uniformity's sake.\ntimestamp\nrating\nnotes\nos\ngpuDriver\nspecs\nprotonVersion\n\n\n",
+    'long_description': "Lightweight wrapper for the unofficial Proton-DB API (https://protondb.max-p.me/)\n\n\nUsage:\n\nimport proton_db as proton\n\n\nprotonDB = proton.protonDB()\n\n\n\ngetGames()\nLists all the games we have discovered so far. Returns an array of objects with these fields in it:\n\n\nappId\n\ntitle\n\n\n\ngetReports(appId)\nLists all reports for a given game (by Valve's appId), in reverse timestamp order. Returns an array of objects with these fields in it:\n\n\nid - Server's local id\n\nappId - The game ID for this report. Redundant for uniformity's sake.\n\ntimestamp\n\nrating\n\nnotes\n\nos\n\ngpuDriver\n\nspecs\n\nprotonVersion\n\n\n",
     'author': 'BiFr0st',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `proton-db-0.1.4/PKG-INFO` & `proton-db-0.1.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,56 @@
 Metadata-Version: 2.1
 Name: proton-db
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple wrapper for the unofficial Proton-DB API.
 Author: BiFr0st
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 
 Lightweight wrapper for the unofficial Proton-DB API (https://protondb.max-p.me/)
 
+
 Usage:
+
 import proton_db as proton
 
+
 protonDB = proton.protonDB()
 
 
+
 getGames()
 Lists all the games we have discovered so far. Returns an array of objects with these fields in it:
 
+
 appId
+
 title
 
+
+
 getReports(appId)
 Lists all reports for a given game (by Valve's appId), in reverse timestamp order. Returns an array of objects with these fields in it:
 
+
 id - Server's local id
+
 appId - The game ID for this report. Redundant for uniformity's sake.
+
 timestamp
+
 rating
+
 notes
+
 os
+
 gpuDriver
+
 specs
+
 protonVersion
```

