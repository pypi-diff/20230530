# Comparing `tmp/blockpipe_db-0.1.5.tar.gz` & `tmp/blockpipe_db-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockpipe_db-0.1.5.tar", max compression
+gzip compressed data, was "blockpipe_db-0.1.6.tar", max compression
```

## Comparing `blockpipe_db-0.1.5.tar` & `blockpipe_db-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       28 2023-05-28 13:20:46.955674 blockpipe_db-0.1.5/README.md
--rw-r--r--   0        0        0       27 2023-05-28 13:31:46.448380 blockpipe_db-0.1.5/blockpipe_db/__init__.py
--rw-r--r--   0        0        0     1220 2023-05-30 01:03:57.630757 blockpipe_db-0.1.5/blockpipe_db/client.py
--rw-r--r--   0        0        0      393 2023-05-30 01:04:07.362800 blockpipe_db-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 blockpipe_db-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       28 2023-05-28 13:20:46.955674 blockpipe_db-0.1.6/README.md
+-rw-r--r--   0        0        0       27 2023-05-28 13:31:46.448380 blockpipe_db-0.1.6/blockpipe_db/__init__.py
+-rw-r--r--   0        0        0     1956 2023-05-30 09:27:03.186902 blockpipe_db-0.1.6/blockpipe_db/client.py
+-rw-r--r--   0        0        0      595 2023-05-30 09:20:34.775341 blockpipe_db-0.1.6/blockpipe_db/msg.py
+-rw-r--r--   0        0        0      393 2023-05-30 09:28:09.292471 blockpipe_db-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 blockpipe_db-0.1.6/PKG-INFO
```

### Comparing `blockpipe_db-0.1.5/PKG-INFO` & `blockpipe_db-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockpipe-db
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Sorawit Suriyakarn
 Author-email: thepsint@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

