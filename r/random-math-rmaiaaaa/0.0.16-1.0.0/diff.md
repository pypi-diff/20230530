# Comparing `tmp/random_math_rmaiaaaa-0.0.16.tar.gz` & `tmp/random_math_rmaiaaaa-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/random-math/random-math/dist/.tmp-95uuhm78/random_math_rmaiaaaa-0.0.16.tar", last modified: Mon May 29 23:11:00 2023, max compression
+gzip compressed data, was "/home/runner/work/random-math/random-math/dist/.tmp-inmwd0a_/random_math_rmaiaaaa-1.0.0.tar", last modified: Tue May 30 01:10:05 2023, max compression
```

## Comparing `random_math_rmaiaaaa-0.0.16.tar` & `random_math_rmaiaaaa-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:11:00.000000 random_math_rmaiaaaa-0.0.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-29 23:10:47.000000 random_math_rmaiaaaa-0.0.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 23:11:00.000000 random_math_rmaiaaaa-0.0.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 23:10:47.000000 random_math_rmaiaaaa-0.0.16/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 23:10:47.000000 random_math_rmaiaaaa-0.0.16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 23:11:00.000000 random_math_rmaiaaaa-0.0.16/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:11:00.000000 random_math_rmaiaaaa-0.0.16/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:11:00.000000 random_math_rmaiaaaa-0.0.16/src/RandomMath/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-29 23:10:47.000000 random_math_rmaiaaaa-0.0.16/src/RandomMath/RandomMathOperations.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 23:10:47.000000 random_math_rmaiaaaa-0.0.16/src/RandomMath/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:11:00.000000 random_math_rmaiaaaa-0.0.16/src/apiRandomMath/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:10:47.000000 random_math_rmaiaaaa-0.0.16/src/apiRandomMath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-29 23:10:47.000000 random_math_rmaiaaaa-0.0.16/src/apiRandomMath/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:11:00.000000 random_math_rmaiaaaa-0.0.16/src/random_math_rmaiaaaa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 23:11:00.000000 random_math_rmaiaaaa-0.0.16/src/random_math_rmaiaaaa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-29 23:11:00.000000 random_math_rmaiaaaa-0.0.16/src/random_math_rmaiaaaa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:11:00.000000 random_math_rmaiaaaa-0.0.16/src/random_math_rmaiaaaa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-29 23:11:00.000000 random_math_rmaiaaaa-0.0.16/src/random_math_rmaiaaaa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 01:10:05.000000 random_math_rmaiaaaa-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-30 01:09:50.000000 random_math_rmaiaaaa-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-30 01:10:05.000000 random_math_rmaiaaaa-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 01:09:50.000000 random_math_rmaiaaaa-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-30 01:09:50.000000 random_math_rmaiaaaa-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 01:10:05.000000 random_math_rmaiaaaa-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 01:10:05.000000 random_math_rmaiaaaa-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 01:10:05.000000 random_math_rmaiaaaa-1.0.0/src/RandomMath/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-30 01:09:50.000000 random_math_rmaiaaaa-1.0.0/src/RandomMath/RandomMathOperations.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 01:09:50.000000 random_math_rmaiaaaa-1.0.0/src/RandomMath/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 01:10:05.000000 random_math_rmaiaaaa-1.0.0/src/apiRandomMath/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 01:09:50.000000 random_math_rmaiaaaa-1.0.0/src/apiRandomMath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-30 01:09:50.000000 random_math_rmaiaaaa-1.0.0/src/apiRandomMath/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 01:10:05.000000 random_math_rmaiaaaa-1.0.0/src/random_math_rmaiaaaa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-30 01:10:05.000000 random_math_rmaiaaaa-1.0.0/src/random_math_rmaiaaaa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-30 01:10:05.000000 random_math_rmaiaaaa-1.0.0/src/random_math_rmaiaaaa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 01:10:05.000000 random_math_rmaiaaaa-1.0.0/src/random_math_rmaiaaaa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 01:10:05.000000 random_math_rmaiaaaa-1.0.0/src/random_math_rmaiaaaa.egg-info/top_level.txt
```

### Comparing `random_math_rmaiaaaa-0.0.16/LICENSE` & `random_math_rmaiaaaa-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `random_math_rmaiaaaa-0.0.16/PKG-INFO` & `random_math_rmaiaaaa-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: random_math_rmaiaaaa
-Version: 0.0.16
+Version: 1.0.0
 Summary: Random Math Package
 Author-email: Rafael Maia de Souza <rmaiadesouza@gmail.com>
 Project-URL: Homepage, https://github.com/rmaiaaaa/random-math
 Project-URL: Bug Tracker, https://github.com/rmaiaaaa/random-math/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `random_math_rmaiaaaa-0.0.16/pyproject.toml` & `random_math_rmaiaaaa-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "random_math_rmaiaaaa"
-version = "v0.0.16"
+version = "v1.0.0"
 authors = [
   { name="Rafael Maia de Souza", email="rmaiadesouza@gmail.com" },
 ]
 description = "Random Math Package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `random_math_rmaiaaaa-0.0.16/src/random_math_rmaiaaaa.egg-info/PKG-INFO` & `random_math_rmaiaaaa-1.0.0/src/random_math_rmaiaaaa.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: random-math-rmaiaaaa
-Version: 0.0.16
+Version: 1.0.0
 Summary: Random Math Package
 Author-email: Rafael Maia de Souza <rmaiadesouza@gmail.com>
 Project-URL: Homepage, https://github.com/rmaiaaaa/random-math
 Project-URL: Bug Tracker, https://github.com/rmaiaaaa/random-math/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

