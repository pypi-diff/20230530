# Comparing `tmp/photcalib-0.0.tar.gz` & `tmp/photcalib-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photcalib-0.0.tar", last modified: Fri May 19 14:50:12 2023, max compression
+gzip compressed data, was "photcalib-0.1.tar", last modified: Tue May 30 12:54:04 2023, max compression
```

## Comparing `photcalib-0.0.tar` & `photcalib-0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zyuan      (502) staff       (20)        0 2023-05-19 14:50:12.602103 photcalib-0.0/
--rw-r--r--   0 zyuan      (502) staff       (20)     1089 2023-05-19 07:26:16.000000 photcalib-0.0/LICENSE
--rw-r--r--   0 zyuan      (502) staff       (20)     2463 2023-05-19 14:50:12.601963 photcalib-0.0/PKG-INFO
--rw-r--r--   0 zyuan      (502) staff       (20)     1979 2023-05-19 14:44:00.000000 photcalib-0.0/README.rst
-drwxr-xr-x   0 zyuan      (502) staff       (20)        0 2023-05-19 14:50:12.600521 photcalib-0.0/photcalib/
--rw-r--r--   0 zyuan      (502) staff       (20)      490 2023-05-19 06:46:54.000000 photcalib-0.0/photcalib/__init__.py
--rw-r--r--   0 zyuan      (502) staff       (20)     1878 2023-05-19 06:26:13.000000 photcalib-0.0/photcalib/apply_calib.py
--rw-r--r--   0 zyuan      (502) staff       (20)    28839 2023-05-19 07:03:49.000000 photcalib-0.0/photcalib/make_plots.py
--rw-r--r--   0 zyuan      (502) staff       (20)     1900 2023-05-19 06:47:00.000000 photcalib-0.0/photcalib/model_nn.py
--rw-r--r--   0 zyuan      (502) staff       (20)     1277 2023-05-19 06:50:53.000000 photcalib-0.0/photcalib/model_old.py
--rw-r--r--   0 zyuan      (502) staff       (20)     3456 2023-05-19 07:01:27.000000 photcalib-0.0/photcalib/set_argparse.py
--rw-r--r--   0 zyuan      (502) staff       (20)     6281 2023-05-19 07:05:19.000000 photcalib-0.0/photcalib/training.py
-drwxr-xr-x   0 zyuan      (502) staff       (20)        0 2023-05-19 14:50:12.601719 photcalib-0.0/photcalib.egg-info/
--rw-r--r--   0 zyuan      (502) staff       (20)     2463 2023-05-19 14:50:12.000000 photcalib-0.0/photcalib.egg-info/PKG-INFO
--rw-r--r--   0 zyuan      (502) staff       (20)      355 2023-05-19 14:50:12.000000 photcalib-0.0/photcalib.egg-info/SOURCES.txt
--rw-r--r--   0 zyuan      (502) staff       (20)        1 2023-05-19 14:50:12.000000 photcalib-0.0/photcalib.egg-info/dependency_links.txt
--rw-r--r--   0 zyuan      (502) staff       (20)        1 2023-05-18 09:18:41.000000 photcalib-0.0/photcalib.egg-info/not-zip-safe
--rw-r--r--   0 zyuan      (502) staff       (20)       10 2023-05-19 14:50:12.000000 photcalib-0.0/photcalib.egg-info/top_level.txt
--rw-r--r--   0 zyuan      (502) staff       (20)       38 2023-05-19 14:50:12.602147 photcalib-0.0/setup.cfg
--rw-r--r--   0 zyuan      (502) staff       (20)      766 2023-05-19 14:49:59.000000 photcalib-0.0/setup.py
+drwxr-xr-x   0 zyuan      (502) staff       (20)        0 2023-05-30 12:54:04.651829 photcalib-0.1/
+-rw-r--r--   0 zyuan      (502) staff       (20)     1089 2023-05-19 07:26:16.000000 photcalib-0.1/LICENSE
+-rw-r--r--   0 zyuan      (502) staff       (20)     2463 2023-05-30 12:54:04.651690 photcalib-0.1/PKG-INFO
+-rw-r--r--   0 zyuan      (502) staff       (20)     1979 2023-05-19 14:44:00.000000 photcalib-0.1/README.rst
+drwxr-xr-x   0 zyuan      (502) staff       (20)        0 2023-05-30 12:54:04.650646 photcalib-0.1/photcalib/
+-rw-r--r--   0 zyuan      (502) staff       (20)      493 2023-05-30 12:45:58.000000 photcalib-0.1/photcalib/__init__.py
+-rw-r--r--   0 zyuan      (502) staff       (20)     1878 2023-05-30 12:52:57.000000 photcalib-0.1/photcalib/apply_calib.py
+-rw-r--r--   0 zyuan      (502) staff       (20)     1900 2023-05-30 12:52:21.000000 photcalib-0.1/photcalib/deform_norm.py
+-rw-r--r--   0 zyuan      (502) staff       (20)    28842 2023-05-30 12:46:47.000000 photcalib-0.1/photcalib/make_plots.py
+-rw-r--r--   0 zyuan      (502) staff       (20)     1277 2023-05-19 06:50:53.000000 photcalib-0.1/photcalib/model_old.py
+-rw-r--r--   0 zyuan      (502) staff       (20)     3456 2023-05-19 07:01:27.000000 photcalib-0.1/photcalib/set_argparse.py
+-rw-r--r--   0 zyuan      (502) staff       (20)     6281 2023-05-19 07:05:19.000000 photcalib-0.1/photcalib/training.py
+drwxr-xr-x   0 zyuan      (502) staff       (20)        0 2023-05-30 12:54:04.651500 photcalib-0.1/photcalib.egg-info/
+-rw-r--r--   0 zyuan      (502) staff       (20)     2463 2023-05-30 12:54:04.000000 photcalib-0.1/photcalib.egg-info/PKG-INFO
+-rw-r--r--   0 zyuan      (502) staff       (20)      358 2023-05-30 12:54:04.000000 photcalib-0.1/photcalib.egg-info/SOURCES.txt
+-rw-r--r--   0 zyuan      (502) staff       (20)        1 2023-05-30 12:54:04.000000 photcalib-0.1/photcalib.egg-info/dependency_links.txt
+-rw-r--r--   0 zyuan      (502) staff       (20)        1 2023-05-18 09:18:41.000000 photcalib-0.1/photcalib.egg-info/not-zip-safe
+-rw-r--r--   0 zyuan      (502) staff       (20)       10 2023-05-30 12:54:04.000000 photcalib-0.1/photcalib.egg-info/top_level.txt
+-rw-r--r--   0 zyuan      (502) staff       (20)       38 2023-05-30 12:54:04.651873 photcalib-0.1/setup.cfg
+-rw-r--r--   0 zyuan      (502) staff       (20)      766 2023-05-19 16:02:16.000000 photcalib-0.1/setup.py
```

### Comparing `photcalib-0.0/LICENSE` & `photcalib-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `photcalib-0.0/PKG-INFO` & `photcalib-0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photcalib
-Version: 0.0
+Version: 0.1
 Summary: calibration tool for photometric data
 Home-page: https://github.com/zyuan-astro/PhotCalib
 Author: Zhen Yuan
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
```

