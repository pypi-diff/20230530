# Comparing `tmp/funcx-2.0.3.tar.gz` & `tmp/funcx-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcx-2.0.3.tar", last modified: Wed May 10 20:42:05 2023, max compression
+gzip compressed data, was "funcx-2.1.0.tar", last modified: Tue May 30 18:49:34 2023, max compression
```

## Comparing `funcx-2.0.3.tar` & `funcx-2.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:05.831533 funcx-2.0.3/
--rw-r--r--   0 chris      (501) staff       (20)    11330 2023-04-12 14:51:48.000000 funcx-2.0.3/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)       16 2023-04-17 20:09:04.000000 funcx-2.0.3/MANIFEST.in
--rw-r--r--   0 chris      (501) staff       (20)     1995 2023-05-10 20:42:05.831621 funcx-2.0.3/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     1051 2023-04-17 20:09:04.000000 funcx-2.0.3/PyPI.md
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:05.828889 funcx-2.0.3/funcx/
--rw-r--r--   0 chris      (501) staff       (20)      467 2023-04-12 14:51:48.000000 funcx-2.0.3/funcx/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:05.830835 funcx-2.0.3/funcx/sdk/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-20 15:45:45.000000 funcx-2.0.3/funcx/sdk/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)       78 2023-04-25 18:54:41.000000 funcx-2.0.3/funcx/sdk/client.py
--rw-r--r--   0 chris      (501) staff       (20)       84 2023-04-25 18:54:41.000000 funcx-2.0.3/funcx/sdk/executor.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:05.831051 funcx-2.0.3/funcx/sdk/login_manager/
--rw-r--r--   0 chris      (501) staff       (20)      445 2023-04-12 14:51:48.000000 funcx-2.0.3/funcx/sdk/login_manager/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)       88 2023-04-12 14:51:48.000000 funcx-2.0.3/funcx/sdk/web_client.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:05.831323 funcx-2.0.3/funcx/serialize/
--rw-r--r--   0 chris      (501) staff       (20)      110 2023-04-12 14:51:48.000000 funcx-2.0.3/funcx/serialize/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     1144 2023-05-10 20:21:03.000000 funcx-2.0.3/funcx/version.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:05.829652 funcx-2.0.3/funcx.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     1995 2023-05-10 20:42:05.000000 funcx-2.0.3/funcx.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      377 2023-05-10 20:42:05.000000 funcx-2.0.3/funcx.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-10 20:42:05.000000 funcx-2.0.3/funcx.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)       26 2023-05-10 20:42:05.000000 funcx-2.0.3/funcx.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)        6 2023-05-10 20:42:05.000000 funcx-2.0.3/funcx.egg-info/top_level.txt
--rw-r--r--   0 chris      (501) staff       (20)      305 2023-05-10 20:42:05.831977 funcx-2.0.3/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)     1913 2023-05-10 20:20:40.000000 funcx-2.0.3/setup.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-30 18:49:34.031169 funcx-2.1.0/
+-rw-rw-r--   0 reid      (1000) reid      (1000)    11330 2023-04-19 22:57:38.000000 funcx-2.1.0/LICENSE
+-rw-rw-r--   0 reid      (1000) reid      (1000)       16 2023-04-19 22:57:38.000000 funcx-2.1.0/MANIFEST.in
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1995 2023-05-30 18:49:34.031169 funcx-2.1.0/PKG-INFO
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1051 2023-04-19 22:57:38.000000 funcx-2.1.0/PyPI.md
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-30 18:49:34.027169 funcx-2.1.0/funcx/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      467 2023-04-19 22:57:38.000000 funcx-2.1.0/funcx/__init__.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-30 18:49:34.031169 funcx-2.1.0/funcx/sdk/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 funcx-2.1.0/funcx/sdk/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)       78 2023-05-01 20:50:52.000000 funcx-2.1.0/funcx/sdk/client.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)       84 2023-05-01 20:50:52.000000 funcx-2.1.0/funcx/sdk/executor.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-30 18:49:34.031169 funcx-2.1.0/funcx/sdk/login_manager/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      445 2023-04-19 22:57:38.000000 funcx-2.1.0/funcx/sdk/login_manager/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)       88 2023-04-19 22:57:38.000000 funcx-2.1.0/funcx/sdk/web_client.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-30 18:49:34.031169 funcx-2.1.0/funcx/serialize/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      110 2023-04-19 22:57:38.000000 funcx-2.1.0/funcx/serialize/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1144 2023-05-30 18:44:59.000000 funcx-2.1.0/funcx/version.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-30 18:49:34.027169 funcx-2.1.0/funcx.egg-info/
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1995 2023-05-30 18:49:34.000000 funcx-2.1.0/funcx.egg-info/PKG-INFO
+-rw-rw-r--   0 reid      (1000) reid      (1000)      377 2023-05-30 18:49:34.000000 funcx-2.1.0/funcx.egg-info/SOURCES.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)        1 2023-05-30 18:49:34.000000 funcx-2.1.0/funcx.egg-info/dependency_links.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)       26 2023-05-30 18:49:34.000000 funcx-2.1.0/funcx.egg-info/requires.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)        6 2023-05-30 18:49:34.000000 funcx-2.1.0/funcx.egg-info/top_level.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)      305 2023-05-30 18:49:34.031169 funcx-2.1.0/setup.cfg
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1913 2023-05-30 18:44:59.000000 funcx-2.1.0/setup.py
```

### Comparing `funcx-2.0.3/LICENSE` & `funcx-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `funcx-2.0.3/PKG-INFO` & `funcx-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcx
-Version: 2.0.3
+Version: 2.1.0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: The Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `funcx-2.0.3/PyPI.md` & `funcx-2.1.0/PyPI.md`

 * *Files identical despite different names*

### Comparing `funcx-2.0.3/funcx/version.py` & `funcx-2.1.0/funcx/version.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from globus_compute_sdk.errors import VersionMismatch
 from packaging.version import Version
 
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.0.3"
+__version__ = "2.1.0"
 
 DEPRECATION_FUNCX = """
 The funcX SDK has been renamed to Globus Compute SDK and the new package is
 available on PyPI:
     https://pypi.org/project/globus-compute-sdk/
 
 Please consider upgrading to Globus Compute.  More information can be found at:
```

### Comparing `funcx-2.0.3/funcx.egg-info/PKG-INFO` & `funcx-2.1.0/funcx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcx
-Version: 2.0.3
+Version: 2.1.0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: The Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `funcx-2.0.3/setup.py` & `funcx-2.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import re
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
-    "globus-compute-sdk==2.0.3",
+    "globus-compute-sdk==2.1.0",
 ]
 
 
 def parse_version():
     # single source of truth for package version
     version_string = ""
     version_pattern = re.compile(r'__version__ = "([^"]*)"')
```

