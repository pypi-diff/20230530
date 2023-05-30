# Comparing `tmp/max-ard-1.7.2.tar.gz` & `tmp/max_ard-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "max-ard-1.7.2.tar", max compression
+gzip compressed data, was "max_ard-1.7.3.tar", max compression
```

## Comparing `max-ard-1.7.2.tar` & `max_ard-1.7.3.tar`

### file list

```diff
@@ -1,34 +1,33 @@
--rw-r--r--   0        0        0      375 2023-02-08 18:34:56.063513 max-ard-1.7.2/README.md
--rw-r--r--   0        0        0      427 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/__init__.py
--rw-r--r--   0        0        0    10412 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/admin.py
--rw-r--r--   0        0        0    24648 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/ard_collection.py
--rw-r--r--   0        0        0    14488 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/base_collections.py
--rw-r--r--   0        0        0       33 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/commands/__init__.py
--rw-r--r--   0        0        0     5149 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/commands/command.py
--rw-r--r--   0        0        0     2269 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/commands/grid.py
--rw-r--r--   0        0        0    11045 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/commands/order.py
--rw-r--r--   0        0        0    14257 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/commands/select.py
--rw-r--r--   0        0        0     4167 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/commands/storage.py
--rw-r--r--   0        0        0      624 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/dependency_support/__init__.py
--rw-r--r--   0        0        0     2611 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/dependency_support/azure.py
--rw-r--r--   0        0        0     3457 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/exceptions.py
--rw-r--r--   0        0        0      920 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/io/__init__.py
--rw-r--r--   0        0        0     4058 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/io/inputs.py
--rw-r--r--   0        0        0     3003 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/io/kml_format.py
--rw-r--r--   0        0        0     1066 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/io/kmz_format.py
--rw-r--r--   0        0        0    46445 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/io/qlr_format.py
--rw-r--r--   0        0        0     1692 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/io/shp_format.py
--rw-r--r--   0        0        0    23056 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/metadata.py
--rw-r--r--   0        0        0    11053 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/monitor.py
--rw-r--r--   0        0        0    17814 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/order.py
--rw-r--r--   0        0        0      512 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/outputs/kml_format.py
--rw-r--r--   0        0        0      632 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/outputs/kmz_format.py
--rw-r--r--   0        0        0     1127 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/outputs/qlr_format.py
--rw-r--r--   0        0        0      549 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/outputs/shp_format.py
--rw-r--r--   0        0        0    13119 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/processing.py
--rw-r--r--   0        0        0    18182 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/select.py
--rw-r--r--   0        0        0    18402 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/session.py
--rw-r--r--   0        0        0     5339 2023-02-08 18:34:56.071513 max-ard-1.7.2/max_ard/storage.py
--rw-r--r--   0        0        0     1916 2023-02-08 18:34:56.151510 max-ard-1.7.2/pyproject.toml
--rw-r--r--   0        0        0     1654 2023-02-08 18:35:13.201579 max-ard-1.7.2/setup.py
--rw-r--r--   0        0        0     1554 2023-02-08 18:35:13.201955 max-ard-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0      375 2023-05-30 21:42:11.552824 max_ard-1.7.3/README.md
+-rw-r--r--   0        0        0      427 2023-05-30 21:42:11.556824 max_ard-1.7.3/max_ard/__init__.py
+-rw-r--r--   0        0        0    10412 2023-05-30 21:42:11.556824 max_ard-1.7.3/max_ard/admin.py
+-rw-r--r--   0        0        0    24648 2023-05-30 21:42:11.556824 max_ard-1.7.3/max_ard/ard_collection.py
+-rw-r--r--   0        0        0    14488 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/base_collections.py
+-rw-r--r--   0        0        0       33 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/commands/__init__.py
+-rw-r--r--   0        0        0     5149 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/commands/command.py
+-rw-r--r--   0        0        0     2269 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/commands/grid.py
+-rw-r--r--   0        0        0    11045 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/commands/order.py
+-rw-r--r--   0        0        0    14257 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/commands/select.py
+-rw-r--r--   0        0        0     4167 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/commands/storage.py
+-rw-r--r--   0        0        0      624 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/dependency_support/__init__.py
+-rw-r--r--   0        0        0     2611 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/dependency_support/azure.py
+-rw-r--r--   0        0        0     3457 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/exceptions.py
+-rw-r--r--   0        0        0      920 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/io/__init__.py
+-rw-r--r--   0        0        0     4058 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/io/inputs.py
+-rw-r--r--   0        0        0     3003 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/io/kml_format.py
+-rw-r--r--   0        0        0     1066 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/io/kmz_format.py
+-rw-r--r--   0        0        0    46445 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/io/qlr_format.py
+-rw-r--r--   0        0        0     1692 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/io/shp_format.py
+-rw-r--r--   0        0        0    23056 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/metadata.py
+-rw-r--r--   0        0        0    11053 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/monitor.py
+-rw-r--r--   0        0        0    17795 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/order.py
+-rw-r--r--   0        0        0      512 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/outputs/kml_format.py
+-rw-r--r--   0        0        0      632 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/outputs/kmz_format.py
+-rw-r--r--   0        0        0     1127 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/outputs/qlr_format.py
+-rw-r--r--   0        0        0      549 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/outputs/shp_format.py
+-rw-r--r--   0        0        0    13119 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/processing.py
+-rw-r--r--   0        0        0    18182 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/select.py
+-rw-r--r--   0        0        0    18786 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/session.py
+-rw-r--r--   0        0        0     5339 2023-05-30 21:42:11.560824 max_ard-1.7.3/max_ard/storage.py
+-rw-r--r--   0        0        0     1916 2023-05-30 21:42:11.648829 max_ard-1.7.3/pyproject.toml
+-rw-r--r--   0        0        0     1607 1970-01-01 00:00:00.000000 max_ard-1.7.3/PKG-INFO
```

### Comparing `max-ard-1.7.2/max_ard/admin.py` & `max_ard-1.7.3/max_ard/admin.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/ard_collection.py` & `max_ard-1.7.3/max_ard/ard_collection.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/base_collections.py` & `max_ard-1.7.3/max_ard/base_collections.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/commands/command.py` & `max_ard-1.7.3/max_ard/commands/command.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/commands/grid.py` & `max_ard-1.7.3/max_ard/commands/grid.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/commands/order.py` & `max_ard-1.7.3/max_ard/commands/order.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/commands/select.py` & `max_ard-1.7.3/max_ard/commands/select.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/commands/storage.py` & `max_ard-1.7.3/max_ard/commands/storage.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/dependency_support/__init__.py` & `max_ard-1.7.3/max_ard/dependency_support/__init__.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/dependency_support/azure.py` & `max_ard-1.7.3/max_ard/dependency_support/azure.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/exceptions.py` & `max_ard-1.7.3/max_ard/exceptions.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/io/__init__.py` & `max_ard-1.7.3/max_ard/io/__init__.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/io/inputs.py` & `max_ard-1.7.3/max_ard/io/inputs.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/io/kml_format.py` & `max_ard-1.7.3/max_ard/io/kml_format.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/io/kmz_format.py` & `max_ard-1.7.3/max_ard/io/kmz_format.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/io/qlr_format.py` & `max_ard-1.7.3/max_ard/io/qlr_format.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/io/shp_format.py` & `max_ard-1.7.3/max_ard/io/shp_format.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/metadata.py` & `max_ard-1.7.3/max_ard/metadata.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/monitor.py` & `max_ard-1.7.3/max_ard/monitor.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/order.py` & `max_ard-1.7.3/max_ard/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -490,15 +490,15 @@
         instance = cls()
         instance.response = OrderResponse(**response)
         return instance
 
     @classmethod
     def list_orders(
         cls,
-        limit=10,
+        limit=None,
         starting_after="",
         ending_before="",
         start_date="",
         end_date="",
         filter=None,
         session=None,
     ):
