# Comparing `tmp/yugal-8.0.0.tar.gz` & `tmp/yugal-8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yugal-8.0.0.tar", last modified: Tue May 30 12:44:09 2023, max compression
+gzip compressed data, was "yugal-8.0.1.tar", last modified: Tue May 30 12:51:22 2023, max compression
```

## Comparing `yugal-8.0.0.tar` & `yugal-8.0.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxr-x   0 vostro    (1000) vostro    (1000)        0 2023-05-30 12:44:09.021082 yugal-8.0.0/
--rw-rw-r--   0 vostro    (1000) vostro    (1000)      130 2023-05-30 12:44:09.021082 yugal-8.0.0/PKG-INFO
--rw-rw-r--   0 vostro    (1000) vostro    (1000)       38 2023-05-30 12:44:09.021082 yugal-8.0.0/setup.cfg
--rwxrwxrwx   0 vostro    (1000) vostro    (1000)      268 2023-05-30 12:44:06.000000 yugal-8.0.0/setup.py
-drwxrwxr-x   0 vostro    (1000) vostro    (1000)        0 2023-05-30 12:44:09.021082 yugal-8.0.0/yugal.egg-info/
--rw-rw-r--   0 vostro    (1000) vostro    (1000)      130 2023-05-30 12:44:08.000000 yugal-8.0.0/yugal.egg-info/PKG-INFO
--rw-rw-r--   0 vostro    (1000) vostro    (1000)      184 2023-05-30 12:44:08.000000 yugal-8.0.0/yugal.egg-info/SOURCES.txt
--rw-rw-r--   0 vostro    (1000) vostro    (1000)        1 2023-05-30 12:44:08.000000 yugal-8.0.0/yugal.egg-info/dependency_links.txt
--rw-rw-r--   0 vostro    (1000) vostro    (1000)       38 2023-05-30 12:44:08.000000 yugal-8.0.0/yugal.egg-info/entry_points.txt
--rw-rw-r--   0 vostro    (1000) vostro    (1000)        6 2023-05-30 12:44:08.000000 yugal-8.0.0/yugal.egg-info/requires.txt
--rw-rw-r--   0 vostro    (1000) vostro    (1000)        1 2023-05-30 12:44:08.000000 yugal-8.0.0/yugal.egg-info/top_level.txt
+drwxrwxr-x   0 vostro    (1000) vostro    (1000)        0 2023-05-30 12:51:22.456228 yugal-8.0.1/
+-rw-rw-r--   0 vostro    (1000) vostro    (1000)      130 2023-05-30 12:51:22.456228 yugal-8.0.1/PKG-INFO
+-rw-rw-r--   0 vostro    (1000) vostro    (1000)      836 2023-05-30 12:50:46.000000 yugal-8.0.1/README.md
+-rw-rw-r--   0 vostro    (1000) vostro    (1000)       38 2023-05-30 12:51:22.456228 yugal-8.0.1/setup.cfg
+-rwxrwxrwx   0 vostro    (1000) vostro    (1000)      268 2023-05-30 12:50:58.000000 yugal-8.0.1/setup.py
+drwxrwxr-x   0 vostro    (1000) vostro    (1000)        0 2023-05-30 12:51:22.452229 yugal-8.0.1/yugal.egg-info/
+-rw-rw-r--   0 vostro    (1000) vostro    (1000)      130 2023-05-30 12:51:22.000000 yugal-8.0.1/yugal.egg-info/PKG-INFO
+-rw-rw-r--   0 vostro    (1000) vostro    (1000)      194 2023-05-30 12:51:22.000000 yugal-8.0.1/yugal.egg-info/SOURCES.txt
+-rw-rw-r--   0 vostro    (1000) vostro    (1000)        1 2023-05-30 12:51:22.000000 yugal-8.0.1/yugal.egg-info/dependency_links.txt
+-rw-rw-r--   0 vostro    (1000) vostro    (1000)       38 2023-05-30 12:51:22.000000 yugal-8.0.1/yugal.egg-info/entry_points.txt
+-rw-rw-r--   0 vostro    (1000) vostro    (1000)        6 2023-05-30 12:51:22.000000 yugal-8.0.1/yugal.egg-info/requires.txt
+-rw-rw-r--   0 vostro    (1000) vostro    (1000)        1 2023-05-30 12:51:22.000000 yugal-8.0.1/yugal.egg-info/top_level.txt
```

