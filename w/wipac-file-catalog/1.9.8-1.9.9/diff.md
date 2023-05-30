# Comparing `tmp/wipac-file-catalog-1.9.8.tar.gz` & `tmp/wipac-file-catalog-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wipac-file-catalog-1.9.8.tar", last modified: Tue May 30 14:15:46 2023, max compression
+gzip compressed data, was "wipac-file-catalog-1.9.9.tar", last modified: Tue May 30 15:01:24 2023, max compression
```

## Comparing `wipac-file-catalog-1.9.8.tar` & `wipac-file-catalog-1.9.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:15:46.597885 wipac-file-catalog-1.9.8/
--rw-r--r--   0 root         (0) root         (0)     1080 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)    12047 2023-05-30 14:15:46.597885 wipac-file-catalog-1.9.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11079 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:15:46.597885 wipac-file-catalog-1.9.8/file_catalog/
--rw-r--r--   0 root         (0) root         (0)      570 2023-05-30 14:15:44.000000 wipac-file-catalog-1.9.8/file_catalog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2325 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/file_catalog/__main__.py
--rw-r--r--   0 root         (0) root         (0)     3373 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/file_catalog/argbuilder.py
--rw-r--r--   0 root         (0) root         (0)     2602 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/file_catalog/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:15:46.593885 wipac-file-catalog-1.9.8/file_catalog/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:15:46.597885 wipac-file-catalog-1.9.8/file_catalog/data/www/
--rw-r--r--   0 root         (0) root         (0)      345 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/file_catalog/data/www/base.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:15:46.597885 wipac-file-catalog-1.9.8/file_catalog/data/www_templates/
--rw-r--r--   0 root         (0) root         (0)      443 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/file_catalog/data/www_templates/account.html
--rw-r--r--   0 root         (0) root         (0)     1948 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/file_catalog/data/www_templates/base.html
--rw-r--r--   0 root         (0) root         (0)      129 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/file_catalog/data/www_templates/index.html
--rw-r--r--   0 root         (0) root         (0)      747 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/file_catalog/data/www_templates/login.html
--rw-r--r--   0 root         (0) root         (0)     4063 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/file_catalog/deconfliction.py
--rw-r--r--   0 root         (0) root         (0)    13560 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/file_catalog/mongo.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/file_catalog/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:15:46.597885 wipac-file-catalog-1.9.8/file_catalog/schema/
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/file_catalog/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4145 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/file_catalog/schema/types.py
--rw-r--r--   0 root         (0) root         (0)     6388 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/file_catalog/schema/validation.py
--rw-r--r--   0 root         (0) root         (0)    35370 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/file_catalog/server.py
--rw-r--r--   0 root         (0) root         (0)     8639 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/file_catalog/urlargparse.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/file_catalog/utils.py
--rw-r--r--   0 root         (0) root         (0)     2138 2023-05-30 14:15:46.601884 wipac-file-catalog-1.9.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       99 2023-05-30 14:15:43.000000 wipac-file-catalog-1.9.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:15:46.597885 wipac-file-catalog-1.9.8/wipac_file_catalog.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12047 2023-05-30 14:15:46.000000 wipac-file-catalog-1.9.8/wipac_file_catalog.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      791 2023-05-30 14:15:46.000000 wipac-file-catalog-1.9.8/wipac_file_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 14:15:46.000000 wipac-file-catalog-1.9.8/wipac_file_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      247 2023-05-30 14:15:46.000000 wipac-file-catalog-1.9.8/wipac_file_catalog.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 14:15:46.000000 wipac-file-catalog-1.9.8/wipac_file_catalog.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:01:24.921260 wipac-file-catalog-1.9.9/
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    12047 2023-05-30 15:01:24.921260 wipac-file-catalog-1.9.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11079 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:01:24.921260 wipac-file-catalog-1.9.9/file_catalog/
+-rw-r--r--   0 root         (0) root         (0)      570 2023-05-30 15:01:22.000000 wipac-file-catalog-1.9.9/file_catalog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2325 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/file_catalog/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     3373 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/file_catalog/argbuilder.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/file_catalog/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:01:24.917260 wipac-file-catalog-1.9.9/file_catalog/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:01:24.921260 wipac-file-catalog-1.9.9/file_catalog/data/www/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/file_catalog/data/www/base.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:01:24.921260 wipac-file-catalog-1.9.9/file_catalog/data/www_templates/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/file_catalog/data/www_templates/account.html
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/file_catalog/data/www_templates/base.html
+-rw-r--r--   0 root         (0) root         (0)      129 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/file_catalog/data/www_templates/index.html
+-rw-r--r--   0 root         (0) root         (0)      747 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/file_catalog/data/www_templates/login.html
+-rw-r--r--   0 root         (0) root         (0)     4063 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/file_catalog/deconfliction.py
+-rw-r--r--   0 root         (0) root         (0)    13560 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/file_catalog/mongo.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/file_catalog/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:01:24.921260 wipac-file-catalog-1.9.9/file_catalog/schema/
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/file_catalog/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4145 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/file_catalog/schema/types.py
+-rw-r--r--   0 root         (0) root         (0)     6388 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/file_catalog/schema/validation.py
+-rw-r--r--   0 root         (0) root         (0)    35370 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/file_catalog/server.py
+-rw-r--r--   0 root         (0) root         (0)     8639 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/file_catalog/urlargparse.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/file_catalog/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2023-05-30 15:01:24.925260 wipac-file-catalog-1.9.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       99 2023-05-30 15:01:21.000000 wipac-file-catalog-1.9.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:01:24.921260 wipac-file-catalog-1.9.9/wipac_file_catalog.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12047 2023-05-30 15:01:24.000000 wipac-file-catalog-1.9.9/wipac_file_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      791 2023-05-30 15:01:24.000000 wipac-file-catalog-1.9.9/wipac_file_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 15:01:24.000000 wipac-file-catalog-1.9.9/wipac_file_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      247 2023-05-30 15:01:24.000000 wipac-file-catalog-1.9.9/wipac_file_catalog.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 15:01:24.000000 wipac-file-catalog-1.9.9/wipac_file_catalog.egg-info/top_level.txt
```

### Comparing `wipac-file-catalog-1.9.8/LICENSE` & `wipac-file-catalog-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-1.9.8/PKG-INFO` & `wipac-file-catalog-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-file-catalog
-Version: 1.9.8
+Version: 1.9.9
 Summary: Store file metadata information in a file catalog
 Home-page: https://github.com/WIPACrepo/file_catalog
 Download-URL: https://pypi.org/project/wipac-file-catalog/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/file_catalog/issues
