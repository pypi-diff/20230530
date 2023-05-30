# Comparing `tmp/api_limit-0.0.1.tar.gz` & `tmp/api_limit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_limit-0.0.1.tar", last modified: Tue May 30 12:02:22 2023, max compression
+gzip compressed data, was "api_limit-0.0.2.tar", last modified: Tue May 30 13:04:45 2023, max compression
```

## Comparing `api_limit-0.0.1.tar` & `api_limit-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)        0 2023-05-30 12:02:22.764914 api_limit-0.0.1/
--rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)      151 2023-05-30 12:02:22.760914 api_limit-0.0.1/PKG-INFO
--rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)        0 2023-05-29 06:37:49.000000 api_limit-0.0.1/README.md
-drwxr-xr-x   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)        0 2023-05-30 12:02:22.760914 api_limit-0.0.1/api_limit/
--rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)       87 2023-05-26 08:39:23.000000 api_limit-0.0.1/api_limit/__init__.py
--rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)     1828 2023-05-29 06:53:50.000000 api_limit-0.0.1/api_limit/algorithm.py
--rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)      942 2023-05-29 05:02:46.000000 api_limit-0.0.1/api_limit/main.py
-drwxr-xr-x   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)        0 2023-05-30 12:02:22.760914 api_limit-0.0.1/api_limit.egg-info/
--rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)      151 2023-05-30 12:02:22.000000 api_limit-0.0.1/api_limit.egg-info/PKG-INFO
--rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)      213 2023-05-30 12:02:22.000000 api_limit-0.0.1/api_limit.egg-info/SOURCES.txt
--rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)        1 2023-05-30 12:02:22.000000 api_limit-0.0.1/api_limit.egg-info/dependency_links.txt
--rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)       10 2023-05-30 12:02:22.000000 api_limit-0.0.1/api_limit.egg-info/top_level.txt
--rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)       38 2023-05-30 12:02:22.764914 api_limit-0.0.1/setup.cfg
--rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)      223 2023-05-30 12:01:12.000000 api_limit-0.0.1/setup.py
+drwxr-xr-x   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)        0 2023-05-30 13:04:45.809438 api_limit-0.0.2/
+-rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)      722 2023-05-30 13:04:45.809438 api_limit-0.0.2/PKG-INFO
+-rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)      538 2023-05-30 13:03:14.000000 api_limit-0.0.2/README.md
+drwxr-xr-x   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)        0 2023-05-30 13:04:45.805437 api_limit-0.0.2/api_limit/
+-rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)       87 2023-05-26 08:39:23.000000 api_limit-0.0.2/api_limit/__init__.py
+-rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)     1828 2023-05-29 06:53:50.000000 api_limit-0.0.2/api_limit/algorithm.py
+-rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)      942 2023-05-29 05:02:46.000000 api_limit-0.0.2/api_limit/main.py
+drwxr-xr-x   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)        0 2023-05-30 13:04:45.809438 api_limit-0.0.2/api_limit.egg-info/
+-rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)      722 2023-05-30 13:04:45.000000 api_limit-0.0.2/api_limit.egg-info/PKG-INFO
+-rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)      245 2023-05-30 13:04:45.000000 api_limit-0.0.2/api_limit.egg-info/SOURCES.txt
+-rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)        1 2023-05-30 13:04:45.000000 api_limit-0.0.2/api_limit.egg-info/dependency_links.txt
+-rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)        1 2023-05-30 13:04:45.000000 api_limit-0.0.2/api_limit.egg-info/not-zip-safe
+-rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)       10 2023-05-30 13:04:45.000000 api_limit-0.0.2/api_limit.egg-info/top_level.txt
+-rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)       38 2023-05-30 13:04:45.809438 api_limit-0.0.2/setup.cfg
+-rw-r--r--   0 nisarg.j@ah.zymrinc.com (688404024) domain users@ah.zymrinc.com (688400513)      449 2023-05-30 13:04:37.000000 api_limit-0.0.2/setup.py
```

### Comparing `api_limit-0.0.1/api_limit/algorithm.py` & `api_limit-0.0.2/api_limit/algorithm.py`

 * *Files identical despite different names*

### Comparing `api_limit-0.0.1/api_limit/main.py` & `api_limit-0.0.2/api_limit/main.py`

 * *Files identical despite different names*

