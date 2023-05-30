# Comparing `tmp/reversibledict-0.2.2.tar.gz` & `tmp/reversibledict-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reversibledict-0.2.2.tar", last modified: Tue May  9 11:20:05 2023, max compression
+gzip compressed data, was "reversibledict-0.2.3.tar", last modified: Tue May 30 19:05:31 2023, max compression
```

## Comparing `reversibledict-0.2.2.tar` & `reversibledict-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-09 11:20:05.315734 reversibledict-0.2.2/
--rw-r--r--   0 tkober     (502) staff       (20)     1078 2023-05-02 11:21:12.000000 reversibledict-0.2.2/LICENSE
--rw-r--r--   0 tkober     (502) staff       (20)       25 2023-05-02 10:51:35.000000 reversibledict-0.2.2/MANIFEST.in
--rw-r--r--   0 tkober     (502) staff       (20)     3670 2023-05-09 11:20:05.315485 reversibledict-0.2.2/PKG-INFO
--rw-r--r--   0 tkober     (502) staff       (20)     1583 2023-05-02 10:51:35.000000 reversibledict-0.2.2/README.md
--rw-r--r--   0 tkober     (502) staff       (20)      758 2023-05-09 11:17:53.000000 reversibledict-0.2.2/pyproject.toml
-drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-09 11:20:05.315044 reversibledict-0.2.2/reversibledict.egg-info/
--rw-r--r--   0 tkober     (502) staff       (20)     3670 2023-05-09 11:20:05.000000 reversibledict-0.2.2/reversibledict.egg-info/PKG-INFO
--rw-r--r--   0 tkober     (502) staff       (20)      293 2023-05-09 11:20:05.000000 reversibledict-0.2.2/reversibledict.egg-info/SOURCES.txt
--rw-r--r--   0 tkober     (502) staff       (20)        1 2023-05-09 11:20:05.000000 reversibledict-0.2.2/reversibledict.egg-info/dependency_links.txt
--rw-r--r--   0 tkober     (502) staff       (20)       39 2023-05-09 11:20:05.000000 reversibledict-0.2.2/reversibledict.egg-info/entry_points.txt
--rw-r--r--   0 tkober     (502) staff       (20)       39 2023-05-09 11:20:05.000000 reversibledict-0.2.2/reversibledict.egg-info/requires.txt
--rw-r--r--   0 tkober     (502) staff       (20)        1 2023-05-09 11:20:05.000000 reversibledict-0.2.2/reversibledict.egg-info/top_level.txt
--rw-r--r--   0 tkober     (502) staff       (20)       38 2023-05-09 11:20:05.315786 reversibledict-0.2.2/setup.cfg
--rw-r--r--   0 tkober     (502) staff       (20)     3165 2023-05-09 11:17:43.000000 reversibledict-0.2.2/setup.py
+drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-30 19:05:31.872759 reversibledict-0.2.3/
+-rw-r--r--   0 tkober     (502) staff       (20)     1078 2023-05-02 11:21:12.000000 reversibledict-0.2.3/LICENSE
+-rw-r--r--   0 tkober     (502) staff       (20)       25 2023-05-02 10:51:35.000000 reversibledict-0.2.3/MANIFEST.in
+-rw-r--r--   0 tkober     (502) staff       (20)     3670 2023-05-30 19:05:31.872528 reversibledict-0.2.3/PKG-INFO
+-rw-r--r--   0 tkober     (502) staff       (20)     1583 2023-05-02 10:51:35.000000 reversibledict-0.2.3/README.md
+-rw-r--r--   0 tkober     (502) staff       (20)      758 2023-05-30 19:04:43.000000 reversibledict-0.2.3/pyproject.toml
+drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-30 19:05:31.872163 reversibledict-0.2.3/reversibledict.egg-info/
+-rw-r--r--   0 tkober     (502) staff       (20)     3670 2023-05-30 19:05:31.000000 reversibledict-0.2.3/reversibledict.egg-info/PKG-INFO
+-rw-r--r--   0 tkober     (502) staff       (20)      293 2023-05-30 19:05:31.000000 reversibledict-0.2.3/reversibledict.egg-info/SOURCES.txt
+-rw-r--r--   0 tkober     (502) staff       (20)        1 2023-05-30 19:05:31.000000 reversibledict-0.2.3/reversibledict.egg-info/dependency_links.txt
+-rw-r--r--   0 tkober     (502) staff       (20)       39 2023-05-30 19:05:31.000000 reversibledict-0.2.3/reversibledict.egg-info/entry_points.txt
+-rw-r--r--   0 tkober     (502) staff       (20)       39 2023-05-30 19:05:31.000000 reversibledict-0.2.3/reversibledict.egg-info/requires.txt
+-rw-r--r--   0 tkober     (502) staff       (20)        1 2023-05-30 19:05:31.000000 reversibledict-0.2.3/reversibledict.egg-info/top_level.txt
+-rw-r--r--   0 tkober     (502) staff       (20)       38 2023-05-30 19:05:31.872824 reversibledict-0.2.3/setup.cfg
+-rw-r--r--   0 tkober     (502) staff       (20)     3165 2023-05-30 19:04:43.000000 reversibledict-0.2.3/setup.py
```

### Comparing `reversibledict-0.2.2/LICENSE` & `reversibledict-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reversibledict-0.2.2/PKG-INFO` & `reversibledict-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reversibledict
-Version: 0.2.2
+Version: 0.2.3
 Summary: Dictionary with value-key lookup ability
 Home-page: https://github.com/tttthomasssss/reversibledict
 Author: Thomas Kober
 Author-email: Thomas Kober <tttthomasssss@gmail.com>
 License: MIT License
         
         Copyright (c) 2017-this very day: Thomas
```

### Comparing `reversibledict-0.2.2/README.md` & `reversibledict-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `reversibledict-0.2.2/pyproject.toml` & `reversibledict-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reversibledict"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Thomas Kober", email="tttthomasssss@gmail.com" },
 ]
 description = "Dictionary with value-key lookup ability"
 readme = "Readme.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `reversibledict-0.2.2/reversibledict.egg-info/PKG-INFO` & `reversibledict-0.2.3/reversibledict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reversibledict
-Version: 0.2.2
+Version: 0.2.3
 Summary: Dictionary with value-key lookup ability
 Home-page: https://github.com/tttthomasssss/reversibledict
 Author: Thomas Kober
 Author-email: Thomas Kober <tttthomasssss@gmail.com>
 License: MIT License
         
         Copyright (c) 2017-this very day: Thomas
```

### Comparing `reversibledict-0.2.2/setup.py` & `reversibledict-0.2.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 setup(
 	name='reversibledict',
 
 	# Versions should comply with PEP440.  For a discussion on single-sourcing
 	# the version across setup.py and the project code, see
 	# https://packaging.python.org/en/latest/single_source_version.html
-	version='0.2.1',
+	version='0.2.3',
 
 	description='Reversible dict',
 	long_description=long_description,
 
 	# The project's main homepage.
 	url='https://github.com/tttthomasssss/reversibledict',
```

