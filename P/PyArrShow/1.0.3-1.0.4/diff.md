# Comparing `tmp/PyArrShow-1.0.3.tar.gz` & `tmp/PyArrShow-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyArrShow-1.0.3.tar", last modified: Tue May 30 02:20:13 2023, max compression
+gzip compressed data, was "PyArrShow-1.0.4.tar", last modified: Tue May 30 02:52:22 2023, max compression
```

## Comparing `PyArrShow-1.0.3.tar` & `PyArrShow-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 02:20:13.432372 PyArrShow-1.0.3/
--rw-rw-rw-   0        0        0     1088 2023-05-29 10:29:19.000000 PyArrShow-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      961 2023-05-30 02:20:13.432993 PyArrShow-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-05-29 10:29:41.000000 PyArrShow-1.0.3/README.md
--rw-rw-rw-   0        0        0      604 2023-05-30 02:18:01.000000 PyArrShow-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-05-30 02:20:13.434991 PyArrShow-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      938 2023-05-30 02:18:58.000000 PyArrShow-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 02:20:13.412086 PyArrShow-1.0.3/src/
--rw-rw-rw-   0        0        0     5088 2023-05-30 01:48:38.000000 PyArrShow-1.0.3/src/DataCursorFrame.py
--rw-rw-rw-   0        0        0     3605 2023-05-05 11:35:48.000000 PyArrShow-1.0.3/src/ImgDisplayFrame.py
--rw-rw-rw-   0        0        0    13988 2023-05-06 08:42:19.000000 PyArrShow-1.0.3/src/PilotFrame.py
-drwxrwxrwx   0        0        0        0 2023-05-30 02:20:13.430349 PyArrShow-1.0.3/src/PyArrShow.egg-info/
--rw-rw-rw-   0        0        0      961 2023-05-30 02:20:12.000000 PyArrShow-1.0.3/src/PyArrShow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-05-30 02:20:13.000000 PyArrShow-1.0.3/src/PyArrShow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 02:20:12.000000 PyArrShow-1.0.3/src/PyArrShow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-30 02:20:13.000000 PyArrShow-1.0.3/src/PyArrShow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       77 2023-05-30 02:20:13.000000 PyArrShow-1.0.3/src/PyArrShow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    47475 2023-05-30 02:02:21.000000 PyArrShow-1.0.3/src/pyArrShow.py
--rw-rw-rw-   0        0        0    67984 2023-05-29 12:06:03.000000 PyArrShow-1.0.3/src/qrc_resources.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:52:22.368609 PyArrShow-1.0.4/
+-rw-rw-rw-   0        0        0     1088 2023-05-29 10:29:19.000000 PyArrShow-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      961 2023-05-30 02:52:22.368609 PyArrShow-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-30 02:52:22.351650 PyArrShow-1.0.4/PyArrShow.egg-info/
+-rw-rw-rw-   0        0        0      961 2023-05-30 02:52:21.000000 PyArrShow-1.0.4/PyArrShow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2023-05-30 02:52:22.000000 PyArrShow-1.0.4/PyArrShow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 02:52:21.000000 PyArrShow-1.0.4/PyArrShow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-30 02:52:22.000000 PyArrShow-1.0.4/PyArrShow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 02:52:22.000000 PyArrShow-1.0.4/PyArrShow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      174 2023-05-29 10:29:41.000000 PyArrShow-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 02:52:22.366616 PyArrShow-1.0.4/pyArrShow/
+-rw-rw-rw-   0        0        0     5088 2023-05-30 01:48:38.000000 PyArrShow-1.0.4/pyArrShow/DataCursorFrame.py
+-rw-rw-rw-   0        0        0     3605 2023-05-05 11:35:48.000000 PyArrShow-1.0.4/pyArrShow/ImgDisplayFrame.py
+-rw-rw-rw-   0        0        0    13988 2023-05-06 08:42:19.000000 PyArrShow-1.0.4/pyArrShow/PilotFrame.py
+-rw-rw-rw-   0        0        0    47475 2023-05-30 02:02:21.000000 PyArrShow-1.0.4/pyArrShow/pyArrShow.py
+-rw-rw-rw-   0        0        0    67984 2023-05-29 12:06:03.000000 PyArrShow-1.0.4/pyArrShow/qrc_resources.py
+-rw-rw-rw-   0        0        0      604 2023-05-30 02:52:08.000000 PyArrShow-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-05-30 02:52:22.370605 PyArrShow-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      938 2023-05-30 02:49:35.000000 PyArrShow-1.0.4/setup.py
```

### Comparing `PyArrShow-1.0.3/LICENSE` & `PyArrShow-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.3/PKG-INFO` & `PyArrShow-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: PyArrShow
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python ArrayShow for MRI data visualization.
 Home-page: https://github.com/15625148866/PyArrShow
