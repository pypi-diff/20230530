# Comparing `tmp/grid2fp-0.0.5.tar.gz` & `tmp/grid2fp-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grid2fp-0.0.5.tar", last modified: Fri May 26 15:24:38 2023, max compression
+gzip compressed data, was "grid2fp-0.0.6.tar", last modified: Tue May 30 19:21:42 2023, max compression
```

## Comparing `grid2fp-0.0.5.tar` & `grid2fp-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:24:38.847999 grid2fp-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 15:24:05.000000 grid2fp-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-26 15:24:38.847999 grid2fp-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-26 15:24:05.000000 grid2fp-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:24:38.847999 grid2fp-0.0.5/grid2fp/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 15:24:05.000000 grid2fp-0.0.5/grid2fp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-05-26 15:24:05.000000 grid2fp-0.0.5/grid2fp/grid2fp.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-26 15:24:05.000000 grid2fp-0.0.5/grid2fp/grid_segment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:24:38.847999 grid2fp-0.0.5/grid2fp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-26 15:24:38.000000 grid2fp-0.0.5/grid2fp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-26 15:24:38.000000 grid2fp-0.0.5/grid2fp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:24:38.000000 grid2fp-0.0.5/grid2fp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 15:24:38.000000 grid2fp-0.0.5/grid2fp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 15:24:38.000000 grid2fp-0.0.5/grid2fp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:24:38.847999 grid2fp-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-26 15:24:05.000000 grid2fp-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:24:38.847999 grid2fp-0.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 15:24:05.000000 grid2fp-0.0.5/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-26 15:24:05.000000 grid2fp-0.0.5/test/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:21:42.169627 grid2fp-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-30 19:21:16.000000 grid2fp-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-30 19:21:42.169627 grid2fp-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-30 19:21:16.000000 grid2fp-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:21:42.165627 grid2fp-0.0.6/grid2fp/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 19:21:16.000000 grid2fp-0.0.6/grid2fp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-05-30 19:21:16.000000 grid2fp-0.0.6/grid2fp/grid2fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-30 19:21:16.000000 grid2fp-0.0.6/grid2fp/grid_segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:21:42.169627 grid2fp-0.0.6/grid2fp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-30 19:21:42.000000 grid2fp-0.0.6/grid2fp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-30 19:21:42.000000 grid2fp-0.0.6/grid2fp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:21:42.000000 grid2fp-0.0.6/grid2fp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 19:21:42.000000 grid2fp-0.0.6/grid2fp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 19:21:42.000000 grid2fp-0.0.6/grid2fp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:21:42.169627 grid2fp-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-30 19:21:16.000000 grid2fp-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:21:42.169627 grid2fp-0.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 19:21:16.000000 grid2fp-0.0.6/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-30 19:21:16.000000 grid2fp-0.0.6/test/test_integration.py
```

### Comparing `grid2fp-0.0.5/LICENSE` & `grid2fp-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `grid2fp-0.0.5/PKG-INFO` & `grid2fp-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grid2fp
-Version: 0.0.5
+Version: 0.0.6
 Summary: A tool to eat grid diagrams and generate its front projection.
 Home-page: https://github.com/Joecstarr/grid2fp
 Author: Casey Duckering
 Keywords: topology,Legendrian,Grid Diagram,knot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -70,15 +70,15 @@
 d.save_svg(svg_path)
 
 ```
 # Sample images
 
 x|o| | |
 -|-|-|-|
- |x|o|
+ |x|o| |
  | |x|o|
 o| | |x|
 
 ![random](https://github.com/Joecstarr/grid2fp/assets/52646388/0e22c161-359d-4bb1-a10a-51011e7eefac)
 
 o| | |x| |
 -|-|-|-|-|
@@ -92,15 +92,15 @@
 x| |o|
 -|-|-|
  | | |
 o| |x|
 
 ![un](https://github.com/Joecstarr/grid2fp/assets/52646388/3a080da3-f5aa-4b23-b4b2-a917140cd95a)
 
- | |o| | |x| |
+‎| |o| | |x| |
 -|-|-|-|-|-|-|
  | | | |o| |x|
  |x| | | |o| |
 o| |x| | | | |
  | | |x| | |o|
  |o| | |x| | |
 x| | |o| | | |
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `grid2fp-0.0.5/README.md` & `grid2fp-0.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 d.save_svg(svg_path)
 
 ```
 # Sample images
 
 x|o| | |
 -|-|-|-|
- |x|o|
+ |x|o| |
  | |x|o|
 o| | |x|
 
 ![random](https://github.com/Joecstarr/grid2fp/assets/52646388/0e22c161-359d-4bb1-a10a-51011e7eefac)
 
 o| | |x| |
 -|-|-|-|-|
@@ -77,15 +77,15 @@
 x| |o|
 -|-|-|
  | | |
 o| |x|
 
 ![un](https://github.com/Joecstarr/grid2fp/assets/52646388/3a080da3-f5aa-4b23-b4b2-a917140cd95a)
 
- | |o| | |x| |
+‎| |o| | |x| |
 -|-|-|-|-|-|-|
  | | | |o| |x|
  |x| | | |o| |
 o| |x| | | | |
  | | |x| | |o|
  |o| | |x| | |
 x| | |o| | | |
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `grid2fp-0.0.5/grid2fp/grid2fp.py` & `grid2fp-0.0.6/grid2fp/grid2fp.py`

 * *Files identical despite different names*

### Comparing `grid2fp-0.0.5/grid2fp.egg-info/PKG-INFO` & `grid2fp-0.0.6/grid2fp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grid2fp
-Version: 0.0.5
+Version: 0.0.6
 Summary: A tool to eat grid diagrams and generate its front projection.
 Home-page: https://github.com/Joecstarr/grid2fp
 Author: Casey Duckering
 Keywords: topology,Legendrian,Grid Diagram,knot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -70,15 +70,15 @@
 d.save_svg(svg_path)
 
 ```
 # Sample images
 
 x|o| | |
 -|-|-|-|
- |x|o|
+ |x|o| |
  | |x|o|
 o| | |x|
 
 ![random](https://github.com/Joecstarr/grid2fp/assets/52646388/0e22c161-359d-4bb1-a10a-51011e7eefac)
 
 o| | |x| |
 -|-|-|-|-|
@@ -92,15 +92,15 @@
 x| |o|
 -|-|-|
  | | |
 o| |x|
 
 ![un](https://github.com/Joecstarr/grid2fp/assets/52646388/3a080da3-f5aa-4b23-b4b2-a917140cd95a)
 
- | |o| | |x| |
+‎| |o| | |x| |
 -|-|-|-|-|-|-|
  | | | |o| |x|
  |x| | | |o| |
 o| |x| | | | |
  | | |x| | |o|
  |o| | |x| | |
 x| | |o| | | |
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `grid2fp-0.0.5/setup.py` & `grid2fp-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import logging
 
 logger = logging.getLogger(__name__)
 
-version = "0.0.5"
+version = "0.0.6"
 
 try:
     with open("README.md", "r") as f:
         long_desc = f.read()
 except:
     logger.warning("Could not open README.md.  long_description will be set to None.")
     long_desc = None
```

### Comparing `grid2fp-0.0.5/test/test_integration.py` & `grid2fp-0.0.6/test/test_integration.py`

 * *Files identical despite different names*

