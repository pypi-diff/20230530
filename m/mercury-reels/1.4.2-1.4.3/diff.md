# Comparing `tmp/mercury-reels-1.4.2.tar.gz` & `tmp/mercury-reels-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-reels-1.4.2.tar", last modified: Mon May 29 11:42:09 2023, max compression
+gzip compressed data, was "mercury-reels-1.4.3.tar", last modified: Tue May 30 10:27:42 2023, max compression
```

## Comparing `mercury-reels-1.4.2.tar` & `mercury-reels-1.4.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:42:09.730301 mercury-reels-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18897 2023-05-29 11:42:09.730301 mercury-reels-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 11:42:09.730301 mercury-reels-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:42:09.726301 mercury-reels-1.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:42:09.726301 mercury-reels-1.4.2/src/mercury_reels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18897 2023-05-29 11:42:09.000000 mercury-reels-1.4.2/src/mercury_reels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-29 11:42:09.000000 mercury-reels-1.4.2/src/mercury_reels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 11:42:09.000000 mercury-reels-1.4.2/src/mercury_reels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-29 11:42:09.000000 mercury-reels-1.4.2/src/mercury_reels.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:42:09.730301 mercury-reels-1.4.2/src/reels/
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/Clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/Clips.py
--rw-r--r--   0 runner    (1001) docker     (123)    13253 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/Events.py
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/Intake.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/Targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/imports.in
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/main.dox
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/py_reels.i
--rw-r--r--   0 runner    (1001) docker     (123)   170626 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/py_reels_wrap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    84431 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/reels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    45065 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/reels.h
--rw-r--r--   0 runner    (1001) docker     (123)    15947 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/reels_main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/reels_main.h
--rw-r--r--   0 runner    (1001) docker     (123)    56793 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/reels_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/reels_test.h
--rw-r--r--   0 runner    (1001) docker     (123)   123064 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/thousand_sequences.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:27:42.675447 mercury-reels-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19000 2023-05-30 10:27:42.675447 mercury-reels-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:27:42.675447 mercury-reels-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:27:42.671446 mercury-reels-1.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:27:42.671446 mercury-reels-1.4.3/src/mercury_reels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19000 2023-05-30 10:27:42.000000 mercury-reels-1.4.3/src/mercury_reels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-30 10:27:42.000000 mercury-reels-1.4.3/src/mercury_reels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:27:42.000000 mercury-reels-1.4.3/src/mercury_reels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 10:27:42.000000 mercury-reels-1.4.3/src/mercury_reels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:27:42.675447 mercury-reels-1.4.3/src/reels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/Clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/Clips.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13253 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/Events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/Intake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/Targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/imports.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/main.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/py_reels.i
+-rw-r--r--   0 runner    (1001) docker     (123)   170626 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/py_reels_wrap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    84431 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/reels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    45065 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/reels.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15947 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/reels_main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/reels_main.h
+-rw-r--r--   0 runner    (1001) docker     (123)    56793 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/reels_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/reels_test.h
+-rw-r--r--   0 runner    (1001) docker     (123)   123064 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/thousand_sequences.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/test_all.py
```

### Comparing `mercury-reels-1.4.2/LICENSE.txt` & `mercury-reels-1.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.2/PKG-INFO` & `mercury-reels-1.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-reels
-Version: 1.4.2
+Version: 1.4.3
 Summary: Reels helps identify patterns in event data and can predict target events.
 Author-email: Mercury Team <mercury.group@bbva.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
         
@@ -202,21 +202,21 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Mercury Reels
 
