# Comparing `tmp/gtfs_kit-5.2.5.tar.gz` & `tmp/gtfs_kit-5.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtfs_kit-5.2.5.tar", max compression
+gzip compressed data, was "gtfs_kit-5.2.6.tar", max compression
```

## Comparing `gtfs_kit-5.2.5.tar` & `gtfs_kit-5.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1083 2020-01-09 20:55:35.590106 gtfs_kit-5.2.5/LICENSE.txt
--rw-r--r--   0        0        0     1937 2023-04-27 00:05:00.839952 gtfs_kit-5.2.5/README.rst
--rw-r--r--   0        0        0      304 2023-04-27 00:05:00.839952 gtfs_kit-5.2.5/gtfs_kit/__init__.py
--rw-r--r--   0        0        0     3426 2021-04-28 23:42:59.436692 gtfs_kit-5.2.5/gtfs_kit/calendar.py
--rw-r--r--   0        0        0    10692 2022-04-12 04:10:10.474482 gtfs_kit-5.2.5/gtfs_kit/cleaners.py
--rw-r--r--   0        0        0     6971 2022-01-17 03:01:47.667252 gtfs_kit-5.2.5/gtfs_kit/constants.py
--rw-r--r--   0        0        0    16515 2022-04-13 02:04:39.526021 gtfs_kit-5.2.5/gtfs_kit/feed.py
--rw-r--r--   0        0        0    19581 2021-11-25 21:52:10.388179 gtfs_kit-5.2.5/gtfs_kit/helpers.py
--rw-r--r--   0        0        0    35644 2023-04-27 00:05:00.843952 gtfs_kit-5.2.5/gtfs_kit/miscellany.py
--rw-r--r--   0        0        0    30514 2022-07-05 02:59:12.080231 gtfs_kit-5.2.5/gtfs_kit/routes.py
--rw-r--r--   0        0        0     6648 2022-07-05 02:59:12.080231 gtfs_kit-5.2.5/gtfs_kit/shapes.py
--rw-r--r--   0        0        0     6231 2022-04-13 02:04:39.526021 gtfs_kit-5.2.5/gtfs_kit/stop_times.py
--rw-r--r--   0        0        0    24935 2022-04-26 01:06:51.650776 gtfs_kit-5.2.5/gtfs_kit/stops.py
--rw-r--r--   0        0        0    21337 2021-11-25 21:52:10.392179 gtfs_kit-5.2.5/gtfs_kit/trips.py
--rw-r--r--   0        0        0    49077 2022-04-26 21:35:43.321257 gtfs_kit-5.2.5/gtfs_kit/validators.py
--rw-r--r--   0        0        0     1077 2023-04-27 00:05:00.847952 gtfs_kit-5.2.5/pyproject.toml
--rw-r--r--   0        0        0     2760 1970-01-01 00:00:00.000000 gtfs_kit-5.2.5/setup.py
--rw-r--r--   0        0        0     2924 1970-01-01 00:00:00.000000 gtfs_kit-5.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1083 2020-01-09 20:55:35.590106 gtfs_kit-5.2.6/LICENSE.txt
+-rw-r--r--   0        0        0     1937 2023-04-27 00:05:00.839952 gtfs_kit-5.2.6/README.rst
+-rw-r--r--   0        0        0      304 2023-05-30 02:41:39.895479 gtfs_kit-5.2.6/gtfs_kit/__init__.py
+-rw-r--r--   0        0        0     3426 2021-04-28 23:42:59.436692 gtfs_kit-5.2.6/gtfs_kit/calendar.py
+-rw-r--r--   0        0        0    10692 2022-04-12 04:10:10.474482 gtfs_kit-5.2.6/gtfs_kit/cleaners.py
+-rw-r--r--   0        0        0     6971 2022-01-17 03:01:47.667252 gtfs_kit-5.2.6/gtfs_kit/constants.py
+-rw-r--r--   0        0        0    16515 2022-04-13 02:04:39.526021 gtfs_kit-5.2.6/gtfs_kit/feed.py
+-rw-r--r--   0        0        0    19581 2021-11-25 21:52:10.388179 gtfs_kit-5.2.6/gtfs_kit/helpers.py
+-rw-r--r--   0        0        0    35644 2023-04-27 00:05:00.843952 gtfs_kit-5.2.6/gtfs_kit/miscellany.py
+-rw-r--r--   0        0        0    30517 2023-05-30 02:41:39.895479 gtfs_kit-5.2.6/gtfs_kit/routes.py
+-rw-r--r--   0        0        0     6648 2022-07-05 02:59:12.080231 gtfs_kit-5.2.6/gtfs_kit/shapes.py
+-rw-r--r--   0        0        0     6231 2022-04-13 02:04:39.526021 gtfs_kit-5.2.6/gtfs_kit/stop_times.py
+-rw-r--r--   0        0        0    24935 2022-04-26 01:06:51.650776 gtfs_kit-5.2.6/gtfs_kit/stops.py
+-rw-r--r--   0        0        0    21337 2021-11-25 21:52:10.392179 gtfs_kit-5.2.6/gtfs_kit/trips.py
+-rw-r--r--   0        0        0    49077 2022-04-26 21:35:43.321257 gtfs_kit-5.2.6/gtfs_kit/validators.py
+-rw-r--r--   0        0        0     1097 2023-05-30 02:41:39.899479 gtfs_kit-5.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 gtfs_kit-5.2.6/setup.py
+-rw-r--r--   0        0        0     2926 1970-01-01 00:00:00.000000 gtfs_kit-5.2.6/PKG-INFO
```

### Comparing `gtfs_kit-5.2.5/LICENSE.txt` & `gtfs_kit-5.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.5/README.rst` & `gtfs_kit-5.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.5/gtfs_kit/calendar.py` & `gtfs_kit-5.2.6/gtfs_kit/calendar.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.5/gtfs_kit/cleaners.py` & `gtfs_kit-5.2.6/gtfs_kit/cleaners.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.5/gtfs_kit/constants.py` & `gtfs_kit-5.2.6/gtfs_kit/constants.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.5/gtfs_kit/feed.py` & `gtfs_kit-5.2.6/gtfs_kit/feed.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.5/gtfs_kit/helpers.py` & `gtfs_kit-5.2.6/gtfs_kit/helpers.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.5/gtfs_kit/miscellany.py` & `gtfs_kit-5.2.6/gtfs_kit/miscellany.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.5/gtfs_kit/routes.py` & `gtfs_kit-5.2.6/gtfs_kit/routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -717,15 +717,15 @@
     if split_directions:
         groupby_cols = ["route_id", "direction_id"]
     else:
         groupby_cols = ["route_id"]
 
     def merge_lines(group):
         d = {}
