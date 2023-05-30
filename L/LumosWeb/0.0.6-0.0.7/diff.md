# Comparing `tmp/LumosWeb-0.0.6.tar.gz` & `tmp/LumosWeb-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LumosWeb-0.0.6.tar", last modified: Tue May 30 11:00:22 2023, max compression
+gzip compressed data, was "LumosWeb-0.0.7.tar", last modified: Tue May 30 11:22:45 2023, max compression
```

## Comparing `LumosWeb-0.0.6.tar` & `LumosWeb-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 11:00:22.744503 LumosWeb-0.0.6/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 11:00:22.367766 LumosWeb-0.0.6/LumosWeb/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-0.0.6/LumosWeb/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4822 2023-05-30 10:42:42.000000 LumosWeb-0.0.6/LumosWeb/api.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-0.0.6/LumosWeb/middleware.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      972 2023-05-29 08:01:54.000000 LumosWeb-0.0.6/LumosWeb/response.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 11:00:22.687615 LumosWeb-0.0.6/LumosWeb.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3941 2023-05-30 11:00:21.000000 LumosWeb-0.0.6/LumosWeb.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      293 2023-05-30 11:00:21.000000 LumosWeb-0.0.6/LumosWeb.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-30 11:00:21.000000 LumosWeb-0.0.6/LumosWeb.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       50 2023-05-30 11:00:21.000000 LumosWeb-0.0.6/LumosWeb.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      121 2023-05-30 11:00:21.000000 LumosWeb-0.0.6/LumosWeb.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-05-30 11:00:21.000000 LumosWeb-0.0.6/LumosWeb.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3941 2023-05-30 11:00:22.738507 LumosWeb-0.0.6/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3760 2023-05-29 14:14:31.000000 LumosWeb-0.0.6/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-30 11:00:22.748196 LumosWeb-0.0.6/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1869 2023-05-30 11:00:08.000000 LumosWeb-0.0.6/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 11:22:45.788421 LumosWeb-0.0.7/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 11:22:45.388703 LumosWeb-0.0.7/LumosWeb/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-0.0.7/LumosWeb/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4163 2023-05-30 11:21:23.000000 LumosWeb-0.0.7/LumosWeb/api.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      662 2023-05-30 11:21:14.000000 LumosWeb-0.0.7/LumosWeb/cli.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-0.0.7/LumosWeb/middleware.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      972 2023-05-29 08:01:54.000000 LumosWeb-0.0.7/LumosWeb/response.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-30 11:22:45.722904 LumosWeb-0.0.7/LumosWeb.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3941 2023-05-30 11:22:44.000000 LumosWeb-0.0.7/LumosWeb.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      309 2023-05-30 11:22:44.000000 LumosWeb-0.0.7/LumosWeb.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-30 11:22:44.000000 LumosWeb-0.0.7/LumosWeb.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-05-30 11:22:44.000000 LumosWeb-0.0.7/LumosWeb.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      105 2023-05-30 11:22:44.000000 LumosWeb-0.0.7/LumosWeb.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-05-30 11:22:44.000000 LumosWeb-0.0.7/LumosWeb.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3941 2023-05-30 11:22:45.780489 LumosWeb-0.0.7/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3760 2023-05-29 14:14:31.000000 LumosWeb-0.0.7/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-30 11:22:45.791765 LumosWeb-0.0.7/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1845 2023-05-30 11:22:40.000000 LumosWeb-0.0.7/setup.py
```

### Comparing `LumosWeb-0.0.6/LumosWeb/middleware.py` & `LumosWeb-0.0.7/LumosWeb/middleware.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-0.0.6/LumosWeb/response.py` & `LumosWeb-0.0.7/LumosWeb/response.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-0.0.6/LumosWeb.egg-info/PKG-INFO` & `LumosWeb-0.0.7/LumosWeb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LumosWeb
-Version: 0.0.6
+Version: 0.0.7
 Summary: LumosWeb is web framework, simple and effective usage
 Author: Sddilora
 Author-email: sumeyyedilaradogan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `LumosWeb-0.0.6/PKG-INFO` & `LumosWeb-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LumosWeb
-Version: 0.0.6
+Version: 0.0.7
 Summary: LumosWeb is web framework, simple and effective usage
 Author: Sddilora
 Author-email: sumeyyedilaradogan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `LumosWeb-0.0.6/README.md` & `LumosWeb-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `LumosWeb-0.0.6/setup.py` & `LumosWeb-0.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,25 +8,24 @@
 
 # Package meta-data.
 NAME = "LumosWeb"
 DESCRIPTION = "LumosWeb is web framework, simple and effective usage"
 EMAIL = "sumeyyedilaradogan@gmail.com"
 AUTHOR = "Sddilora"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 
 # Which packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.2",
     "parse==1.19.0",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
     "WebOb==1.8.7",
     "whitenoise==6.4.0",
-    "waitress==2.1.2",
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 # Note: this will only work if 'README.md' is present in your MANIFEST.in file!
 try:
@@ -61,10 +60,10 @@
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3.6",
     ],
     setup_requires=["wheel"],
     entry_points={
         'console_scripts': [
-            'LumosWeb = lumosweb.api:API.run'
+             'LumosWeb = LumosWeb.cli:main',
         ]},
 )
```

