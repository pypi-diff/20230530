# Comparing `tmp/geosyspy-0.1.3.tar.gz` & `tmp/geosyspy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geosyspy-0.1.3.tar", last modified: Tue May 23 16:19:16 2023, max compression
+gzip compressed data, was "geosyspy-0.1.4.tar", last modified: Tue May 30 14:04:21 2023, max compression
```

## Comparing `geosyspy-0.1.3.tar` & `geosyspy-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:19:16.508660 geosyspy-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-23 16:19:16.508660 geosyspy-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-23 16:17:31.000000 geosyspy-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 16:17:31.000000 geosyspy-0.1.3/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:19:16.508660 geosyspy-0.1.3/geosyspy/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-23 16:17:31.000000 geosyspy-0.1.3/geosyspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33350 2023-05-23 16:17:31.000000 geosyspy-0.1.3/geosyspy/geosys.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 16:17:31.000000 geosyspy-0.1.3/geosyspy/image_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:19:16.508660 geosyspy-0.1.3/geosyspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-23 16:19:16.000000 geosyspy-0.1.3/geosyspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-23 16:19:16.000000 geosyspy-0.1.3/geosyspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:19:16.000000 geosyspy-0.1.3/geosyspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-23 16:19:16.000000 geosyspy-0.1.3/geosyspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 16:19:16.000000 geosyspy-0.1.3/geosyspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 16:19:16.508660 geosyspy-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-23 16:17:31.000000 geosyspy-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:04:21.371617 geosyspy-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-30 14:04:21.371617 geosyspy-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-30 14:02:30.000000 geosyspy-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 14:02:30.000000 geosyspy-0.1.4/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:04:21.371617 geosyspy-0.1.4/geosyspy/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 14:02:30.000000 geosyspy-0.1.4/geosyspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35285 2023-05-30 14:02:30.000000 geosyspy-0.1.4/geosyspy/geosys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-30 14:02:30.000000 geosyspy-0.1.4/geosyspy/image_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:04:21.371617 geosyspy-0.1.4/geosyspy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-30 14:02:30.000000 geosyspy-0.1.4/geosyspy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-30 14:02:30.000000 geosyspy-0.1.4/geosyspy/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-30 14:02:30.000000 geosyspy-0.1.4/geosyspy/utils/geosys_platform_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-30 14:02:30.000000 geosyspy-0.1.4/geosyspy/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-30 14:02:30.000000 geosyspy-0.1.4/geosyspy/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-30 14:02:30.000000 geosyspy-0.1.4/geosyspy/utils/oauth2_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:04:21.371617 geosyspy-0.1.4/geosyspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-30 14:04:21.000000 geosyspy-0.1.4/geosyspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-30 14:04:21.000000 geosyspy-0.1.4/geosyspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:04:21.000000 geosyspy-0.1.4/geosyspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-30 14:04:21.000000 geosyspy-0.1.4/geosyspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 14:04:21.000000 geosyspy-0.1.4/geosyspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 14:04:21.371617 geosyspy-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-30 14:02:30.000000 geosyspy-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:04:21.371617 geosyspy-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:02:30.000000 geosyspy-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-30 14:02:30.000000 geosyspy-0.1.4/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-05-30 14:02:30.000000 geosyspy-0.1.4/tests/test_int_geosys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-05-30 14:02:30.000000 geosyspy-0.1.4/tests/test_unit_geosys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-30 14:02:30.000000 geosyspy-0.1.4/tests/test_unit_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-30 14:02:30.000000 geosyspy-0.1.4/tests/test_unit_oauth2_client.py
```

### Comparing `geosyspy-0.1.3/PKG-INFO` & `geosyspy-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geosyspy
-Version: 0.1.3
+Version: 0.1.4
 Summary: Easy-to-use python wrapper for Geosys APIs (time series, imagery products)
 Author: Geosys
 Description-Content-Type: text/markdown
 
 <div id="top"></div>
 <!-- PROJECT SHIELDS -->
 <!--
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_0jm83wdb_/tmp88c4_zzm_TarContainer/0/1", line 25, column 4: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_0jm83wdb_/tmp88c4_zzm_TarContainer/0/1", line 25, column 4: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: geosyspy Version: 0.1.3 Summary: Easy-to-use python
+Metadata-Version: 2.1 Name: geosyspy Version: 0.1.4 Summary: Easy-to-use python
 wrapper for Geosys APIs (time series, imagery products) Author: Geosys
 Description-Content-Type: text/markdown
 
                                     [Logo]
                             ****** GeosysPy ******
   To be able to discover, request and use imagery products based on  virtual
                    constellation using the &ltgeosys/> API.
