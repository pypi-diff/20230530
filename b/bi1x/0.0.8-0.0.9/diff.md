# Comparing `tmp/bi1x-0.0.8.tar.gz` & `tmp/bi1x-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bi1x-0.0.8.tar", last modified: Mon May 21 07:17:38 2018, max compression
+gzip compressed data, was "dist/bi1x-0.0.9.tar", last modified: Mon May 21 07:31:25 2018, max compression
```

## Comparing `bi1x-0.0.8.tar` & `bi1x-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 bois       (501) staff       (20)        0 2018-05-21 07:17:38.000000 bi1x-0.0.8/
--rw-r--r--   0 bois       (501) staff       (20)      869 2018-05-21 07:17:38.000000 bi1x-0.0.8/PKG-INFO
--rw-r--r--   0 bois       (501) staff       (20)        0 2018-04-07 17:44:01.000000 bi1x-0.0.8/requirements.txt
--rw-r--r--   0 bois       (501) staff       (20)       42 2018-04-07 17:44:01.000000 bi1x-0.0.8/MANIFEST.in
--rw-r--r--   0 bois       (501) staff       (20)      269 2018-04-07 18:41:49.000000 bi1x-0.0.8/README.md
-drwxr-xr-x   0 bois       (501) staff       (20)        0 2018-05-21 07:17:38.000000 bi1x-0.0.8/bi1x/
--rw-r--r--   0 bois       (501) staff       (20)      173 2018-05-21 07:16:46.000000 bi1x-0.0.8/bi1x/__init__.py
--rw-r--r--   0 bois       (501) staff       (20)     1215 2018-04-07 18:19:56.000000 bi1x-0.0.8/bi1x/utils.py
--rw-r--r--   0 bois       (501) staff       (20)    56144 2018-05-21 07:13:12.000000 bi1x-0.0.8/bi1x/viz.py
--rw-r--r--   0 bois       (501) staff       (20)     5228 2018-05-21 07:16:27.000000 bi1x-0.0.8/bi1x/image.py
--rw-r--r--   0 bois       (501) staff       (20)     1330 2018-05-21 07:16:55.000000 bi1x-0.0.8/setup.py
--rw-r--r--   0 bois       (501) staff       (20)      108 2018-05-21 07:17:38.000000 bi1x-0.0.8/setup.cfg
-drwxr-xr-x   0 bois       (501) staff       (20)        0 2018-05-21 07:17:38.000000 bi1x-0.0.8/bi1x.egg-info/
--rw-r--r--   0 bois       (501) staff       (20)      869 2018-05-21 07:17:38.000000 bi1x-0.0.8/bi1x.egg-info/PKG-INFO
--rw-r--r--   0 bois       (501) staff       (20)      226 2018-05-21 07:17:38.000000 bi1x-0.0.8/bi1x.egg-info/SOURCES.txt
--rw-r--r--   0 bois       (501) staff       (20)        5 2018-05-21 07:17:38.000000 bi1x-0.0.8/bi1x.egg-info/top_level.txt
--rw-r--r--   0 bois       (501) staff       (20)        1 2018-05-21 07:17:38.000000 bi1x-0.0.8/bi1x.egg-info/dependency_links.txt
+drwxr-xr-x   0 bois       (501) staff       (20)        0 2018-05-21 07:31:25.000000 bi1x-0.0.9/
+-rw-r--r--   0 bois       (501) staff       (20)      869 2018-05-21 07:31:25.000000 bi1x-0.0.9/PKG-INFO
+-rw-r--r--   0 bois       (501) staff       (20)        0 2018-04-07 17:44:01.000000 bi1x-0.0.9/requirements.txt
+-rw-r--r--   0 bois       (501) staff       (20)       42 2018-04-07 17:44:01.000000 bi1x-0.0.9/MANIFEST.in
+-rw-r--r--   0 bois       (501) staff       (20)      269 2018-04-07 18:41:49.000000 bi1x-0.0.9/README.md
+drwxr-xr-x   0 bois       (501) staff       (20)        0 2018-05-21 07:31:25.000000 bi1x-0.0.9/bi1x/
+-rw-r--r--   0 bois       (501) staff       (20)      173 2018-05-21 07:30:41.000000 bi1x-0.0.9/bi1x/__init__.py
+-rw-r--r--   0 bois       (501) staff       (20)     1215 2018-04-07 18:19:56.000000 bi1x-0.0.9/bi1x/utils.py
+-rw-r--r--   0 bois       (501) staff       (20)    56144 2018-05-21 07:13:12.000000 bi1x-0.0.9/bi1x/viz.py
+-rw-r--r--   0 bois       (501) staff       (20)     5239 2018-05-21 07:30:01.000000 bi1x-0.0.9/bi1x/image.py
+-rw-r--r--   0 bois       (501) staff       (20)     1330 2018-05-21 07:30:58.000000 bi1x-0.0.9/setup.py
+-rw-r--r--   0 bois       (501) staff       (20)      108 2018-05-21 07:31:25.000000 bi1x-0.0.9/setup.cfg
+drwxr-xr-x   0 bois       (501) staff       (20)        0 2018-05-21 07:31:25.000000 bi1x-0.0.9/bi1x.egg-info/
+-rw-r--r--   0 bois       (501) staff       (20)      869 2018-05-21 07:31:25.000000 bi1x-0.0.9/bi1x.egg-info/PKG-INFO
+-rw-r--r--   0 bois       (501) staff       (20)      226 2018-05-21 07:31:25.000000 bi1x-0.0.9/bi1x.egg-info/SOURCES.txt
+-rw-r--r--   0 bois       (501) staff       (20)        5 2018-05-21 07:31:25.000000 bi1x-0.0.9/bi1x.egg-info/top_level.txt
+-rw-r--r--   0 bois       (501) staff       (20)        1 2018-05-21 07:31:25.000000 bi1x-0.0.9/bi1x.egg-info/dependency_links.txt
```

### Comparing `bi1x-0.0.8/PKG-INFO` & `bi1x-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: bi1x
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python utilities for the Caltech course Bi 1x: The Great Ideas of Biology
 Home-page: https://github.com/justinbois/bi1x
 Author: Justin Bois
 Author-email: bois@caltech.edu
 License: BSD
