# Comparing `tmp/readlog-1.1.0.tar.gz` & `tmp/readlog-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readlog-1.1.0.tar", last modified: Tue May 30 14:26:32 2023, max compression
+gzip compressed data, was "readlog-1.1.1.tar", last modified: Tue May 30 15:54:11 2023, max compression
```

## Comparing `readlog-1.1.0.tar` & `readlog-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 14:26:32.919185 readlog-1.1.0/
--rw-rw-rw-   0        0        0      225 2023-05-30 14:26:32.918177 readlog-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      553 2023-05-30 14:22:34.000000 readlog-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-30 14:26:32.919185 readlog-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      549 2023-05-30 14:21:12.000000 readlog-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 14:26:32.903128 readlog-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-30 14:26:32.912653 readlog-1.1.0/src/ReadLog.egg-info/
--rw-rw-rw-   0        0        0      225 2023-05-30 14:26:32.000000 readlog-1.1.0/src/ReadLog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-05-30 14:26:32.000000 readlog-1.1.0/src/ReadLog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 14:26:32.000000 readlog-1.1.0/src/ReadLog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-30 14:26:32.000000 readlog-1.1.0/src/ReadLog.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 14:26:32.000000 readlog-1.1.0/src/ReadLog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3029 2023-05-30 13:09:29.000000 readlog-1.1.0/src/ReadLog.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:54:11.010317 readlog-1.1.1/
+-rw-rw-rw-   0        0        0      780 2023-05-30 15:54:11.009331 readlog-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2023-05-30 14:22:34.000000 readlog-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-30 15:54:11.010317 readlog-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      710 2023-05-30 15:54:05.000000 readlog-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:54:10.992328 readlog-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 15:54:11.006322 readlog-1.1.1/src/readlog.egg-info/
+-rw-rw-rw-   0        0        0      780 2023-05-30 15:54:10.000000 readlog-1.1.1/src/readlog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-05-30 15:54:10.000000 readlog-1.1.1/src/readlog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 15:54:10.000000 readlog-1.1.1/src/readlog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-30 15:54:10.000000 readlog-1.1.1/src/readlog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 15:54:10.000000 readlog-1.1.1/src/readlog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3029 2023-05-30 13:09:29.000000 readlog-1.1.1/src/readlog.py
```

### Comparing `readlog-1.1.0/README.md` & `readlog-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `readlog-1.1.0/src/ReadLog.py` & `readlog-1.1.1/src/readlog.py`

 * *Files identical despite different names*

