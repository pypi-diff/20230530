# Comparing `tmp/fdserver-23.2.7.1.tar.gz` & `tmp/fdserver-23.5.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdserver-23.2.7.1.tar", last modified: Tue Feb  7 19:30:17 2023, max compression
+gzip compressed data, was "fdserver-23.5.30.tar", last modified: Tue May 30 16:10:27 2023, max compression
```

## Comparing `fdserver-23.2.7.1.tar` & `fdserver-23.5.30.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-02-07 19:30:17.686375 fdserver-23.2.7.1/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7652 2022-06-28 19:46:07.000000 fdserver-23.2.7.1/LICENSE.md
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4267 2023-02-07 19:30:17.685375 fdserver-23.2.7.1/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3486 2023-02-01 20:54:55.000000 fdserver-23.2.7.1/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-02-07 19:30:17.683375 fdserver-23.2.7.1/fdserver/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-12-28 15:00:34.000000 fdserver-23.2.7.1/fdserver/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    33920 2023-02-07 19:28:09.000000 fdserver-23.2.7.1/fdserver/__main__.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-02-07 19:30:17.684375 fdserver-23.2.7.1/fdserver/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5445 2023-02-01 20:40:07.000000 fdserver-23.2.7.1/fdserver/data/k6gte-fdserver-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1271 2023-02-01 20:38:54.000000 fdserver-23.2.7.1/fdserver/data/k6gte-fdserver-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2649 2023-02-01 20:39:12.000000 fdserver-23.2.7.1/fdserver/data/k6gte-fdserver-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      302 2023-02-01 20:41:35.000000 fdserver-23.2.7.1/fdserver/data/k6gte-fdserver.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13503 2023-02-01 20:40:13.000000 fdserver-23.2.7.1/fdserver/data/k6gte.fdserver.svg
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1216 2023-02-06 19:43:18.000000 fdserver-23.2.7.1/fdserver/data/server_preferences.json
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-02-07 19:30:17.685375 fdserver-23.2.7.1/fdserver/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-12-28 15:01:16.000000 fdserver-23.2.7.1/fdserver/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11955 2023-02-01 14:55:26.000000 fdserver-23.2.7.1/fdserver/lib/server_database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       48 2023-02-07 19:28:44.000000 fdserver-23.2.7.1/fdserver/lib/version.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1289 2022-12-28 03:38:12.000000 fdserver-23.2.7.1/fdserver/lib/versiontest.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-02-07 19:30:17.684375 fdserver-23.2.7.1/fdserver.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4267 2023-02-07 19:30:17.000000 fdserver-23.2.7.1/fdserver.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      566 2023-02-07 19:30:17.000000 fdserver-23.2.7.1/fdserver.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-02-07 19:30:17.000000 fdserver-23.2.7.1/fdserver.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-02-07 19:30:17.000000 fdserver-23.2.7.1/fdserver.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       19 2023-02-07 19:30:17.000000 fdserver-23.2.7.1/fdserver.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1001 2023-02-07 19:29:22.000000 fdserver-23.2.7.1/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-02-07 19:30:17.686375 fdserver-23.2.7.1/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-30 16:10:27.029061 fdserver-23.5.30/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7652 2022-06-28 19:46:07.000000 fdserver-23.5.30/LICENSE.md
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4186 2023-05-30 16:10:27.028061 fdserver-23.5.30/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3406 2023-05-30 16:06:27.000000 fdserver-23.5.30/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-30 16:10:27.026061 fdserver-23.5.30/fdserver/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-12-28 15:00:34.000000 fdserver-23.5.30/fdserver/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    33920 2023-02-07 19:28:09.000000 fdserver-23.5.30/fdserver/__main__.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-30 16:10:27.028061 fdserver-23.5.30/fdserver/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5445 2023-02-01 20:40:07.000000 fdserver-23.5.30/fdserver/data/k6gte-fdserver-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1271 2023-02-01 20:38:54.000000 fdserver-23.5.30/fdserver/data/k6gte-fdserver-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2649 2023-02-01 20:39:12.000000 fdserver-23.5.30/fdserver/data/k6gte-fdserver-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      302 2023-02-01 20:41:35.000000 fdserver-23.5.30/fdserver/data/k6gte-fdserver.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13503 2023-02-01 20:40:13.000000 fdserver-23.5.30/fdserver/data/k6gte.fdserver.svg
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1216 2023-05-30 16:06:27.000000 fdserver-23.5.30/fdserver/data/server_preferences.json
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-30 16:10:27.028061 fdserver-23.5.30/fdserver/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-12-28 15:01:16.000000 fdserver-23.5.30/fdserver/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11955 2023-02-01 14:55:26.000000 fdserver-23.5.30/fdserver/lib/server_database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-30 16:06:27.000000 fdserver-23.5.30/fdserver/lib/version.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1289 2022-12-28 03:38:12.000000 fdserver-23.5.30/fdserver/lib/versiontest.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-30 16:10:27.027061 fdserver-23.5.30/fdserver.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4186 2023-05-30 16:10:27.000000 fdserver-23.5.30/fdserver.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      566 2023-05-30 16:10:27.000000 fdserver-23.5.30/fdserver.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-30 16:10:27.000000 fdserver-23.5.30/fdserver.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-05-30 16:10:27.000000 fdserver-23.5.30/fdserver.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       19 2023-05-30 16:10:27.000000 fdserver-23.5.30/fdserver.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1000 2023-05-30 16:06:27.000000 fdserver-23.5.30/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-30 16:10:27.029061 fdserver-23.5.30/setup.cfg
```

### Comparing `fdserver-23.2.7.1/LICENSE.md` & `fdserver-23.5.30/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fdserver-23.2.7.1/PKG-INFO` & `fdserver-23.5.30/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdserver
-Version: 23.2.7.1
+Version: 23.5.30
 Summary: Field Day group logging server
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/fdserver
 Project-URL: Bug Tracker, https://github.com/mbridak/fdserver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,20 +15,20 @@
 Classifier: Topic :: Communications :: Ham Radio
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Field Day log aggregating server
 
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg?style=for-the-badge)](https://www.gnu.org/licenses/gpl-3.0)
-[![Python: 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg?logo=python&style=for-the-badge)](https://www.python.org/downloads/)
-![Made With: Ancient Technology](https://img.shields.io/badge/Made%20with-Ancient%20technology-red?style=for-the-badge)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/fdserver?label=PYPI-Downloads&logo=pypi&style=for-the-badge)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![Python: 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg?logo=python)](https://www.python.org/downloads/)
+![Made With: Ancient Technology](https://img.shields.io/badge/Made%20with-Ancient%20technology-red)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/fdserver?label=PYPI-Downloads&logo=pypi)
 
-![logo](https://github.com/mbridak/fdserver/raw/master/fdserver/data/k6gte.fdserver-128.png)
+![logo](https://github.com/mbridak/fdserver/raw/master/fdserver/data/k6gte-fdserver-128.png)
 
 ## TOC
 
 - [Field Day log aggregating server](#field-day-log-aggregating-server)
   - [TOC](#toc)
   - [What is it](#what-is-it)
   - [No really what is it](#no-really-what-is-it)
@@ -112,15 +112,15 @@
     "name": "Hiram Maxim",
     "address": "225 Main Street",
     "city": "Newington",
     "state": "CT",
     "postalcode": "06111",
     "country": "USA",
     "email": "Hiram.Maxim@arrl.net",
-    "mullticast_group": "224.1.1.1",
+    "mullticast_group": "239.1.1.1",
     "multicast_port": 2239,
     "interface_ip": "0.0.0.0",
     "node_red_server_ip": "127.0.0.1",
     "node_red_server_port": 12062
 }
 ```
```

### Comparing `fdserver-23.2.7.1/README.md` & `fdserver-23.5.30/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Field Day log aggregating server
 
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg?style=for-the-badge)](https://www.gnu.org/licenses/gpl-3.0)
-[![Python: 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg?logo=python&style=for-the-badge)](https://www.python.org/downloads/)
-![Made With: Ancient Technology](https://img.shields.io/badge/Made%20with-Ancient%20technology-red?style=for-the-badge)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/fdserver?label=PYPI-Downloads&logo=pypi&style=for-the-badge)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![Python: 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg?logo=python)](https://www.python.org/downloads/)
+![Made With: Ancient Technology](https://img.shields.io/badge/Made%20with-Ancient%20technology-red)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/fdserver?label=PYPI-Downloads&logo=pypi)
 
-![logo](https://github.com/mbridak/fdserver/raw/master/fdserver/data/k6gte.fdserver-128.png)
+![logo](https://github.com/mbridak/fdserver/raw/master/fdserver/data/k6gte-fdserver-128.png)
 
 ## TOC
 
 - [Field Day log aggregating server](#field-day-log-aggregating-server)
   - [TOC](#toc)
   - [What is it](#what-is-it)
   - [No really what is it](#no-really-what-is-it)
@@ -93,15 +93,15 @@
     "name": "Hiram Maxim",
     "address": "225 Main Street",
     "city": "Newington",
     "state": "CT",
     "postalcode": "06111",
     "country": "USA",
     "email": "Hiram.Maxim@arrl.net",
-    "mullticast_group": "224.1.1.1",
+    "mullticast_group": "239.1.1.1",
     "multicast_port": 2239,
     "interface_ip": "0.0.0.0",
     "node_red_server_ip": "127.0.0.1",
     "node_red_server_port": 12062
 }
 ```
```

### Comparing `fdserver-23.2.7.1/fdserver/__main__.py` & `fdserver-23.5.30/fdserver/__main__.py`

 * *Files identical despite different names*

### Comparing `fdserver-23.2.7.1/fdserver/data/k6gte-fdserver-128.png` & `fdserver-23.5.30/fdserver/data/k6gte-fdserver-128.png`

 * *Files identical despite different names*

### Comparing `fdserver-23.2.7.1/fdserver/data/k6gte-fdserver-32.png` & `fdserver-23.5.30/fdserver/data/k6gte-fdserver-32.png`

 * *Files identical despite different names*

### Comparing `fdserver-23.2.7.1/fdserver/data/k6gte-fdserver-64.png` & `fdserver-23.5.30/fdserver/data/k6gte-fdserver-64.png`

 * *Files identical despite different names*

### Comparing `fdserver-23.2.7.1/fdserver/data/k6gte.fdserver.svg` & `fdserver-23.5.30/fdserver/data/k6gte.fdserver.svg`

 * *Files identical despite different names*

### Comparing `fdserver-23.2.7.1/fdserver/data/server_preferences.json` & `fdserver-23.5.30/fdserver/data/server_preferences.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'mullticast_group'": "'239.1.1.1'"}*

```diff
@@ -29,15 +29,15 @@
         }
     },
     "city": "Newington",
     "clubname": "Insert your club name here.",
     "country": "USA",
     "email": "Hiram.Maxim@arrl.net",
     "interface_ip": "0.0.0.0",
-    "mullticast_group": "224.1.1.1",
+    "mullticast_group": "239.1.1.1",
     "multicast_port": 2239,
     "name": "Hiram Maxim",
     "node_red_server_ip": "127.0.0.1",
     "node_red_server_port": 12062,
     "ourcall": "W1AW",
     "ourclass": "3A",
     "oursection": "ORG",
```

### Comparing `fdserver-23.2.7.1/fdserver/lib/server_database.py` & `fdserver-23.5.30/fdserver/lib/server_database.py`

 * *Files identical despite different names*

### Comparing `fdserver-23.2.7.1/fdserver/lib/versiontest.py` & `fdserver-23.5.30/fdserver/lib/versiontest.py`

 * *Files identical despite different names*

### Comparing `fdserver-23.2.7.1/fdserver.egg-info/PKG-INFO` & `fdserver-23.5.30/fdserver.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdserver
-Version: 23.2.7.1
+Version: 23.5.30
 Summary: Field Day group logging server
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/fdserver
 Project-URL: Bug Tracker, https://github.com/mbridak/fdserver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,20 +15,20 @@
 Classifier: Topic :: Communications :: Ham Radio
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Field Day log aggregating server
 
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg?style=for-the-badge)](https://www.gnu.org/licenses/gpl-3.0)
-[![Python: 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg?logo=python&style=for-the-badge)](https://www.python.org/downloads/)
-![Made With: Ancient Technology](https://img.shields.io/badge/Made%20with-Ancient%20technology-red?style=for-the-badge)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/fdserver?label=PYPI-Downloads&logo=pypi&style=for-the-badge)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![Python: 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg?logo=python)](https://www.python.org/downloads/)
+![Made With: Ancient Technology](https://img.shields.io/badge/Made%20with-Ancient%20technology-red)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/fdserver?label=PYPI-Downloads&logo=pypi)
 
-![logo](https://github.com/mbridak/fdserver/raw/master/fdserver/data/k6gte.fdserver-128.png)
+![logo](https://github.com/mbridak/fdserver/raw/master/fdserver/data/k6gte-fdserver-128.png)
 
 ## TOC
 
 - [Field Day log aggregating server](#field-day-log-aggregating-server)
   - [TOC](#toc)
   - [What is it](#what-is-it)
   - [No really what is it](#no-really-what-is-it)
@@ -112,15 +112,15 @@
     "name": "Hiram Maxim",
     "address": "225 Main Street",
     "city": "Newington",
     "state": "CT",
     "postalcode": "06111",
     "country": "USA",
     "email": "Hiram.Maxim@arrl.net",
-    "mullticast_group": "224.1.1.1",
+    "mullticast_group": "239.1.1.1",
     "multicast_port": 2239,
     "interface_ip": "0.0.0.0",
     "node_red_server_ip": "127.0.0.1",
     "node_red_server_port": 12062
 }
 ```
```

### Comparing `fdserver-23.2.7.1/fdserver.egg-info/SOURCES.txt` & `fdserver-23.5.30/fdserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fdserver-23.2.7.1/pyproject.toml` & `fdserver-23.5.30/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fdserver" 
-version = "23.2.7.1"
+version = "23.5.30"
 description = "Field Day group logging server"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

