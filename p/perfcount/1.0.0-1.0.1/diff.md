# Comparing `tmp/perfcount-1.0.0.tar.gz` & `tmp/perfcount-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perfcount-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "perfcount-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `perfcount-1.0.0.tar` & `perfcount-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1100 2023-05-29 16:45:47.191510 perfcount-1.0.0/LICENSE
--rw-r--r--   0        0        0      546 2023-05-29 16:53:17.395933 perfcount-1.0.0/README.md
--rw-r--r--   0        0        0     5749 2023-05-29 16:45:13.008983 perfcount-1.0.0/perfcount/__init__.py
--rw-r--r--   0        0        0      247 2023-05-29 16:49:14.240543 perfcount-1.0.0/perfcount/__main__.py
--rw-r--r--   0        0        0      500 2023-04-13 21:51:34.628112 perfcount-1.0.0/perfcount/time_this_program.py
--rw-r--r--   0        0        0      465 2023-05-29 16:52:32.564583 perfcount-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 perfcount-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-05-29 16:45:47.191510 perfcount-1.0.1/LICENSE
+-rw-r--r--   0        0        0      546 2023-05-29 16:53:17.395933 perfcount-1.0.1/README.md
+-rw-r--r--   0        0        0     5749 2023-05-30 02:25:52.157018 perfcount-1.0.1/perfcount/__init__.py
+-rw-r--r--   0        0        0      247 2023-05-29 16:49:14.240543 perfcount-1.0.1/perfcount/__main__.py
+-rw-r--r--   0        0        0      500 2023-04-13 21:51:34.628112 perfcount-1.0.1/perfcount/time_this_program.py
+-rw-r--r--   0        0        0      879 2023-05-30 02:26:22.075095 perfcount-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 perfcount-1.0.1/PKG-INFO
```

### Comparing `perfcount-1.0.0/LICENSE` & `perfcount-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `perfcount-1.0.0/README.md` & `perfcount-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `perfcount-1.0.0/perfcount/__init__.py` & `perfcount-1.0.1/perfcount/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Useful Python library for performance testing that contains multiple function decorators"""
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 import time
 import threading
 import warnings
 import traceback
 import unittest.mock
 import contextlib
```

### Comparing `perfcount-1.0.0/PKG-INFO` & `perfcount-1.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 Metadata-Version: 2.1
 Name: perfcount
-Version: 1.0.0
+Version: 1.0.1
 Summary: Useful Python library for performance testing that contains multiple function decorators
+Keywords: testing,performance,timing,timeout,debugger,acceptance
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Debuggers
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Testing :: Acceptance
 Project-URL: Home, https://github.com/User0332/perfcount
 
 # PerfCount - a Python library used for performance testing
 
 Install it with `pip install perfcount`.
 
 There are multiple decorators included for testing in the library, including `perf.perf`, `perfcount.perf_ns`, `perfcount.shouldtake`, and `perfcount.timeout`. The `perfcount.time_this_program` module can be imported to time the program from the time of importing the `perfcount.time_this_program` module to interpreter exit.
```

