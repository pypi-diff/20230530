# Comparing `tmp/objverify-1.0.0.tar.gz` & `tmp/objverify-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objverify-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "objverify-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `objverify-1.0.0.tar` & `objverify-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0        3 2023-03-02 23:37:45.689608 objverify-1.0.0/.vscode/settings.json
--rw-r--r--   0        0        0     1100 2023-05-29 16:59:44.011606 objverify-1.0.0/LICENSE
--rw-r--r--   0        0        0      223 2023-02-15 02:34:33.700634 objverify-1.0.0/README.md
--rw-r--r--   0        0        0     4682 2023-05-29 16:59:03.848393 objverify-1.0.0/objverify/__init__.py
--rw-r--r--   0        0        0      407 2023-05-29 16:59:53.047351 objverify-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      872 2023-03-03 22:57:57.906020 objverify-1.0.0/test.py
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 objverify-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-05-29 16:59:44.011606 objverify-1.0.1/LICENSE
+-rw-r--r--   0        0        0      223 2023-02-15 02:34:33.700634 objverify-1.0.1/README.md
+-rw-r--r--   0        0        0     4682 2023-05-30 02:21:12.435347 objverify-1.0.1/objverify/__init__.py
+-rw-r--r--   0        0        0      670 2023-05-30 02:20:11.606219 objverify-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      872 2023-03-03 22:57:57.906020 objverify-1.0.1/test.py
+-rw-r--r--   0        0        0      799 1970-01-01 00:00:00.000000 objverify-1.0.1/PKG-INFO
```

### Comparing `objverify-1.0.0/LICENSE` & `objverify-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `objverify-1.0.0/objverify/__init__.py` & `objverify-1.0.1/objverify/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Super useful library for Python object validation"""
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 import inspect # for more function validation later
 import copy
 from typing import Union
 
 AnyNumber = Union[int, float]
```

### Comparing `objverify-1.0.0/test.py` & `objverify-1.0.1/test.py`

 * *Files identical despite different names*

