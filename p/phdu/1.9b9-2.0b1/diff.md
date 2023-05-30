# Comparing `tmp/phdu-1.9b9.tar.gz` & `tmp/phdu-2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-1.9b9.tar", last modified: Tue May  9 13:23:46 2023, max compression
+gzip compressed data, was "phdu-2.0b1.tar", last modified: Tue May 30 10:06:10 2023, max compression
```

## Comparing `phdu-1.9b9.tar` & `phdu-2.0b1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 13:23:46.424078 phdu-1.9b9/
--rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-1.9b9/LICENSE.md
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-05-09 13:23:46.428078 phdu-1.9b9/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-1.9b9/README.md
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 13:23:46.352075 phdu-1.9b9/phdu/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      486 2023-03-07 15:15:16.000000 phdu-1.9b9/phdu/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      608 2023-02-14 14:36:41.000000 phdu-1.9b9/phdu/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2828 2023-03-16 13:46:54.000000 phdu-1.9b9/phdu/clustering.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-1.9b9/phdu/decomposition.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2628 2023-02-14 17:21:31.000000 phdu-1.9b9/phdu/np_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     5912 2023-03-16 10:33:06.000000 phdu-1.9b9/phdu/pd_utils.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 13:23:46.384076 phdu-1.9b9/phdu/plots/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-1.9b9/phdu/plots/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-1.9b9/phdu/plots/_mpl.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3359 2022-11-09 08:55:15.000000 phdu-1.9b9/phdu/plots/base.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    14228 2023-05-09 13:23:15.000000 phdu-1.9b9/phdu/plots/plotly_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-1.9b9/phdu/script_fmt.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 13:23:46.408077 phdu-1.9b9/phdu/stats/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-1.9b9/phdu/stats/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-1.9b9/phdu/stats/_integration.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-1.9b9/phdu/stats/_plots.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-1.9b9/phdu/stats/_preprocess.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    31968 2023-05-09 10:58:12.000000 phdu-1.9b9/phdu/stats/bootstrap.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-1.9b9/phdu/stats/conf_interval.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-1.9b9/phdu/stats/corr.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 13:23:46.416078 phdu-1.9b9/phdu/stats/rtopy/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-1.9b9/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-1.9b9/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-1.9b9/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 13:23:46.424078 phdu-1.9b9/phdu/stats/test/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-1.9b9/phdu/stats/test/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-1.9b9/phdu/stats/test/_adherence.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-1.9b9/phdu/stats/test/permutation.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4179 2023-04-25 11:08:38.000000 phdu-1.9b9/phdu/storage.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 13:23:46.372076 phdu-1.9b9/phdu.egg-info/
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-05-09 13:23:46.000000 phdu-1.9b9/phdu.egg-info/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)      752 2023-05-09 13:23:46.000000 phdu-1.9b9/phdu.egg-info/SOURCES.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-05-09 13:23:46.000000 phdu-1.9b9/phdu.egg-info/dependency_links.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2023-05-09 13:23:46.000000 phdu-1.9b9/phdu.egg-info/requires.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2023-05-09 13:23:46.000000 phdu-1.9b9/phdu.egg-info/top_level.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-05-09 13:23:46.432078 phdu-1.9b9/setup.cfg
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1660 2023-05-09 13:23:40.000000 phdu-1.9b9/setup.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-30 10:06:10.434967 phdu-2.0b1/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-2.0b1/LICENSE.md
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-05-30 10:06:10.434967 phdu-2.0b1/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-2.0b1/README.md
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-30 10:06:10.314962 phdu-2.0b1/phdu/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      486 2023-03-07 15:15:16.000000 phdu-2.0b1/phdu/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      608 2023-02-14 14:36:41.000000 phdu-2.0b1/phdu/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2828 2023-03-16 13:46:54.000000 phdu-2.0b1/phdu/clustering.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-2.0b1/phdu/decomposition.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2628 2023-02-14 17:21:31.000000 phdu-2.0b1/phdu/np_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     5912 2023-03-16 10:33:06.000000 phdu-2.0b1/phdu/pd_utils.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-30 10:06:10.362964 phdu-2.0b1/phdu/plots/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-2.0b1/phdu/plots/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-2.0b1/phdu/plots/_mpl.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3359 2022-11-09 08:55:15.000000 phdu-2.0b1/phdu/plots/base.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    14228 2023-05-09 13:23:15.000000 phdu-2.0b1/phdu/plots/plotly_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-2.0b1/phdu/script_fmt.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-30 10:06:10.406966 phdu-2.0b1/phdu/stats/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-2.0b1/phdu/stats/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-2.0b1/phdu/stats/_integration.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-2.0b1/phdu/stats/_plots.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-2.0b1/phdu/stats/_preprocess.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    32227 2023-05-30 10:04:40.000000 phdu-2.0b1/phdu/stats/bootstrap.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-2.0b1/phdu/stats/conf_interval.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-2.0b1/phdu/stats/corr.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-30 10:06:10.418967 phdu-2.0b1/phdu/stats/rtopy/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-2.0b1/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-2.0b1/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-2.0b1/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-30 10:06:10.430967 phdu-2.0b1/phdu/stats/test/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-2.0b1/phdu/stats/test/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-2.0b1/phdu/stats/test/_adherence.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-2.0b1/phdu/stats/test/permutation.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4179 2023-04-25 11:08:38.000000 phdu-2.0b1/phdu/storage.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-30 10:06:10.342963 phdu-2.0b1/phdu.egg-info/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-05-30 10:06:09.000000 phdu-2.0b1/phdu.egg-info/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      752 2023-05-30 10:06:10.000000 phdu-2.0b1/phdu.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-05-30 10:06:10.000000 phdu-2.0b1/phdu.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2023-05-30 10:06:10.000000 phdu-2.0b1/phdu.egg-info/requires.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2023-05-30 10:06:10.000000 phdu-2.0b1/phdu.egg-info/top_level.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-05-30 10:06:10.442968 phdu-2.0b1/setup.cfg
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1660 2023-05-30 10:05:26.000000 phdu-2.0b1/setup.py
```

### Comparing `phdu-1.9b9/LICENSE.md` & `phdu-2.0b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-1.9b9/PKG-INFO` & `phdu-2.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.9b9
+Version: 2.0b1
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.9b9/README.md` & `phdu-2.0b1/README.md`

 * *Files identical despite different names*

### Comparing `phdu-1.9b9/phdu/_helper.py` & `phdu-2.0b1/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b9/phdu/clustering.py` & `phdu-2.0b1/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b9/phdu/decomposition.py` & `phdu-2.0b1/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b9/phdu/np_utils.py` & `phdu-2.0b1/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b9/phdu/pd_utils.py` & `phdu-2.0b1/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b9/phdu/plots/base.py` & `phdu-2.0b1/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b9/phdu/plots/plotly_utils.py` & `phdu-2.0b1/phdu/plots/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b9/phdu/script_fmt.py` & `phdu-2.0b1/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b9/phdu/stats/_integration.py` & `phdu-2.0b1/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b9/phdu/stats/_plots.py` & `phdu-2.0b1/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b9/phdu/stats/bootstrap.py` & `phdu-2.0b1/phdu/stats/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,19 @@
     """
     np.random.seed(seed)
     R_T = R * R_B
     boot_sample = np.empty((R_T, output_len))
 
     num_blocks = len(X)
     assert num_blocks == len(Y), "X and Y must have the same # blocks"
+    # Take only common blocks (x, y) where x and y have at least 1 element.
+    idxs_common_blocks = [i for i, (x, y) in enumerate(zip(X, Y)) if len(x) > 0 and len(y) > 0]
+    X = [X[i] for i in idxs_common_blocks]
+    Y = [Y[i] for i in idxs_common_blocks]
+
     idxs_resampling_blocks = np.random.randint(low=0, high=num_blocks, size=R*num_blocks).reshape(R, num_blocks)
 
     for i, idx_blocks in enumerate(idxs_resampling_blocks):
         Xi = [X[k] for k in idx_blocks]
         Yi = [Y[k] for k in idx_blocks]
         n_Xi = [len(x) for x in Xi]
         n_Yi = [len(y) for y in Yi]
```

### Comparing `phdu-1.9b9/phdu/stats/conf_interval.py` & `phdu-2.0b1/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b9/phdu/stats/corr.py` & `phdu-2.0b1/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b9/phdu/stats/rtopy/_helper.py` & `phdu-2.0b1/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b9/phdu/stats/rtopy/resample.py` & `phdu-2.0b1/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b9/phdu/stats/test/permutation.py` & `phdu-2.0b1/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b9/phdu/storage.py` & `phdu-2.0b1/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b9/phdu.egg-info/PKG-INFO` & `phdu-2.0b1/phdu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.9b9
+Version: 2.0b1
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.9b9/phdu.egg-info/SOURCES.txt` & `phdu-2.0b1/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-1.9b9/setup.py` & `phdu-2.0b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='1.9.b9',
+    version='2.0.b1',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```

