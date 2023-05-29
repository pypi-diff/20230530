# Comparing `tmp/ebeer-0.0.20.tar.gz` & `tmp/ebeer-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebeer-0.0.20.tar", last modified: Mon May 29 23:08:02 2023, max compression
+gzip compressed data, was "ebeer-0.0.21.tar", last modified: Mon May 29 23:22:08 2023, max compression
```

## Comparing `ebeer-0.0.20.tar` & `ebeer-0.0.21.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:08:02.784763 ebeer-0.0.20/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 23:06:43.000000 ebeer-0.0.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-29 23:06:43.000000 ebeer-0.0.20/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-29 23:08:02.784763 ebeer-0.0.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-29 23:06:43.000000 ebeer-0.0.20/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-29 23:06:43.000000 ebeer-0.0.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 23:08:02.784763 ebeer-0.0.20/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:08:02.776763 ebeer-0.0.20/src/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-29 23:06:43.000000 ebeer-0.0.20/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:08:02.776763 ebeer-0.0.20/src/ebeer/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-29 23:06:43.000000 ebeer-0.0.20/src/ebeer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-29 23:06:43.000000 ebeer-0.0.20/src/ebeer/beer_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-29 23:06:43.000000 ebeer-0.0.20/src/ebeer/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)  6671560 2023-05-29 23:06:43.000000 ebeer-0.0.20/src/ebeer/trained_model.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:08:02.784763 ebeer-0.0.20/src/ebeer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-29 23:08:02.000000 ebeer-0.0.20/src/ebeer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-29 23:08:02.000000 ebeer-0.0.20/src/ebeer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:08:02.000000 ebeer-0.0.20/src/ebeer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-29 23:08:02.000000 ebeer-0.0.20/src/ebeer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 23:08:02.000000 ebeer-0.0.20/src/ebeer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:08:02.784763 ebeer-0.0.20/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-29 23:06:43.000000 ebeer-0.0.20/tests/test_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:22:08.541025 ebeer-0.0.21/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 23:20:39.000000 ebeer-0.0.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-29 23:20:39.000000 ebeer-0.0.21/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-29 23:22:08.537025 ebeer-0.0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-29 23:20:39.000000 ebeer-0.0.21/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-29 23:20:39.000000 ebeer-0.0.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 23:22:08.541025 ebeer-0.0.21/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:22:08.529024 ebeer-0.0.21/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-29 23:20:39.000000 ebeer-0.0.21/src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:22:08.529024 ebeer-0.0.21/src/ebeer/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-29 23:20:39.000000 ebeer-0.0.21/src/ebeer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-29 23:20:39.000000 ebeer-0.0.21/src/ebeer/beer_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-29 23:20:39.000000 ebeer-0.0.21/src/ebeer/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)  6671560 2023-05-29 23:20:39.000000 ebeer-0.0.21/src/ebeer/trained_model.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:22:08.537025 ebeer-0.0.21/src/ebeer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-29 23:22:08.000000 ebeer-0.0.21/src/ebeer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-29 23:22:08.000000 ebeer-0.0.21/src/ebeer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:22:08.000000 ebeer-0.0.21/src/ebeer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-29 23:22:08.000000 ebeer-0.0.21/src/ebeer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 23:22:08.000000 ebeer-0.0.21/src/ebeer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:22:08.537025 ebeer-0.0.21/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-29 23:20:39.000000 ebeer-0.0.21/tests/test_classify.py
```

### Comparing `ebeer-0.0.20/LICENSE` & `ebeer-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `ebeer-0.0.20/PKG-INFO` & `ebeer-0.0.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebeer
-Version: 0.0.20
+Version: 0.0.21
 Summary: CNN Trained to predict brazilian beers
 Author-email: diego vasque maldonado <diegoomal13@gmail.com>
 Project-URL: Homepage, https://github.com/Diegoomal/proj_integrado_trabalho_final
 Project-URL: Bug Tracker, https://github.com/Diegoomal/proj_integrado_trabalho_final/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ebeer-0.0.20/README.md` & `ebeer-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `ebeer-0.0.20/pyproject.toml` & `ebeer-0.0.21/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.0", "wheel", "build"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ebeer"
-version = "0.0.20"
+version = "0.0.21"
 authors = [
     { name="diego vasque maldonado", email="diegoomal13@gmail.com" }
 ]
 description = "CNN Trained to predict brazilian beers"
 readme = "src/README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ebeer-0.0.20/src/ebeer/beer_classifier.py` & `ebeer-0.0.21/src/ebeer/beer_classifier.py`

 * *Files identical despite different names*

### Comparing `ebeer-0.0.20/src/ebeer/metadata.json` & `ebeer-0.0.21/src/ebeer/metadata.json`

 * *Files identical despite different names*

### Comparing `ebeer-0.0.20/src/ebeer/trained_model.h5` & `ebeer-0.0.21/src/ebeer/trained_model.h5`

 * *Files identical despite different names*

### Comparing `ebeer-0.0.20/src/ebeer.egg-info/PKG-INFO` & `ebeer-0.0.21/src/ebeer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebeer
-Version: 0.0.20
+Version: 0.0.21
 Summary: CNN Trained to predict brazilian beers
 Author-email: diego vasque maldonado <diegoomal13@gmail.com>
 Project-URL: Homepage, https://github.com/Diegoomal/proj_integrado_trabalho_final
 Project-URL: Bug Tracker, https://github.com/Diegoomal/proj_integrado_trabalho_final/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ebeer-0.0.20/tests/test_classify.py` & `ebeer-0.0.21/tests/test_classify.py`

 * *Files identical despite different names*

