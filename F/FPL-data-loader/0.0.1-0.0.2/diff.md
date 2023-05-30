# Comparing `tmp/FPL-data-loader-0.0.1.tar.gz` & `tmp/FPL-data-loader-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FPL-data-loader-0.0.1.tar", last modified: Tue May 23 11:12:36 2023, max compression
+gzip compressed data, was "FPL-data-loader-0.0.2.tar", last modified: Tue May 30 20:53:12 2023, max compression
```

## Comparing `FPL-data-loader-0.0.1.tar` & `FPL-data-loader-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:12:36.715682 FPL-data-loader-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-23 11:12:22.000000 FPL-data-loader-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-23 11:12:36.715682 FPL-data-loader-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-23 11:12:22.000000 FPL-data-loader-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-23 11:12:22.000000 FPL-data-loader-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 11:12:36.715682 FPL-data-loader-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:12:36.711682 FPL-data-loader-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:12:36.715682 FPL-data-loader-0.0.1/src/FPL_data_loader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-23 11:12:36.000000 FPL-data-loader-0.0.1/src/FPL_data_loader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-23 11:12:36.000000 FPL-data-loader-0.0.1/src/FPL_data_loader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 11:12:36.000000 FPL-data-loader-0.0.1/src/FPL_data_loader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 11:12:36.000000 FPL-data-loader-0.0.1/src/FPL_data_loader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 11:12:36.000000 FPL-data-loader-0.0.1/src/FPL_data_loader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:53:12.947864 FPL-data-loader-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-30 20:52:45.000000 FPL-data-loader-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-30 20:53:12.947864 FPL-data-loader-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 20:52:45.000000 FPL-data-loader-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-30 20:52:45.000000 FPL-data-loader-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 20:53:12.947864 FPL-data-loader-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:53:12.943864 FPL-data-loader-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:53:12.947864 FPL-data-loader-0.0.2/src/FPL_data_loader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-30 20:53:12.000000 FPL-data-loader-0.0.2/src/FPL_data_loader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-30 20:53:12.000000 FPL-data-loader-0.0.2/src/FPL_data_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:53:12.000000 FPL-data-loader-0.0.2/src/FPL_data_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 20:53:12.000000 FPL-data-loader-0.0.2/src/FPL_data_loader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 20:53:12.000000 FPL-data-loader-0.0.2/src/FPL_data_loader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:53:12.947864 FPL-data-loader-0.0.2/src/fpl_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-30 20:52:45.000000 FPL-data-loader-0.0.2/src/fpl_data/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-30 20:52:45.000000 FPL-data-loader-0.0.2/src/fpl_data/utils.py
```

### Comparing `FPL-data-loader-0.0.1/LICENSE` & `FPL-data-loader-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FPL-data-loader-0.0.1/pyproject.toml` & `FPL-data-loader-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 requires = [
   "setuptools>=67"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "FPL-data-loader"
-version = "0.0.1"
+version = "0.0.2"
 description = "Tools for working with Fantasy Premier League data"
 authors = [
   { name="James Leslie", email="contactjamesleslie@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
-  "tqdm==4.65.0"
+  "tqdm==4.65.0",
+  "jsonschema==4.17.3"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/James-Leslie/fpl-data"
 "Bug Tracker" = "https://github.com/James-Leslie/fpl-data/issues"
 
 [tool.setuptools]
```