```

### Comparing `wipac-file-catalog-1.9.8/README.md` & `wipac-file-catalog-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-1.9.8/file_catalog/__init__.py` & `wipac-file-catalog-1.9.9/file_catalog/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.9.8"
+__version__ = "1.9.9"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `wipac-file-catalog-1.9.8/file_catalog/__main__.py` & `wipac-file-catalog-1.9.9/file_catalog/__main__.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-1.9.8/file_catalog/argbuilder.py` & `wipac-file-catalog-1.9.9/file_catalog/argbuilder.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-1.9.8/file_catalog/config.py` & `wipac-file-catalog-1.9.9/file_catalog/config.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-1.9.8/file_catalog/data/www_templates/base.html` & `wipac-file-catalog-1.9.9/file_catalog/data/www_templates/base.html`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-1.9.8/file_catalog/data/www_templates/login.html` & `wipac-file-catalog-1.9.9/file_catalog/data/www_templates/login.html`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-1.9.8/file_catalog/deconfliction.py` & `wipac-file-catalog-1.9.9/file_catalog/deconfliction.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-1.9.8/file_catalog/mongo.py` & `wipac-file-catalog-1.9.9/file_catalog/mongo.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-1.9.8/file_catalog/schema/types.py` & `wipac-file-catalog-1.9.9/file_catalog/schema/types.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-1.9.8/file_catalog/schema/validation.py` & `wipac-file-catalog-1.9.9/file_catalog/schema/validation.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-1.9.8/file_catalog/server.py` & `wipac-file-catalog-1.9.9/file_catalog/server.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-1.9.8/file_catalog/urlargparse.py` & `wipac-file-catalog-1.9.9/file_catalog/urlargparse.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-1.9.8/file_catalog/utils.py` & `wipac-file-catalog-1.9.9/file_catalog/utils.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-1.9.8/setup.cfg` & `wipac-file-catalog-1.9.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-1.9.8/wipac_file_catalog.egg-info/PKG-INFO` & `wipac-file-catalog-1.9.9/wipac_file_catalog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-file-catalog
-Version: 1.9.8
+Version: 1.9.9
 Summary: Store file metadata information in a file catalog
 Home-page: https://github.com/WIPACrepo/file_catalog
 Download-URL: https://pypi.org/project/wipac-file-catalog/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/file_catalog/issues
```

### Comparing `wipac-file-catalog-1.9.8/wipac_file_catalog.egg-info/SOURCES.txt` & `wipac-file-catalog-1.9.9/wipac_file_catalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