-[![Build Status](https://travis-ci.com/BBVA/mercury-reels.svg?branch=master)](https://travis-ci.com/BBVA/mercury-reels)
+![](https://img.shields.io/badge/-c++-black?logo=c%2B%2B&style=social)
+![](https://img.shields.io/pypi/v/mercury-reels?label=latest%20pypi%20build)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-3816/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-3916/)
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3113/)
 [![Apache 2 license](https://shields.io/badge/license-Apache%202-blue)](http://www.apache.org/licenses/LICENSE-2.0)
-[![codecov](https://codecov.io/gh/BBVA/mercury-reels/branch/master/graph/badge.svg)](https://codecov.io/gh/BBVA/mercury-reels)
 [![Ask Me Anything !](https://img.shields.io/badge/Ask%20me-anything-1abc9c.svg)](https://github.com/BBVA/mercury-reels/issues)
 
 ## What is this?
 
 ### TLDR: Reels helps identify patterns in event data and can predict target events.
 
 **Reels** is a library to analyze sequences of events extracted from transactional data. These events can be automatically discovered
@@ -247,41 +247,41 @@
   * 100% pythonic interface: objects are serializable, use iterators, interfaces with pandas and pyspark.
 
 ## The Python API
 
 Reels is implemented in four classes.
 
 ### The Events class
-<img src="notebooks/images/events.png" width = "640" />
+<img src="https://raw.githubusercontent.com/BBVA/mercury-reels/master/notebooks/images/events.png" width = "640" />
 
   * [Python API](https://bbva.github.io/mercury-reels/reference/python/reference/events/)
   * [C++ API](https://bbva.github.io/mercury-reels/reference/html/classreels_1_1Events.html)
 
 ### The Clients class
-<img src="notebooks/images/clients.png" width = "640" />
+<img src="https://raw.githubusercontent.com/BBVA/mercury-reels/master/notebooks/images/clients.png" width = "640" />
 
   * [Python API](https://bbva.github.io/mercury-reels/reference/python/reference/clients/)
   * [C++ API](https://bbva.github.io/mercury-reels/reference/html/classreels_1_1Clients.html)
 
 ### The Clips class
-<img src="notebooks/images/clips.png" width = "640" />
+<img src="https://raw.githubusercontent.com/BBVA/mercury-reels/master/notebooks/images/clips.png" width = "640" />
 
   * [Python API](https://bbva.github.io/mercury-reels/reference/python/reference/clips/)
   * [C++ API](https://bbva.github.io/mercury-reels/reference/html/classreels_1_1Clips.html)
 
 ### The Targets class
-<img src="notebooks/images/targets.png" width = "640" />
+<img src="https://raw.githubusercontent.com/BBVA/mercury-reels/master/notebooks/images/targets.png" width = "640" />
 
   * [Python API](https://bbva.github.io/mercury-reels/reference/python/reference/targets/)
   * [C++ API](https://bbva.github.io/mercury-reels/reference/html/classreels_1_1Targets.html)
 
 ## Try it without any installation on Google Colab
 
-  * **Introductory**: A walk through Reels [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ZgkLtBlqEZBtW_V83R6vYNKJ_jVZaLTA)
-  * **Advanced**: Event optimization -- How to do assisted event discovery [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1bjj8kzZdhaOmNilU31W4Af5Rp9VQ-1YY)
+  * **Introductory**: A walk through Reels [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/BBVA/mercury-reels/blob/master/notebooks/reels_walkthrough_colab.ipynb)
+  * **Advanced**: Event optimization -- How to do assisted event discovery [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/BBVA/mercury-reels/blob/master/notebooks/reels_event_optimization_colab.ipynb)
 
 ## Install
 
 ```bash
 pip install mercury-reels
 ```
 
@@ -304,15 +304,14 @@
 
 Make without arguments gives help. Try all the options. Everything should work assuming the tools are installed.
 
 ## Documentation
 
   * [Python API](https://bbva.github.io/mercury-reels/reference/python/index.html)
   * [C++ API](https://bbva.github.io/mercury-reels/reference/html/index.html)
-  * [Algorithm description: Reels -- An efficient tree-based event prediction algorithm](__doc__/reference/reels_paper/)
 
 ## License
 
 ```text
                          Apache License
                    Version 2.0, January 2004
                 http://www.apache.org/licenses/
```

### Comparing `mercury-reels-1.4.2/README.md` & `mercury-reels-1.4.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Mercury Reels
 
-[![Build Status](https://travis-ci.com/BBVA/mercury-reels.svg?branch=master)](https://travis-ci.com/BBVA/mercury-reels)
+![](https://img.shields.io/badge/-c++-black?logo=c%2B%2B&style=social)
+![](https://img.shields.io/pypi/v/mercury-reels?label=latest%20pypi%20build)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-3816/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-3916/)
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3113/)
 [![Apache 2 license](https://shields.io/badge/license-Apache%202-blue)](http://www.apache.org/licenses/LICENSE-2.0)
-[![codecov](https://codecov.io/gh/BBVA/mercury-reels/branch/master/graph/badge.svg)](https://codecov.io/gh/BBVA/mercury-reels)
 [![Ask Me Anything !](https://img.shields.io/badge/Ask%20me-anything-1abc9c.svg)](https://github.com/BBVA/mercury-reels/issues)
 
 ## What is this?
 
 ### TLDR: Reels helps identify patterns in event data and can predict target events.
 
 **Reels** is a library to analyze sequences of events extracted from transactional data. These events can be automatically discovered
@@ -41,41 +41,41 @@
   * 100% pythonic interface: objects are serializable, use iterators, interfaces with pandas and pyspark.
 
 ## The Python API
 
 Reels is implemented in four classes.
 
 ### The Events class
-<img src="notebooks/images/events.png" width = "640" />
+<img src="https://raw.githubusercontent.com/BBVA/mercury-reels/master/notebooks/images/events.png" width = "640" />
 
   * [Python API](https://bbva.github.io/mercury-reels/reference/python/reference/events/)
   * [C++ API](https://bbva.github.io/mercury-reels/reference/html/classreels_1_1Events.html)
 
 ### The Clients class
-<img src="notebooks/images/clients.png" width = "640" />
+<img src="https://raw.githubusercontent.com/BBVA/mercury-reels/master/notebooks/images/clients.png" width = "640" />
 
   * [Python API](https://bbva.github.io/mercury-reels/reference/python/reference/clients/)
   * [C++ API](https://bbva.github.io/mercury-reels/reference/html/classreels_1_1Clients.html)
 
 ### The Clips class
-<img src="notebooks/images/clips.png" width = "640" />
+<img src="https://raw.githubusercontent.com/BBVA/mercury-reels/master/notebooks/images/clips.png" width = "640" />
 
   * [Python API](https://bbva.github.io/mercury-reels/reference/python/reference/clips/)
   * [C++ API](https://bbva.github.io/mercury-reels/reference/html/classreels_1_1Clips.html)
 
 ### The Targets class
-<img src="notebooks/images/targets.png" width = "640" />
+<img src="https://raw.githubusercontent.com/BBVA/mercury-reels/master/notebooks/images/targets.png" width = "640" />
 
   * [Python API](https://bbva.github.io/mercury-reels/reference/python/reference/targets/)
   * [C++ API](https://bbva.github.io/mercury-reels/reference/html/classreels_1_1Targets.html)
 
 ## Try it without any installation on Google Colab
 
-  * **Introductory**: A walk through Reels [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ZgkLtBlqEZBtW_V83R6vYNKJ_jVZaLTA)
-  * **Advanced**: Event optimization -- How to do assisted event discovery [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1bjj8kzZdhaOmNilU31W4Af5Rp9VQ-1YY)
+  * **Introductory**: A walk through Reels [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/BBVA/mercury-reels/blob/master/notebooks/reels_walkthrough_colab.ipynb)
+  * **Advanced**: Event optimization -- How to do assisted event discovery [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/BBVA/mercury-reels/blob/master/notebooks/reels_event_optimization_colab.ipynb)
 
 ## Install
 
 ```bash
 pip install mercury-reels
 ```
 
@@ -98,15 +98,14 @@
 
 Make without arguments gives help. Try all the options. Everything should work assuming the tools are installed.
 
 ## Documentation
 
   * [Python API](https://bbva.github.io/mercury-reels/reference/python/index.html)
   * [C++ API](https://bbva.github.io/mercury-reels/reference/html/index.html)
-  * [Algorithm description: Reels -- An efficient tree-based event prediction algorithm](__doc__/reference/reels_paper/)
 
 ## License
 
 ```text
                          Apache License
                    Version 2.0, January 2004
                 http://www.apache.org/licenses/
```

### Comparing `mercury-reels-1.4.2/pyproject.toml` & `mercury-reels-1.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires		= ['setuptools>=61.0']
 build-backend	= 'setuptools.build_meta'
 
 [project]
 name			= 'mercury-reels'
-version			= '1.4.2'
+version			= '1.4.3'
 description		= 'Reels helps identify patterns in event data and can predict target events.'
 license			= {file = "LICENSE.txt"}
 requires-python = '>=3.8'
 classifiers		= ['Programming Language :: Python :: 3',
 					'License :: OSI Approved :: Apache Software License',
 					'Operating System :: OS Independent']
 keywords		= ['event detection', 'event prediction', 'time series']
```

### Comparing `mercury-reels-1.4.2/src/mercury_reels.egg-info/PKG-INFO` & `mercury-reels-1.4.3/src/mercury_reels.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-reels
-Version: 1.4.2
+Version: 1.4.3
 Summary: Reels helps identify patterns in event data and can predict target events.
 Author-email: Mercury Team <mercury.group@bbva.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
         
@@ -202,21 +202,21 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Mercury Reels
 
-[![Build Status](https://travis-ci.com/BBVA/mercury-reels.svg?branch=master)](https://travis-ci.com/BBVA/mercury-reels)
+![](https://img.shields.io/badge/-c++-black?logo=c%2B%2B&style=social)
+![](https://img.shields.io/pypi/v/mercury-reels?label=latest%20pypi%20build)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-3816/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-3916/)
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3113/)
 [![Apache 2 license](https://shields.io/badge/license-Apache%202-blue)](http://www.apache.org/licenses/LICENSE-2.0)
-[![codecov](https://codecov.io/gh/BBVA/mercury-reels/branch/master/graph/badge.svg)](https://codecov.io/gh/BBVA/mercury-reels)
 [![Ask Me Anything !](https://img.shields.io/badge/Ask%20me-anything-1abc9c.svg)](https://github.com/BBVA/mercury-reels/issues)
 
 ## What is this?
 
 ### TLDR: Reels helps identify patterns in event data and can predict target events.
 
 **Reels** is a library to analyze sequences of events extracted from transactional data. These events can be automatically discovered
@@ -247,41 +247,41 @@
   * 100% pythonic interface: objects are serializable, use iterators, interfaces with pandas and pyspark.
 
 ## The Python API
 
 Reels is implemented in four classes.
 
 ### The Events class
-<img src="notebooks/images/events.png" width = "640" />
+<img src="https://raw.githubusercontent.com/BBVA/mercury-reels/master/notebooks/images/events.png" width = "640" />
 
   * [Python API](https://bbva.github.io/mercury-reels/reference/python/reference/events/)
   * [C++ API](https://bbva.github.io/mercury-reels/reference/html/classreels_1_1Events.html)
 
 ### The Clients class
-<img src="notebooks/images/clients.png" width = "640" />
+<img src="https://raw.githubusercontent.com/BBVA/mercury-reels/master/notebooks/images/clients.png" width = "640" />
 
   * [Python API](https://bbva.github.io/mercury-reels/reference/python/reference/clients/)
   * [C++ API](https://bbva.github.io/mercury-reels/reference/html/classreels_1_1Clients.html)
 
 ### The Clips class
-<img src="notebooks/images/clips.png" width = "640" />
+<img src="https://raw.githubusercontent.com/BBVA/mercury-reels/master/notebooks/images/clips.png" width = "640" />
 
   * [Python API](https://bbva.github.io/mercury-reels/reference/python/reference/clips/)
   * [C++ API](https://bbva.github.io/mercury-reels/reference/html/classreels_1_1Clips.html)
 
 ### The Targets class
-<img src="notebooks/images/targets.png" width = "640" />
+<img src="https://raw.githubusercontent.com/BBVA/mercury-reels/master/notebooks/images/targets.png" width = "640" />
 
   * [Python API](https://bbva.github.io/mercury-reels/reference/python/reference/targets/)
   * [C++ API](https://bbva.github.io/mercury-reels/reference/html/classreels_1_1Targets.html)
 
 ## Try it without any installation on Google Colab
 
-  * **Introductory**: A walk through Reels [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ZgkLtBlqEZBtW_V83R6vYNKJ_jVZaLTA)
-  * **Advanced**: Event optimization -- How to do assisted event discovery [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1bjj8kzZdhaOmNilU31W4Af5Rp9VQ-1YY)
+  * **Introductory**: A walk through Reels [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/BBVA/mercury-reels/blob/master/notebooks/reels_walkthrough_colab.ipynb)
+  * **Advanced**: Event optimization -- How to do assisted event discovery [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/BBVA/mercury-reels/blob/master/notebooks/reels_event_optimization_colab.ipynb)
 
 ## Install
 
 ```bash
 pip install mercury-reels
 ```
 
@@ -304,15 +304,14 @@
 
 Make without arguments gives help. Try all the options. Everything should work assuming the tools are installed.
 
 ## Documentation
 
   * [Python API](https://bbva.github.io/mercury-reels/reference/python/index.html)
   * [C++ API](https://bbva.github.io/mercury-reels/reference/html/index.html)
-  * [Algorithm description: Reels -- An efficient tree-based event prediction algorithm](__doc__/reference/reels_paper/)
 
 ## License
 
 ```text
                          Apache License
                    Version 2.0, January 2004
                 http://www.apache.org/licenses/
```

### Comparing `mercury-reels-1.4.2/src/mercury_reels.egg-info/SOURCES.txt` & `mercury-reels-1.4.3/src/mercury_reels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.2/src/reels/Clients.py` & `mercury-reels-1.4.3/src/reels/Clients.py`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.2/src/reels/Clips.py` & `mercury-reels-1.4.3/src/reels/Clips.py`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.2/src/reels/Events.py` & `mercury-reels-1.4.3/src/reels/Events.py`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.2/src/reels/Intake.py` & `mercury-reels-1.4.3/src/reels/Intake.py`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.2/src/reels/Targets.py` & `mercury-reels-1.4.3/src/reels/Targets.py`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.2/src/reels/__init__.py` & `mercury-reels-1.4.3/src/reels/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,14 +210,14 @@
     return _py_reels.next_binary_image_iterator(image_id)
 
 def destroy_binary_image_iterator(image_id):
     return _py_reels.destroy_binary_image_iterator(image_id)
 
 
 # The source version file is <proj>/src/version.py, anything else is auto generated.
-__version__ = '1.4.1'
+__version__ = '1.4.3'
 
 from reels.Clients import Clients
 from reels.Events import Events
 from reels.Clips import Clips
 from reels.Targets import Targets
 from reels.Intake import Intake
```

### Comparing `mercury-reels-1.4.2/src/reels/main.dox` & `mercury-reels-1.4.3/src/reels/main.dox`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.2/src/reels/py_reels.i` & `mercury-reels-1.4.3/src/reels/py_reels.i`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.2/src/reels/py_reels_wrap.cpp` & `mercury-reels-1.4.3/src/reels/py_reels_wrap.cpp`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.2/src/reels/reels.cpp` & `mercury-reels-1.4.3/src/reels/reels.cpp`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.2/src/reels/reels.h` & `mercury-reels-1.4.3/src/reels/reels.h`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.2/src/reels/reels_main.cpp` & `mercury-reels-1.4.3/src/reels/reels_main.cpp`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.2/src/reels/reels_main.h` & `mercury-reels-1.4.3/src/reels/reels_main.h`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.2/src/reels/reels_test.cpp` & `mercury-reels-1.4.3/src/reels/reels_test.cpp`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.2/src/reels/reels_test.h` & `mercury-reels-1.4.3/src/reels/reels_test.h`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.2/src/reels/thousand_sequences.hpp` & `mercury-reels-1.4.3/src/reels/thousand_sequences.hpp`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.2/src/test_all.py` & `mercury-reels-1.4.3/src/test_all.py`

 * *Files identical despite different names*

