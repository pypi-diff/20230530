# Comparing `tmp/wayback-0.4.1.tar.gz` & `tmp/wayback-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wayback-0.4.1.tar", last modified: Wed Mar  8 05:06:26 2023, max compression
+gzip compressed data, was "wayback-0.4.2.tar", last modified: Tue May 30 06:10:43 2023, max compression
```

## Comparing `wayback-0.4.1.tar` & `wayback-0.4.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 rbrackett   (501) staff       (20)        0 2023-03-08 05:06:26.741010 wayback-0.4.1/
--rw-r--r--   0 rbrackett   (501) staff       (20)     3259 2023-03-08 05:02:50.000000 wayback-0.4.1/CONTRIBUTING.rst
--rw-r--r--   0 rbrackett   (501) staff       (20)     1560 2023-03-08 05:02:50.000000 wayback-0.4.1/LICENSE
--rw-r--r--   0 rbrackett   (501) staff       (20)      340 2023-03-08 05:02:50.000000 wayback-0.4.1/MANIFEST.in
--rw-r--r--   0 rbrackett   (501) staff       (20)     4462 2023-03-08 05:06:26.741073 wayback-0.4.1/PKG-INFO
--rw-r--r--   0 rbrackett   (501) staff       (20)     3670 2023-03-08 05:02:50.000000 wayback-0.4.1/README.rst
-drwxr-xr-x   0 rbrackett   (501) staff       (20)        0 2023-03-08 05:06:26.738461 wayback-0.4.1/docs/
--rw-r--r--   0 rbrackett   (501) staff       (20)      673 2023-03-08 05:02:50.000000 wayback-0.4.1/docs/Makefile
--rw-r--r--   0 rbrackett   (501) staff       (20)      797 2023-03-08 05:02:50.000000 wayback-0.4.1/docs/make.bat
-drwxr-xr-x   0 rbrackett   (501) staff       (20)        0 2023-03-08 05:06:26.739019 wayback-0.4.1/docs/source/
--rw-r--r--   0 rbrackett   (501) staff       (20)     6452 2023-03-08 05:02:50.000000 wayback-0.4.1/docs/source/conf.py
--rw-r--r--   0 rbrackett   (501) staff       (20)      934 2023-03-08 05:02:50.000000 wayback-0.4.1/docs/source/index.rst
--rw-r--r--   0 rbrackett   (501) staff       (20)      170 2023-03-08 05:02:50.000000 wayback-0.4.1/docs/source/installation.rst
--rw-r--r--   0 rbrackett   (501) staff       (20)    26637 2023-03-08 05:02:50.000000 wayback-0.4.1/docs/source/release-history.rst
--rw-r--r--   0 rbrackett   (501) staff       (20)     4344 2023-03-08 05:02:50.000000 wayback-0.4.1/docs/source/usage.rst
--rw-r--r--   0 rbrackett   (501) staff       (20)       17 2023-03-08 05:02:50.000000 wayback-0.4.1/requirements.txt
--rw-r--r--   0 rbrackett   (501) staff       (20)      178 2023-03-08 05:06:26.741279 wayback-0.4.1/setup.cfg
--rw-r--r--   0 rbrackett   (501) staff       (20)     2519 2023-03-08 05:02:50.000000 wayback-0.4.1/setup.py
--rw-r--r--   0 rbrackett   (501) staff       (20)    68611 2023-03-08 05:02:50.000000 wayback-0.4.1/versioneer.py
-drwxr-xr-x   0 rbrackett   (501) staff       (20)        0 2023-03-08 05:06:26.741404 wayback-0.4.1/wayback/
--rw-r--r--   0 rbrackett   (501) staff       (20)      279 2023-03-08 05:02:50.000000 wayback-0.4.1/wayback/__init__.py
--rw-r--r--   0 rbrackett   (501) staff       (20)    48496 2023-03-08 05:02:50.000000 wayback-0.4.1/wayback/_client.py
--rw-r--r--   0 rbrackett   (501) staff       (20)    12748 2023-03-08 05:02:50.000000 wayback-0.4.1/wayback/_models.py
--rw-r--r--   0 rbrackett   (501) staff       (20)    11686 2023-03-08 05:02:50.000000 wayback-0.4.1/wayback/_utils.py
--rw-r--r--   0 rbrackett   (501) staff       (20)      497 2023-03-08 05:06:26.741433 wayback-0.4.1/wayback/_version.py
--rw-r--r--   0 rbrackett   (501) staff       (20)     3843 2023-03-08 05:02:50.000000 wayback-0.4.1/wayback/exceptions.py
-drwxr-xr-x   0 rbrackett   (501) staff       (20)        0 2023-03-08 05:06:26.740910 wayback-0.4.1/wayback/tests/
--rw-r--r--   0 rbrackett   (501) staff       (20)        0 2023-03-08 05:02:50.000000 wayback-0.4.1/wayback/tests/__init__.py
--rw-r--r--   0 rbrackett   (501) staff       (20)        0 2023-03-08 05:02:50.000000 wayback-0.4.1/wayback/tests/conftest.py
--rw-r--r--   0 rbrackett   (501) staff       (20)    33965 2023-03-08 05:02:50.000000 wayback-0.4.1/wayback/tests/test_client.py
--rw-r--r--   0 rbrackett   (501) staff       (20)     3188 2023-03-08 05:02:50.000000 wayback-0.4.1/wayback/tests/test_utils.py
-drwxr-xr-x   0 rbrackett   (501) staff       (20)        0 2023-03-08 05:06:26.740465 wayback-0.4.1/wayback.egg-info/
--rw-r--r--   0 rbrackett   (501) staff       (20)     4462 2023-03-08 05:06:26.000000 wayback-0.4.1/wayback.egg-info/PKG-INFO
--rw-r--r--   0 rbrackett   (501) staff       (20)      665 2023-03-08 05:06:26.000000 wayback-0.4.1/wayback.egg-info/SOURCES.txt
--rw-r--r--   0 rbrackett   (501) staff       (20)        1 2023-03-08 05:06:26.000000 wayback-0.4.1/wayback.egg-info/dependency_links.txt
--rw-r--r--   0 rbrackett   (501) staff       (20)       20 2023-03-08 05:06:26.000000 wayback-0.4.1/wayback.egg-info/entry_points.txt
--rw-r--r--   0 rbrackett   (501) staff       (20)       17 2023-03-08 05:06:26.000000 wayback-0.4.1/wayback.egg-info/requires.txt
--rw-r--r--   0 rbrackett   (501) staff       (20)        8 2023-03-08 05:06:26.000000 wayback-0.4.1/wayback.egg-info/top_level.txt
+drwxr-xr-x   0 rbrackett   (501) staff       (20)        0 2023-05-30 06:10:43.831173 wayback-0.4.2/
+-rw-r--r--   0 rbrackett   (501) staff       (20)     3259 2023-03-08 05:02:50.000000 wayback-0.4.2/CONTRIBUTING.rst
+-rw-r--r--   0 rbrackett   (501) staff       (20)     1560 2023-03-08 05:02:50.000000 wayback-0.4.2/LICENSE
+-rw-r--r--   0 rbrackett   (501) staff       (20)      340 2023-03-08 05:02:50.000000 wayback-0.4.2/MANIFEST.in
+-rw-r--r--   0 rbrackett   (501) staff       (20)     4462 2023-05-30 06:10:43.831237 wayback-0.4.2/PKG-INFO
+-rw-r--r--   0 rbrackett   (501) staff       (20)     3670 2023-03-08 05:02:50.000000 wayback-0.4.2/README.rst
+drwxr-xr-x   0 rbrackett   (501) staff       (20)        0 2023-05-30 06:10:43.828204 wayback-0.4.2/docs/
+-rw-r--r--   0 rbrackett   (501) staff       (20)      673 2023-03-08 05:02:50.000000 wayback-0.4.2/docs/Makefile
+-rw-r--r--   0 rbrackett   (501) staff       (20)      797 2023-03-08 05:02:50.000000 wayback-0.4.2/docs/make.bat
+drwxr-xr-x   0 rbrackett   (501) staff       (20)        0 2023-05-30 06:10:43.828863 wayback-0.4.2/docs/source/
+-rw-r--r--   0 rbrackett   (501) staff       (20)     6452 2023-03-08 05:02:50.000000 wayback-0.4.2/docs/source/conf.py
+-rw-r--r--   0 rbrackett   (501) staff       (20)      934 2023-03-08 05:02:50.000000 wayback-0.4.2/docs/source/index.rst
+-rw-r--r--   0 rbrackett   (501) staff       (20)      170 2023-03-08 05:02:50.000000 wayback-0.4.2/docs/source/installation.rst
+-rw-r--r--   0 rbrackett   (501) staff       (20)    26913 2023-05-30 06:10:07.000000 wayback-0.4.2/docs/source/release-history.rst
+-rw-r--r--   0 rbrackett   (501) staff       (20)     4344 2023-03-08 05:02:50.000000 wayback-0.4.2/docs/source/usage.rst
+-rw-r--r--   0 rbrackett   (501) staff       (20)       28 2023-05-30 06:10:07.000000 wayback-0.4.2/requirements.txt
+-rw-r--r--   0 rbrackett   (501) staff       (20)      178 2023-05-30 06:10:43.831455 wayback-0.4.2/setup.cfg
+-rw-r--r--   0 rbrackett   (501) staff       (20)     2519 2023-03-08 05:02:50.000000 wayback-0.4.2/setup.py
+-rw-r--r--   0 rbrackett   (501) staff       (20)    68611 2023-03-08 05:02:50.000000 wayback-0.4.2/versioneer.py
+drwxr-xr-x   0 rbrackett   (501) staff       (20)        0 2023-05-30 06:10:43.831590 wayback-0.4.2/wayback/
+-rw-r--r--   0 rbrackett   (501) staff       (20)      279 2023-03-08 05:02:50.000000 wayback-0.4.2/wayback/__init__.py
+-rw-r--r--   0 rbrackett   (501) staff       (20)    48496 2023-03-08 05:02:50.000000 wayback-0.4.2/wayback/_client.py
+-rw-r--r--   0 rbrackett   (501) staff       (20)    12748 2023-03-08 05:02:50.000000 wayback-0.4.2/wayback/_models.py
+-rw-r--r--   0 rbrackett   (501) staff       (20)    11686 2023-03-08 05:02:50.000000 wayback-0.4.2/wayback/_utils.py
+-rw-r--r--   0 rbrackett   (501) staff       (20)      497 2023-05-30 06:10:43.831619 wayback-0.4.2/wayback/_version.py
+-rw-r--r--   0 rbrackett   (501) staff       (20)     3843 2023-03-08 05:02:50.000000 wayback-0.4.2/wayback/exceptions.py
+drwxr-xr-x   0 rbrackett   (501) staff       (20)        0 2023-05-30 06:10:43.831051 wayback-0.4.2/wayback/tests/
+-rw-r--r--   0 rbrackett   (501) staff       (20)        0 2023-03-08 05:02:50.000000 wayback-0.4.2/wayback/tests/__init__.py
+-rw-r--r--   0 rbrackett   (501) staff       (20)        0 2023-03-08 05:02:50.000000 wayback-0.4.2/wayback/tests/conftest.py
+-rw-r--r--   0 rbrackett   (501) staff       (20)    33965 2023-03-08 05:02:50.000000 wayback-0.4.2/wayback/tests/test_client.py
+-rw-r--r--   0 rbrackett   (501) staff       (20)     3188 2023-03-08 05:02:50.000000 wayback-0.4.2/wayback/tests/test_utils.py
+drwxr-xr-x   0 rbrackett   (501) staff       (20)        0 2023-05-30 06:10:43.830302 wayback-0.4.2/wayback.egg-info/
+-rw-r--r--   0 rbrackett   (501) staff       (20)     4462 2023-05-30 06:10:43.000000 wayback-0.4.2/wayback.egg-info/PKG-INFO
+-rw-r--r--   0 rbrackett   (501) staff       (20)      665 2023-05-30 06:10:43.000000 wayback-0.4.2/wayback.egg-info/SOURCES.txt
+-rw-r--r--   0 rbrackett   (501) staff       (20)        1 2023-05-30 06:10:43.000000 wayback-0.4.2/wayback.egg-info/dependency_links.txt
+-rw-r--r--   0 rbrackett   (501) staff       (20)       20 2023-05-30 06:10:43.000000 wayback-0.4.2/wayback.egg-info/entry_points.txt
+-rw-r--r--   0 rbrackett   (501) staff       (20)       26 2023-05-30 06:10:43.000000 wayback-0.4.2/wayback.egg-info/requires.txt
+-rw-r--r--   0 rbrackett   (501) staff       (20)        8 2023-05-30 06:10:43.000000 wayback-0.4.2/wayback.egg-info/top_level.txt
```

### Comparing `wayback-0.4.1/CONTRIBUTING.rst` & `wayback-0.4.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `wayback-0.4.1/LICENSE` & `wayback-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wayback-0.4.1/PKG-INFO` & `wayback-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wayback
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python API to Internet Archive Wayback Machine
 Home-page: https://github.com/edgi-govdata-archiving/wayback
 Author: Environmental Data Governance Initiative
 Author-email: EnviroDGI@protonmail.com
 License: BSD (3-clause)
 Project-URL: Documentation, https://wayback.readthedocs.io/en/stable/
 Project-URL: Changelog, https://wayback.readthedocs.io/en/stable/release-history.html
```

