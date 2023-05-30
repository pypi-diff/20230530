# Comparing `tmp/msgraphy-0.3.6.tar.gz` & `tmp/msgraphy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgraphy-0.3.6.tar", max compression
+gzip compressed data, was "msgraphy-0.4.0.tar", max compression
```

## Comparing `msgraphy-0.3.6.tar` & `msgraphy-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1068 2023-05-04 15:38:13.606407 msgraphy-0.3.6/LICENSE
--rw-r--r--   0        0        0       91 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/__init__.py
--rw-r--r--   0        0        0     1300 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/api.py
--rw-r--r--   0        0        0        0 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/auth/__init__.py
--rw-r--r--   0        0        0     3406 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/auth/config.py
--rw-r--r--   0        0        0     5056 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/auth/graph_auth.py
--rw-r--r--   0        0        0     3057 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/cli/__commands.py
--rw-r--r--   0        0        0       57 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/cli/__init__.py
--rw-r--r--   0        0        0      153 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/cli/__settings.py
--rw-r--r--   0        0        0        0 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/client/__init__.py
--rw-r--r--   0        0        0     3626 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/client/graph_batch.py
--rw-r--r--   0        0        0     3662 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/client/graph_client.py
--rw-r--r--   0        0        0     3601 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/__init__.py
--rw-r--r--   0        0        0     2469 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/file.py
--rw-r--r--   0        0        0     1355 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/group.py
--rw-r--r--   0        0        0      274 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/identity.py
--rw-r--r--   0        0        0      584 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/list.py
--rw-r--r--   0        0        0      533 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/monitor.py
--rw-r--r--   0        0        0     1051 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/sharepoint.py
--rw-r--r--   0        0        0      576 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/site_page.py
--rw-r--r--   0        0        0      727 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/team.py
--rw-r--r--   0        0        0      796 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/user.py
--rw-r--r--   0        0        0     1432 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/data/workbook.py
--rw-r--r--   0        0        0        0 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/domains/__init__.py
--rw-r--r--   0        0        0     7187 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/domains/files.py
--rw-r--r--   0        0        0     1192 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/domains/group.py
--rw-r--r--   0        0        0     3009 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/domains/list.py
--rw-r--r--   0        0        0      295 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/domains/monitor.py
--rw-r--r--   0        0        0     1768 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/domains/sharepoint.py
--rw-r--r--   0        0        0     2772 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/domains/team.py
--rw-r--r--   0        0        0     1425 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/domains/user.py
--rw-r--r--   0        0        0     6299 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/domains/workbook.py
--rw-r--r--   0        0        0        0 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/fs/__init__.py
--rw-r--r--   0        0        0     8125 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/fs/onedrivefs.py
--rw-r--r--   0        0        0      606 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/fs/opener.py
--rw-r--r--   0        0        0     3258 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/sharepoint_classic/__init__.py
--rw-r--r--   0        0        0     1006 2023-05-04 15:38:13.610407 msgraphy-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 msgraphy-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-30 07:35:08.655231 msgraphy-0.4.0/LICENSE
+-rw-r--r--   0        0        0       91 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/__init__.py
+-rw-r--r--   0        0        0     1300 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/api.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/auth/__init__.py
+-rw-r--r--   0        0        0     3406 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/auth/config.py
+-rw-r--r--   0        0        0     5056 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/auth/graph_auth.py
+-rw-r--r--   0        0        0     6297 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/cli/__commands.py
+-rw-r--r--   0        0        0       57 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/cli/__init__.py
+-rw-r--r--   0        0        0      153 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/cli/__settings.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/client/__init__.py
+-rw-r--r--   0        0        0     3626 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/client/graph_batch.py
+-rw-r--r--   0        0        0     3662 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/client/graph_client.py
+-rw-r--r--   0        0        0     3601 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/data/__init__.py
+-rw-r--r--   0        0        0     2469 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/data/file.py
+-rw-r--r--   0        0        0     1355 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/data/group.py
+-rw-r--r--   0        0        0      274 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/data/identity.py
+-rw-r--r--   0        0        0      828 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/data/list.py
+-rw-r--r--   0        0        0      533 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/data/monitor.py
+-rw-r--r--   0        0        0     1051 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/data/sharepoint.py
+-rw-r--r--   0        0        0      576 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/data/site_page.py
+-rw-r--r--   0        0        0      727 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/data/team.py
+-rw-r--r--   0        0        0      796 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/data/user.py
+-rw-r--r--   0        0        0     1432 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/data/workbook.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/domains/__init__.py
+-rw-r--r--   0        0        0     7187 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/domains/files.py
+-rw-r--r--   0        0        0     1192 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/domains/group.py
+-rw-r--r--   0        0        0     3139 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/domains/list.py
+-rw-r--r--   0        0        0      295 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/domains/monitor.py
+-rw-r--r--   0        0        0     2033 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/domains/sharepoint.py
+-rw-r--r--   0        0        0     2772 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/domains/team.py
+-rw-r--r--   0        0        0     1425 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/domains/user.py
+-rw-r--r--   0        0        0     6299 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/domains/workbook.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:35:08.655231 msgraphy-0.4.0/msgraphy/fs/__init__.py
+-rw-r--r--   0        0        0     8125 2023-05-30 07:35:08.659231 msgraphy-0.4.0/msgraphy/fs/onedrivefs.py
+-rw-r--r--   0        0        0      606 2023-05-30 07:35:08.659231 msgraphy-0.4.0/msgraphy/fs/opener.py
+-rw-r--r--   0        0        0     3258 2023-05-30 07:35:08.659231 msgraphy-0.4.0/msgraphy/sharepoint_classic/__init__.py
+-rw-r--r--   0        0        0     1006 2023-05-30 07:35:08.659231 msgraphy-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 msgraphy-0.4.0/PKG-INFO
```

### Comparing `msgraphy-0.3.6/LICENSE` & `msgraphy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/api.py` & `msgraphy-0.4.0/msgraphy/api.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/auth/config.py` & `msgraphy-0.4.0/msgraphy/auth/config.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/auth/graph_auth.py` & `msgraphy-0.4.0/msgraphy/auth/graph_auth.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/client/graph_batch.py` & `msgraphy-0.4.0/msgraphy/client/graph_batch.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/client/graph_client.py` & `msgraphy-0.4.0/msgraphy/client/graph_client.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/data/__init__.py` & `msgraphy-0.4.0/msgraphy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/data/file.py` & `msgraphy-0.4.0/msgraphy/data/file.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/data/group.py` & `msgraphy-0.4.0/msgraphy/data/group.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/data/list.py` & `msgraphy-0.4.0/msgraphy/data/site_page.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,36 @@
-import typing
+from typing import List
+
 from msgraphy.data import graphdataclass
 from msgraphy.data.file import BaseItem
 
 
 @graphdataclass
