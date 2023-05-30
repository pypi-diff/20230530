# Comparing `tmp/zensvi-0.3.1.tar.gz` & `tmp/zensvi-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zensvi-0.3.1.tar", max compression
+gzip compressed data, was "zensvi-0.3.2.tar", max compression
```

## Comparing `zensvi-0.3.1.tar` & `zensvi-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.3.1/LICENSE
--rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.3.1/README.md
--rwxr-xr-x   0        0        0      713 2023-05-30 09:07:08.808023 zensvi-0.3.1/pyproject.toml
--rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.3.1/src/zensvi/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.3.1/src/zensvi/cv/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.3.1/src/zensvi/cv/segmentation/__init__.py
--rwxr-xr-x   0        0        0    39841 2023-05-25 00:58:05.893778 zensvi-0.3.1/src/zensvi/cv/segmentation/segmentation.py
--rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.3.1/src/zensvi/download/__init__.py
--rwxr-xr-x   0        0        0    46012 2023-05-30 03:03:24.804642 zensvi-0.3.1/src/zensvi/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.3.1/src/zensvi/download/utils/UserAgent.csv
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.3.1/src/zensvi/download/utils/__init__.py
--rwxr-xr-x   0        0        0     8291 2023-05-26 09:00:45.660707 zensvi-0.3.1/src/zensvi/download/utils/geoprocess.py
--rwxr-xr-x   0        0        0     2000 2023-05-14 12:56:31.947491 zensvi-0.3.1/src/zensvi/download/utils/get_pids.py
--rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.3.1/src/zensvi/download/utils/helpers.py
--rwxr-xr-x   0        0        0     8165 2023-05-15 13:48:37.487829 zensvi-0.3.1/src/zensvi/download/utils/imtool.py
--rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.3.1/src/zensvi/download/utils/proxies.csv
--rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.3.1/src/zensvi/transform/__init__.py
--rwxr-xr-x   0        0        0     6500 2023-05-14 01:59:06.778828 zensvi-0.3.1/src/zensvi/transform/transform_image.py
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.3.1/src/zensvi/zensvi.py
--rw-r--r--   0        0        0     1818 1970-01-01 00:00:00.000000 zensvi-0.3.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.3.2/LICENSE
+-rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.3.2/README.md
+-rwxr-xr-x   0        0        0      713 2023-05-30 09:40:06.998466 zensvi-0.3.2/pyproject.toml
+-rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.3.2/src/zensvi/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.3.2/src/zensvi/cv/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.3.2/src/zensvi/cv/segmentation/__init__.py
+-rwxr-xr-x   0        0        0    39841 2023-05-25 00:58:05.893778 zensvi-0.3.2/src/zensvi/cv/segmentation/segmentation.py
+-rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.3.2/src/zensvi/download/__init__.py
+-rwxr-xr-x   0        0        0    46422 2023-05-30 09:39:28.956044 zensvi-0.3.2/src/zensvi/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.3.2/src/zensvi/download/utils/UserAgent.csv
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.3.2/src/zensvi/download/utils/__init__.py
+-rwxr-xr-x   0        0        0     8291 2023-05-26 09:00:45.660707 zensvi-0.3.2/src/zensvi/download/utils/geoprocess.py
+-rwxr-xr-x   0        0        0     2000 2023-05-14 12:56:31.947491 zensvi-0.3.2/src/zensvi/download/utils/get_pids.py
+-rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.3.2/src/zensvi/download/utils/helpers.py
+-rwxr-xr-x   0        0        0     8165 2023-05-15 13:48:37.487829 zensvi-0.3.2/src/zensvi/download/utils/imtool.py
+-rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.3.2/src/zensvi/download/utils/proxies.csv
+-rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.3.2/src/zensvi/transform/__init__.py
+-rwxr-xr-x   0        0        0     6500 2023-05-14 01:59:06.778828 zensvi-0.3.2/src/zensvi/transform/transform_image.py
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.3.2/src/zensvi/zensvi.py
+-rw-r--r--   0        0        0     1818 1970-01-01 00:00:00.000000 zensvi-0.3.2/PKG-INFO
```

### Comparing `zensvi-0.3.1/LICENSE` & `zensvi-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zensvi-0.3.1/README.md` & `zensvi-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `zensvi-0.3.1/pyproject.toml` & `zensvi-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zensvi"
-version = "0.3.1"
+version = "0.3.2"
 description = "This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner."
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `zensvi-0.3.1/src/zensvi/cv/segmentation/segmentation.py` & `zensvi-0.3.2/src/zensvi/cv/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.3.1/src/zensvi/download/streetview_downloader.py` & `zensvi-0.3.2/src/zensvi/download/streetview_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,14 +342,19 @@
         return results_df
 
     def _get_pids_from_gdf(self, gdf, id_columns, closest=False, disp=False):  
         if self.cache_lat_lon.exists():
             df = pd.read_csv(self.cache_lat_lon)
             print("The lat and lon have been read from the cache")
         else:
+            if gdf.crs is None:
+                gdf = gdf.set_crs('EPSG:4326')
+            elif gdf.crs != 'EPSG:4326':
+                # convert to EPSG:4326
+                gdf = gdf.to_crs('EPSG:4326')
             # read shapefile
             gp = GeoProcessor(gdf, distance=self.distance, grid=self.grid, grid_size=self.grid_size, id_columns = id_columns)
             df = gp.get_lat_lon()
             df['lat_lon_id'] = np.arange(1, len(df) + 1)
             # save df to cache
             df.to_csv(self.cache_lat_lon, index=False)
 
@@ -695,14 +700,19 @@
         return results_df
 
     def _get_pids_from_gdf(self, gdf, id_columns, **kwargs):
         if self.cache_lat_lon.exists():
             df = pd.read_csv(self.cache_lat_lon)
             print("The lat and lon have been read from the cache")
         else:
+            if gdf.crs is None:
+                gdf = gdf.set_crs('EPSG:4326')
+            elif gdf.crs != 'EPSG:4326':
+                # convert to EPSG:4326
+                gdf = gdf.to_crs('EPSG:4326')
             # read shapefile
             gp = GeoProcessor(gdf, distance=self.distance, grid=self.grid, grid_size=self.grid_size, id_columns = id_columns)
             df = gp.get_lat_lon()
             df['lat_lon_id'] = np.arange(1, len(df) + 1)
             # save df to cache
             df.to_csv(self.cache_lat_lon, index=False)
```

### Comparing `zensvi-0.3.1/src/zensvi/download/utils/UserAgent.csv` & `zensvi-0.3.2/src/zensvi/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.3.1/src/zensvi/download/utils/geoprocess.py` & `zensvi-0.3.2/src/zensvi/download/utils/geoprocess.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.3.1/src/zensvi/download/utils/get_pids.py` & `zensvi-0.3.2/src/zensvi/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.3.1/src/zensvi/download/utils/helpers.py` & `zensvi-0.3.2/src/zensvi/download/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.3.1/src/zensvi/download/utils/imtool.py` & `zensvi-0.3.2/src/zensvi/download/utils/imtool.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.3.1/src/zensvi/download/utils/proxies.csv` & `zensvi-0.3.2/src/zensvi/download/utils/proxies.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.3.1/src/zensvi/transform/transform_image.py` & `zensvi-0.3.2/src/zensvi/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.3.1/PKG-INFO` & `zensvi-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zensvi
-Version: 0.3.1
+Version: 0.3.2
 Summary: This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner.
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

