# Comparing `tmp/proton-db-0.1.1.tar.gz` & `tmp/proton-db-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proton-db-0.1.1.tar", max compression
+gzip compressed data, was "proton-db-0.1.2.tar", max compression
```

## Comparing `proton-db-0.1.1.tar` & `proton-db-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1593 2023-05-30 19:59:58.477476 proton-db-0.1.1/proton_db/__init__.py
--rw-r--r--   0        0        0      295 2023-05-30 20:00:02.157471 proton-db-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      492 2023-05-30 20:00:09.877852 proton-db-0.1.1/setup.py
--rw-r--r--   0        0        0      239 2023-05-30 20:00:09.878173 proton-db-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1593 2023-05-30 20:03:26.393185 proton-db-0.1.2/proton_db/__init__.py
+-rw-r--r--   0        0        0      295 2023-05-30 20:03:29.009182 proton-db-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      492 2023-05-30 20:03:42.170100 proton-db-0.1.2/setup.py
+-rw-r--r--   0        0        0      239 2023-05-30 20:03:42.170386 proton-db-0.1.2/PKG-INFO
```

### Comparing `proton-db-0.1.1/proton_db/__init__.py` & `proton-db-0.1.2/proton_db/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 
 import requests, json
 #Api provided by https://protondb.max-p.me/
 class protonDB():
   def __init__(self,cache=True):
     self.api = "https://protondb.max-p.me/"
     self.cachingEnabled = cache
```