### Comparing `photcalib-0.0/README.rst` & `photcalib-0.1/README.rst`

 * *Files identical despite different names*

### Comparing `photcalib-0.0/photcalib/make_plots.py` & `photcalib-0.1/photcalib/make_plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from math import *
 from matplotlib.pyplot import *
 import matplotlib.gridspec as gridspec
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 import numpy as np
 import torch
-from .model_nn import Deform
+from .deform_norm import deform
 from .model_old import FovOldModel
 
 
 mod_path = "model/"
 out_path = "output/" 
 fig_path = "figure/"
```

### Comparing `photcalib-0.0/photcalib/model_nn.py` & `photcalib-0.1/photcalib/deform_norm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import torch
 import torch.nn.functional as F
 
 
-torch.set_default_dtype(torch.float32)
+torch.set_default_dtype(torch.float64)
 
 ## Define a moduel deform
 from typing import Sequence
-class Deform(torch.nn.Module):
+class deform(torch.nn.Module):
     def __init__(self, n_input: int, 
                  n_hidden: Sequence[int], 
                  n_output: int,
                  n_fields: int):
         super().__init__()
         
         # define a vector for field offset correction
```

### Comparing `photcalib-0.0/photcalib/model_old.py` & `photcalib-0.1/photcalib/model_old.py`

 * *Files identical despite different names*

### Comparing `photcalib-0.0/photcalib/set_argparse.py` & `photcalib-0.1/photcalib/set_argparse.py`

 * *Files identical despite different names*

### Comparing `photcalib-0.0/photcalib/training.py` & `photcalib-0.1/photcalib/training.py`

 * *Files identical despite different names*

### Comparing `photcalib-0.0/photcalib.egg-info/PKG-INFO` & `photcalib-0.1/photcalib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photcalib
-Version: 0.0
+Version: 0.1
 Summary: calibration tool for photometric data
 Home-page: https://github.com/zyuan-astro/PhotCalib
 Author: Zhen Yuan
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
```

### Comparing `photcalib-0.0/setup.py` & `photcalib-0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(name = "photcalib",
-    version = 0.0,
+    version = 0.1,
     description = "calibration tool for photometric data",
     long_description = readme(),
     long_description_content_type="text/x-rst",
     author = "Zhen Yuan",
     author_email = "",
     url = "https://github.com/zyuan-astro/PhotCalib",
     packages = find_packages(),
```

