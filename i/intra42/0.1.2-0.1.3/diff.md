# Comparing `tmp/intra42-0.1.2.tar.gz` & `tmp/intra42-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intra42-0.1.2.tar", last modified: Tue May 30 15:22:35 2023, max compression
+gzip compressed data, was "intra42-0.1.3.tar", last modified: Tue May 30 21:01:34 2023, max compression
```

## Comparing `intra42-0.1.2.tar` & `intra42-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-30 15:22:35.556726 intra42-0.1.2/
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-30 15:22:35.556726 intra42-0.1.2/PKG-INFO
-drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-30 15:22:35.556726 intra42-0.1.2/intra42.egg-info/
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-30 15:22:35.000000 intra42-0.1.2/intra42.egg-info/PKG-INFO
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      216 2023-05-30 15:22:35.000000 intra42-0.1.2/intra42.egg-info/SOURCES.txt
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)        1 2023-05-30 15:22:35.000000 intra42-0.1.2/intra42.egg-info/dependency_links.txt
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-30 15:22:35.000000 intra42-0.1.2/intra42.egg-info/requires.txt
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-30 15:22:35.000000 intra42-0.1.2/intra42.egg-info/top_level.txt
-drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-30 15:22:35.556726 intra42-0.1.2/intrascraper/
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      259 2023-05-30 15:15:57.000000 intra42-0.1.2/intrascraper/__init__.py
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)     5693 2023-05-30 15:15:22.000000 intra42-0.1.2/intrascraper/intrascraper.py
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       38 2023-05-30 15:22:35.556726 intra42-0.1.2/setup.cfg
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      437 2023-05-30 15:22:33.000000 intra42-0.1.2/setup.py
+drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-30 21:01:34.634703 intra42-0.1.3/
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-30 21:01:34.634703 intra42-0.1.3/PKG-INFO
+drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-30 21:01:34.634703 intra42-0.1.3/intra42.egg-info/
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-30 21:01:34.000000 intra42-0.1.3/intra42.egg-info/PKG-INFO
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      216 2023-05-30 21:01:34.000000 intra42-0.1.3/intra42.egg-info/SOURCES.txt
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)        1 2023-05-30 21:01:34.000000 intra42-0.1.3/intra42.egg-info/dependency_links.txt
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-30 21:01:34.000000 intra42-0.1.3/intra42.egg-info/requires.txt
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-30 21:01:34.000000 intra42-0.1.3/intra42.egg-info/top_level.txt
+drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-30 21:01:34.634703 intra42-0.1.3/intrascraper/
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      304 2023-05-30 21:00:14.000000 intra42-0.1.3/intrascraper/__init__.py
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)     5693 2023-05-30 15:15:22.000000 intra42-0.1.3/intrascraper/intrascraper.py
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       38 2023-05-30 21:01:34.634703 intra42-0.1.3/setup.cfg
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      437 2023-05-30 21:01:17.000000 intra42-0.1.3/setup.py
```

### Comparing `intra42-0.1.2/intrascraper/intrascraper.py` & `intra42-0.1.3/intrascraper/intrascraper.py`

 * *Files identical despite different names*

