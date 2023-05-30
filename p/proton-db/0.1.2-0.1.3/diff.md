# Comparing `tmp/proton-db-0.1.2.tar.gz` & `tmp/proton-db-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proton-db-0.1.2.tar", max compression
+gzip compressed data, was "proton-db-0.1.3.tar", max compression
```

## Comparing `proton-db-0.1.2.tar` & `proton-db-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     1593 2023-05-30 20:03:26.393185 proton-db-0.1.2/proton_db/__init__.py
--rw-r--r--   0        0        0      295 2023-05-30 20:03:29.009182 proton-db-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      492 2023-05-30 20:03:42.170100 proton-db-0.1.2/setup.py
--rw-r--r--   0        0        0      239 2023-05-30 20:03:42.170386 proton-db-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      577 2023-05-30 20:03:17.025198 proton-db-0.1.3/README.rst
+-rw-r--r--   0        0        0     1593 2023-05-30 20:08:14.248782 proton-db-0.1.3/proton_db/__init__.py
+-rw-r--r--   0        0        0      347 2023-05-30 20:08:10.904787 proton-db-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1127 2023-05-30 20:08:21.285067 proton-db-0.1.3/setup.py
+-rw-r--r--   0        0        0      873 2023-05-30 20:08:21.285457 proton-db-0.1.3/PKG-INFO
```

### Comparing `proton-db-0.1.2/proton_db/__init__.py` & `proton-db-0.1.3/proton_db/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 import requests, json
 #Api provided by https://protondb.max-p.me/
 class protonDB():
   def __init__(self,cache=True):
     self.api = "https://protondb.max-p.me/"
     self.cachingEnabled = cache
```

