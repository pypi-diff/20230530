# Comparing `tmp/funcx-endpoint-2.0.3.tar.gz` & `tmp/funcx-endpoint-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcx-endpoint-2.0.3.tar", last modified: Wed May 10 20:42:19 2023, max compression
+gzip compressed data, was "funcx-endpoint-2.1.0.tar", last modified: Tue May 30 18:49:55 2023, max compression
```

## Comparing `funcx-endpoint-2.0.3.tar` & `funcx-endpoint-2.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:19.003884 funcx-endpoint-2.0.3/
--rw-r--r--   0 chris      (501) staff       (20)    11330 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.3/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)       16 2023-04-17 20:09:04.000000 funcx-endpoint-2.0.3/MANIFEST.in
--rw-r--r--   0 chris      (501) staff       (20)     2040 2023-05-10 20:42:19.003969 funcx-endpoint-2.0.3/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     1115 2023-04-17 20:09:04.000000 funcx-endpoint-2.0.3/PyPI.md
--rw-r--r--   0 chris      (501) staff       (20)      430 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.3/README.md
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:19.001111 funcx-endpoint-2.0.3/funcx_endpoint/
--rw-r--r--   0 chris      (501) staff       (20)      122 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.3/funcx_endpoint/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:19.002254 funcx-endpoint-2.0.3/funcx_endpoint/endpoint/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-20 15:45:45.000000 funcx-endpoint-2.0.3/funcx_endpoint/endpoint/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:19.002479 funcx-endpoint-2.0.3/funcx_endpoint/endpoint/utils/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-20 15:45:45.000000 funcx-endpoint-2.0.3/funcx_endpoint/endpoint/utils/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)       89 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.3/funcx_endpoint/endpoint/utils/config.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:19.002658 funcx-endpoint-2.0.3/funcx_endpoint/executors/
--rw-r--r--   0 chris      (501) staff       (20)      107 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.3/funcx_endpoint/executors/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:19.003656 funcx-endpoint-2.0.3/funcx_endpoint/executors/high_throughput/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-20 15:45:45.000000 funcx-endpoint-2.0.3/funcx_endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      101 2023-04-17 18:38:33.000000 funcx-endpoint-2.0.3/funcx_endpoint/executors/high_throughput/funcx_manager.py
--rw-r--r--   0 chris      (501) staff       (20)      114 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.3/funcx_endpoint/executors/high_throughput/funcx_worker.py
--rw-r--r--   0 chris      (501) staff       (20)      243 2023-05-10 20:21:13.000000 funcx-endpoint-2.0.3/funcx_endpoint/version.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:19.002116 funcx-endpoint-2.0.3/funcx_endpoint.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     2040 2023-05-10 20:42:18.000000 funcx-endpoint-2.0.3/funcx_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      662 2023-05-10 20:42:18.000000 funcx-endpoint-2.0.3/funcx_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-10 20:42:18.000000 funcx-endpoint-2.0.3/funcx_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)      329 2023-05-10 20:42:18.000000 funcx-endpoint-2.0.3/funcx_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 chris      (501) staff       (20)       31 2023-05-10 20:42:18.000000 funcx-endpoint-2.0.3/funcx_endpoint.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)       15 2023-05-10 20:42:18.000000 funcx-endpoint-2.0.3/funcx_endpoint.egg-info/top_level.txt
--rw-r--r--   0 chris      (501) staff       (20)      305 2023-05-10 20:42:19.004303 funcx-endpoint-2.0.3/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)     2030 2023-05-10 20:20:51.000000 funcx-endpoint-2.0.3/setup.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-30 18:49:55.439187 funcx-endpoint-2.1.0/
+-rw-rw-r--   0 reid      (1000) reid      (1000)    11330 2023-04-19 22:57:38.000000 funcx-endpoint-2.1.0/LICENSE
+-rw-rw-r--   0 reid      (1000) reid      (1000)       16 2023-04-19 22:57:38.000000 funcx-endpoint-2.1.0/MANIFEST.in
+-rw-rw-r--   0 reid      (1000) reid      (1000)     2040 2023-05-30 18:49:55.443188 funcx-endpoint-2.1.0/PKG-INFO
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1115 2023-04-19 22:57:38.000000 funcx-endpoint-2.1.0/PyPI.md
+-rw-rw-r--   0 reid      (1000) reid      (1000)      430 2023-04-19 22:57:38.000000 funcx-endpoint-2.1.0/README.md
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-30 18:49:55.439187 funcx-endpoint-2.1.0/funcx_endpoint/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      122 2023-04-19 22:57:38.000000 funcx-endpoint-2.1.0/funcx_endpoint/__init__.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-30 18:49:55.439187 funcx-endpoint-2.1.0/funcx_endpoint/endpoint/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 funcx-endpoint-2.1.0/funcx_endpoint/endpoint/__init__.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-30 18:49:55.439187 funcx-endpoint-2.1.0/funcx_endpoint/endpoint/utils/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 funcx-endpoint-2.1.0/funcx_endpoint/endpoint/utils/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)       89 2023-05-30 18:44:57.000000 funcx-endpoint-2.1.0/funcx_endpoint/endpoint/utils/config.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-30 18:49:55.439187 funcx-endpoint-2.1.0/funcx_endpoint/executors/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      107 2023-04-19 22:57:38.000000 funcx-endpoint-2.1.0/funcx_endpoint/executors/__init__.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-30 18:49:55.439187 funcx-endpoint-2.1.0/funcx_endpoint/executors/high_throughput/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 funcx-endpoint-2.1.0/funcx_endpoint/executors/high_throughput/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      101 2023-04-19 22:57:38.000000 funcx-endpoint-2.1.0/funcx_endpoint/executors/high_throughput/funcx_manager.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      114 2023-04-19 22:57:38.000000 funcx-endpoint-2.1.0/funcx_endpoint/executors/high_throughput/funcx_worker.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      243 2023-05-30 18:44:59.000000 funcx-endpoint-2.1.0/funcx_endpoint/version.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-30 18:49:55.439187 funcx-endpoint-2.1.0/funcx_endpoint.egg-info/
+-rw-rw-r--   0 reid      (1000) reid      (1000)     2040 2023-05-30 18:49:55.000000 funcx-endpoint-2.1.0/funcx_endpoint.egg-info/PKG-INFO
+-rw-rw-r--   0 reid      (1000) reid      (1000)      662 2023-05-30 18:49:55.000000 funcx-endpoint-2.1.0/funcx_endpoint.egg-info/SOURCES.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)        1 2023-05-30 18:49:55.000000 funcx-endpoint-2.1.0/funcx_endpoint.egg-info/dependency_links.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)      329 2023-05-30 18:49:55.000000 funcx-endpoint-2.1.0/funcx_endpoint.egg-info/entry_points.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)       31 2023-05-30 18:49:55.000000 funcx-endpoint-2.1.0/funcx_endpoint.egg-info/requires.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)       15 2023-05-30 18:49:55.000000 funcx-endpoint-2.1.0/funcx_endpoint.egg-info/top_level.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)      305 2023-05-30 18:49:55.443188 funcx-endpoint-2.1.0/setup.cfg
+-rw-rw-r--   0 reid      (1000) reid      (1000)     2030 2023-05-30 18:44:59.000000 funcx-endpoint-2.1.0/setup.py
```

### Comparing `funcx-endpoint-2.0.3/LICENSE` & `funcx-endpoint-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `funcx-endpoint-2.0.3/PKG-INFO` & `funcx-endpoint-2.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcx-endpoint
-Version: 2.0.3
+Version: 2.1.0
 Summary: funcX: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `funcx-endpoint-2.0.3/PyPI.md` & `funcx-endpoint-2.1.0/PyPI.md`

 * *Files identical despite different names*

### Comparing `funcx-endpoint-2.0.3/funcx_endpoint.egg-info/PKG-INFO` & `funcx-endpoint-2.1.0/funcx_endpoint.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcx-endpoint
-Version: 2.0.3
+Version: 2.1.0
 Summary: funcX: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `funcx-endpoint-2.0.3/funcx_endpoint.egg-info/SOURCES.txt` & `funcx-endpoint-2.1.0/funcx_endpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funcx-endpoint-2.0.3/setup.py` & `funcx-endpoint-2.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
-    "globus-compute-endpoint==2.0.3",
+    "globus-compute-endpoint==2.1.0",
 ]
 
 version_ns = {}
 with open(os.path.join("funcx_endpoint", "version.py")) as f:
     exec(f.read(), version_ns)
 version = version_ns["__version__"]
```

