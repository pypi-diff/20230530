# Comparing `tmp/lrservice-0.0.2.tar.gz` & `tmp/lrservice-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lrservice-0.0.2.tar", last modified: Mon May 29 15:44:40 2023, max compression
+gzip compressed data, was "lrservice-0.0.3.tar", last modified: Tue May 30 05:49:10 2023, max compression
```

## Comparing `lrservice-0.0.2.tar` & `lrservice-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,11 @@
-drwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-05-29 15:44:40.617577 lrservice-0.0.2/
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)     1054 2023-05-29 14:57:14.000000 lrservice-0.0.2/LICENSE
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)      601 2023-05-29 15:44:40.617271 lrservice-0.0.2/PKG-INFO
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)      130 2023-05-29 15:01:43.000000 lrservice-0.0.2/README.md
-drwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-05-29 15:44:40.614954 lrservice-0.0.2/lrservice/
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)      159 2023-05-29 15:44:10.000000 lrservice-0.0.2/lrservice/__init__.py
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)     1363 2022-02-16 23:54:46.000000 lrservice-0.0.2/lrservice/benchmark.py
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)     1882 2023-05-29 15:29:59.000000 lrservice-0.0.2/lrservice/main.py
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)     3416 2023-05-29 15:29:52.000000 lrservice-0.0.2/lrservice/simple_linear_regr.py
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)     1840 2023-05-29 15:36:07.000000 lrservice-0.0.2/lrservice/simple_linear_regr_utils.py
-drwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-05-29 15:44:40.616845 lrservice-0.0.2/lrservice.egg-info/
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)      601 2023-05-29 15:44:40.000000 lrservice-0.0.2/lrservice.egg-info/PKG-INFO
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)      291 2023-05-29 15:44:40.000000 lrservice-0.0.2/lrservice.egg-info/SOURCES.txt
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)        1 2023-05-29 15:44:40.000000 lrservice-0.0.2/lrservice.egg-info/dependency_links.txt
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)       10 2023-05-29 15:44:40.000000 lrservice-0.0.2/lrservice.egg-info/top_level.txt
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)       38 2023-05-29 15:44:40.617654 lrservice-0.0.2/setup.cfg
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)      679 2023-05-29 15:41:16.000000 lrservice-0.0.2/setup.py
+drwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-05-30 05:49:10.232677 lrservice-0.0.3/
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)      534 2023-05-30 05:49:10.232385 lrservice-0.0.3/PKG-INFO
+drwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-05-30 05:49:10.231239 lrservice-0.0.3/lrservice.egg-info/
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)      534 2023-05-30 05:49:10.000000 lrservice-0.0.3/lrservice.egg-info/PKG-INFO
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)      182 2023-05-30 05:49:10.000000 lrservice-0.0.3/lrservice.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)        1 2023-05-30 05:49:10.000000 lrservice-0.0.3/lrservice.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)        6 2023-05-30 05:49:10.000000 lrservice-0.0.3/lrservice.egg-info/top_level.txt
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)       38 2023-05-30 05:49:10.232760 lrservice-0.0.3/setup.cfg
+drwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-05-30 05:49:10.231979 lrservice-0.0.3/tests/
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-05-30 04:43:02.000000 lrservice-0.0.3/tests/__init__.py
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)      587 2023-05-30 05:01:17.000000 lrservice-0.0.3/tests/test_simple_linear_regr.py
```

### Comparing `lrservice-0.0.2/PKG-INFO` & `lrservice-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: lrservice
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package for demonstrating how to make REST API service for linear regression
 Home-page: https://github.com/CyberPlayerOne/lrservice
 Author: Tyler Tang
 Author-email: tyler.x.tang@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
-# Simple Linear Regression REST API
-This is a python package for demonstrating how to make REST API service for linear regression.
+A python package for demonstrating how to make REST API service for linear regression
```

### Comparing `lrservice-0.0.2/lrservice.egg-info/PKG-INFO` & `lrservice-0.0.3/lrservice.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: lrservice
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package for demonstrating how to make REST API service for linear regression
 Home-page: https://github.com/CyberPlayerOne/lrservice
 Author: Tyler Tang
 Author-email: tyler.x.tang@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
-# Simple Linear Regression REST API
-This is a python package for demonstrating how to make REST API service for linear regression.
+A python package for demonstrating how to make REST API service for linear regression
```

