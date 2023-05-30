# Comparing `tmp/access_nri_intake-0.0.4.tar.gz` & `tmp/access_nri_intake-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "access_nri_intake-0.0.4.tar", last modified: Wed May 17 00:45:07 2023, max compression
+gzip compressed data, was "access_nri_intake-0.0.5.tar", last modified: Tue May 30 06:16:49 2023, max compression
```

## Comparing `access_nri_intake-0.0.4.tar` & `access_nri_intake-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:45:07.152981 access_nri_intake-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-17 00:45:07.152981 access_nri_intake-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 00:45:07.152981 access_nri_intake-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:45:07.148981 access_nri_intake-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:45:07.152981 access_nri_intake-0.0.4/src/access_nri_intake/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-17 00:45:07.152981 access_nri_intake-0.0.4/src/access_nri_intake/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:45:07.152981 access_nri_intake-0.0.4/src/access_nri_intake/cat/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/cat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/cat/metacatalog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:45:07.152981 access_nri_intake-0.0.4/src/access_nri_intake/esmcat/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/esmcat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/esmcat/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/esmcat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:45:07.152981 access_nri_intake-0.0.4/src/access_nri_intake/metacat/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/metacat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/metacat/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/metacat/translators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/src/access_nri_intake/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:45:07.152981 access_nri_intake-0.0.4/src/access_nri_intake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-17 00:45:07.000000 access_nri_intake-0.0.4/src/access_nri_intake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-17 00:45:07.000000 access_nri_intake-0.0.4/src/access_nri_intake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 00:45:07.000000 access_nri_intake-0.0.4/src/access_nri_intake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-17 00:45:07.000000 access_nri_intake-0.0.4/src/access_nri_intake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-17 00:45:07.000000 access_nri_intake-0.0.4/src/access_nri_intake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-17 00:45:07.000000 access_nri_intake-0.0.4/src/access_nri_intake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-05-17 00:44:53.000000 access_nri_intake-0.0.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:49.976885 access_nri_intake-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-30 06:16:49.976885 access_nri_intake-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 06:16:49.976885 access_nri_intake-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:49.972885 access_nri_intake-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:49.976885 access_nri_intake-0.0.5/src/access_nri_intake/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-30 06:16:49.976885 access_nri_intake-0.0.5/src/access_nri_intake/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:49.972885 access_nri_intake-0.0.5/src/access_nri_intake/cat/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/cat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:49.976885 access_nri_intake-0.0.5/src/access_nri_intake/esmcat/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/esmcat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/esmcat/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/esmcat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:49.976885 access_nri_intake-0.0.5/src/access_nri_intake/metacat/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/metacat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/metacat/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/metacat/translators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/src/access_nri_intake/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:49.972885 access_nri_intake-0.0.5/src/access_nri_intake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-30 06:16:49.000000 access_nri_intake-0.0.5/src/access_nri_intake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-30 06:16:49.000000 access_nri_intake-0.0.5/src/access_nri_intake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:16:49.000000 access_nri_intake-0.0.5/src/access_nri_intake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-30 06:16:49.000000 access_nri_intake-0.0.5/src/access_nri_intake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-30 06:16:49.000000 access_nri_intake-0.0.5/src/access_nri_intake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 06:16:49.000000 access_nri_intake-0.0.5/src/access_nri_intake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-05-30 06:16:36.000000 access_nri_intake-0.0.5/versioneer.py
```

### Comparing `access_nri_intake-0.0.4/LICENSE` & `access_nri_intake-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.4/PKG-INFO` & `access_nri_intake-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access_nri_intake
-Version: 0.0.4
+Version: 0.0.5
 Summary: Intake catalog managed by ACCESS-NRI and associated tools
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `access_nri_intake-0.0.4/README.rst` & `access_nri_intake-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.4/pyproject.toml` & `access_nri_intake-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "cftime",
     "ecgtools>=2022.10.07",
-    "intake-dataframe-catalog>=0.1.0",
+    "intake>=0.7.0",
+    "intake-dataframe-catalog>=0.2.2",
     "intake-esm>=2023.4.20",
     "jsonschema",
     "pooch",
     "xarray",
 ]
 dynamic = ["version"]
```

### Comparing `access_nri_intake-0.0.4/src/access_nri_intake/esmcat/__init__.py` & `access_nri_intake-0.0.5/src/access_nri_intake/esmcat/__init__.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.4/src/access_nri_intake/esmcat/builders.py` & `access_nri_intake-0.0.5/src/access_nri_intake/esmcat/builders.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.4/src/access_nri_intake/esmcat/utils.py` & `access_nri_intake-0.0.5/src/access_nri_intake/esmcat/utils.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.4/src/access_nri_intake/metacat/__init__.py` & `access_nri_intake-0.0.5/src/access_nri_intake/metacat/__init__.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.4/src/access_nri_intake/metacat/manager.py` & `access_nri_intake-0.0.5/src/access_nri_intake/metacat/manager.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.4/src/access_nri_intake/metacat/translators.py` & `access_nri_intake-0.0.5/src/access_nri_intake/metacat/translators.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.4/src/access_nri_intake/utils.py` & `access_nri_intake-0.0.5/src/access_nri_intake/utils.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.4/src/access_nri_intake.egg-info/PKG-INFO` & `access_nri_intake-0.0.5/src/access_nri_intake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access-nri-intake
-Version: 0.0.4
+Version: 0.0.5
 Summary: Intake catalog managed by ACCESS-NRI and associated tools
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `access_nri_intake-0.0.4/src/access_nri_intake.egg-info/SOURCES.txt` & `access_nri_intake-0.0.5/src/access_nri_intake.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,13 @@
 src/access_nri_intake.egg-info/PKG-INFO
 src/access_nri_intake.egg-info/SOURCES.txt
 src/access_nri_intake.egg-info/dependency_links.txt
 src/access_nri_intake.egg-info/entry_points.txt
 src/access_nri_intake.egg-info/requires.txt
 src/access_nri_intake.egg-info/top_level.txt
 src/access_nri_intake/cat/__init__.py
-src/access_nri_intake/cat/metacatalog.yaml
 src/access_nri_intake/esmcat/__init__.py
 src/access_nri_intake/esmcat/builders.py
 src/access_nri_intake/esmcat/utils.py
 src/access_nri_intake/metacat/__init__.py
 src/access_nri_intake/metacat/manager.py
 src/access_nri_intake/metacat/translators.py
```

### Comparing `access_nri_intake-0.0.4/versioneer.py` & `access_nri_intake-0.0.5/versioneer.py`

 * *Files identical despite different names*

