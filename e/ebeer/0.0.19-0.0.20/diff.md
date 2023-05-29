# Comparing `tmp/ebeer-0.0.19.tar.gz` & `tmp/ebeer-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebeer-0.0.19.tar", last modified: Tue May 23 13:08:24 2023, max compression
+gzip compressed data, was "ebeer-0.0.20.tar", last modified: Mon May 29 23:08:02 2023, max compression
```

## Comparing `ebeer-0.0.19.tar` & `ebeer-0.0.20.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:08:24.554558 ebeer-0.0.19/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 13:07:14.000000 ebeer-0.0.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-23 13:07:14.000000 ebeer-0.0.19/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-23 13:08:24.554558 ebeer-0.0.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-23 13:07:14.000000 ebeer-0.0.19/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-23 13:07:14.000000 ebeer-0.0.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:08:24.554558 ebeer-0.0.19/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:08:24.546558 ebeer-0.0.19/src/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-23 13:07:14.000000 ebeer-0.0.19/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:08:24.546558 ebeer-0.0.19/src/ebeer/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-23 13:07:14.000000 ebeer-0.0.19/src/ebeer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-23 13:07:14.000000 ebeer-0.0.19/src/ebeer/beer_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12715 2023-05-23 13:07:14.000000 ebeer-0.0.19/src/ebeer/data_label.py
--rw-r--r--   0 runner    (1001) docker     (123)  6684424 2023-05-23 13:07:14.000000 ebeer-0.0.19/src/ebeer/trained_model.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:08:24.554558 ebeer-0.0.19/src/ebeer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-23 13:08:24.000000 ebeer-0.0.19/src/ebeer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-23 13:08:24.000000 ebeer-0.0.19/src/ebeer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:08:24.000000 ebeer-0.0.19/src/ebeer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-23 13:08:24.000000 ebeer-0.0.19/src/ebeer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 13:08:24.000000 ebeer-0.0.19/src/ebeer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:08:24.554558 ebeer-0.0.19/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-23 13:07:14.000000 ebeer-0.0.19/tests/test_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:08:02.784763 ebeer-0.0.20/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 23:06:43.000000 ebeer-0.0.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-29 23:06:43.000000 ebeer-0.0.20/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-29 23:08:02.784763 ebeer-0.0.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-29 23:06:43.000000 ebeer-0.0.20/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-29 23:06:43.000000 ebeer-0.0.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 23:08:02.784763 ebeer-0.0.20/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:08:02.776763 ebeer-0.0.20/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-29 23:06:43.000000 ebeer-0.0.20/src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:08:02.776763 ebeer-0.0.20/src/ebeer/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-29 23:06:43.000000 ebeer-0.0.20/src/ebeer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-29 23:06:43.000000 ebeer-0.0.20/src/ebeer/beer_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-29 23:06:43.000000 ebeer-0.0.20/src/ebeer/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)  6671560 2023-05-29 23:06:43.000000 ebeer-0.0.20/src/ebeer/trained_model.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:08:02.784763 ebeer-0.0.20/src/ebeer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-29 23:08:02.000000 ebeer-0.0.20/src/ebeer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-29 23:08:02.000000 ebeer-0.0.20/src/ebeer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:08:02.000000 ebeer-0.0.20/src/ebeer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-29 23:08:02.000000 ebeer-0.0.20/src/ebeer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 23:08:02.000000 ebeer-0.0.20/src/ebeer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:08:02.784763 ebeer-0.0.20/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-29 23:06:43.000000 ebeer-0.0.20/tests/test_classify.py
```

### Comparing `ebeer-0.0.19/LICENSE` & `ebeer-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `ebeer-0.0.19/PKG-INFO` & `ebeer-0.0.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebeer
-Version: 0.0.19
+Version: 0.0.20
 Summary: CNN Trained to predict brazilian beers
 Author-email: diego vasque maldonado <diegoomal13@gmail.com>
 Project-URL: Homepage, https://github.com/Diegoomal/proj_integrado_trabalho_final
 Project-URL: Bug Tracker, https://github.com/Diegoomal/proj_integrado_trabalho_final/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ebeer-0.0.19/pyproject.toml` & `ebeer-0.0.20/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.0", "wheel", "build"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ebeer"
-version = "0.0.19"
+version = "0.0.20"
 authors = [
     { name="diego vasque maldonado", email="diegoomal13@gmail.com" }
 ]
 description = "CNN Trained to predict brazilian beers"
 readme = "src/README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -32,8 +32,9 @@
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-file_cnn_weights = ["trained_model.h5"]
+file_cnn_weights = ["trained_model.h5"]
+metadata_json = ["general_metadata.json"]
```

### Comparing `ebeer-0.0.19/src/ebeer.egg-info/PKG-INFO` & `ebeer-0.0.20/src/ebeer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebeer
-Version: 0.0.19
+Version: 0.0.20
 Summary: CNN Trained to predict brazilian beers
 Author-email: diego vasque maldonado <diegoomal13@gmail.com>
 Project-URL: Homepage, https://github.com/Diegoomal/proj_integrado_trabalho_final
 Project-URL: Bug Tracker, https://github.com/Diegoomal/proj_integrado_trabalho_final/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

