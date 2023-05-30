# Comparing `tmp/seepeeyou-1.tar.gz` & `tmp/seepeeyou-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seepeeyou-1.tar", last modified: Fri Feb 17 22:57:39 2023, max compression
+gzip compressed data, was "seepeeyou-2.tar", last modified: Tue May 30 13:50:31 2023, max compression
```

## Comparing `seepeeyou-1.tar` & `seepeeyou-2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 coco      (1001) coco      (1001)        0 2023-02-17 22:57:39.081085 seepeeyou-1/
--rw-rw-r--   0 coco      (1001) coco      (1001)      540 2023-02-17 22:57:39.081085 seepeeyou-1/PKG-INFO
--rw-rw-r--   0 coco      (1001) coco      (1001)     1290 2023-02-17 22:56:13.000000 seepeeyou-1/cpu.py
-drwxrwxr-x   0 coco      (1001) coco      (1001)        0 2023-02-17 22:57:39.081085 seepeeyou-1/seepeeyou.egg-info/
--rw-rw-r--   0 coco      (1001) coco      (1001)      540 2023-02-17 22:57:39.000000 seepeeyou-1/seepeeyou.egg-info/PKG-INFO
--rw-rw-r--   0 coco      (1001) coco      (1001)      147 2023-02-17 22:57:39.000000 seepeeyou-1/seepeeyou.egg-info/SOURCES.txt
--rw-rw-r--   0 coco      (1001) coco      (1001)        1 2023-02-17 22:57:39.000000 seepeeyou-1/seepeeyou.egg-info/dependency_links.txt
--rw-rw-r--   0 coco      (1001) coco      (1001)        4 2023-02-17 22:57:39.000000 seepeeyou-1/seepeeyou.egg-info/top_level.txt
--rw-rw-r--   0 coco      (1001) coco      (1001)       38 2023-02-17 22:57:39.081085 seepeeyou-1/setup.cfg
--rw-rw-r--   0 coco      (1001) coco      (1001)      545 2023-02-17 22:56:26.000000 seepeeyou-1/setup.py
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-05-30 13:50:31.041568 seepeeyou-2/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      529 2023-05-30 13:50:31.041568 seepeeyou-2/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1309 2023-05-30 13:49:30.000000 seepeeyou-2/cpu.py
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-05-30 13:50:31.041568 seepeeyou-2/seepeeyou.egg-info/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      529 2023-05-30 13:50:31.000000 seepeeyou-2/seepeeyou.egg-info/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)      147 2023-05-30 13:50:31.000000 seepeeyou-2/seepeeyou.egg-info/SOURCES.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-05-30 13:50:31.000000 seepeeyou-2/seepeeyou.egg-info/dependency_links.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        4 2023-05-30 13:50:31.000000 seepeeyou-2/seepeeyou.egg-info/top_level.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-05-30 13:50:31.045568 seepeeyou-2/setup.cfg
+-rw-rw-r--   0 coco      (1000) coco      (1000)      545 2023-05-30 13:49:21.000000 seepeeyou-2/setup.py
```

### Comparing `seepeeyou-1/PKG-INFO` & `seepeeyou-2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: seepeeyou
-Version: 1
+Version: 2
 Summary: The Definitive Interface for Image Processing Practitioners
 Home-page: https://github.com/mnhrdt/imscript
 Author: Enric Meinhardt-Llopis
 Author-email: enric.meinhardt@fastmail.com
 License: UNKNOWN
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Mathematics
+
+UNKNOWN
+
```

### Comparing `seepeeyou-1/cpu.py` & `seepeeyou-2/cpu.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 		else:
 			return s
 	except (NameError, KeyError):
 		return s
 
 # API
 def cpu(x):
-	if x == "version":
+	if type(x) == str and x == "version":
 		global version
 		return version
 
 	if x.shape[0] > 4000:
 		x = x.reshape(__heuristic_reshape(x.shape))
 
 	import tempfile, iio, os
@@ -40,9 +40,9 @@
 	os.system(c)
 
 # auxiliary function to import the module as a function
 def __export_cpu():
 	import sys
 	sys.modules[__name__] = cpu
 
-version = 1
+version = 2
 __export_cpu()
```

### Comparing `seepeeyou-1/seepeeyou.egg-info/PKG-INFO` & `seepeeyou-2/seepeeyou.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: seepeeyou
-Version: 1
+Version: 2
 Summary: The Definitive Interface for Image Processing Practitioners
 Home-page: https://github.com/mnhrdt/imscript
 Author: Enric Meinhardt-Llopis
 Author-email: enric.meinhardt@fastmail.com
 License: UNKNOWN
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Mathematics
+
+UNKNOWN
+
```

### Comparing `seepeeyou-1/setup.py` & `seepeeyou-2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 import setuptools
 
 setuptools.setup(
 	name = "seepeeyou",
-	version = "1",
+	version = "2",
 	author = "Enric Meinhardt-Llopis",
 	author_email = "enric.meinhardt@fastmail.com",
 	description = "The Definitive Interface for Image Processing Practitioners",
 	url = "https://github.com/mnhrdt/imscript",
 	classifiers = [
 		"Operating System :: OS Independent",
 		"License :: OSI Approved :: GNU Affero General Public License v3",
```

