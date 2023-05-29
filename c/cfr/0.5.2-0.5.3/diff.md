# Comparing `tmp/cfr-0.5.2.tar.gz` & `tmp/cfr-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-0.5.2.tar", last modified: Mon May 29 21:58:35 2023, max compression
+gzip compressed data, was "cfr-0.5.3.tar", last modified: Mon May 29 23:40:25 2023, max compression
```

## Comparing `cfr-0.5.2.tar` & `cfr-0.5.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 21:58:35.718806 cfr-0.5.2/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-0.5.2/LICENSE
--rw-r--r--   0 fengzhu    (502) staff       (20)     1771 2023-05-29 21:58:35.718629 cfr-0.5.2/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)     1207 2023-05-29 21:16:00.000000 cfr-0.5.2/README.md
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 21:58:35.708847 cfr-0.5.2/bin/
--rw-r--r--   0 fengzhu    (502) staff       (20)     3905 2022-07-04 04:11:55.000000 cfr-0.5.2/bin/cfr
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 21:58:35.714622 cfr-0.5.2/cfr/
--rw-r--r--   0 fengzhu    (502) staff       (20)      640 2023-03-24 23:03:50.000000 cfr-0.5.2/cfr/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    20667 2023-05-29 21:16:00.000000 cfr-0.5.2/cfr/climate.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 21:58:35.718135 cfr-0.5.2/cfr/da/
--rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-0.5.2/cfr/da/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-0.5.2/cfr/da/enkf.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-0.5.2/cfr/gcm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-0.5.2/cfr/ml.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    63265 2023-05-29 21:16:00.000000 cfr-0.5.2/cfr/proxy.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    44993 2023-05-29 21:16:00.000000 cfr-0.5.2/cfr/psm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    49995 2023-05-29 21:16:00.000000 cfr-0.5.2/cfr/reconjob.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     2311 2023-03-27 02:39:30.000000 cfr-0.5.2/cfr/reconres.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-05-29 21:16:00.000000 cfr-0.5.2/cfr/ts.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    26581 2023-05-29 21:16:00.000000 cfr-0.5.2/cfr/utils.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    54810 2023-04-17 19:25:37.000000 cfr-0.5.2/cfr/visual.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 21:58:35.717304 cfr-0.5.2/cfr.egg-info/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1771 2023-05-29 21:58:35.000000 cfr-0.5.2/cfr.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-05-29 21:58:35.000000 cfr-0.5.2/cfr.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-05-29 21:58:35.000000 cfr-0.5.2/cfr.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-0.5.2/cfr.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu    (502) staff       (20)      203 2023-05-29 21:58:35.000000 cfr-0.5.2/cfr.egg-info/requires.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-05-29 21:58:35.000000 cfr-0.5.2/cfr.egg-info/top_level.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-05-29 21:58:35.718864 cfr-0.5.2/setup.cfg
--rw-r--r--   0 fengzhu    (502) staff       (20)     1414 2023-05-29 21:57:43.000000 cfr-0.5.2/setup.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 23:40:25.535761 cfr-0.5.3/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-0.5.3/LICENSE
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1771 2023-05-29 23:40:25.535558 cfr-0.5.3/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1207 2023-05-29 21:16:00.000000 cfr-0.5.3/README.md
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 23:40:25.524985 cfr-0.5.3/bin/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     3905 2022-07-04 04:11:55.000000 cfr-0.5.3/bin/cfr
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 23:40:25.530969 cfr-0.5.3/cfr/
+-rw-r--r--   0 fengzhu    (502) staff       (20)      640 2023-03-24 23:03:50.000000 cfr-0.5.3/cfr/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22467 2023-05-29 23:34:35.000000 cfr-0.5.3/cfr/climate.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 23:40:25.534929 cfr-0.5.3/cfr/da/
+-rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-0.5.3/cfr/da/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-0.5.3/cfr/da/enkf.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-0.5.3/cfr/gcm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-0.5.3/cfr/ml.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    63265 2023-05-29 21:16:00.000000 cfr-0.5.3/cfr/proxy.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    44993 2023-05-29 21:16:00.000000 cfr-0.5.3/cfr/psm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    49995 2023-05-29 21:16:00.000000 cfr-0.5.3/cfr/reconjob.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     2311 2023-03-27 02:39:30.000000 cfr-0.5.3/cfr/reconres.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-05-29 21:16:00.000000 cfr-0.5.3/cfr/ts.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    26581 2023-05-29 21:16:00.000000 cfr-0.5.3/cfr/utils.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    54810 2023-04-17 19:25:37.000000 cfr-0.5.3/cfr/visual.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 23:40:25.534067 cfr-0.5.3/cfr.egg-info/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1771 2023-05-29 23:40:25.000000 cfr-0.5.3/cfr.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-05-29 23:40:25.000000 cfr-0.5.3/cfr.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-05-29 23:40:25.000000 cfr-0.5.3/cfr.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-0.5.3/cfr.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu    (502) staff       (20)      203 2023-05-29 23:40:25.000000 cfr-0.5.3/cfr.egg-info/requires.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-05-29 23:40:25.000000 cfr-0.5.3/cfr.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-05-29 23:40:25.535820 cfr-0.5.3/setup.cfg
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1414 2023-05-29 23:40:02.000000 cfr-0.5.3/setup.py
```

### Comparing `cfr-0.5.2/LICENSE` & `cfr-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-0.5.2/PKG-INFO` & `cfr-0.5.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.5.2
+Version: 0.5.3
 Summary: cfr: the Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: paleocliamte reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-0.5.2/README.md` & `cfr-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `cfr-0.5.2/bin/cfr` & `cfr-0.5.3/bin/cfr`

 * *Files identical despite different names*