-class List(BaseItem):
-    display_name: str = None
-    list_info: dict = None
-    system: dict = None
-    fields: typing.List = None
+class ContentTypeInfo:
+    id: str = None
+    name: str = None
+
+
+@graphdataclass
+class WebPart:
+    type: str = None
+    data: dict = None
+
+
+@graphdataclass
+class PublicationFacet:
+    level: str = None
+    version_id: str = None
 
 
 @graphdataclass
-class ListColumn:
-    id: str
-    column_group: str
-    description: str
-    display_name: str
-    enforce_unique_values: bool
-    hidden: bool
-    indexed: bool
-    name: str
-    read_only: bool
-    required: bool
-    lookup: dict = None
-    person_or_group = None
-    text = None
-    date_time = None
-    number = None
+class SitePage(BaseItem):
+    content_type: ContentTypeInfo = None
+
+    title: str = None
+    page_layout: str = None
+    web_parts: List[WebPart] = None
+
+    publishing_state: PublicationFacet = None
+
+
+
```

### Comparing `msgraphy-0.3.6/msgraphy/data/monitor.py` & `msgraphy-0.4.0/msgraphy/data/monitor.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/data/sharepoint.py` & `msgraphy-0.4.0/msgraphy/data/sharepoint.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/data/team.py` & `msgraphy-0.4.0/msgraphy/data/team.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/data/user.py` & `msgraphy-0.4.0/msgraphy/data/user.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/data/workbook.py` & `msgraphy-0.4.0/msgraphy/data/workbook.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/domains/files.py` & `msgraphy-0.4.0/msgraphy/domains/files.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/domains/group.py` & `msgraphy-0.4.0/msgraphy/domains/group.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/domains/list.py` & `msgraphy-0.4.0/msgraphy/domains/list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing
 from typing import Union
 
 from msgraphy.client.graph_client import GraphResponse
 from msgraphy.data import ApiIterable, ListResponse
