# Comparing `tmp/jianglab-0.2.2.tar.gz` & `tmp/jianglab-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.2.2.tar", last modified: Tue May 30 15:33:16 2023, max compression
+gzip compressed data, was "jianglab-0.2.3.tar", last modified: Tue May 30 15:36:45 2023, max compression
```

## Comparing `jianglab-0.2.2.tar` & `jianglab-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:33:16.040814 jianglab-0.2.2/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-05-30 15:33:16.040482 jianglab-0.2.2/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.2.2/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:33:16.037052 jianglab-0.2.2/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:33:06.000000 jianglab-0.2.2/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    12499 2023-05-30 15:33:07.000000 jianglab-0.2.2/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:33:09.000000 jianglab-0.2.2/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:33:16.039845 jianglab-0.2.2/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-05-30 15:33:15.000000 jianglab-0.2.2/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-05-30 15:33:15.000000 jianglab-0.2.2/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-05-30 15:33:15.000000 jianglab-0.2.2/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       93 2023-05-30 15:33:15.000000 jianglab-0.2.2/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-05-30 15:33:15.000000 jianglab-0.2.2/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-05-30 15:33:16.040926 jianglab-0.2.2/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      909 2023-05-30 15:33:03.000000 jianglab-0.2.2/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:36:45.218863 jianglab-0.2.3/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-05-30 15:36:45.218546 jianglab-0.2.3/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.2.3/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:36:45.215427 jianglab-0.2.3/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:33:06.000000 jianglab-0.2.3/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    12499 2023-05-30 15:33:07.000000 jianglab-0.2.3/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:33:09.000000 jianglab-0.2.3/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:36:45.218029 jianglab-0.2.3/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-05-30 15:36:45.000000 jianglab-0.2.3/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-05-30 15:36:45.000000 jianglab-0.2.3/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-05-30 15:36:45.000000 jianglab-0.2.3/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       86 2023-05-30 15:36:45.000000 jianglab-0.2.3/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-05-30 15:36:45.000000 jianglab-0.2.3/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-05-30 15:36:45.218977 jianglab-0.2.3/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      891 2023-05-30 15:36:37.000000 jianglab-0.2.3/setup.py
```

### Comparing `jianglab-0.2.2/PKG-INFO` & `jianglab-0.2.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.2.2/README.md` & `jianglab-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.2.2/jianglab/common_functions.py` & `jianglab-0.2.3/jianglab/common_functions.py`

 * *Files identical despite different names*

### Comparing `jianglab-0.2.2/jianglab.egg-info/PKG-INFO` & `jianglab-0.2.3/jianglab.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.2.2/setup.py` & `jianglab-0.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.2.2',
+    version='0.2.3',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
         "tqdm",
         "scipy",
         "gspread",
         "oauth2client",
-        "parmas",
         "pickle"
 
     ],
     author = "Jiang Zheng",
     author_email = "zjiang314@gmail.com",
     description = "A package for Jiang lab",
     url = "https://github.com/jiang-lab-retina/jianglab.git",
```