```

### Comparing `geosyspy-0.1.3/README.md` & `geosyspy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `geosyspy-0.1.3/geosyspy/geosys.py` & `geosyspy-0.1.4/geosyspy/geosys.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from datetime import datetime
 import json
+import re
 from urllib.parse import urljoin
 import pandas as pd
 import logging
 import io
 import zipfile
 from rasterio.io import MemoryFile
 from requests import HTTPError
@@ -16,42 +17,39 @@
 
 from geosyspy.utils.helper import *
 from geosyspy.utils.constants import *
 from geosyspy.utils.http_client import *
 from geosyspy.utils.geosys_platform_urls import *
 
 class Geosys:
+
+    """Geosys is the main client class to access all the Geosys APIs capabilities.
+
+    `client = Geosys(api_client_id, api_client_secret, api_username, api_password, env, region)`
+
+    Parameters:
+        enum_env: 'Env.PROD' or 'Env.PREPROD'
+        enum_region: 'Region.NA' or 'Region.EU'
+        priority_queue: 'realtime' or 'bulk'
+    """
     def __init__(self, client_id: str,
                  client_secret: str,
                  username: str,
                  password: str,
                  enum_env: Env,
                  enum_region: Region,
                  priority_queue: str = "realtime",
                  ):
-        """Initializes a Geosys instance with the required credentials
-        to connect to the GEOSYS API.
-        """
         self.region: str = enum_region.value
         self.env: str = enum_env.value
         self.base_url: str = GEOSYS_API_URLS[enum_region.value][enum_env.value]
         self.priority_queue: str = priority_queue
         self.http_client: HttpClient = HttpClient(client_id, client_secret, username, password, enum_env.value,
                                                   enum_region.value)
 
-    """Geosys is the main client class to access all the Geosys APIs capabilities.
-
-    `client = Geosys(api_client_id, api_client_secret, api_username, api_password, env, region)`
-
-    Parameters:
-        enum_env: 'Env.PROD' or 'Env.PREPROD'
-        enum_region: 'Region.NA' or 'Region.EU'
-        priority_queue: 'realtime' or 'bulk'
-    """
-
 
     def __create_season_field_id(self, polygon: str) -> object:
         """Posts the payload below to the master data management endpoint.
 
         This method returns a season field id. The season field id is required
         to request other APIs endpoints.
 
@@ -308,24 +306,24 @@
 
         Returns:
             (tuple): images list and image references for downloading
         """
 
         df = self.__get_satellite_coverage(polygon, start_date, end_date, "", collections)
         images_references = {}
-
-        for i, image in df.iterrows():
-            images_references[
-                (image["image.date"], image["image.sensor"])
-            ] = image_reference.ImageReference(
-                image["image.id"],
-                image["image.date"],
-                image["image.sensor"],
-                image["seasonField.id"],
-            )
+        if df is not None:
+            for i, image in df.iterrows():
+                images_references[
+                    (image["image.date"], image["image.sensor"])
+                ] = image_reference.ImageReference(
+                    image["image.id"],
+                    image["image.date"],
+                    image["image.sensor"],
+                    image["seasonField.id"],
+                )
 
         return df, images_references
 
     def __get_satellite_coverage(self, polygon: str,
                                  start_date: datetime,
                                  end_date: datetime,
                                  indicator,
@@ -639,29 +637,72 @@
         )
         response = self.http_client.post(af_url, payload)
         if response.status_code == 201:
             return response.content
         else:
             logging.info(response.status_code)
 
-    def _get_s3_path(self, task_id: str):
+    def __get_s3_path(self, task_id: str):
+        """Returns S3 path related to task_id
+
+        Args:
+            task_id : A string representing a task id
+
+        Returns:
+            path : uri
 
+        """
         endpoint: str = GeosysApiEndpoints.MRTS_PROCESSOR_EVENTS_ENDPOINT.value + "/" + task_id
         response = self.http_client.get(endpoint)
         if response.ok:
             dict_resp = json.loads(response.content)
             customer_code: str = dict_resp["customerCode"].lower().replace("_", "-")
             user_id: str = dict_resp["userId"]
             task_id = dict_resp["taskId"]
             return "s3://geosys-" + customer_code + "/" + user_id + "/mrts/" + task_id
         else:
             logging.info(response.status_code)
 
-    def get_mr_time_series(self, start_date: str, end_date: str, list_sensors, denoiser: bool, smoother: str, eoc: bool,
-                           func: str, index: str, raw_data: bool, polygon: str):
+
+    def get_mr_time_series(self,
+                           polygon,
+                           start_date: str ="2010-01-01",
+                           end_date=None,
+                           list_sensors=["micasense", "sequoia", "m4c", "sentinel_2",
+                                         "landsat_8", "landsat_9", "cbers4", "kazstsat",
+                                         "alsat_1b", "huanjing_2", "deimos", "gaofen_1", "gaofen_6",
+                                        "resourcesat2","dmc_2","landsat_5","landsat_7",
+                                        "spot","rapideye_3a", "rapideye_1b"],
+                            denoiser: bool =True,
+                            smoother: str ="ww",
+                            eoc: bool =True,
+                            func: str ="mean",
+                            index: str ="ndvi",
+                            raw_data: bool =False
+                            ):
+
+        """Retrieve mr time series on the collection targeted.
+
+        Args:
+            start_date : The start date of the time series
+            end_date : The end date of the time series
+            list_sensors : The Satellite Imagery Collection targeted
+            denoiser : A boolean value indicating whether a denoising operation should be applied or not.
+            smoother : The type or name of the smoothing technique or algorithm to be used.
+            eoc : A boolean value indicating whether the "end of curve" detection should be performed.
+            func : The type or name of the function to be applied to the data.
+            index : The type or name of the index used for data manipulation or referencing
+            raw_data : A boolean value indicating whether the data is in its raw/unprocessed form.
+            polygon : A string representing a polygon.
+
+        Returns:
+            string : s3 bucket path
+        """
+        if end_date is None:
+            end_date = datetime.today().strftime("%Y-%m-%d")
         payload = {
             "parametersProfile": {
                 "code": "mrts_default",
                 "version": 1
             },
             "parameters": {
                 "start_date": start_date,
@@ -679,15 +720,15 @@
             ]
         }
 
         response = self.http_client.post(GeosysApiEndpoints.MRTS_PROCESSOR_ENDPOINT.value, payload)
 
         if response.ok:
             task_id = json.loads(response.content)["taskId"]
-            return self._get_s3_path(task_id)
+            return self.__get_s3_path(task_id)
         else:
             logging.info(response.status_code)
 
     def get_metrics(self, polygon: str,
                     schema_id: str,
                     start_date: datetime,
                     end_date: datetime):
@@ -696,15 +737,15 @@
         Args:
             polygon : A string representing a polygon.
             start_date : A datetime object representing the start date of the date interval the user wants to filter on.
             end_date : A datetime object representing the final date of the date interval the user wants to filter on.
             schema_id : A string representing a schema existing in Analytics Fabrics
 
         Returns:
-            df : A Pandas DataFrame containing several's columns with metrics
+            df : A Pandas DataFrame containing severals columns with metrics
 
         """
         season_field_id: str = self.__extract_season_field_id(polygon)
         logging.info("Calling APIs for metrics")
         start_date: str = start_date.strftime("%Y-%m-%d")
         end_date: str = end_date.strftime("%Y-%m-%d")
         parameters: str = f'?%24limit=9999&Timestamp=$between:{start_date}|{end_date}&$filter=Entity.ExternalTypedIds.Contains("SeasonField:{season_field_id}@LEGACY_ID_{self.region.upper()}")&$filter=Schema.Id=={schema_id}'
```