-        d["geometry"] = so.linemerge(group.geometry.tolist())
+        d["geometry"] = so.linemerge(group["geometry"].tolist())
         return pd.Series(d)
 
     return (
         feed.geometrize_trips(trip_ids, use_utm=use_utm)
         .filter(["route_id", "direction_id", "geometry"])
         .groupby(groupby_cols)
         .apply(merge_lines)
```

### Comparing `gtfs_kit-5.2.5/gtfs_kit/shapes.py` & `gtfs_kit-5.2.6/gtfs_kit/shapes.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.5/gtfs_kit/stop_times.py` & `gtfs_kit-5.2.6/gtfs_kit/stop_times.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.5/gtfs_kit/stops.py` & `gtfs_kit-5.2.6/gtfs_kit/stops.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.5/gtfs_kit/trips.py` & `gtfs_kit-5.2.6/gtfs_kit/trips.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.5/gtfs_kit/validators.py` & `gtfs_kit-5.2.6/gtfs_kit/validators.py`

 * *Files identical despite different names*

### Comparing `gtfs_kit-5.2.5/pyproject.toml` & `gtfs_kit-5.2.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "gtfs_kit"
-version = "5.2.5"
+version = "5.2.6"
 description = "A Python 3.8+ library for analyzing GTFS feeds."
 authors = ["Alex Raichev <araichev@mrcagney.com>"]
 readme = "README.rst"
 license = "MIT"
 repository = "https://github.com/mrcagney/gtfs_kit"
 documentation = "https://mrcagney.github.io/gtfs_kit_docs"
 exclude = ["tests", "docs"]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4"
 pandas = ">=1"
 shapely = ">=1.8"
 pycountry = ">=19"
-utm = ">=0"
+utm = ">=0.6"
 json2html = ">=1"
 geopandas = ">=0"
 rtree = ">=0"
 folium = ">=0"
 requests = ">=2"
 
 [tool.poetry.group.dev.dependencies]
-jupyter = "*"
+jupyter = ">=1"
 pytest = ">=6"
 sphinx = ">=3"
 pre-commit = ">=0"
 matplotlib = ">=1"
 pytest-socket = ">=0"
 black = ">22"
 nbstripout = ">=0.5"
@@ -42,8 +42,8 @@
     "slow: marks tests as slow (deselect with '-m \"not slow\"')",
     "serial",
 ]
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
 select = ["E", "F"]