@@ -526,26 +526,25 @@
         -------
         list
             Order objects matching parameters"""
 
         session = session or get_user_session()
 
         params = {
-            "limit": limit,
             "starting_after": starting_after,
             "ending_before": ending_before,
             "start_date": start_date,
             "end_date": end_date,
         }
 
         if filter is not None:
             params["filter"] = filter
 
         key = lambda order: order["id"]
-        responses = paginated_response(session, ard_url("order"), key, **params)
+        responses = paginated_response(session, ard_url("order"), key, limit, **params)
 
         return hydrate_with_responses(Order, OrderResponse, responses, session=session)
 
     @classmethod
     def get_order(cls, order_id, session=None):
         """Fetch raw data about an Order from an ID
```

### Comparing `max-ard-1.7.2/max_ard/outputs/kml_format.py` & `max_ard-1.7.3/max_ard/outputs/kml_format.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/outputs/kmz_format.py` & `max_ard-1.7.3/max_ard/outputs/kmz_format.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/outputs/qlr_format.py` & `max_ard-1.7.3/max_ard/outputs/qlr_format.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/outputs/shp_format.py` & `max_ard-1.7.3/max_ard/outputs/shp_format.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/processing.py` & `max_ard-1.7.3/max_ard/processing.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/select.py` & `max_ard-1.7.3/max_ard/select.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/max_ard/session.py` & `max_ard-1.7.3/max_ard/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 """ Authenticated sessions for communicating with the ARD API endpoints"""
 
 import base64
 import json
 import os
 import warnings
-
 from configparser import ConfigParser
+from platform import python_version, system
+
 from oauthlib.oauth2 import BackendApplicationClient, LegacyApplicationClient
 from oauthlib.oauth2.rfc6749.errors import MissingTokenError
-from platform import python_version, system
-from requests.auth import HTTPBasicAuth
 from requests.adapters import HTTPAdapter
