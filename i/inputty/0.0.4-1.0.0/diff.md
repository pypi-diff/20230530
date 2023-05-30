# Comparing `tmp/inputty-0.0.4.tar.gz` & `tmp/inputty-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inputty-0.0.4.tar", last modified: Tue May  9 16:07:03 2023, max compression
+gzip compressed data, was "inputty-1.0.0.tar", last modified: Tue May 30 11:45:26 2023, max compression
```

## Comparing `inputty-0.0.4.tar` & `inputty-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-09 16:07:03.891454 inputty-0.0.4/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 inputty-0.0.4/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)      825 2023-05-09 16:07:03.891454 inputty-0.0.4/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)       96 2023-05-09 13:23:03.000000 inputty-0.0.4/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-09 16:07:03.888121 inputty-0.0.4/inputty/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      124 2023-05-09 13:45:56.000000 inputty-0.0.4/inputty/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-09 16:05:13.000000 inputty-0.0.4/inputty/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-09 16:07:03.891454 inputty-0.0.4/inputty/src/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 inputty-0.0.4/inputty/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     6491 2023-05-09 16:05:05.000000 inputty-0.0.4/inputty/src/input.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-09 16:07:03.891454 inputty-0.0.4/inputty.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      825 2023-05-09 16:07:03.000000 inputty-0.0.4/inputty.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      249 2023-05-09 16:07:03.000000 inputty-0.0.4/inputty.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-09 16:07:03.000000 inputty-0.0.4/inputty.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        8 2023-05-09 16:07:03.000000 inputty-0.0.4/inputty.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-09 16:07:03.891454 inputty-0.0.4/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1157 2023-05-09 13:25:02.000000 inputty-0.0.4/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-30 11:45:26.441095 inputty-1.0.0/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 inputty-1.0.0/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      898 2023-05-30 11:45:26.441095 inputty-1.0.0/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)       96 2023-05-09 13:23:03.000000 inputty-1.0.0/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-30 11:45:26.441095 inputty-1.0.0/inputty/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      124 2023-05-09 13:45:56.000000 inputty-1.0.0/inputty/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-30 11:44:18.000000 inputty-1.0.0/inputty/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-30 11:45:26.441095 inputty-1.0.0/inputty/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 inputty-1.0.0/inputty/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     7598 2023-05-30 11:43:57.000000 inputty-1.0.0/inputty/src/input.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-30 11:45:26.441095 inputty-1.0.0/inputty/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-29 12:23:03.000000 inputty-1.0.0/inputty/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3230 2023-05-30 11:09:18.000000 inputty-1.0.0/inputty/tests/test_input.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-30 11:45:26.441095 inputty-1.0.0/inputty.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      898 2023-05-30 11:45:26.000000 inputty-1.0.0/inputty.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      303 2023-05-30 11:45:26.000000 inputty-1.0.0/inputty.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-30 11:45:26.000000 inputty-1.0.0/inputty.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        8 2023-05-30 11:45:26.000000 inputty-1.0.0/inputty.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-30 11:45:26.444428 inputty-1.0.0/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1157 2023-05-09 13:25:02.000000 inputty-1.0.0/setup.py
```

### Comparing `inputty-0.0.4/LICENSE.txt` & `inputty-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inputty-0.0.4/PKG-INFO` & `inputty-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inputty
-Version: 0.0.4
+Version: 1.0.0
 Summary: """A collection of modules that supports cCLI inputs."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: cli,input
@@ -20,14 +20,21 @@
 ```bash
 pip install inputty
 ```
 
 
 # Version History
 
+Version 1.0.0 30 May 2023
+
+1. Major refactor
+2. Implement tests
+
+------
+
 Version 0.0.4 9 May 2023
 
 1. Fix integer index bug (in _get_valid_input_list)
 
 ------
 
 Version 0.0.3 9 May 2023
```

### Comparing `inputty-0.0.4/inputty.egg-info/PKG-INFO` & `inputty-1.0.0/inputty.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inputty
-Version: 0.0.4
+Version: 1.0.0
 Summary: """A collection of modules that supports cCLI inputs."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: cli,input
@@ -20,14 +20,21 @@
 ```bash
 pip install inputty
 ```
 
 
 # Version History
 
+Version 1.0.0 30 May 2023
+
+1. Major refactor
+2. Implement tests
+
+------
+
 Version 0.0.4 9 May 2023
 
 1. Fix integer index bug (in _get_valid_input_list)
 
 ------
 
 Version 0.0.3 9 May 2023
```

### Comparing `inputty-0.0.4/setup.py` & `inputty-1.0.0/setup.py`

 * *Files identical despite different names*