-from msgraphy.data.list import List, ListColumn
+from msgraphy.data.list import List, ListColumn, ListItem
 from msgraphy.data.sharepoint import SiteResource
 
 
 class ListGraphApi:
 
     def __init__(self, api):
         self._api = api
@@ -18,27 +18,30 @@
     def get_columns(self, site: SiteResource, list_name: str) -> GraphResponse[ListResponse[ListColumn]]:
         response_type = ApiIterable(self._api.client, ListColumn)
         return self._api.client.make_request(url=f"{site.resource}/lists/{list_name}/columns",
                                              response_type=response_type)
 
     def get_items(self, site: SiteResource, list_name: str,
                   fields: Union[str, bool] = None,
+                  drive_item: bool = False,
                   filter: str = None,
-                  ) -> GraphResponse[ListResponse[List]]:
+                  ) -> GraphResponse[ListResponse[ListItem]]:
 
         params = {}
         if isinstance(fields, bool) and fields:
             params['expand'] = "fields"
         elif isinstance(fields, str):
             params['expand'] = f"fields(select={fields})"
+        elif drive_item:
+            params['expand'] = "driveItem"
 
         if filter is not None:
             params['filter'] = filter
 
-        response_type = ApiIterable(self._api.client, List)
+        response_type = ApiIterable(self._api.client, ListItem)
 
         response = self._api.client.make_request(
             url=f"{site.resource}/lists/{list_name}/items",
             params=params,
             response_type=response_type,
         )
         return response
```

### Comparing `msgraphy-0.3.6/msgraphy/domains/sharepoint.py` & `msgraphy-0.4.0/msgraphy/domains/sharepoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Union
 
 from msgraphy.data import ListResponse, ApiIterable
 from msgraphy.data.file import DriveList, Drive
+from msgraphy.data.list import ListList, List as SharepointList
 from msgraphy.data.sharepoint import SiteResource, Site
 from msgraphy.client.graph_client import GraphResponse
 
 
 class SharepointGraphApi:
     def __init__(self, api):
         self._api = api
@@ -31,14 +32,18 @@
 
         return self._api.client.make_request(url="/sites", params=params, response_type=response_type)
 
     def list_drives(self, site: SiteResource) -> GraphResponse[DriveList]:
         resource = site.resource + "/drives"
         return self._api.client.make_request(url=resource, response_type=DriveList)
 
+    def list_lists(self, site: SiteResource) -> GraphResponse[ListList]:
+        resource = site.resource + "/lists"
+        return self._api.client.make_request(url=resource, response_type=ListList)
+
     def get_drive_by_name(self, site: SiteResource, name: str = "Documents") -> GraphResponse[Union[Drive, None]]:
         def name_filter(data):
             drives = DriveList(data)
             for d in drives:
                 if d.name == name:
                     return d
```

### Comparing `msgraphy-0.3.6/msgraphy/domains/team.py` & `msgraphy-0.4.0/msgraphy/domains/team.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/domains/user.py` & `msgraphy-0.4.0/msgraphy/domains/user.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/domains/workbook.py` & `msgraphy-0.4.0/msgraphy/domains/workbook.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/fs/onedrivefs.py` & `msgraphy-0.4.0/msgraphy/fs/onedrivefs.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/fs/opener.py` & `msgraphy-0.4.0/msgraphy/fs/opener.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/msgraphy/sharepoint_classic/__init__.py` & `msgraphy-0.4.0/msgraphy/sharepoint_classic/__init__.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.6/pyproject.toml` & `msgraphy-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msgraphy"
-version = "0.3.6"
+version = "0.4.0"
 description = "An API generator for the MS Graph API"
 authors = ["Kaj Siebert <kaj@k-si.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.7, <4"
 msal = "^1.10.0"
```

### Comparing `msgraphy-0.3.6/PKG-INFO` & `msgraphy-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgraphy
-Version: 0.3.6
+Version: 0.4.0
 Summary: An API generator for the MS Graph API
 License: MIT
 Author: Kaj Siebert
 Author-email: kaj@k-si.com
 Requires-Python: >=3.7,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

