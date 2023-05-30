# Comparing `tmp/zensvi-0.2.0.tar.gz` & `tmp/zensvi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zensvi-0.2.0.tar", max compression
+gzip compressed data, was "zensvi-0.3.0.tar", max compression
```

## Comparing `zensvi-0.2.0.tar` & `zensvi-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.2.0/LICENSE
--rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.2.0/README.md
--rwxr-xr-x   0        0        0      694 2023-05-26 08:59:44.901237 zensvi-0.2.0/pyproject.toml
--rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.2.0/src/zensvi/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.2.0/src/zensvi/cv/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.2.0/src/zensvi/cv/segmentation/__init__.py
--rwxr-xr-x   0        0        0    39841 2023-05-25 00:58:05.893778 zensvi-0.2.0/src/zensvi/cv/segmentation/segmentation.py
--rwxr-xr-x   0        0        0       55 2023-05-14 01:59:06.771355 zensvi-0.2.0/src/zensvi/download/__init__.py
--rwxr-xr-x   0        0        0    22836 2023-05-26 08:59:23.004525 zensvi-0.2.0/src/zensvi/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.2.0/src/zensvi/download/utils/UserAgent.csv
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.2.0/src/zensvi/download/utils/__init__.py
--rwxr-xr-x   0        0        0     8291 2023-05-26 08:32:40.233104 zensvi-0.2.0/src/zensvi/download/utils/geoprocess.py
--rwxr-xr-x   0        0        0     2000 2023-05-14 12:56:31.947491 zensvi-0.2.0/src/zensvi/download/utils/get_pids.py
--rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.2.0/src/zensvi/download/utils/helpers.py
--rwxr-xr-x   0        0        0     8165 2023-05-15 13:48:37.487829 zensvi-0.2.0/src/zensvi/download/utils/imtool.py
--rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.2.0/src/zensvi/download/utils/proxies.csv
--rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.2.0/src/zensvi/transform/__init__.py
--rwxr-xr-x   0        0        0     6500 2023-05-14 01:59:06.778828 zensvi-0.2.0/src/zensvi/transform/transform_image.py
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.2.0/src/zensvi/zensvi.py
--rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 zensvi-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.3.0/LICENSE
+-rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.3.0/README.md
+-rwxr-xr-x   0        0        0      694 2023-05-30 03:03:52.706926 zensvi-0.3.0/pyproject.toml
+-rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.3.0/src/zensvi/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.3.0/src/zensvi/cv/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.3.0/src/zensvi/cv/segmentation/__init__.py
+-rwxr-xr-x   0        0        0    39841 2023-05-25 00:58:05.893778 zensvi-0.3.0/src/zensvi/cv/segmentation/segmentation.py
+-rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.3.0/src/zensvi/download/__init__.py
+-rwxr-xr-x   0        0        0    46012 2023-05-30 03:03:24.804642 zensvi-0.3.0/src/zensvi/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.3.0/src/zensvi/download/utils/UserAgent.csv
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.3.0/src/zensvi/download/utils/__init__.py
+-rwxr-xr-x   0        0        0     8291 2023-05-26 09:00:45.660707 zensvi-0.3.0/src/zensvi/download/utils/geoprocess.py
+-rwxr-xr-x   0        0        0     2000 2023-05-14 12:56:31.947491 zensvi-0.3.0/src/zensvi/download/utils/get_pids.py
+-rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.3.0/src/zensvi/download/utils/helpers.py
+-rwxr-xr-x   0        0        0     8165 2023-05-15 13:48:37.487829 zensvi-0.3.0/src/zensvi/download/utils/imtool.py
+-rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.3.0/src/zensvi/download/utils/proxies.csv
+-rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.3.0/src/zensvi/transform/__init__.py
+-rwxr-xr-x   0        0        0     6500 2023-05-14 01:59:06.778828 zensvi-0.3.0/src/zensvi/transform/transform_image.py
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.3.0/src/zensvi/zensvi.py
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 zensvi-0.3.0/PKG-INFO
```

### Comparing `zensvi-0.2.0/LICENSE` & `zensvi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zensvi-0.2.0/README.md` & `zensvi-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `zensvi-0.2.0/pyproject.toml` & `zensvi-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zensvi"
-version = "0.2.0"
+version = "0.3.0"
 description = "This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner."
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `zensvi-0.2.0/src/zensvi/cv/segmentation/segmentation.py` & `zensvi-0.3.0/src/zensvi/cv/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.2.0/src/zensvi/download/utils/UserAgent.csv` & `zensvi-0.3.0/src/zensvi/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.2.0/src/zensvi/download/utils/geoprocess.py` & `zensvi-0.3.0/src/zensvi/download/utils/geoprocess.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.2.0/src/zensvi/download/utils/get_pids.py` & `zensvi-0.3.0/src/zensvi/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.2.0/src/zensvi/download/utils/helpers.py` & `zensvi-0.3.0/src/zensvi/download/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.2.0/src/zensvi/download/utils/imtool.py` & `zensvi-0.3.0/src/zensvi/download/utils/imtool.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.2.0/src/zensvi/download/utils/proxies.csv` & `zensvi-0.3.0/src/zensvi/download/utils/proxies.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.2.0/src/zensvi/transform/transform_image.py` & `zensvi-0.3.0/src/zensvi/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.2.0/PKG-INFO` & `zensvi-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zensvi
-Version: 0.2.0
+Version: 0.3.0
 Summary: This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner.
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

