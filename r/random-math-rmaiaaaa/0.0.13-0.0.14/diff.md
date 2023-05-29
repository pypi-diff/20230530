# Comparing `tmp/random_math_rmaiaaaa-0.0.13.tar.gz` & `tmp/random_math_rmaiaaaa-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/random-math/random-math/dist/.tmp-zixg_2eb/random_math_rmaiaaaa-0.0.13.tar", last modified: Mon May 29 20:47:49 2023, max compression
+gzip compressed data, was "/home/runner/work/random-math/random-math/dist/.tmp-boec1rxg/random_math_rmaiaaaa-0.0.14.tar", last modified: Mon May 29 22:03:40 2023, max compression
```

## Comparing `random_math_rmaiaaaa-0.0.13.tar` & `random_math_rmaiaaaa-0.0.14.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-29 20:47:37.000000 random_math_rmaiaaaa-0.0.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 20:47:37.000000 random_math_rmaiaaaa-0.0.13/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 20:47:37.000000 random_math_rmaiaaaa-0.0.13/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/src/RandomMath/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-29 20:47:37.000000 random_math_rmaiaaaa-0.0.13/src/RandomMath/RandomMathOperations.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 20:47:37.000000 random_math_rmaiaaaa-0.0.13/src/RandomMath/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/src/apiRandomMath/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 20:47:37.000000 random_math_rmaiaaaa-0.0.13/src/apiRandomMath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-29 20:47:37.000000 random_math_rmaiaaaa-0.0.13/src/apiRandomMath/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/src/random_math_rmaiaaaa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/src/random_math_rmaiaaaa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/src/random_math_rmaiaaaa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/src/random_math_rmaiaaaa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/src/random_math_rmaiaaaa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:03:40.000000 random_math_rmaiaaaa-0.0.14/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-29 22:03:27.000000 random_math_rmaiaaaa-0.0.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 22:03:40.000000 random_math_rmaiaaaa-0.0.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 22:03:27.000000 random_math_rmaiaaaa-0.0.14/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 22:03:27.000000 random_math_rmaiaaaa-0.0.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 22:03:40.000000 random_math_rmaiaaaa-0.0.14/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:03:40.000000 random_math_rmaiaaaa-0.0.14/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:03:40.000000 random_math_rmaiaaaa-0.0.14/src/RandomMath/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-29 22:03:27.000000 random_math_rmaiaaaa-0.0.14/src/RandomMath/RandomMathOperations.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 22:03:27.000000 random_math_rmaiaaaa-0.0.14/src/RandomMath/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:03:40.000000 random_math_rmaiaaaa-0.0.14/src/apiRandomMath/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:03:27.000000 random_math_rmaiaaaa-0.0.14/src/apiRandomMath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-29 22:03:27.000000 random_math_rmaiaaaa-0.0.14/src/apiRandomMath/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:03:40.000000 random_math_rmaiaaaa-0.0.14/src/random_math_rmaiaaaa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 22:03:40.000000 random_math_rmaiaaaa-0.0.14/src/random_math_rmaiaaaa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-29 22:03:40.000000 random_math_rmaiaaaa-0.0.14/src/random_math_rmaiaaaa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 22:03:40.000000 random_math_rmaiaaaa-0.0.14/src/random_math_rmaiaaaa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-29 22:03:40.000000 random_math_rmaiaaaa-0.0.14/src/random_math_rmaiaaaa.egg-info/top_level.txt
```

### Comparing `random_math_rmaiaaaa-0.0.13/LICENSE` & `random_math_rmaiaaaa-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `random_math_rmaiaaaa-0.0.13/PKG-INFO` & `random_math_rmaiaaaa-0.0.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: random_math_rmaiaaaa
-Version: 0.0.13
+Version: 0.0.14
 Summary: Random Math Package
 Author-email: Rafael Maia de Souza <rmaiadesouza@gmail.com>
 Project-URL: Homepage, https://github.com/rmaiaaaa/random-math
 Project-URL: Bug Tracker, https://github.com/rmaiaaaa/random-math/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `random_math_rmaiaaaa-0.0.13/pyproject.toml` & `random_math_rmaiaaaa-0.0.14/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "random_math_rmaiaaaa"
-version = "v0.0.13"
+version = "v0.0.14"
 authors = [
   { name="Rafael Maia de Souza", email="rmaiadesouza@gmail.com" },
 ]
 description = "Random Math Package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `random_math_rmaiaaaa-0.0.13/src/random_math_rmaiaaaa.egg-info/PKG-INFO` & `random_math_rmaiaaaa-0.0.14/src/random_math_rmaiaaaa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: random-math-rmaiaaaa
-Version: 0.0.13
+Version: 0.0.14
 Summary: Random Math Package
 Author-email: Rafael Maia de Souza <rmaiadesouza@gmail.com>
 Project-URL: Homepage, https://github.com/rmaiaaaa/random-math
 Project-URL: Bug Tracker, https://github.com/rmaiaaaa/random-math/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

