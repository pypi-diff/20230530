# Comparing `tmp/asynciomultiplexer-1.0.tar.gz` & `tmp/asynciomultiplexer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asynciomultiplexer-1.0.tar", last modified: Mon May 29 23:04:47 2023, max compression
+gzip compressed data, was "asynciomultiplexer-1.0.1.tar", last modified: Mon May 29 23:40:40 2023, max compression
```

## Comparing `asynciomultiplexer-1.0.tar` & `asynciomultiplexer-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-05-29 23:04:47.623923 asynciomultiplexer-1.0/
--rw-rw-r--   0 pi        (1000) pi        (1000)     1490 2023-05-29 22:44:19.000000 asynciomultiplexer-1.0/LICENSE
--rw-rw-r--   0 pi        (1000) pi        (1000)       82 2023-05-29 23:04:47.623923 asynciomultiplexer-1.0/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      106 2023-05-29 22:44:19.000000 asynciomultiplexer-1.0/README.md
--rw-rw-r--   0 pi        (1000) pi        (1000)       38 2023-05-29 23:04:47.623923 asynciomultiplexer-1.0/setup.cfg
--rw-rw-r--   0 pi        (1000) pi        (1000)      306 2023-05-29 23:04:30.000000 asynciomultiplexer-1.0/setup.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-05-29 23:04:47.623923 asynciomultiplexer-1.0/src/
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-05-29 23:04:47.623923 asynciomultiplexer-1.0/src/asynciomultiplexer.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)       82 2023-05-29 23:04:47.000000 asynciomultiplexer-1.0/src/asynciomultiplexer.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      236 2023-05-29 23:04:47.000000 asynciomultiplexer-1.0/src/asynciomultiplexer.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-05-29 23:04:47.000000 asynciomultiplexer-1.0/src/asynciomultiplexer.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-05-29 23:04:47.000000 asynciomultiplexer-1.0/src/asynciomultiplexer.egg-info/top_level.txt
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-05-29 23:04:47.623923 asynciomultiplexer-1.0/test/
--rw-rw-r--   0 pi        (1000) pi        (1000)      524 2023-05-29 23:04:29.000000 asynciomultiplexer-1.0/test/test_multiplexing.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-05-29 23:40:40.125461 asynciomultiplexer-1.0.1/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1490 2023-05-29 22:44:19.000000 asynciomultiplexer-1.0.1/LICENSE
+-rw-rw-r--   0 pi        (1000) pi        (1000)      138 2023-05-29 23:40:40.125461 asynciomultiplexer-1.0.1/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      106 2023-05-29 22:44:19.000000 asynciomultiplexer-1.0.1/README.md
+-rw-rw-r--   0 pi        (1000) pi        (1000)       38 2023-05-29 23:40:40.125461 asynciomultiplexer-1.0.1/setup.cfg
+-rw-rw-r--   0 pi        (1000) pi        (1000)      345 2023-05-29 23:40:23.000000 asynciomultiplexer-1.0.1/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-05-29 23:40:40.125461 asynciomultiplexer-1.0.1/src/
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-05-29 23:40:40.125461 asynciomultiplexer-1.0.1/src/asynciomultiplexer/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4669 2023-05-29 23:40:23.000000 asynciomultiplexer-1.0.1/src/asynciomultiplexer/asynciomultiplexer.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-05-29 23:40:40.125461 asynciomultiplexer-1.0.1/src/asynciomultiplexer.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      138 2023-05-29 23:40:40.000000 asynciomultiplexer-1.0.1/src/asynciomultiplexer.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      281 2023-05-29 23:40:40.000000 asynciomultiplexer-1.0.1/src/asynciomultiplexer.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-05-29 23:40:40.000000 asynciomultiplexer-1.0.1/src/asynciomultiplexer.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       19 2023-05-29 23:40:40.000000 asynciomultiplexer-1.0.1/src/asynciomultiplexer.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-05-29 23:40:40.125461 asynciomultiplexer-1.0.1/test/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      524 2023-05-29 23:04:29.000000 asynciomultiplexer-1.0.1/test/test_multiplexing.py
```

### Comparing `asynciomultiplexer-1.0/LICENSE` & `asynciomultiplexer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asynciomultiplexer-1.0/test/test_multiplexing.py` & `asynciomultiplexer-1.0.1/test/test_multiplexing.py`

 * *Files identical despite different names*

