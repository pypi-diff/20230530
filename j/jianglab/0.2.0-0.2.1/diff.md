# Comparing `tmp/jianglab-0.2.0.tar.gz` & `tmp/jianglab-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.2.0.tar", last modified: Tue May 30 15:05:25 2023, max compression
+gzip compressed data, was "jianglab-0.2.1.tar", last modified: Tue May 30 15:19:58 2023, max compression
```

## Comparing `jianglab-0.2.0.tar` & `jianglab-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:05:25.474161 jianglab-0.2.0/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-05-30 15:05:25.473878 jianglab-0.2.0/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.2.0/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:05:25.470936 jianglab-0.2.0/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       54 2023-04-13 12:28:44.000000 jianglab-0.2.0/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    12499 2023-05-30 15:04:44.000000 jianglab-0.2.0/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:03:09.000000 jianglab-0.2.0/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:05:25.473360 jianglab-0.2.0/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-05-30 15:05:25.000000 jianglab-0.2.0/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-05-30 15:05:25.000000 jianglab-0.2.0/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-05-30 15:05:25.000000 jianglab-0.2.0/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       93 2023-05-30 15:05:25.000000 jianglab-0.2.0/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-05-30 15:05:25.000000 jianglab-0.2.0/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-05-30 15:05:25.474279 jianglab-0.2.0/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      909 2023-05-30 15:04:43.000000 jianglab-0.2.0/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:19:58.841572 jianglab-0.2.1/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-05-30 15:19:58.841235 jianglab-0.2.1/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.2.1/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:19:58.838275 jianglab-0.2.1/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:19:52.000000 jianglab-0.2.1/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    12499 2023-05-30 15:19:50.000000 jianglab-0.2.1/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:19:55.000000 jianglab-0.2.1/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:19:58.840597 jianglab-0.2.1/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-05-30 15:19:58.000000 jianglab-0.2.1/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-05-30 15:19:58.000000 jianglab-0.2.1/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-05-30 15:19:58.000000 jianglab-0.2.1/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       93 2023-05-30 15:19:58.000000 jianglab-0.2.1/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-05-30 15:19:58.000000 jianglab-0.2.1/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-05-30 15:19:58.841704 jianglab-0.2.1/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      909 2023-05-30 15:19:54.000000 jianglab-0.2.1/setup.py
```

### Comparing `jianglab-0.2.0/PKG-INFO` & `jianglab-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.2.0/README.md` & `jianglab-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.2.0/jianglab/common_functions.py` & `jianglab-0.2.1/jianglab/common_functions.py`

 * *Files identical despite different names*

### Comparing `jianglab-0.2.0/jianglab.egg-info/PKG-INFO` & `jianglab-0.2.1/jianglab.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.2.0/setup.py` & `jianglab-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.2.0',
+    version='0.2.1',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

