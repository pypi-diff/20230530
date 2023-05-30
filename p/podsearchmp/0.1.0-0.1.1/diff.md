# Comparing `tmp/podsearchmp-0.1.0.tar.gz` & `tmp/podsearchmp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podsearchmp-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "podsearchmp-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `podsearchmp-0.1.0.tar` & `podsearchmp-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1101 2023-05-30 18:20:36.385143 podsearchmp-0.1.0/LICENSE
--rw-r--r--   0        0        0      692 2023-05-30 19:00:43.716977 podsearchmp-0.1.0/podsearchmp/__init__.py
--rw-r--r--   0        0        0      372 2023-05-30 18:20:36.386143 podsearchmp-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      235 1970-01-01 00:00:00.000000 podsearchmp-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-05-30 18:20:36.385143 podsearchmp-0.1.1/LICENSE
+-rw-r--r--   0        0        0      692 2023-05-30 19:05:15.406876 podsearchmp-0.1.1/podsearchmp/__init__.py
+-rw-r--r--   0        0        0      431 2023-05-30 19:05:06.636342 podsearchmp-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      235 1970-01-01 00:00:00.000000 podsearchmp-0.1.1/PKG-INFO
```

### Comparing `podsearchmp-0.1.0/LICENSE` & `podsearchmp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `podsearchmp-0.1.0/podsearchmp/__init__.py` & `podsearchmp-0.1.1/podsearchmp/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from cgi import parse
 from dataclasses import dataclass
 from typing import Optional, List
 
 from requests import get
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 
 SEARCH_URL = "https://itunes.apple.com/search"
 
 @dataclass
 class Podcast:
     """Podcast metadata."""
```