-ignore = ["F403"]
+ignore = ["E501", "F401", "F403"]
```

### Comparing `gtfs_kit-5.2.5/setup.py` & `gtfs_kit-5.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
  'geopandas>=0',
  'json2html>=1',
  'pandas>=1',
  'pycountry>=19',
  'requests>=2',
  'rtree>=0',
  'shapely>=1.8',
- 'utm>=0']
+ 'utm>=0.6']
 
 setup_kwargs = {
     'name': 'gtfs-kit',
-    'version': '5.2.5',
+    'version': '5.2.6',
     'description': 'A Python 3.8+ library for analyzing GTFS feeds.',
     'long_description': "GTFS Kit\n********\n.. image:: https://github.com/mrcagney/gtfs_kit/actions/workflows/test.yml/badge.svg\n\nGTFS Kit is a Python 3.8+ library for analyzing `General Transit Feed Specification (GTFS) <https://en.wikipedia.org/wiki/GTFS>`_ data in memory without a database.\nIt uses Pandas and Shapely to do the heavy lifting.\n\n\nInstallation\n=============\n``poetry add gtfs_kit``.\n\n\nExamples\n========\nYou can find examples in the Jupyter notebook ``notebooks/examples.ipynb``.\n\n\nAuthors\n=========\n- Alex Raichev (2019-09), maintainer\n\n\nDocumentation\n=============\nDocumentation is built via Sphinx from the source code in the ``docs`` directory then published to Github Pages at `mrcagney.github.io/gtfs_kit_docs <https://mrcagney.github.io/gtfs_kit_docs>`_.\n\n\nNotes\n=====\n- This project's development status is Alpha.\n  I use GTFS Kit for work and change it breakingly to suit my needs.\n- This project uses semantic versioning.\n- I aim for GTFS Kit to handle `the current GTFS <https://developers.google.com/transit/gtfs/reference>`_.\n  In particular, i avoid handling `GTFS extensions <https://developers.google.com/transit/gtfs/reference/gtfs-extensions>`_.\n  That is the most reasonable scope boundary i can draw at present, given this project's tiny budget.\n  If you would like to fund me to expand that scope, feel free to email me.\n- Thanks to `MRCagney <http://www.mrcagney.com/>`_ for periodically donating to this project.\n- Constructive feedback and contributions are welcome.\n  Please issue pull requests from a feature branch into the ``develop`` branch and include tests.\n- GTFS time is measured relative noon minus 12 hours, which can mess things up when crossing into daylight savings time.\n  I don't think this issue causes any bugs in GTFS Kit, but you and i have been warned.\n  Thanks to user derhuerst for bringing this to my attention in `closed Issue 8 <https://github.com/mrcagney/gtfs_kit/issues/8#issue-1063633457>`_.\n",
     'author': 'Alex Raichev',
     'author_email': 'araichev@mrcagney.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mrcagney/gtfs_kit',
```

### Comparing `gtfs_kit-5.2.5/PKG-INFO` & `gtfs_kit-5.2.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtfs-kit
-Version: 5.2.5
+Version: 5.2.6
 Summary: A Python 3.8+ library for analyzing GTFS feeds.
 Home-page: https://github.com/mrcagney/gtfs_kit
 License: MIT
 Author: Alex Raichev
 Author-email: araichev@mrcagney.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,15 @@
 Requires-Dist: geopandas (>=0)
 Requires-Dist: json2html (>=1)
 Requires-Dist: pandas (>=1)
 Requires-Dist: pycountry (>=19)
 Requires-Dist: requests (>=2)
 Requires-Dist: rtree (>=0)
 Requires-Dist: shapely (>=1.8)
-Requires-Dist: utm (>=0)
+Requires-Dist: utm (>=0.6)
 Project-URL: Documentation, https://mrcagney.github.io/gtfs_kit_docs
 Project-URL: Repository, https://github.com/mrcagney/gtfs_kit
 Description-Content-Type: text/x-rst
 
 GTFS Kit
 ********
 .. image:: https://github.com/mrcagney/gtfs_kit/actions/workflows/test.yml/badge.svg
```

