# Comparing `tmp/mbox2m365-3.0.6.tar.gz` & `tmp/mbox2m365-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbox2m365-3.0.6.tar", last modified: Thu Mar 30 20:04:30 2023, max compression
+gzip compressed data, was "mbox2m365-3.0.8.tar", last modified: Thu Mar 30 20:07:13 2023, max compression
```

## Comparing `mbox2m365-3.0.6.tar` & `mbox2m365-3.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-03-30 20:04:30.771833 mbox2m365-3.0.6/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11456 2023-03-30 20:04:30.771833 mbox2m365-3.0.6/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11135 2023-03-30 19:52:19.000000 mbox2m365-3.0.6/README.rst
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-03-30 20:04:30.770833 mbox2m365-3.0.6/jobber/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     5167 2022-09-19 13:44:42.000000 mbox2m365-3.0.6/jobber/jobber.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-03-30 20:04:30.770833 mbox2m365-3.0.6/mbox2m365/
--rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)      268 2022-09-19 20:24:22.000000 mbox2m365-3.0.6/mbox2m365/__init__.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11546 2022-09-20 13:57:52.000000 mbox2m365-3.0.6/mbox2m365/__main__.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    30539 2023-03-30 19:26:06.000000 mbox2m365-3.0.6/mbox2m365/mbox2m365.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-03-30 20:04:30.771833 mbox2m365-3.0.6/mbox2m365.egg-info/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11456 2023-03-30 20:04:30.000000 mbox2m365-3.0.6/mbox2m365.egg-info/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      328 2023-03-30 20:04:30.000000 mbox2m365-3.0.6/mbox2m365.egg-info/SOURCES.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2023-03-30 20:04:30.000000 mbox2m365-3.0.6/mbox2m365.egg-info/dependency_links.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       54 2023-03-30 20:04:30.000000 mbox2m365-3.0.6/mbox2m365.egg-info/entry_points.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       20 2023-03-30 20:04:30.000000 mbox2m365-3.0.6/mbox2m365.egg-info/requires.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       17 2023-03-30 20:04:30.000000 mbox2m365-3.0.6/mbox2m365.egg-info/top_level.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      260 2023-03-30 19:56:19.000000 mbox2m365-3.0.6/pyproject.toml
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      449 2023-03-30 20:04:30.771833 mbox2m365-3.0.6/setup.cfg
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      399 2023-03-30 20:03:26.000000 mbox2m365-3.0.6/setup.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-03-30 20:07:13.379853 mbox2m365-3.0.8/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11456 2023-03-30 20:07:13.379853 mbox2m365-3.0.8/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11135 2023-03-30 19:52:19.000000 mbox2m365-3.0.8/README.rst
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-03-30 20:07:13.378853 mbox2m365-3.0.8/jobber/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     5167 2022-09-19 13:44:42.000000 mbox2m365-3.0.8/jobber/jobber.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-03-30 20:07:13.379853 mbox2m365-3.0.8/mbox2m365/
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)      268 2022-09-19 20:24:22.000000 mbox2m365-3.0.8/mbox2m365/__init__.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11546 2022-09-20 13:57:52.000000 mbox2m365-3.0.8/mbox2m365/__main__.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    30539 2023-03-30 19:26:06.000000 mbox2m365-3.0.8/mbox2m365/mbox2m365.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-03-30 20:07:13.379853 mbox2m365-3.0.8/mbox2m365.egg-info/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11456 2023-03-30 20:07:12.000000 mbox2m365-3.0.8/mbox2m365.egg-info/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      328 2023-03-30 20:07:13.000000 mbox2m365-3.0.8/mbox2m365.egg-info/SOURCES.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2023-03-30 20:07:12.000000 mbox2m365-3.0.8/mbox2m365.egg-info/dependency_links.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       54 2023-03-30 20:07:13.000000 mbox2m365-3.0.8/mbox2m365.egg-info/entry_points.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       20 2023-03-30 20:07:13.000000 mbox2m365-3.0.8/mbox2m365.egg-info/requires.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       17 2023-03-30 20:07:13.000000 mbox2m365-3.0.8/mbox2m365.egg-info/top_level.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      260 2023-03-30 20:06:34.000000 mbox2m365-3.0.8/pyproject.toml
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      449 2023-03-30 20:07:13.380853 mbox2m365-3.0.8/setup.cfg
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      399 2023-03-30 20:03:26.000000 mbox2m365-3.0.8/setup.py
```

### Comparing `mbox2m365-3.0.6/PKG-INFO` & `mbox2m365-3.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbox2m365
-Version: 3.0.6
+Version: 3.0.8
 Summary: 'Send a message stored within an mbox using m365 (Office365)'
 Home-page: https://github.com/FNNDSC/mbox2m365
 Author: Rudolph Pienaar
 Author-email: rudolph.pienaar@childrens.harvard.edu
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mbox2m365-3.0.6/README.rst` & `mbox2m365-3.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `mbox2m365-3.0.6/jobber/jobber.py` & `mbox2m365-3.0.8/jobber/jobber.py`

 * *Files identical despite different names*

### Comparing `mbox2m365-3.0.6/mbox2m365/__main__.py` & `mbox2m365-3.0.8/mbox2m365/__main__.py`

 * *Files identical despite different names*

### Comparing `mbox2m365-3.0.6/mbox2m365/mbox2m365.py` & `mbox2m365-3.0.8/mbox2m365/mbox2m365.py`

 * *Files identical despite different names*

### Comparing `mbox2m365-3.0.6/mbox2m365.egg-info/PKG-INFO` & `mbox2m365-3.0.8/mbox2m365.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbox2m365
-Version: 3.0.6
+Version: 3.0.8
 Summary: 'Send a message stored within an mbox using m365 (Office365)'
 Home-page: https://github.com/FNNDSC/mbox2m365
 Author: Rudolph Pienaar
 Author-email: rudolph.pienaar@childrens.harvard.edu
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

