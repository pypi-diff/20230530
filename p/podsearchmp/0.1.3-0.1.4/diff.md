# Comparing `tmp/podsearchmp-0.1.3.tar.gz` & `tmp/podsearchmp-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podsearchmp-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "podsearchmp-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `podsearchmp-0.1.3.tar` & `podsearchmp-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1101 2023-05-30 18:20:36.385143 podsearchmp-0.1.3/LICENSE
--rw-r--r--   0        0        0      692 2023-05-30 19:12:43.329279 podsearchmp-0.1.3/podsearchmp/__init__.py
--rw-r--r--   0        0        0      463 2023-05-30 19:12:17.484515 podsearchmp-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      235 1970-01-01 00:00:00.000000 podsearchmp-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-05-30 18:20:36.385143 podsearchmp-0.1.4/LICENSE
+-rw-r--r--   0        0        0      692 2023-05-30 19:16:15.427343 podsearchmp-0.1.4/podsearchmp/__init__.py
+-rw-r--r--   0        0        0      433 2023-05-30 19:16:09.005407 podsearchmp-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      258 1970-01-01 00:00:00.000000 podsearchmp-0.1.4/PKG-INFO
```

### Comparing `podsearchmp-0.1.3/LICENSE` & `podsearchmp-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `podsearchmp-0.1.3/podsearchmp/__init__.py` & `podsearchmp-0.1.4/podsearchmp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from cgi import parse
 from dataclasses import dataclass
 from typing import Optional, List
 
 from requests import get
 
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 
 SEARCH_URL = "https://itunes.apple.com/search"
 
 @dataclass
 class Podcast:
     """Podcast metadata."""
```

