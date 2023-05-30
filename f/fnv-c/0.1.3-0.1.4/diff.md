# Comparing `tmp/fnv-c-0.1.3.tar.gz` & `tmp/fnv-c-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fnv-c-0.1.3.tar", last modified: Tue May 30 14:58:32 2023, max compression
+gzip compressed data, was "dist/fnv-c-0.1.4.tar", last modified: Tue May 30 15:55:23 2023, max compression
```

## Comparing `fnv-c-0.1.3.tar` & `fnv-c-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:32.000000 fnv-c-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-30 14:58:32.000000 fnv-c-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-30 14:58:21.000000 fnv-c-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:32.000000 fnv-c-0.1.3/fnv_c/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-30 14:58:21.000000 fnv-c-0.1.3/fnv_c/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:32.000000 fnv-c-0.1.3/fnv_c/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:21.000000 fnv-c-0.1.3/fnv_c/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-30 14:58:21.000000 fnv-c-0.1.3/fnv_c/ext/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-30 14:58:21.000000 fnv-c-0.1.3/fnv_c/ext/fnv.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:32.000000 fnv-c-0.1.3/fnv_c.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-30 14:58:32.000000 fnv-c-0.1.3/fnv_c.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-30 14:58:32.000000 fnv-c-0.1.3/fnv_c.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:58:32.000000 fnv-c-0.1.3/fnv_c.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 14:58:32.000000 fnv-c-0.1.3/fnv_c.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 14:58:32.000000 fnv-c-0.1.3/fnv_c.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-30 14:58:21.000000 fnv-c-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:58:32.000000 fnv-c-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-30 14:58:32.000000 fnv-c-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:55:23.000000 fnv-c-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-30 15:55:09.000000 fnv-c-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-30 15:55:23.000000 fnv-c-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-30 15:55:09.000000 fnv-c-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:55:23.000000 fnv-c-0.1.4/fnv_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-30 15:55:09.000000 fnv-c-0.1.4/fnv_c/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:55:23.000000 fnv-c-0.1.4/fnv_c/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:55:09.000000 fnv-c-0.1.4/fnv_c/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-30 15:55:09.000000 fnv-c-0.1.4/fnv_c/ext/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-30 15:55:09.000000 fnv-c-0.1.4/fnv_c/ext/fnv.c
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-30 15:55:09.000000 fnv-c-0.1.4/fnv_c/ext/fnv.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:55:23.000000 fnv-c-0.1.4/fnv_c.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-30 15:55:23.000000 fnv-c-0.1.4/fnv_c.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-30 15:55:23.000000 fnv-c-0.1.4/fnv_c.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:55:23.000000 fnv-c-0.1.4/fnv_c.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 15:55:23.000000 fnv-c-0.1.4/fnv_c.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 15:55:23.000000 fnv-c-0.1.4/fnv_c.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-30 15:55:09.000000 fnv-c-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 15:55:23.000000 fnv-c-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-30 15:55:21.000000 fnv-c-0.1.4/setup.py
```

### Comparing `fnv-c-0.1.3/PKG-INFO` & `fnv-c-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnv-c
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python 3.7+ FNV (fnv0, fnv1, fnv1a) non-cryptographic hash library implemented in C through libffi
 Home-page: https://github.com/botify-labs/fnv-c
 Author: Fabien MARTY
 Author-email: fabien.marty@botify.com
 License: UNKNOWN
 Description: # fnv-c
```

### Comparing `fnv-c-0.1.3/README.md` & `fnv-c-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fnv-c-0.1.3/fnv_c/__init__.py` & `fnv-c-0.1.4/fnv_c/__init__.py`

 * *Files identical despite different names*

### Comparing `fnv-c-0.1.3/fnv_c/ext/fnv.c` & `fnv-c-0.1.4/fnv_c/ext/fnv.c`

 * *Files identical despite different names*

### Comparing `fnv-c-0.1.3/fnv_c.egg-info/PKG-INFO` & `fnv-c-0.1.4/fnv_c.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnv-c
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python 3.7+ FNV (fnv0, fnv1, fnv1a) non-cryptographic hash library implemented in C through libffi
 Home-page: https://github.com/botify-labs/fnv-c
 Author: Fabien MARTY
 Author-email: fabien.marty@botify.com
 License: UNKNOWN
 Description: # fnv-c
```

### Comparing `fnv-c-0.1.3/setup.py` & `fnv-c-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.1.3"
+VERSION = "0.1.4"
 
 DESCRIPTION = "Python 3.7+ FNV (fnv0, fnv1, fnv1a) non-cryptographic hash library implemented in C through libffi"
 with open("README.md") as f:
     LONG_DESCRIPTION = f.read()
 
 
 setup(
```

