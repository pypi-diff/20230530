# Comparing `tmp/smartdash-0.0.1.dev4.tar.gz` & `tmp/smartdash-0.0.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartdash-0.0.1.dev4.tar", last modified: Wed May 24 17:15:49 2023, max compression
+gzip compressed data, was "smartdash-0.0.1.dev5.tar", last modified: Tue May 30 10:15:46 2023, max compression
```

## Comparing `smartdash-0.0.1.dev4.tar` & `smartdash-0.0.1.dev5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:15:49.490669 smartdash-0.0.1.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-24 17:15:49.490669 smartdash-0.0.1.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 17:15:49.490669 smartdash-0.0.1.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-24 17:15:40.000000 smartdash-0.0.1.dev4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:15:49.486669 smartdash-0.0.1.dev4/smartdash/
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-24 17:15:40.000000 smartdash-0.0.1.dev4/smartdash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-24 17:15:40.000000 smartdash-0.0.1.dev4/smartdash/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-05-24 17:15:40.000000 smartdash-0.0.1.dev4/smartdash/dash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-05-24 17:15:40.000000 smartdash-0.0.1.dev4/smartdash/smartdash_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:15:49.490669 smartdash-0.0.1.dev4/smartdash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-24 17:15:49.000000 smartdash-0.0.1.dev4/smartdash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-24 17:15:49.000000 smartdash-0.0.1.dev4/smartdash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:15:49.000000 smartdash-0.0.1.dev4/smartdash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-24 17:15:49.000000 smartdash-0.0.1.dev4/smartdash.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-24 17:15:49.000000 smartdash-0.0.1.dev4/smartdash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 17:15:49.000000 smartdash-0.0.1.dev4/smartdash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:15:46.599138 smartdash-0.0.1.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-30 10:15:46.599138 smartdash-0.0.1.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:15:46.599138 smartdash-0.0.1.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-30 10:15:34.000000 smartdash-0.0.1.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:15:46.595138 smartdash-0.0.1.dev5/smartdash/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-30 10:15:34.000000 smartdash-0.0.1.dev5/smartdash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 10:15:34.000000 smartdash-0.0.1.dev5/smartdash/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-30 10:15:34.000000 smartdash-0.0.1.dev5/smartdash/dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-05-30 10:15:34.000000 smartdash-0.0.1.dev5/smartdash/smartdash_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:15:46.599138 smartdash-0.0.1.dev5/smartdash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-30 10:15:46.000000 smartdash-0.0.1.dev5/smartdash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-30 10:15:46.000000 smartdash-0.0.1.dev5/smartdash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:15:46.000000 smartdash-0.0.1.dev5/smartdash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-30 10:15:46.000000 smartdash-0.0.1.dev5/smartdash.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-30 10:15:46.000000 smartdash-0.0.1.dev5/smartdash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 10:15:46.000000 smartdash-0.0.1.dev5/smartdash.egg-info/top_level.txt
```

### Comparing `smartdash-0.0.1.dev4/PKG-INFO` & `smartdash-0.0.1.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdash
-Version: 0.0.1.dev4
+Version: 0.0.1.dev5
 Summary: python logging client for SmartDash
 Home-page: https://github.com/notAI-tech/smartdash
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `smartdash-0.0.1.dev4/setup.py` & `smartdash-0.0.1.dev5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "smartdash"
 DESCRIPTION = "python logging client for SmartDash"
 URL = "https://github.com/notAI-tech/smartdash"
 EMAIL = "praneeth@bpraneeth.com"
 AUTHOR = "BEDAPUDI PRANEETH"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.1.dev4"
+VERSION = "0.0.1.dev5"
 
 # What packages are required for this module to be executed?
 REQUIRED = ["requests", "liteindex", "streamlit", "plotly"]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

### Comparing `smartdash-0.0.1.dev4/smartdash.egg-info/PKG-INFO` & `smartdash-0.0.1.dev5/smartdash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdash
-Version: 0.0.1.dev4
+Version: 0.0.1.dev5
 Summary: python logging client for SmartDash
 Home-page: https://github.com/notAI-tech/smartdash
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