### Comparing `geosyspy-0.1.3/geosyspy.egg-info/PKG-INFO` & `geosyspy-0.1.4/geosyspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geosyspy
-Version: 0.1.3
+Version: 0.1.4
 Summary: Easy-to-use python wrapper for Geosys APIs (time series, imagery products)
 Author: Geosys
 Description-Content-Type: text/markdown
 
 <div id="top"></div>
 <!-- PROJECT SHIELDS -->
 <!--
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_0jm83wdb_/tmp88c4_zzm_TarContainer/0/9", line 25, column 4: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_0jm83wdb_/tmp88c4_zzm_TarContainer/0/9", line 25, column 4: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: geosyspy Version: 0.1.3 Summary: Easy-to-use python
+Metadata-Version: 2.1 Name: geosyspy Version: 0.1.4 Summary: Easy-to-use python
 wrapper for Geosys APIs (time series, imagery products) Author: Geosys
 Description-Content-Type: text/markdown
 
                                     [Logo]
                             ****** GeosysPy ******
   To be able to discover, request and use imagery products based on  virtual
                    constellation using the &ltgeosys/> API.
```

### Comparing `geosyspy-0.1.3/setup.py` & `geosyspy-0.1.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup script for geosyspy"""
 
 # Standard library imports
 import pathlib
 
 # Third party imports
-from setuptools import setup
+from setuptools import setup, find_packages
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).resolve().parent
 
 # The text of the README file is used as a description
 README = (HERE / "README.md").read_text()
 
@@ -18,12 +18,12 @@
 setup(
     name="geosyspy",
     version=VERSION,
     description="Easy-to-use python wrapper for Geosys APIs (time series, imagery products)",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Geosys",
-    packages=["geosyspy"],
+    packages=find_packages(),
     include_package_data=True,
     data_files=[('', ['VERSION.txt'])],
     install_requires=["requests", "requests-oauthlib", "oauthlib", "scipy", "pandas==1.3.5", "shapely", "rasterio", "xarray", "boto3"]
 )
```