### Comparing `cfr-0.5.2/cfr/__init__.py` & `cfr-0.5.3/cfr/__init__.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.2/cfr/climate.py` & `cfr-0.5.3/cfr/climate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 from datetime import datetime
+import cftime
 import xarray as xr
 import pandas as pd
 import numpy as np
 import copy
 import plotly.express as px
 from tqdm import tqdm
 from . import visual
@@ -19,26 +20,72 @@
         da (xarray.DataArray): the gridded data array.
     '''
     def __init__(self, da=None):
         self.da = da
 
     def __getitem__(self, key):
         ''' This makes the object subscriptable. '''
-        if type(key) is int or type(key) is list:
+        if type(key) is int:
+            # one index
             da = self.da[key]
-        else:
-            if type(key) is str: 
-                key = slice(key, key, None)
-            elif type(key) is not slice:
-                raise TypeError('Wrong type for key!')
-
+        elif type(key) is str:
+            # one timestamp
+            # key = slice(key, key, None)
+            # da = self.da.sel({'time': key})
+            # if len(da.values) == 0:
+            #     mask = (self.da['time']>=float(key.start)) & (self.da['time']<=float(key.stop))
+            #     da = self.da.sel({'time': mask})
             try:
-                da = self.da.sel({'time': slice(float(key.start), float(key.stop), key.step)})
+                mask = (utils.datetime2year_float(self.da['time'].values)>=float(key)) & (utils.datetime2year_float(self.da['time'].values)<float(key)+1)
             except:
-                da = self.da.loc[key]
+                mask = (self.da['time'].values>=float(key)) & (self.da['time'].values<float(key)+1)
+
+            da = self.da.sel({'time': mask})
+
+        elif type(key) is list:
+            # multiple discrete items
+            if type(key[0]) is int:
+                # index
+                da = self.da[key]
+            elif type(key[0]) is str:
+                # timestamp
+                da_list = []
+                for k in key:
+                    da_list.append(self[k].da)
+                da = xr.concat(da_list, dim='time')
+                
+        elif type(key) is slice:
+            if key.start is not None:
+                dtype = type(key.start)
+            else:
+                key.start = self.da['time'][0]
+
+            if key.stop is not None:
+                dtype = type(key.stop)
+            else:
+                key.stop = self.da['time'][-1]
+
+            if dtype is int:
+                # index
+                da = self.da[key]
+            elif dtype is str:
+                # timestamp
+                try:
+                    mask = (utils.datetime2year_float(self.da['time'].values)>=float(key.start)) & (utils.datetime2year_float(self.da['time'].values)<float(key.stop))
+                except:
+                    mask = (self.da['time'].values>=float(key.start)) & (self.da['time'].values<float(key.stop))
+
+                da = self.da.sel({'time': mask})
+                if key.step is not None:
+                    da = da[::int(key.step)]
+
+            else:
+                raise TypeError('Wrong type for key!')
+        else:
+            raise TypeError('Wrong type for key!')
 
         fd = ClimateField(da)
 
         return fd
 
     def __len__(self):
         return len(self.time)
```

### Comparing `cfr-0.5.2/cfr/da/enkf.py` & `cfr-0.5.3/cfr/da/enkf.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.2/cfr/gcm.py` & `cfr-0.5.3/cfr/gcm.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.2/cfr/ml.py` & `cfr-0.5.3/cfr/ml.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.2/cfr/proxy.py` & `cfr-0.5.3/cfr/proxy.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.2/cfr/psm.py` & `cfr-0.5.3/cfr/psm.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.2/cfr/reconjob.py` & `cfr-0.5.3/cfr/reconjob.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.2/cfr/reconres.py` & `cfr-0.5.3/cfr/reconres.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.2/cfr/ts.py` & `cfr-0.5.3/cfr/ts.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.2/cfr/utils.py` & `cfr-0.5.3/cfr/utils.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.2/cfr/visual.py` & `cfr-0.5.3/cfr/visual.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.2/cfr.egg-info/PKG-INFO` & `cfr-0.5.3/cfr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.5.2
+Version: 0.5.3
 Summary: cfr: the Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: paleocliamte reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-0.5.2/setup.py` & `cfr-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='cfr',  # required
-    version='0.5.2',
+    version='0.5.3',
     description='cfr: the Python package for Climate Field Reconstruction',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr',
     packages=find_packages(),
```

