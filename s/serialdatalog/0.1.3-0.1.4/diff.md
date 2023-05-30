# Comparing `tmp/serialdatalog-0.1.3.tar.gz` & `tmp/serialdatalog-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialdatalog-0.1.3.tar", max compression
+gzip compressed data, was "serialdatalog-0.1.4.tar", max compression
```

## Comparing `serialdatalog-0.1.3.tar` & `serialdatalog-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      976 2023-04-25 12:59:02.329965 serialdatalog-0.1.3/README.md
--rw-r--r--   0        0        0      364 2023-05-30 13:34:32.277531 serialdatalog-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       41 2023-04-25 12:48:30.669977 serialdatalog-0.1.3/serialdatalog/__init__.py
--rw-r--r--   0        0        0     5623 2023-05-30 13:34:02.626979 serialdatalog-0.1.3/serialdatalog/datalog.py
--rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 serialdatalog-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      976 2023-04-25 12:59:02.329965 serialdatalog-0.1.4/README.md
+-rw-r--r--   0        0        0      364 2023-05-30 20:52:27.707201 serialdatalog-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-04-25 12:48:30.669977 serialdatalog-0.1.4/serialdatalog/__init__.py
+-rw-r--r--   0        0        0     5631 2023-05-30 20:38:31.011039 serialdatalog-0.1.4/serialdatalog/datalog.py
+-rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 serialdatalog-0.1.4/PKG-INFO
```

### Comparing `serialdatalog-0.1.3/README.md` & `serialdatalog-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `serialdatalog-0.1.3/serialdatalog/datalog.py` & `serialdatalog-0.1.4/serialdatalog/datalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 import logging
 from datetime import datetime
 
 # Console logger
 clogger = logging.getLogger(__name__)
 def logger(
         table_dict,
-        source="/dev/ttyACM0", dest="datalog.sqlite3",
+        source="/dev/ttyACM0",
+        dest="datalog.sqlite3",
         encoding='utf-8',
         timeout=10,
         rtn_results=False,
     ):
     """Logs serial readings
 
     Args:
```

### Comparing `serialdatalog-0.1.3/PKG-INFO` & `serialdatalog-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serialdatalog
-Version: 0.1.3
+Version: 0.1.4
 Summary: Logs data coming from a serial port
 Author: Alex
 Author-email: adrysdale@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

