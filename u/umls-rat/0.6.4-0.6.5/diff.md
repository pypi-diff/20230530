# Comparing `tmp/umls-rat-0.6.4.tar.gz` & `tmp/umls-rat-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umls-rat-0.6.4.tar", last modified: Tue Mar 21 20:27:00 2023, max compression
+gzip compressed data, was "umls-rat-0.6.5.tar", last modified: Tue May 30 14:51:50 2023, max compression
```

## Comparing `umls-rat-0.6.4.tar` & `umls-rat-0.6.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 20:27:00.819931 umls-rat-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-21 20:26:45.000000 umls-rat-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-03-21 20:27:00.819931 umls-rat-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-03-21 20:26:45.000000 umls-rat-0.6.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-21 20:26:45.000000 umls-rat-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 20:27:00.819931 umls-rat-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-03-21 20:26:45.000000 umls-rat-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 20:27:00.815931 umls-rat-0.6.4/umls_rat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-03-21 20:27:00.000000 umls-rat-0.6.4/umls_rat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-21 20:27:00.000000 umls-rat-0.6.4/umls_rat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 20:27:00.000000 umls-rat-0.6.4/umls_rat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-21 20:27:00.000000 umls-rat-0.6.4/umls_rat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-21 20:27:00.000000 umls-rat-0.6.4/umls_rat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 20:27:00.815931 umls-rat-0.6.4/umlsrat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 20:26:45.000000 umls-rat-0.6.4/umlsrat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 20:27:00.815931 umls-rat-0.6.4/umlsrat/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 20:26:45.000000 umls-rat-0.6.4/umlsrat/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32137 2023-03-21 20:26:45.000000 umls-rat-0.6.4/umlsrat/api/metathesaurus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-03-21 20:26:45.000000 umls-rat-0.6.4/umlsrat/api/rat_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-21 20:26:45.000000 umls-rat-0.6.4/umlsrat/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 20:27:00.819931 umls-rat-0.6.4/umlsrat/lookup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 20:26:45.000000 umls-rat-0.6.4/umlsrat/lookup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-03-21 20:26:45.000000 umls-rat-0.6.4/umlsrat/lookup/graph_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-03-21 20:26:45.000000 umls-rat-0.6.4/umlsrat/lookup/lookup_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-03-21 20:26:45.000000 umls-rat-0.6.4/umlsrat/lookup/lookup_desc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-03-21 20:26:45.000000 umls-rat-0.6.4/umlsrat/lookup/lookup_umls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 20:27:00.819931 umls-rat-0.6.4/umlsrat/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 20:26:45.000000 umls-rat-0.6.4/umlsrat/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-21 20:26:45.000000 umls-rat-0.6.4/umlsrat/util/args_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-03-21 20:26:45.000000 umls-rat-0.6.4/umlsrat/util/cui_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-03-21 20:26:45.000000 umls-rat-0.6.4/umlsrat/util/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-03-21 20:26:45.000000 umls-rat-0.6.4/umlsrat/util/orderedset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-03-21 20:26:45.000000 umls-rat-0.6.4/umlsrat/util/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:51:50.800332 umls-rat-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-30 14:51:39.000000 umls-rat-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-30 14:51:50.800332 umls-rat-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-30 14:51:39.000000 umls-rat-0.6.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-30 14:51:39.000000 umls-rat-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:51:50.800332 umls-rat-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-30 14:51:39.000000 umls-rat-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:51:50.796332 umls-rat-0.6.5/umls_rat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-30 14:51:50.000000 umls-rat-0.6.5/umls_rat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-30 14:51:50.000000 umls-rat-0.6.5/umls_rat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:51:50.000000 umls-rat-0.6.5/umls_rat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-30 14:51:50.000000 umls-rat-0.6.5/umls_rat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 14:51:50.000000 umls-rat-0.6.5/umls_rat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:51:50.800332 umls-rat-0.6.5/umlsrat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:51:39.000000 umls-rat-0.6.5/umlsrat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:51:50.800332 umls-rat-0.6.5/umlsrat/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:51:39.000000 umls-rat-0.6.5/umlsrat/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32137 2023-05-30 14:51:39.000000 umls-rat-0.6.5/umlsrat/api/metathesaurus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-05-30 14:51:39.000000 umls-rat-0.6.5/umlsrat/api/rat_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-30 14:51:39.000000 umls-rat-0.6.5/umlsrat/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:51:50.800332 umls-rat-0.6.5/umlsrat/lookup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:51:39.000000 umls-rat-0.6.5/umlsrat/lookup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-30 14:51:39.000000 umls-rat-0.6.5/umlsrat/lookup/graph_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-05-30 14:51:39.000000 umls-rat-0.6.5/umlsrat/lookup/lookup_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-30 14:51:39.000000 umls-rat-0.6.5/umlsrat/lookup/lookup_desc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-05-30 14:51:39.000000 umls-rat-0.6.5/umlsrat/lookup/lookup_umls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:51:50.800332 umls-rat-0.6.5/umlsrat/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:51:39.000000 umls-rat-0.6.5/umlsrat/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-30 14:51:39.000000 umls-rat-0.6.5/umlsrat/util/args_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-30 14:51:39.000000 umls-rat-0.6.5/umlsrat/util/cui_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-30 14:51:39.000000 umls-rat-0.6.5/umlsrat/util/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-30 14:51:39.000000 umls-rat-0.6.5/umlsrat/util/orderedset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-30 14:51:39.000000 umls-rat-0.6.5/umlsrat/util/text.py
```

### Comparing `umls-rat-0.6.4/LICENSE` & `umls-rat-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `umls-rat-0.6.4/PKG-INFO` & `umls-rat-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umls-rat
-Version: 0.6.4
+Version: 0.6.5
 Summary: UMLS RAT (REST API Tool) provides a reasonable interface to the UMLS MetaThesaurus via the REST API.
 Home-page: https://github.com/3mcloud/umls-rat
 Author: Russell Klopfer
 Author-email: rklopfer@mmm.com
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `umls-rat-0.6.4/README.rst` & `umls-rat-0.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `umls-rat-0.6.4/setup.py` & `umls-rat-0.6.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-version = "0.6.4"
+version = "0.6.5"
 
 setup(
     name="umls-rat",
     version=version,
     description="UMLS RAT (REST API Tool) provides a reasonable "
     "interface to the UMLS MetaThesaurus via the REST API.",
     long_description=long_description,
```