-Download-URL: https://github.com/15625148866/PyArrShow/archive/refs/tags/v1.0.3.tar.gz
+Download-URL: https://github.com/15625148866/PyArrShow/archive/refs/tags/v1.0.4.tar.gz
 Author: kaixuan,zhao
 Author-email: "Kaixuan,Zhao" <kaixuan_zhao@163.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/15625148866/PyArrShow
 Project-URL: Bug Tracker, https://github.com/15625148866/PyArrShow/issues
 Keywords: MRI,visualization
 Platform: UNKNOWN
```

### Comparing `PyArrShow-1.0.3/pyproject.toml` & `PyArrShow-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["hatchling"]
 build-backend="hatchling.build"
 
 [project]
 name = "PyArrShow"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Kaixuan,Zhao", email="kaixuan_zhao@163.com" },
 ]
 description = "Python ArrayShow for MRI data visualization."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `PyArrShow-1.0.3/setup.py` & `PyArrShow-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #! /usr/bin/env python
 from io import open
 from setuptools import setup, find_packages
 setup(
     name='PyArrShow',
-    version='1.0.3',
+    version='1.0.4',
     description='Python ArrayShow for MRI data visualization.',
     long_description='Python ArrayShow for MRI data visualization.',
     author="kaixuan,zhao",
     author_email='kaixuan_zhao@163.com',
     license='Apache License 2.0',
     url="https://github.com/15625148866/PyArrShow",
-    download_url="https://github.com/15625148866/PyArrShow/archive/refs/tags/v1.0.3.tar.gz",
+    download_url="https://github.com/15625148866/PyArrShow/archive/refs/tags/v1.0.4.tar.gz",
     keywords = ["MRI",'visualization'],
     install_requires=[
         'numpy',
         'PySide6',
         'matplotlib'
     ],
     classifiers=[
```

### Comparing `PyArrShow-1.0.3/src/DataCursorFrame.py` & `PyArrShow-1.0.4/pyArrShow/DataCursorFrame.py`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.3/src/ImgDisplayFrame.py` & `PyArrShow-1.0.4/pyArrShow/ImgDisplayFrame.py`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.3/src/PilotFrame.py` & `PyArrShow-1.0.4/pyArrShow/PilotFrame.py`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.3/src/PyArrShow.egg-info/PKG-INFO` & `PyArrShow-1.0.4/PyArrShow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: PyArrShow
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python ArrayShow for MRI data visualization.
 Home-page: https://github.com/15625148866/PyArrShow
-Download-URL: https://github.com/15625148866/PyArrShow/archive/refs/tags/v1.0.3.tar.gz
+Download-URL: https://github.com/15625148866/PyArrShow/archive/refs/tags/v1.0.4.tar.gz
 Author: kaixuan,zhao
 Author-email: "Kaixuan,Zhao" <kaixuan_zhao@163.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/15625148866/PyArrShow
 Project-URL: Bug Tracker, https://github.com/15625148866/PyArrShow/issues
 Keywords: MRI,visualization
 Platform: UNKNOWN
```

### Comparing `PyArrShow-1.0.3/src/pyArrShow.py` & `PyArrShow-1.0.4/pyArrShow/pyArrShow.py`

 * *Files identical despite different names*

### Comparing `PyArrShow-1.0.3/src/qrc_resources.py` & `PyArrShow-1.0.4/pyArrShow/qrc_resources.py`

 * *Files identical despite different names*

