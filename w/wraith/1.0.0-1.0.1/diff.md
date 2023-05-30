# Comparing `tmp/wraith-1.0.0.tar.gz` & `tmp/wraith-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wraith-1.0.0.tar", last modified: Tue May 30 18:56:31 2023, max compression
+gzip compressed data, was "wraith-1.0.1.tar", last modified: Tue May 30 19:09:57 2023, max compression
```

## Comparing `wraith-1.0.0.tar` & `wraith-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 18:56:31.386546 wraith-1.0.0/
--rw-rw-rw-   0        0        0     1359 2023-05-24 05:25:07.000000 wraith-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1231 2023-05-30 18:56:31.384546 wraith-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1972 2023-05-30 18:40:49.000000 wraith-1.0.0/README.md
--rw-rw-rw-   0        0        0      104 2023-05-24 03:36:59.000000 wraith-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 18:56:31.387546 wraith-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1339 2023-05-30 18:41:43.000000 wraith-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:56:31.380551 wraith-1.0.0/wraith.egg-info/
--rw-rw-rw-   0        0        0     1231 2023-05-30 18:56:31.000000 wraith-1.0.0/wraith.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-05-30 18:56:31.000000 wraith-1.0.0/wraith.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 18:56:31.000000 wraith-1.0.0/wraith.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 18:56:31.000000 wraith-1.0.0/wraith.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-30 18:56:31.000000 wraith-1.0.0/wraith.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13660 2023-05-30 18:53:17.000000 wraith-1.0.0/wraith.py
+drwxrwxrwx   0        0        0        0 2023-05-30 19:09:57.388242 wraith-1.0.1/
+-rw-rw-rw-   0        0        0     1359 2023-05-24 05:25:07.000000 wraith-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1231 2023-05-30 19:09:57.372620 wraith-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1972 2023-05-30 18:40:49.000000 wraith-1.0.1/README.md
+-rw-rw-rw-   0        0        0      104 2023-05-24 03:36:59.000000 wraith-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 19:09:57.388242 wraith-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1339 2023-05-30 19:06:43.000000 wraith-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 19:09:57.372620 wraith-1.0.1/wraith.egg-info/
+-rw-rw-rw-   0        0        0     1231 2023-05-30 19:09:57.000000 wraith-1.0.1/wraith.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-05-30 19:09:57.000000 wraith-1.0.1/wraith.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 19:09:57.000000 wraith-1.0.1/wraith.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 19:09:57.000000 wraith-1.0.1/wraith.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-30 19:09:57.000000 wraith-1.0.1/wraith.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13657 2023-05-30 19:07:34.000000 wraith-1.0.1/wraith.py
```

### Comparing `wraith-1.0.0/LICENSE` & `wraith-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wraith-1.0.0/PKG-INFO` & `wraith-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wraith
-Version: 1.0.0
+Version: 1.0.1
 Summary: All the power of Python...in the palm of your hand.
 Author: Omer Drkić
 Author-email: omerdrkic2501@gmail.com
 License: Boost Software License 1.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Jupyter
```

### Comparing `wraith-1.0.0/README.md` & `wraith-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `wraith-1.0.0/setup.py` & `wraith-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ﻿from setuptools import setup
 
 setup(
   name = "wraith",
-  version = "1.0.0",
+  version = "1.0.1",
   description = "All the power of Python...in the palm of your hand.",
   long_description = "Wraith is a module programmed by Omer Drkić that adds loads of new features and makes Python easier to use. The module adds some features that the developer felt like they were missing from Python. It also adds some extension to the 'math' library and to the actual Python environment, as well as some useful data manipulation tools.",
   author = "Omer Drkić",
   author_email = "omerdrkic2501@gmail.com",
   py_modules = [
     "wraith"
   ],
```

### Comparing `wraith-1.0.0/wraith.egg-info/PKG-INFO` & `wraith-1.0.1/wraith.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wraith
-Version: 1.0.0
+Version: 1.0.1
 Summary: All the power of Python...in the palm of your hand.
 Author: Omer Drkić
 Author-email: omerdrkic2501@gmail.com
 License: Boost Software License 1.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Jupyter
```

### Comparing `wraith-1.0.0/wraith.py` & `wraith-1.0.1/wraith.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
   """
   return int(value * (10 ** dp)) / 10 ** dp
 
 def run(path: str):
   """
   Runs an external Python script.
   """
-  s.call(["python", f"{path}.py"])
+  s.call(["python", f"{path}"])
 
 def time():
   """
   Returns the number of seconds that passed since the beginning of the program.
   """
   return int(t.time() - timer)
```

