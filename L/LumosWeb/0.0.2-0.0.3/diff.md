# Comparing `tmp/LumosWeb-0.0.2.tar.gz` & `tmp/LumosWeb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LumosWeb-0.0.2.tar", last modified: Mon May 29 12:59:23 2023, max compression
+gzip compressed data, was "LumosWeb-0.0.3.tar", last modified: Mon May 29 20:11:55 2023, max compression
```

## Comparing `LumosWeb-0.0.2.tar` & `LumosWeb-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:59:23.463206 LumosWeb-0.0.2/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:59:23.159403 LumosWeb-0.0.2/LumosWeb/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-0.0.2/LumosWeb/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4085 2023-05-29 11:58:23.000000 LumosWeb-0.0.2/LumosWeb/api.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-0.0.2/LumosWeb/middleware.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      972 2023-05-29 08:01:54.000000 LumosWeb-0.0.2/LumosWeb/response.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:59:23.403240 LumosWeb-0.0.2/LumosWeb.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3836 2023-05-29 12:59:22.000000 LumosWeb-0.0.2/LumosWeb.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      258 2023-05-29 12:59:22.000000 LumosWeb-0.0.2/LumosWeb.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-29 12:59:22.000000 LumosWeb-0.0.2/LumosWeb.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      105 2023-05-29 12:59:22.000000 LumosWeb-0.0.2/LumosWeb.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-05-29 12:59:22.000000 LumosWeb-0.0.2/LumosWeb.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3836 2023-05-29 12:59:23.456203 LumosWeb-0.0.2/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3653 2023-05-29 12:56:35.000000 LumosWeb-0.0.2/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-29 12:59:23.466218 LumosWeb-0.0.2/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1740 2023-05-29 12:59:06.000000 LumosWeb-0.0.2/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-29 20:11:55.210936 LumosWeb-0.0.3/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-29 20:11:54.940992 LumosWeb-0.0.3/LumosWeb/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-0.0.3/LumosWeb/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4085 2023-05-29 11:58:23.000000 LumosWeb-0.0.3/LumosWeb/api.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-0.0.3/LumosWeb/middleware.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      972 2023-05-29 08:01:54.000000 LumosWeb-0.0.3/LumosWeb/response.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-29 20:11:55.156616 LumosWeb-0.0.3/LumosWeb.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3941 2023-05-29 20:11:54.000000 LumosWeb-0.0.3/LumosWeb.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      258 2023-05-29 20:11:54.000000 LumosWeb-0.0.3/LumosWeb.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-29 20:11:54.000000 LumosWeb-0.0.3/LumosWeb.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      105 2023-05-29 20:11:54.000000 LumosWeb-0.0.3/LumosWeb.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-05-29 20:11:54.000000 LumosWeb-0.0.3/LumosWeb.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3941 2023-05-29 20:11:55.204935 LumosWeb-0.0.3/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3760 2023-05-29 14:14:31.000000 LumosWeb-0.0.3/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-29 20:11:55.212984 LumosWeb-0.0.3/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1740 2023-05-29 20:11:51.000000 LumosWeb-0.0.3/setup.py
```

### Comparing `LumosWeb-0.0.2/LumosWeb/api.py` & `LumosWeb-0.0.3/LumosWeb/api.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-0.0.2/LumosWeb/middleware.py` & `LumosWeb-0.0.3/LumosWeb/middleware.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-0.0.2/LumosWeb/response.py` & `LumosWeb-0.0.3/LumosWeb/response.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-0.0.2/LumosWeb.egg-info/PKG-INFO` & `LumosWeb-0.0.3/LumosWeb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: LumosWeb
-Version: 0.0.2
+Version: 0.0.3
 Summary: LumosWeb is web framework, simple and effective usage
 Author: Sddilora
 Author-email: sumeyyedilaradogan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 
-## LumosWeb
+## LumosWeb ![PyPI](https://img.shields.io/pypi/v/LumosWeb.svg)
 
 - LumosWeb is web framework written in python
 - It's a WSGI framework and can be used with any WSGI application server such as Gunicorn.
+- [PyPI Release](https://pypi.org/project/LumosWeb/)
+
 
-![PyPI](https://img.shields.io/pypi/v/LumosWeb.svg)
 
 ## Installation
 ```shell
-pip install LumosWeb
+pip install LumosWeb==<latest_version>
+e.g. pip install LumosWeb==0.0.2
 ```
 
 ## Getting Started
 
 ### Basic usage
 
 ```python
```

### Comparing `LumosWeb-0.0.2/PKG-INFO` & `LumosWeb-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: LumosWeb
-Version: 0.0.2
+Version: 0.0.3
 Summary: LumosWeb is web framework, simple and effective usage
 Author: Sddilora
 Author-email: sumeyyedilaradogan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 
-## LumosWeb
+## LumosWeb ![PyPI](https://img.shields.io/pypi/v/LumosWeb.svg)
 
 - LumosWeb is web framework written in python
 - It's a WSGI framework and can be used with any WSGI application server such as Gunicorn.
+- [PyPI Release](https://pypi.org/project/LumosWeb/)
+
 
-![PyPI](https://img.shields.io/pypi/v/LumosWeb.svg)
 
 ## Installation
 ```shell
-pip install LumosWeb
+pip install LumosWeb==<latest_version>
+e.g. pip install LumosWeb==0.0.2
 ```
 
 ## Getting Started
 
 ### Basic usage
 
 ```python
```

### Comparing `LumosWeb-0.0.2/README.md` & `LumosWeb-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-## LumosWeb
+## LumosWeb ![PyPI](https://img.shields.io/pypi/v/LumosWeb.svg)
 
 - LumosWeb is web framework written in python
 - It's a WSGI framework and can be used with any WSGI application server such as Gunicorn.
+- [PyPI Release](https://pypi.org/project/LumosWeb/)
+
 
-![PyPI](https://img.shields.io/pypi/v/LumosWeb.svg)
 
 ## Installation
 ```shell
-pip install LumosWeb
+pip install LumosWeb==<latest_version>
+e.g. pip install LumosWeb==0.0.2
 ```
 
 ## Getting Started
 
 ### Basic usage
 
 ```python
```

### Comparing `LumosWeb-0.0.2/setup.py` & `LumosWeb-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Package meta-data.
 NAME = "LumosWeb"
 DESCRIPTION = "LumosWeb is web framework, simple and effective usage"
 EMAIL = "sumeyyedilaradogan@gmail.com"
 AUTHOR = "Sddilora"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 # Which packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.2",
     "parse==1.19.0",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

