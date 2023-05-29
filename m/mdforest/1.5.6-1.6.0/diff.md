# Comparing `tmp/mdforest-1.5.6.tar.gz` & `tmp/mdforest-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdforest-1.5.6.tar", last modified: Mon May 29 23:42:41 2023, max compression
+gzip compressed data, was "mdforest-1.6.0.tar", last modified: Mon May 29 23:50:25 2023, max compression
```

## Comparing `mdforest-1.5.6.tar` & `mdforest-1.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-29 23:42:41.568204 mdforest-1.5.6/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 12:19:37.000000 mdforest-1.5.6/LICENSE
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3045 2023-05-29 23:42:41.568204 mdforest-1.5.6/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2641 2023-05-19 13:52:26.000000 mdforest-1.5.6/README.rst
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-29 23:42:41.558204 mdforest-1.5.6/mdforest/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1659 2023-05-29 23:42:13.000000 mdforest-1.5.6/mdforest/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3542 2023-05-29 23:42:13.000000 mdforest-1.5.6/mdforest/mdforest.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-29 23:42:41.568204 mdforest-1.5.6/mdforest/tree/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 14:40:51.000000 mdforest-1.5.6/mdforest/tree/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     4283 2023-05-29 23:42:27.000000 mdforest-1.5.6/mdforest/tree/types.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6325 2023-05-18 19:23:23.000000 mdforest-1.5.6/mdforest/treebuild.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-29 23:42:41.568204 mdforest-1.5.6/mdforest.egg-info/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3045 2023-05-29 23:42:41.000000 mdforest-1.5.6/mdforest.egg-info/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      335 2023-05-29 23:42:41.000000 mdforest-1.5.6/mdforest.egg-info/SOURCES.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-05-29 23:42:41.000000 mdforest-1.5.6/mdforest.egg-info/dependency_links.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       43 2023-05-29 23:42:41.000000 mdforest-1.5.6/mdforest.egg-info/requires.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        9 2023-05-29 23:42:41.000000 mdforest-1.5.6/mdforest.egg-info/top_level.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-11 12:19:37.000000 mdforest-1.5.6/pyproject.toml
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-05-29 23:42:41.568204 mdforest-1.5.6/setup.cfg
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      918 2023-05-29 23:42:33.000000 mdforest-1.5.6/setup.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-29 23:42:41.568204 mdforest-1.5.6/tests/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1196 2023-05-18 14:40:51.000000 mdforest-1.5.6/tests/test_mdtree.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-29 23:50:25.629771 mdforest-1.6.0/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 12:19:37.000000 mdforest-1.6.0/LICENSE
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3045 2023-05-29 23:50:25.629771 mdforest-1.6.0/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2641 2023-05-19 13:52:26.000000 mdforest-1.6.0/README.rst
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-29 23:50:25.619773 mdforest-1.6.0/mdforest/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1659 2023-05-29 23:42:13.000000 mdforest-1.6.0/mdforest/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3569 2023-05-29 23:49:48.000000 mdforest-1.6.0/mdforest/mdforest.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-29 23:50:25.629771 mdforest-1.6.0/mdforest/tree/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 14:40:51.000000 mdforest-1.6.0/mdforest/tree/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     4283 2023-05-29 23:42:27.000000 mdforest-1.6.0/mdforest/tree/types.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6325 2023-05-18 19:23:23.000000 mdforest-1.6.0/mdforest/treebuild.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-29 23:50:25.619773 mdforest-1.6.0/mdforest.egg-info/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3045 2023-05-29 23:50:25.000000 mdforest-1.6.0/mdforest.egg-info/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      335 2023-05-29 23:50:25.000000 mdforest-1.6.0/mdforest.egg-info/SOURCES.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-05-29 23:50:25.000000 mdforest-1.6.0/mdforest.egg-info/dependency_links.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       43 2023-05-29 23:50:25.000000 mdforest-1.6.0/mdforest.egg-info/requires.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        9 2023-05-29 23:50:25.000000 mdforest-1.6.0/mdforest.egg-info/top_level.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-11 12:19:37.000000 mdforest-1.6.0/pyproject.toml
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-05-29 23:50:25.629771 mdforest-1.6.0/setup.cfg
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      918 2023-05-29 23:50:22.000000 mdforest-1.6.0/setup.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-29 23:50:25.629771 mdforest-1.6.0/tests/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1196 2023-05-18 14:40:51.000000 mdforest-1.6.0/tests/test_mdtree.py
```

### Comparing `mdforest-1.5.6/LICENSE` & `mdforest-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mdforest-1.5.6/PKG-INFO` & `mdforest-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mdforest
-Version: 1.5.6
+Version: 1.6.0
 Summary: A package to convert between Markdown and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/mdforest
-Download-URL: https://github.com/kj3moraes/mdforest/archive/1.5.6.zip
+Download-URL: https://github.com/kj3moraes/mdforest/archive/1.6.0.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 .. image:: media/forest-icon.png
```

### Comparing `mdforest-1.5.6/README.rst` & `mdforest-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `mdforest-1.5.6/mdforest/__init__.py` & `mdforest-1.6.0/mdforest/__init__.py`

 * *Files identical despite different names*

### Comparing `mdforest-1.5.6/mdforest/mdforest.py` & `mdforest-1.6.0/mdforest/mdforest.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .treebuild import __TreeOfContents
 from .tree.types import *
 
 def generateRootNodeFromContents(currTree:__TreeOfContents, parent:Node=None) -> Node:
     """ Function to generate the tree of a specific header's section.
     """    
     # BASE CASE: If there is no depth, then it is just a paragraph
-    if currTree.depth == None:
+    if currTree.getHeadingLevel(currTree.source) == None:
         return TextNode(currTree.source.string, parent=parent)
     
     # Get the current header of the tree
     headerText = currTree.source.string
     currentHeaderLevel = currTree.getHeadingLevel(currTree.source)
     rootNode = HeaderNode(headerText, headerNumber=currentHeaderLevel, parent=parent)
```

### Comparing `mdforest-1.5.6/mdforest/tree/types.py` & `mdforest-1.6.0/mdforest/tree/types.py`

 * *Files identical despite different names*

### Comparing `mdforest-1.5.6/mdforest/treebuild.py` & `mdforest-1.6.0/mdforest/treebuild.py`

 * *Files identical despite different names*

### Comparing `mdforest-1.5.6/mdforest.egg-info/PKG-INFO` & `mdforest-1.6.0/mdforest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mdforest
-Version: 1.5.6
+Version: 1.6.0
 Summary: A package to convert between Markdown and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/mdforest
-Download-URL: https://github.com/kj3moraes/mdforest/archive/1.5.6.zip
+Download-URL: https://github.com/kj3moraes/mdforest/archive/1.6.0.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 .. image:: media/forest-icon.png
```

### Comparing `mdforest-1.5.6/setup.py` & `mdforest-1.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.rst").read_text()
 
-VERSION = '1.5.6'
+VERSION = '1.6.0'
 DESCRIPTION = 'A package to convert between Markdown and a forest data structure for efficient processing.'
 
 setup(
     name = "mdforest",
     version = VERSION,
     author = "Keane Moraes",
     author_email = 'lordvader3002@gmail.com',
```

### Comparing `mdforest-1.5.6/tests/test_mdtree.py` & `mdforest-1.6.0/tests/test_mdtree.py`

 * *Files identical despite different names*

