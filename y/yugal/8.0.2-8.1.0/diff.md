# Comparing `tmp/yugal-8.0.2.tar.gz` & `tmp/yugal-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yugal-8.0.2.tar", last modified: Tue May 30 12:57:24 2023, max compression
+gzip compressed data, was "yugal-8.1.0.tar", last modified: Tue May 30 13:09:51 2023, max compression
```

## Comparing `yugal-8.0.2.tar` & `yugal-8.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 vostro    (1000) vostro    (1000)        0 2023-05-30 12:57:24.768892 yugal-8.0.2/
--rw-rw-r--   0 vostro    (1000) vostro    (1000)      130 2023-05-30 12:57:24.768892 yugal-8.0.2/PKG-INFO
--rw-rw-r--   0 vostro    (1000) vostro    (1000)      836 2023-05-30 12:50:46.000000 yugal-8.0.2/README.md
--rw-rw-r--   0 vostro    (1000) vostro    (1000)       38 2023-05-30 12:57:24.768892 yugal-8.0.2/setup.cfg
--rwxrwxrwx   0 vostro    (1000) vostro    (1000)      269 2023-05-30 12:57:01.000000 yugal-8.0.2/setup.py
-drwxrwxr-x   0 vostro    (1000) vostro    (1000)        0 2023-05-30 12:57:24.764891 yugal-8.0.2/yugal.egg-info/
--rw-rw-r--   0 vostro    (1000) vostro    (1000)      130 2023-05-30 12:57:24.000000 yugal-8.0.2/yugal.egg-info/PKG-INFO
--rw-rw-r--   0 vostro    (1000) vostro    (1000)      194 2023-05-30 12:57:24.000000 yugal-8.0.2/yugal.egg-info/SOURCES.txt
--rw-rw-r--   0 vostro    (1000) vostro    (1000)        1 2023-05-30 12:57:24.000000 yugal-8.0.2/yugal.egg-info/dependency_links.txt
--rw-rw-r--   0 vostro    (1000) vostro    (1000)       39 2023-05-30 12:57:24.000000 yugal-8.0.2/yugal.egg-info/entry_points.txt
--rw-rw-r--   0 vostro    (1000) vostro    (1000)        6 2023-05-30 12:57:24.000000 yugal-8.0.2/yugal.egg-info/requires.txt
--rw-rw-r--   0 vostro    (1000) vostro    (1000)        1 2023-05-30 12:57:24.000000 yugal-8.0.2/yugal.egg-info/top_level.txt
+drwxrwxr-x   0 vostro    (1000) vostro    (1000)        0 2023-05-30 13:09:51.572701 yugal-8.1.0/
+-rw-rw-r--   0 vostro    (1000) vostro    (1000)      194 2023-05-30 13:09:51.572701 yugal-8.1.0/PKG-INFO
+-rw-rw-r--   0 vostro    (1000) vostro    (1000)      836 2023-05-30 12:50:46.000000 yugal-8.1.0/README.md
+-rw-rw-r--   0 vostro    (1000) vostro    (1000)       38 2023-05-30 13:09:51.572701 yugal-8.1.0/setup.cfg
+-rwxrwxrwx   0 vostro    (1000) vostro    (1000)      308 2023-05-30 13:09:35.000000 yugal-8.1.0/setup.py
+drwxrwxr-x   0 vostro    (1000) vostro    (1000)        0 2023-05-30 13:09:51.572701 yugal-8.1.0/yugal.egg-info/
+-rw-rw-r--   0 vostro    (1000) vostro    (1000)      194 2023-05-30 13:09:51.000000 yugal-8.1.0/yugal.egg-info/PKG-INFO
+-rw-rw-r--   0 vostro    (1000) vostro    (1000)      175 2023-05-30 13:09:51.000000 yugal-8.1.0/yugal.egg-info/SOURCES.txt
+-rw-rw-r--   0 vostro    (1000) vostro    (1000)        1 2023-05-30 13:09:51.000000 yugal-8.1.0/yugal.egg-info/dependency_links.txt
+-rw-rw-r--   0 vostro    (1000) vostro    (1000)       39 2023-05-30 13:09:51.000000 yugal-8.1.0/yugal.egg-info/entry_points.txt
+-rw-rw-r--   0 vostro    (1000) vostro    (1000)        6 2023-05-30 13:09:51.000000 yugal-8.1.0/yugal.egg-info/top_level.txt
+-rwxrwxrwx   0 vostro    (1000) vostro    (1000)     4578 2023-05-30 12:37:33.000000 yugal-8.1.0/yugal.py
```

### Comparing `yugal-8.0.2/README.md` & `yugal-8.1.0/README.md`

 * *Files identical despite different names*

