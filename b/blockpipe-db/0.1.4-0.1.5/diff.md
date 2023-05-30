# Comparing `tmp/blockpipe_db-0.1.4.tar.gz` & `tmp/blockpipe_db-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockpipe_db-0.1.4.tar", max compression
+gzip compressed data, was "blockpipe_db-0.1.5.tar", max compression
```

## Comparing `blockpipe_db-0.1.4.tar` & `blockpipe_db-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       28 2023-05-28 13:20:46.955674 blockpipe_db-0.1.4/README.md
--rw-r--r--   0        0        0       27 2023-05-28 13:31:46.448380 blockpipe_db-0.1.4/blockpipe_db/__init__.py
--rw-r--r--   0        0        0     1220 2023-05-29 07:59:30.024936 blockpipe_db-0.1.4/blockpipe_db/client.py
--rw-r--r--   0        0        0      393 2023-05-29 07:59:42.608662 blockpipe_db-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 blockpipe_db-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       28 2023-05-28 13:20:46.955674 blockpipe_db-0.1.5/README.md
+-rw-r--r--   0        0        0       27 2023-05-28 13:31:46.448380 blockpipe_db-0.1.5/blockpipe_db/__init__.py
+-rw-r--r--   0        0        0     1220 2023-05-30 01:03:57.630757 blockpipe_db-0.1.5/blockpipe_db/client.py
+-rw-r--r--   0        0        0      393 2023-05-30 01:04:07.362800 blockpipe_db-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 blockpipe_db-0.1.5/PKG-INFO
```

### Comparing `blockpipe_db-0.1.4/blockpipe_db/client.py` & `blockpipe_db-0.1.5/blockpipe_db/client.py`

 * *Files identical despite different names*

### Comparing `blockpipe_db-0.1.4/PKG-INFO` & `blockpipe_db-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockpipe-db
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Sorawit Suriyakarn
 Author-email: thepsint@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