### Comparing `wayback-0.4.1/README.rst` & `wayback-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `wayback-0.4.1/docs/Makefile` & `wayback-0.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wayback-0.4.1/docs/make.bat` & `wayback-0.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wayback-0.4.1/docs/source/conf.py` & `wayback-0.4.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `wayback-0.4.1/docs/source/index.rst` & `wayback-0.4.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `wayback-0.4.1/docs/source/release-history.rst` & `wayback-0.4.2/docs/source/release-history.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 ===============
 Release History
 ===============
 
+v0.4.2 (2023-05-29)
+-------------------
+
+Wayback is not compatible with urllib3 v2, and this release updates the package's requirements to make sure Pip and other package managers install compatible versions of Wayback and urllib3. There are no other fixes or new features.
+
+
 v0.4.1 (2023-03-07)
 -------------------
 
 Features
 ^^^^^^^^
 
 :class:`wayback.Memento` now has a ``links`` property with information about other URLs that are related to the memento, such as the previous or next mementos in time. It’s a dict where the keys identify the relationship (e.g. ``'prev memento'``) and the values are dicts with additional information about the link. (:issue:`57`) For example::
```

### Comparing `wayback-0.4.1/docs/source/usage.rst` & `wayback-0.4.2/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `wayback-0.4.1/setup.py` & `wayback-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `wayback-0.4.1/versioneer.py` & `wayback-0.4.2/versioneer.py`

 * *Files identical despite different names*

### Comparing `wayback-0.4.1/wayback/_client.py` & `wayback-0.4.2/wayback/_client.py`

 * *Files identical despite different names*

### Comparing `wayback-0.4.1/wayback/_models.py` & `wayback-0.4.2/wayback/_models.py`

 * *Files identical despite different names*

### Comparing `wayback-0.4.1/wayback/_utils.py` & `wayback-0.4.2/wayback/_utils.py`

 * *Files identical despite different names*

### Comparing `wayback-0.4.1/wayback/exceptions.py` & `wayback-0.4.2/wayback/exceptions.py`

 * *Files identical despite different names*

### Comparing `wayback-0.4.1/wayback/tests/test_client.py` & `wayback-0.4.2/wayback/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `wayback-0.4.1/wayback/tests/test_utils.py` & `wayback-0.4.2/wayback/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wayback-0.4.1/wayback.egg-info/PKG-INFO` & `wayback-0.4.2/wayback.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wayback
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python API to Internet Archive Wayback Machine
 Home-page: https://github.com/edgi-govdata-archiving/wayback
 Author: Environmental Data Governance Initiative
 Author-email: EnviroDGI@protonmail.com
 License: BSD (3-clause)
 Project-URL: Documentation, https://wayback.readthedocs.io/en/stable/
 Project-URL: Changelog, https://wayback.readthedocs.io/en/stable/release-history.html
```

### Comparing `wayback-0.4.1/wayback.egg-info/SOURCES.txt` & `wayback-0.4.2/wayback.egg-info/SOURCES.txt`

 * *Files identical despite different names*