-Download-URL: https://github.com/justinbois/bi1x/tarball/0.0.8
+Download-URL: https://github.com/justinbois/bi1x/tarball/0.0.9
 Description: # bi1x
         
         Utilities Caltech Bi 1x: The Great Ideas of Biology: Exploration through Experimentation
         
         
         ## Installation / Usage
```

### Comparing `bi1x-0.0.8/bi1x/utils.py` & `bi1x-0.0.9/bi1x/utils.py`

 * *Files identical despite different names*

### Comparing `bi1x-0.0.8/bi1x/viz.py` & `bi1x-0.0.9/bi1x/viz.py`

 * *Files identical despite different names*

### Comparing `bi1x-0.0.8/bi1x/image.py` & `bi1x-0.0.9/bi1x/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,21 +133,21 @@
     # Set up points we want to check in subimage
     i = np.arange(*i_range)
     j = np.arange(*j_range)
     ii, jj = np.meshgrid(i, j)
     pts = np.array(list(zip(ii.ravel(), jj.ravel())))
 
     # Make a path object from vertices
-    if shift:
-        p = path.Path(verts + 0.5)
-    else:
-        p = path.Path(verts)
+    p = path.Path(verts)
 
     # Get list of points that are in roi
-    in_roi = p.contains_points(pts)
+    if shift:
+        in_roi = p.contains_points(pts + 0.5)
+    else:
+        in_roi = p.contains_points(pts)
 
     # Subimage ROI
     sub_roi = in_roi.reshape((sub_j_size, sub_i_size)).astype(np.bool)
 
     # Build full ROI
     roi = np.zeros(shape, dtype=bool)
     roi[j_range[0]:j_range[1], i_range[0]:i_range[1]] = sub_roi
```

### Comparing `bi1x-0.0.8/setup.py` & `bi1x-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
```

### Comparing `bi1x-0.0.8/bi1x.egg-info/PKG-INFO` & `bi1x-0.0.9/bi1x.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: bi1x
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python utilities for the Caltech course Bi 1x: The Great Ideas of Biology
 Home-page: https://github.com/justinbois/bi1x
 Author: Justin Bois
 Author-email: bois@caltech.edu
 License: BSD
-Download-URL: https://github.com/justinbois/bi1x/tarball/0.0.8
+Download-URL: https://github.com/justinbois/bi1x/tarball/0.0.9
 Description: # bi1x
         
         Utilities Caltech Bi 1x: The Great Ideas of Biology: Exploration through Experimentation
         
         
         ## Installation / Usage
```

