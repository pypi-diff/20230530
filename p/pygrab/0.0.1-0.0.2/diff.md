# Comparing `tmp/pygrab-0.0.1.tar.gz` & `tmp/pygrab-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrab-0.0.1.tar", last modified: Tue May 30 02:56:00 2023, max compression
+gzip compressed data, was "pygrab-0.0.2.tar", last modified: Tue May 30 03:21:07 2023, max compression
```

## Comparing `pygrab-0.0.1.tar` & `pygrab-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 02:56:00.993719 pygrab-0.0.1/
--rw-rw-rw-   0        0        0      183 2023-05-30 02:56:00.992958 pygrab-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-05-30 02:43:17.000000 pygrab-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 02:56:00.987506 pygrab-0.0.1/pygrab/
--rw-rw-rw-   0        0        0        0 2023-05-30 00:29:33.000000 pygrab-0.0.1/pygrab/__init__.py
--rw-rw-rw-   0        0        0     8586 2023-05-30 02:35:16.000000 pygrab-0.0.1/pygrab/pygrab.py
-drwxrwxrwx   0        0        0        0 2023-05-30 02:56:00.991862 pygrab-0.0.1/pygrab.egg-info/
--rw-rw-rw-   0        0        0      183 2023-05-30 02:56:00.000000 pygrab-0.0.1/pygrab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-05-30 02:56:00.000000 pygrab-0.0.1/pygrab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 02:56:00.000000 pygrab-0.0.1/pygrab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-30 02:56:00.000000 pygrab-0.0.1/pygrab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-30 02:56:00.000000 pygrab-0.0.1/pygrab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 02:56:00.993719 pygrab-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      343 2023-05-30 02:31:20.000000 pygrab-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 03:21:07.562798 pygrab-0.0.2/
+-rw-rw-rw-   0        0        0      183 2023-05-30 03:21:07.561640 pygrab-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-05-30 02:43:17.000000 pygrab-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 03:21:07.552008 pygrab-0.0.2/pygrab/
+-rw-rw-rw-   0        0        0       21 2023-05-30 03:16:15.000000 pygrab-0.0.2/pygrab/__init__.py
+-rw-rw-rw-   0        0        0     8586 2023-05-30 03:15:50.000000 pygrab-0.0.2/pygrab/pygrab.py
+drwxrwxrwx   0        0        0        0 2023-05-30 03:21:07.558308 pygrab-0.0.2/pygrab.egg-info/
+-rw-rw-rw-   0        0        0      183 2023-05-30 03:21:07.000000 pygrab-0.0.2/pygrab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-05-30 03:21:07.000000 pygrab-0.0.2/pygrab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 03:21:07.000000 pygrab-0.0.2/pygrab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-30 03:21:07.000000 pygrab-0.0.2/pygrab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-30 03:21:07.000000 pygrab-0.0.2/pygrab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 03:21:07.563289 pygrab-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      343 2023-05-30 03:20:34.000000 pygrab-0.0.2/setup.py
```

### Comparing `pygrab-0.0.1/pygrab/pygrab.py` & `pygrab-0.0.2/pygrab/pygrab.py`

 * *Files identical despite different names*