### Comparing `umls-rat-0.6.4/umls_rat.egg-info/PKG-INFO` & `umls-rat-0.6.5/umls_rat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umls-rat
-Version: 0.6.4
+Version: 0.6.5
 Summary: UMLS RAT (REST API Tool) provides a reasonable interface to the UMLS MetaThesaurus via the REST API.
 Home-page: https://github.com/3mcloud/umls-rat
 Author: Russell Klopfer
 Author-email: rklopfer@mmm.com
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `umls-rat-0.6.4/umls_rat.egg-info/SOURCES.txt` & `umls-rat-0.6.5/umls_rat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `umls-rat-0.6.4/umlsrat/api/metathesaurus.py` & `umls-rat-0.6.5/umlsrat/api/metathesaurus.py`

 * *Files identical despite different names*

### Comparing `umls-rat-0.6.4/umlsrat/api/rat_session.py` & `umls-rat-0.6.5/umlsrat/api/rat_session.py`

 * *Files identical despite different names*

### Comparing `umls-rat-0.6.4/umlsrat/lookup/graph_fn.py` & `umls-rat-0.6.5/umlsrat/lookup/graph_fn.py`

 * *Files identical despite different names*

### Comparing `umls-rat-0.6.4/umlsrat/lookup/lookup_defs.py` & `umls-rat-0.6.5/umlsrat/lookup/lookup_defs.py`

 * *Files identical despite different names*

### Comparing `umls-rat-0.6.4/umlsrat/lookup/lookup_desc.py` & `umls-rat-0.6.5/umlsrat/lookup/lookup_desc.py`

 * *Files identical despite different names*

### Comparing `umls-rat-0.6.4/umlsrat/lookup/lookup_umls.py` & `umls-rat-0.6.5/umlsrat/lookup/lookup_umls.py`

 * *Files identical despite different names*

### Comparing `umls-rat-0.6.4/umlsrat/util/cui_order.py` & `umls-rat-0.6.5/umlsrat/util/cui_order.py`

 * *Files identical despite different names*

### Comparing `umls-rat-0.6.4/umlsrat/util/iterators.py` & `umls-rat-0.6.5/umlsrat/util/iterators.py`

 * *Files identical despite different names*

### Comparing `umls-rat-0.6.4/umlsrat/util/orderedset.py` & `umls-rat-0.6.5/umlsrat/util/orderedset.py`

 * *Files identical despite different names*

### Comparing `umls-rat-0.6.4/umlsrat/util/text.py` & `umls-rat-0.6.5/umlsrat/util/text.py`

 * *Files identical despite different names*

