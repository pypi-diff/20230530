# Comparing `tmp/clubscore-0.1.8.tar.gz` & `tmp/clubscore-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clubscore-0.1.8.tar", last modified: Fri May 19 15:36:16 2023, max compression
+gzip compressed data, was "clubscore-0.1.9.tar", last modified: Mon May 29 22:28:21 2023, max compression
```

## Comparing `clubscore-0.1.8.tar` & `clubscore-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-19 15:36:16.000000 clubscore-0.1.8/
--rw-r--r--   0 dave       (501) staff       (20)     1071 2023-05-05 17:29:41.000000 clubscore-0.1.8/LICENSE
--rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-19 15:36:16.000000 clubscore-0.1.8/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)       23 2023-05-06 09:41:10.000000 clubscore-0.1.8/README.md
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-19 15:36:16.000000 clubscore-0.1.8/clubscore/
--rw-r--r--   0 dave       (501) staff       (20)      752 2023-05-09 16:58:15.000000 clubscore-0.1.8/clubscore/API.py
--rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.1.8/clubscore/__init__.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-19 15:36:16.000000 clubscore-0.1.8/clubscore/objects/
--rw-r--r--   0 dave       (501) staff       (20)     5233 2023-05-16 22:07:16.000000 clubscore-0.1.8/clubscore/objects/CONTAINER.py
--rw-r--r--   0 dave       (501) staff       (20)     2408 2023-05-16 22:07:16.000000 clubscore-0.1.8/clubscore/objects/IMG.py
--rw-r--r--   0 dave       (501) staff       (20)     1151 2023-02-04 00:33:04.000000 clubscore-0.1.8/clubscore/objects/RECTANGLE.py
--rw-r--r--   0 dave       (501) staff       (20)     3966 2023-05-16 22:26:38.000000 clubscore-0.1.8/clubscore/objects/TEXT.py
--rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.1.8/clubscore/objects/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)     4201 2023-05-19 15:30:42.000000 clubscore-0.1.8/clubscore/utils.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-19 15:36:16.000000 clubscore-0.1.8/clubscore.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-19 15:36:16.000000 clubscore-0.1.8/clubscore.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)      435 2023-05-19 15:36:16.000000 clubscore-0.1.8/clubscore.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)        1 2023-05-19 15:36:16.000000 clubscore-0.1.8/clubscore.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)       85 2023-05-19 15:36:16.000000 clubscore-0.1.8/clubscore.egg-info/requires.txt
--rw-r--r--   0 dave       (501) staff       (20)       10 2023-05-19 15:36:16.000000 clubscore-0.1.8/clubscore.egg-info/top_level.txt
--rw-r--r--   0 dave       (501) staff       (20)       38 2023-05-19 15:36:16.000000 clubscore-0.1.8/setup.cfg
--rw-r--r--   0 dave       (501) staff       (20)     1220 2023-05-19 15:32:29.000000 clubscore-0.1.8/setup.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-19 15:36:16.000000 clubscore-0.1.8/tests/
--rw-r--r--   0 dave       (501) staff       (20)     1961 2023-05-11 23:19:07.000000 clubscore-0.1.8/tests/test_templates.py
--rw-r--r--   0 dave       (501) staff       (20)      881 2023-05-11 23:17:53.000000 clubscore-0.1.8/tests/test_utils.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-29 22:28:21.387741 clubscore-0.1.9/
+-rw-r--r--   0 dave       (501) staff       (20)     1071 2023-05-05 17:29:41.000000 clubscore-0.1.9/LICENSE
+-rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-29 22:28:21.387363 clubscore-0.1.9/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)       23 2023-05-06 09:41:10.000000 clubscore-0.1.9/README.md
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-29 22:28:21.377835 clubscore-0.1.9/clubscore/
+-rw-r--r--   0 dave       (501) staff       (20)      752 2023-05-09 16:58:15.000000 clubscore-0.1.9/clubscore/API.py
+-rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.1.9/clubscore/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)     4441 2023-05-29 22:20:16.000000 clubscore-0.1.9/clubscore/bot.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-29 22:28:21.384274 clubscore-0.1.9/clubscore/objects/
+-rw-r--r--   0 dave       (501) staff       (20)     5233 2023-05-16 22:07:16.000000 clubscore-0.1.9/clubscore/objects/CONTAINER.py
+-rw-r--r--   0 dave       (501) staff       (20)     2408 2023-05-16 22:07:16.000000 clubscore-0.1.9/clubscore/objects/IMG.py
+-rw-r--r--   0 dave       (501) staff       (20)     1151 2023-02-04 00:33:04.000000 clubscore-0.1.9/clubscore/objects/RECTANGLE.py
+-rw-r--r--   0 dave       (501) staff       (20)     3966 2023-05-16 22:26:38.000000 clubscore-0.1.9/clubscore/objects/TEXT.py
+-rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.1.9/clubscore/objects/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)     4203 2023-05-27 10:59:14.000000 clubscore-0.1.9/clubscore/utils.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-29 22:28:21.380936 clubscore-0.1.9/clubscore.egg-info/
+-rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-29 22:28:21.000000 clubscore-0.1.9/clubscore.egg-info/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)      452 2023-05-29 22:28:21.000000 clubscore-0.1.9/clubscore.egg-info/SOURCES.txt
+-rw-r--r--   0 dave       (501) staff       (20)        1 2023-05-29 22:28:21.000000 clubscore-0.1.9/clubscore.egg-info/dependency_links.txt
+-rw-r--r--   0 dave       (501) staff       (20)       85 2023-05-29 22:28:21.000000 clubscore-0.1.9/clubscore.egg-info/requires.txt
+-rw-r--r--   0 dave       (501) staff       (20)       10 2023-05-29 22:28:21.000000 clubscore-0.1.9/clubscore.egg-info/top_level.txt
+-rw-r--r--   0 dave       (501) staff       (20)       38 2023-05-29 22:28:21.387860 clubscore-0.1.9/setup.cfg
+-rw-r--r--   0 dave       (501) staff       (20)     1220 2023-05-29 22:23:33.000000 clubscore-0.1.9/setup.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-29 22:28:21.386078 clubscore-0.1.9/tests/
+-rw-r--r--   0 dave       (501) staff       (20)     1961 2023-05-11 23:19:07.000000 clubscore-0.1.9/tests/test_templates.py
+-rw-r--r--   0 dave       (501) staff       (20)      881 2023-05-11 23:17:53.000000 clubscore-0.1.9/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `clubscore-0.1.8/LICENSE` & `clubscore-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.8/PKG-INFO` & `clubscore-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clubscore
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for creating customizable templates in XML
 Home-page: https://github.com/davegimo/clubscore
 Author: Davide Gimondo
 Author-email: davegimo@gmail.com
 License: MIT
 Keywords: my-package,example,demo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clubscore-0.1.8/clubscore/API.py` & `clubscore-0.1.9/clubscore/API.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.8/clubscore/objects/CONTAINER.py` & `clubscore-0.1.9/clubscore/objects/CONTAINER.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.8/clubscore/objects/IMG.py` & `clubscore-0.1.9/clubscore/objects/IMG.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.8/clubscore/objects/RECTANGLE.py` & `clubscore-0.1.9/clubscore/objects/RECTANGLE.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.8/clubscore/objects/TEXT.py` & `clubscore-0.1.9/clubscore/objects/TEXT.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.8/clubscore/utils.py` & `clubscore-0.1.9/clubscore/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,7 +179,9 @@
 
 def super_print(*args, **kwargs):
     for arg in args:
         print(f"{arg} = {eval(arg)}")
 
     for name, value in kwargs.items():
         print(f"{name} = {value}")
+
+
```

### Comparing `clubscore-0.1.8/clubscore.egg-info/PKG-INFO` & `clubscore-0.1.9/clubscore.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clubscore
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for creating customizable templates in XML
 Home-page: https://github.com/davegimo/clubscore
 Author: Davide Gimondo
 Author-email: davegimo@gmail.com
 License: MIT
 Keywords: my-package,example,demo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clubscore-0.1.8/setup.py` & `clubscore-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='clubscore',
-    version='0.1.8',
+    version='0.1.9',
     author='Davide Gimondo',
     author_email='davegimo@gmail.com',
     description='A package for creating customizable templates in XML',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/davegimo/clubscore',
     packages=find_packages(),
```

### Comparing `clubscore-0.1.8/tests/test_templates.py` & `clubscore-0.1.9/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.8/tests/test_utils.py` & `clubscore-0.1.9/tests/test_utils.py`

 * *Files identical despite different names*

