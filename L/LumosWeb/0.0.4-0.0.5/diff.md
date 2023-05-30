# Comparing `tmp/LumosWeb-0.0.4.tar.gz` & `tmp/LumosWeb-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LumosWeb-0.0.4.tar", last modified: Tue May 30 10:43:44 2023, max compression
+gzip compressed data, was "LumosWeb-0.0.5.tar", last modified: Tue May 30 10:50:00 2023, max compression
```

## Comparing `LumosWeb-0.0.4.tar` & `LumosWeb-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 10:43:44.688902 LumosWeb-0.0.4/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 10:43:44.281028 LumosWeb-0.0.4/LumosWeb/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-0.0.4/LumosWeb/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4822 2023-05-30 10:42:42.000000 LumosWeb-0.0.4/LumosWeb/api.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-0.0.4/LumosWeb/middleware.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      972 2023-05-29 08:01:54.000000 LumosWeb-0.0.4/LumosWeb/response.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 10:43:44.611434 LumosWeb-0.0.4/LumosWeb.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3941 2023-05-30 10:43:43.000000 LumosWeb-0.0.4/LumosWeb.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      293 2023-05-30 10:43:43.000000 LumosWeb-0.0.4/LumosWeb.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-30 10:43:43.000000 LumosWeb-0.0.4/LumosWeb.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       49 2023-05-30 10:43:43.000000 LumosWeb-0.0.4/LumosWeb.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      121 2023-05-30 10:43:43.000000 LumosWeb-0.0.4/LumosWeb.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-05-30 10:43:43.000000 LumosWeb-0.0.4/LumosWeb.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3941 2023-05-30 10:43:44.679998 LumosWeb-0.0.4/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3760 2023-05-29 14:14:31.000000 LumosWeb-0.0.4/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-30 10:43:44.692282 LumosWeb-0.0.4/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1868 2023-05-30 10:43:40.000000 LumosWeb-0.0.4/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 10:50:00.865183 LumosWeb-0.0.5/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 10:50:00.468665 LumosWeb-0.0.5/LumosWeb/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-0.0.5/LumosWeb/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4822 2023-05-30 10:42:42.000000 LumosWeb-0.0.5/LumosWeb/api.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-0.0.5/LumosWeb/middleware.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      972 2023-05-29 08:01:54.000000 LumosWeb-0.0.5/LumosWeb/response.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 10:50:00.798993 LumosWeb-0.0.5/LumosWeb.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3941 2023-05-30 10:49:59.000000 LumosWeb-0.0.5/LumosWeb.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      293 2023-05-30 10:50:00.000000 LumosWeb-0.0.5/LumosWeb.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-30 10:49:59.000000 LumosWeb-0.0.5/LumosWeb.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       46 2023-05-30 10:49:59.000000 LumosWeb-0.0.5/LumosWeb.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      121 2023-05-30 10:49:59.000000 LumosWeb-0.0.5/LumosWeb.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-05-30 10:49:59.000000 LumosWeb-0.0.5/LumosWeb.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3941 2023-05-30 10:50:00.858271 LumosWeb-0.0.5/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3760 2023-05-29 14:14:31.000000 LumosWeb-0.0.5/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-30 10:50:00.868835 LumosWeb-0.0.5/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1865 2023-05-30 10:49:44.000000 LumosWeb-0.0.5/setup.py
```

### Comparing `LumosWeb-0.0.4/LumosWeb/api.py` & `LumosWeb-0.0.5/LumosWeb/api.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-0.0.4/LumosWeb/middleware.py` & `LumosWeb-0.0.5/LumosWeb/middleware.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-0.0.4/LumosWeb/response.py` & `LumosWeb-0.0.5/LumosWeb/response.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-0.0.4/LumosWeb.egg-info/PKG-INFO` & `LumosWeb-0.0.5/LumosWeb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LumosWeb
-Version: 0.0.4
+Version: 0.0.5
 Summary: LumosWeb is web framework, simple and effective usage
 Author: Sddilora
 Author-email: sumeyyedilaradogan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `LumosWeb-0.0.4/PKG-INFO` & `LumosWeb-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LumosWeb
-Version: 0.0.4
+Version: 0.0.5
 Summary: LumosWeb is web framework, simple and effective usage
 Author: Sddilora
 Author-email: sumeyyedilaradogan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `LumosWeb-0.0.4/README.md` & `LumosWeb-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `LumosWeb-0.0.4/setup.py` & `LumosWeb-0.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Package meta-data.
 NAME = "LumosWeb"
 DESCRIPTION = "LumosWeb is web framework, simple and effective usage"
 EMAIL = "sumeyyedilaradogan@gmail.com"
 AUTHOR = "Sddilora"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 
 # Which packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.2",
     "parse==1.19.0",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
@@ -61,10 +61,10 @@
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3.6",
     ],
     setup_requires=["wheel"],
     entry_points={
         'console_scripts': [
-            'LumosWeb = lumosweb_entry:main'
+            'LumosWeb = LumosWeb.api:run'
         ]},
 )
```

