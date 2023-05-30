# Comparing `tmp/podsearchmp-0.1.4.tar.gz` & `tmp/podsearchmp-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podsearchmp-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "podsearchmp-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `podsearchmp-0.1.4.tar` & `podsearchmp-0.1.5.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     1101 2023-05-30 18:20:36.385143 podsearchmp-0.1.4/LICENSE
--rw-r--r--   0        0        0      692 2023-05-30 19:16:15.427343 podsearchmp-0.1.4/podsearchmp/__init__.py
--rw-r--r--   0        0        0      433 2023-05-30 19:16:09.005407 podsearchmp-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      258 1970-01-01 00:00:00.000000 podsearchmp-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-05-30 18:20:36.385143 podsearchmp-0.1.5/LICENSE
+-rw-r--r--   0        0        0      266 2023-05-30 19:14:38.588419 podsearchmp-0.1.5/README.md
+-rw-r--r--   0        0        0      692 2023-05-30 19:19:46.936888 podsearchmp-0.1.5/podsearchmp/__init__.py
+-rw-r--r--   0        0        0      423 2023-05-30 19:19:42.087889 podsearchmp-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 podsearchmp-0.1.5/PKG-INFO
```

### Comparing `podsearchmp-0.1.4/LICENSE` & `podsearchmp-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `podsearchmp-0.1.4/podsearchmp/__init__.py` & `podsearchmp-0.1.5/podsearchmp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from cgi import parse
 from dataclasses import dataclass
 from typing import Optional, List
 
 from requests import get
 
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 
 SEARCH_URL = "https://itunes.apple.com/search"
 
 @dataclass
 class Podcast:
     """Podcast metadata."""
```

