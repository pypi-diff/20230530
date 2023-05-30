# Comparing `tmp/py-xdrlib-4.0.0.tar.gz` & `tmp/py-xdrlib-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-xdrlib-4.0.0.tar", last modified: Wed Mar 15 05:07:09 2023, max compression
+gzip compressed data, was "py-xdrlib-4.0.1.tar", last modified: Tue May 30 03:06:20 2023, max compression
```

## Comparing `py-xdrlib-4.0.0.tar` & `py-xdrlib-4.0.1.tar`

### file list

```diff
@@ -1,4 +1,11 @@
--rw-r--r--   0        0        0        9 2023-03-15 01:19:58.087777 py-xdrlib-4.0.0/README.md
--rw-r--r--   0        0        0      630 2023-03-15 05:07:04.563830 py-xdrlib-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     5920 2023-03-15 01:37:01.618749 py-xdrlib-4.0.0/xdrlib.py
--rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 py-xdrlib-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0       26 2023-03-15 13:54:37.335946 py-xdrlib-4.0.1/.gitignore
+-rw-r--r--   0        0        0     2450 2023-03-15 07:03:17.027519 py-xdrlib-4.0.1/LICENSE
+-rw-r--r--   0        0        0     3055 2023-03-15 14:47:14.611252 py-xdrlib-4.0.1/README.md
+-rw-r--r--   0        0        0    38198 2023-03-15 13:48:09.891788 py-xdrlib-4.0.1/doc/rfc1014.txt
+-rw-r--r--   0        0        0    47418 2023-03-15 13:48:09.892480 py-xdrlib-4.0.1/doc/rfc1832.txt
+-rw-r--r--   0        0        0    55477 2023-03-15 13:48:09.893654 py-xdrlib-4.0.1/doc/rfc4506.txt
+-rw-r--r--   0        0        0      654 2023-05-30 03:06:06.249901 py-xdrlib-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2307 2023-03-15 14:07:46.390717 py-xdrlib-4.0.1/tests/test_xdrlib.py
+-rw-r--r--   0        0        0     5977 2023-03-15 06:58:51.126540 py-xdrlib-4.0.1/xdrlib.py
+-rw-r--r--   0        0        0     8220 2023-03-15 13:43:44.104251 py-xdrlib-4.0.1/xdrlib.rst
+-rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 py-xdrlib-4.0.1/PKG-INFO
```

### Comparing `py-xdrlib-4.0.0/pyproject.toml` & `py-xdrlib-4.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name = "py-xdrlib"
-version = "4.0.0"
+version = "4.0.1"
 authors = [
     { name = "David Arnold", email = "davida@pobox.com" },
 ]
 description = "Encode or decode XDR (IETF RFC-4506/1832/1014)"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: Python Software Foundation License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/da4089/py-xdrlib"
 "Bug Tracker" = "https://github.com/da4089/py-xdrlib/issues"
 
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [tool.flit.module]
-name = "xdrlib"
+name = "xdrlib"
```

### Comparing `py-xdrlib-4.0.0/xdrlib.py` & `py-xdrlib-4.0.1/xdrlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-"""Implements (a subset of) Sun XDR -- eXternal Data Representation."""
+"""Implements (a subset of) Sun XDR -- eXternal Data Representation.
 
-__version__ = "4.0.0"
+See: RFC 1014
+
+"""
 
 import struct
 from io import BytesIO
 from functools import wraps
+import warnings
 
+warnings._deprecated(__name__, remove=(3, 13))
 
 __all__ = ["Error", "Packer", "Unpacker", "ConversionError"]
 
 # exceptions
 class Error(Exception):
     """Exception class for this module. Use:
```