+from requests.auth import HTTPBasicAuth
 from requests.packages.urllib3.util.retry import Retry
 from requests_oauthlib import OAuth2Session
 
 from max_ard.exceptions import (
     ard_server_request_hook,
     bad_ard_request_hook,
     bad_geom_request_hook,
+    missing_resource_hook,
     oversize_request_hook,
     unauth_request_hook,
-    missing_resource_hook,
 )
 
-
 try:
     from importlib import metadata
 except ImportError:  # for Python<3.8
     import importlib_metadata as metadata
 
 __all__ = ("get_user_session", "get_client_session", "get_self")
 
@@ -103,78 +102,88 @@
     version = metadata.version("max_ard")
     session.headers.update(
         {"User-Agent": f"max_ard/{version} (Python {python_version()}/{system()})"}
     )
     return session
 
 
-def link_paginated_response(session, url, **params):
+def link_paginated_response(session, url, limit=None, **params):
     """Follow responses with paginated links and gather up objects
 
     Newer paginated endpoints give you a link to retrieve the next set of objects.
     For older endpoints that only return object IDs, see the next function.
 
     Parameters
     ----------
-    session: Requests session
+    session: Requests sessionj
         A session through which to make the requests, usually an ARD session
     url: str
         URL to start fetching objects
     **params: any
         Additional parameters to pass through to the session's GET method
 
     Returns
     -------
     list: any
         A list of objects returned by the endpoint"""
 
     response = {"has_more": True}
     things = []
+    # bump up the default fetch limit
+    params["limit"] = 100
     while response["has_more"]:
         response = session.get(url, params=params).json()
         for thing in response["data"]:
             things.append(thing)
+            if limit and len(things) == limit:
+                return things
         # nothing returned
         if len(things) == 0:
             return []
         if response["has_more"]:
             url = response["links"]["next_page"]
 
     return things
 
 
-def paginated_response(session, url, key, **params):
+def paginated_response(session, url, key, limit=None, **params):
     """Follow paginated responses with object IDs and gather up objects
 
     This uses `starting_after` to grab the next batch of objects after the last
     object's ID.
 
     Parameters
     ----------
     session: Requests session
         A session through which to make the requests, usually an ARD session
     url: str
         URL to start fetching objects
     key: callable
         A callable that given the object, returns the object's ID.
+    limit: int or None, default None
+        Limit number of objects returned
     **params: any
         Additional parameters to pass through to the session's GET method
 
     Returns
     -------
     list: any
         A list of objects returned by the endpoint"""
 
     response = {"has_more": True}
     things = []
+    # bump up the default fetch limit
+    params["limit"] = 100
     while response["has_more"]:
         response = session.get(url, params=params).json()
         for thing in response["data"]:
             things.append(thing)
             last_id = key(thing)
+            if limit and len(things) == limit:
+                return things
         # nothing returned
         if len(things) == 0:
             return []
         params["starting_after"] = last_id
 
     return things
```

### Comparing `max-ard-1.7.2/max_ard/storage.py` & `max_ard-1.7.3/max_ard/storage.py`

 * *Files identical despite different names*

### Comparing `max-ard-1.7.2/pyproject.toml` & `max_ard-1.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "max-ard"
-version = "1.7.2"
+version = "1.7.3"
 description = "ARD SDK and CLI tools"
 authors = [
     "Marc Pfister <marc.pfister@maxar.com>",
     "Mike Connor <mike.connor@maxar.com>",
     "Maja Cannavo <maja.cannavo@maxar.com>",
     "Josie Allamby <josie.allamby@maxar.com>"
     ]
```

### Comparing `max-ard-1.7.2/PKG-INFO` & `max_ard-1.7.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: max-ard
-Version: 1.7.2
+Version: 1.7.3
 Summary: ARD SDK and CLI tools
 Home-page: https://ard.maxar.com/docs/
 Author: Marc Pfister
 Author-email: marc.pfister@maxar.com
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: full
-Requires-Dist: Fiona (>=1.8.19,<2.0.0); extra == "full"
+Requires-Dist: Fiona (>=1.8.19,<2.0.0) ; extra == "full"
 Requires-Dist: Shapely (>=1.7.1,<2.0.0)
 Requires-Dist: backports.cached-property (>=1.0.1,<2.0.0)
 Requires-Dist: boto3 (>=1.17.73,<2.0.0)
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: maxar-ard-grid (>=1.2.1,<2.0.0)
 Requires-Dist: pdoc3 (>=0.10.0,<0.11.0)
 Requires-Dist: pydantic (>=1.7.4,<2.0.0)
-Requires-Dist: rasterio (>=1.2.10,<2.0.0); extra == "full"
+Requires-Dist: rasterio (>=1.2.10,<2.0.0) ; extra == "full"
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: requests-futures (>=1.0.0,<2.0.0)
 Requires-Dist: requests-oauthlib (>=1.3.0,<2.0.0)
 Requires-Dist: s3fs (>=0.4.2,<0.5.0)
 Project-URL: Documentation, https://ard.maxar.com/docs/sdk
 Description-Content-Type: text/markdown
```

