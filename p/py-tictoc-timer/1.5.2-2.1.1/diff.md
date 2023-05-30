# Comparing `tmp/py_tictoc_timer-1.5.2.tar.gz` & `tmp/py_tictoc_timer-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_tictoc_timer-1.5.2.tar", max compression
+gzip compressed data, was "py_tictoc_timer-2.1.1.tar", max compression
```

## Comparing `py_tictoc_timer-1.5.2.tar` & `py_tictoc_timer-2.1.1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-01-05 01:29:41.180432 py_tictoc_timer-1.5.2/LICENSE
--rw-r--r--   0        0        0     8956 2023-01-05 01:29:41.180432 py_tictoc_timer-1.5.2/README.md
--rw-r--r--   0        0        0       51 2023-01-05 01:29:41.180432 py_tictoc_timer-1.5.2/py_tictoc_timer/__init__.py
--rw-r--r--   0        0        0    11972 2023-01-05 01:29:41.180432 py_tictoc_timer-1.5.2/py_tictoc_timer/tictoc.py
--rw-r--r--   0        0        0     1128 2023-01-05 01:29:41.180432 py_tictoc_timer-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     9949 1970-01-01 00:00:00.000000 py_tictoc_timer-1.5.2/setup.py
--rw-r--r--   0        0        0     9778 1970-01-01 00:00:00.000000 py_tictoc_timer-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-30 04:22:56.574202 py_tictoc_timer-2.1.1/LICENSE
+-rw-r--r--   0        0        0     8956 2023-05-30 04:22:56.574202 py_tictoc_timer-2.1.1/README.md
+-rw-r--r--   0        0        0       51 2023-05-30 04:22:56.574202 py_tictoc_timer-2.1.1/py_tictoc_timer/__init__.py
+-rw-r--r--   0        0        0    12057 2023-05-30 04:22:56.574202 py_tictoc_timer-2.1.1/py_tictoc_timer/tictoc.py
+-rw-r--r--   0        0        0     2088 2023-05-30 04:22:56.574202 py_tictoc_timer-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9727 1970-01-01 00:00:00.000000 py_tictoc_timer-2.1.1/PKG-INFO
```

### Comparing `py_tictoc_timer-1.5.2/LICENSE` & `py_tictoc_timer-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_tictoc_timer-1.5.2/README.md` & `py_tictoc_timer-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `py_tictoc_timer-1.5.2/py_tictoc_timer/tictoc.py` & `py_tictoc_timer-2.1.1/py_tictoc_timer/tictoc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+# Future Python Library Imports
 from __future__ import annotations
 
+# Python StdLib Imports
 from timeit import default_timer
 from typing import Optional
 
+# Python Open Source Imports
 from typeguard import typechecked
 
 
 __all__ = ["TicToc"]
 
 
 class TicToc:
```

### Comparing `py_tictoc_timer-1.5.2/PKG-INFO` & `py_tictoc_timer-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: py-tictoc-timer
-Version: 1.5.2
+Version: 2.1.1
 Summary: Time the execution of Python code using syntax similar to MATLAB's tic and toc functions.
 Home-page: https://github.com/chrimaho/py-tictoc-timer.git
 License: MIT
 Author: Chris Mahoney
 Author-email: chrismahoney@hotmail.com
-Requires-Python: >=3.7,<4
+Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: typeguard (>=2.13,<3.0)
+Requires-Dist: typeguard (>=4.0,<5.0)
 Project-URL: Repository, https://github.com/chrimaho/py-tictoc-timer.git
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # `py-tictoc-timer`
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: py-tictoc-timer Version: 1.5.2 Summary: Time the
+Metadata-Version: 2.1 Name: py-tictoc-timer Version: 2.1.1 Summary: Time the
 execution of Python code using syntax similar to MATLAB's tic and toc
 functions. Home-page: https://github.com/chrimaho/py-tictoc-timer.git License:
 MIT Author: Chris Mahoney Author-email: chrismahoney@hotmail.com Requires-
-Python: >=3.7,<4 Classifier: License :: OSI Approved :: MIT License Classifier:
+Python: >=3.8,<4 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Dist: typeguard (>=2.13,<3.0) Project-URL: Repository, https://github.com/
-chrimaho/py-tictoc-timer.git Description-Content-Type: text/markdown
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Dist: typeguard (>=4.0,<5.0) Project-URL: Repository,
+https://github.com/chrimaho/py-tictoc-timer.git Description-Content-Type: text/
+markdown
  # `py-tictoc-timer` [![PyPI version](https://img.shields.io/pypi/v/py-tictoc-
  timer?label=version&logo=git)](https://pypi.org/project/py-tictoc-timer/) [!
           [Python](https://img.shields.io/pypi/pyversions/py-tictoc-
    timer.svg?style=plastic&logo=python&logoColor=FFDE50)](https://pypi.org/
                            project/py-tictoc-timer/)
   [![Released](https://img.shields.io/github/release-date/chrimaho/py-tictoc-
 timer?label=released&logo=google-calendar&logoColor=FF7143)](https://pypi.org/
```

