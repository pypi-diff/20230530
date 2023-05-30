# Comparing `tmp/meilisearchdsl-0.1.6.tar.gz` & `tmp/meilisearchdsl-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearchdsl-0.1.6.tar", last modified: Tue May 30 09:20:00 2023, max compression
+gzip compressed data, was "meilisearchdsl-0.1.7.tar", last modified: Tue May 30 10:06:41 2023, max compression
```

## Comparing `meilisearchdsl-0.1.6.tar` & `meilisearchdsl-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:20:00.416088 meilisearchdsl-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-30 09:19:44.000000 meilisearchdsl-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-30 09:20:00.416088 meilisearchdsl-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-30 09:19:44.000000 meilisearchdsl-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:20:00.416088 meilisearchdsl-0.1.6/meilisearchdsl/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-30 09:19:44.000000 meilisearchdsl-0.1.6/meilisearchdsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-30 09:19:44.000000 meilisearchdsl-0.1.6/meilisearchdsl/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-05-30 09:19:44.000000 meilisearchdsl-0.1.6/meilisearchdsl/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-30 09:19:44.000000 meilisearchdsl-0.1.6/meilisearchdsl/index_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-05-30 09:19:44.000000 meilisearchdsl-0.1.6/meilisearchdsl/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-30 09:19:44.000000 meilisearchdsl-0.1.6/meilisearchdsl/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:20:00.416088 meilisearchdsl-0.1.6/meilisearchdsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-30 09:20:00.000000 meilisearchdsl-0.1.6/meilisearchdsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-30 09:20:00.000000 meilisearchdsl-0.1.6/meilisearchdsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:20:00.000000 meilisearchdsl-0.1.6/meilisearchdsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 09:20:00.000000 meilisearchdsl-0.1.6/meilisearchdsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 09:20:00.000000 meilisearchdsl-0.1.6/meilisearchdsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 09:20:00.416088 meilisearchdsl-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-30 09:19:51.000000 meilisearchdsl-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:41.462048 meilisearchdsl-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-30 10:06:27.000000 meilisearchdsl-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-30 10:06:41.462048 meilisearchdsl-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-30 10:06:27.000000 meilisearchdsl-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:41.462048 meilisearchdsl-0.1.7/meilisearchdsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-30 10:06:27.000000 meilisearchdsl-0.1.7/meilisearchdsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-30 10:06:27.000000 meilisearchdsl-0.1.7/meilisearchdsl/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24142 2023-05-30 10:06:27.000000 meilisearchdsl-0.1.7/meilisearchdsl/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-30 10:06:27.000000 meilisearchdsl-0.1.7/meilisearchdsl/index_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-05-30 10:06:27.000000 meilisearchdsl-0.1.7/meilisearchdsl/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-30 10:06:27.000000 meilisearchdsl-0.1.7/meilisearchdsl/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:41.462048 meilisearchdsl-0.1.7/meilisearchdsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-30 10:06:41.000000 meilisearchdsl-0.1.7/meilisearchdsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-30 10:06:41.000000 meilisearchdsl-0.1.7/meilisearchdsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:06:41.000000 meilisearchdsl-0.1.7/meilisearchdsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 10:06:41.000000 meilisearchdsl-0.1.7/meilisearchdsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 10:06:41.000000 meilisearchdsl-0.1.7/meilisearchdsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:06:41.462048 meilisearchdsl-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-30 10:06:33.000000 meilisearchdsl-0.1.7/setup.py
```

### Comparing `meilisearchdsl-0.1.6/LICENSE` & `meilisearchdsl-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearchdsl-0.1.6/PKG-INFO` & `meilisearchdsl-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearchdsl
-Version: 0.1.6
+Version: 0.1.7
 Summary: MeiliSearch DSL is a Python package providing a Django-like Q object syntax for querying MeiliSearch, an open-source search engine. It simplifies search query building and offers a convenient wrapper for MeiliSearch indexes and clients, streamlining search interactions and improving maintainability.
 Home-page: https://github.com/UnattendedFlight/meilisearch-dsl
 Author: Adrian Leo
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `meilisearchdsl-0.1.6/README.md` & `meilisearchdsl-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `meilisearchdsl-0.1.6/meilisearchdsl/client.py` & `meilisearchdsl-0.1.7/meilisearchdsl/client.py`

 * *Files identical despite different names*

### Comparing `meilisearchdsl-0.1.6/meilisearchdsl/index.py` & `meilisearchdsl-0.1.7/meilisearchdsl/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from typing import Any, Dict, List, Optional, Union
 
 import meilisearch
 from meilisearch.errors import MeilisearchApiError
 from meilisearch.index import Index
 from meilisearch.models.task import TaskInfo, Task
 
+from .index_query import IndexSearch
+
 from .query import Q
 
 
 class MeiliIndex:
     """MeiliIndex class."""
 
     def __init__(self, index_name: str, client: meilisearch.Client, primary_key: str):
```

### Comparing `meilisearchdsl-0.1.6/meilisearchdsl/index_query.py` & `meilisearchdsl-0.1.7/meilisearchdsl/index_query.py`

 * *Files identical despite different names*

### Comparing `meilisearchdsl-0.1.6/meilisearchdsl/query.py` & `meilisearchdsl-0.1.7/meilisearchdsl/query.py`

 * *Files identical despite different names*

### Comparing `meilisearchdsl-0.1.6/meilisearchdsl/test.py` & `meilisearchdsl-0.1.7/meilisearchdsl/test.py`

 * *Files identical despite different names*

### Comparing `meilisearchdsl-0.1.6/meilisearchdsl.egg-info/PKG-INFO` & `meilisearchdsl-0.1.7/meilisearchdsl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearchdsl
-Version: 0.1.6
+Version: 0.1.7
 Summary: MeiliSearch DSL is a Python package providing a Django-like Q object syntax for querying MeiliSearch, an open-source search engine. It simplifies search query building and offers a convenient wrapper for MeiliSearch indexes and clients, streamlining search interactions and improving maintainability.
 Home-page: https://github.com/UnattendedFlight/meilisearch-dsl
 Author: Adrian Leo
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `meilisearchdsl-0.1.6/setup.py` & `meilisearchdsl-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pylint: disable=missing-docstring, invalid-name, line-too-long, R1732
 from setuptools import setup, find_packages
 
 setup(
     name="meilisearchdsl",
-    version="0.1.6",
+    version="0.1.7",
     description="MeiliSearch DSL is a Python package providing a Django-like Q object syntax for"
     + " querying MeiliSearch, an open-source search engine."
     + " It simplifies search query building and offers a convenient wrapper"
     + " for MeiliSearch indexes and clients, streamlining search interactions"
     + " and improving maintainability.",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
```

