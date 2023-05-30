# Comparing `tmp/ango-1.0.5.tar.gz` & `tmp/ango-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ango-1.0.5.tar", last modified: Wed May 24 13:28:44 2023, max compression
+gzip compressed data, was "ango-1.0.6.tar", last modified: Tue May 30 11:23:42 2023, max compression
```

## Comparing `ango-1.0.5.tar` & `ango-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-24 13:28:44.399697 ango-1.0.5/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-24 13:28:44.399697 ango-1.0.5/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.0.5/README.md
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-24 13:28:44.399697 ango-1.0.5/ango/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.5/ango/__init__.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-24 13:28:44.399697 ango-1.0.5/ango/models/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.5/ango/models/__init__.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 ango-1.0.5/ango/models/enums.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5421 2023-01-23 13:16:24.000000 ango-1.0.5/ango/models/label_category.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 ango-1.0.5/ango/plugin_logger.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5434 2023-05-24 13:28:41.000000 ango-1.0.5/ango/plugins.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)    14425 2023-05-17 14:28:05.000000 ango-1.0.5/ango/sdk.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-24 13:28:44.399697 ango-1.0.5/ango.egg-info/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-24 13:28:44.000000 ango-1.0.5/ango.egg-info/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-05-24 13:28:44.000000 ango-1.0.5/ango.egg-info/SOURCES.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-05-24 13:28:44.000000 ango-1.0.5/ango.egg-info/dependency_links.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      130 2023-05-24 13:28:44.000000 ango-1.0.5/ango.egg-info/requires.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-05-24 13:28:44.000000 ango-1.0.5/ango.egg-info/top_level.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-05-24 13:28:44.399697 ango-1.0.5/setup.cfg
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      864 2023-05-24 13:28:41.000000 ango-1.0.5/setup.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-30 11:23:42.908386 ango-1.0.6/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-30 11:23:42.908386 ango-1.0.6/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.0.6/README.md
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-30 11:23:42.908386 ango-1.0.6/ango/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.6/ango/__init__.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-30 11:23:42.908386 ango-1.0.6/ango/models/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.6/ango/models/__init__.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 ango-1.0.6/ango/models/enums.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5452 2023-05-30 11:15:47.000000 ango-1.0.6/ango/models/label_category.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 ango-1.0.6/ango/plugin_logger.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5437 2023-05-30 11:15:47.000000 ango-1.0.6/ango/plugins.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)    14429 2023-05-30 11:15:47.000000 ango-1.0.6/ango/sdk.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-30 11:23:42.908386 ango-1.0.6/ango.egg-info/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-30 11:23:42.000000 ango-1.0.6/ango.egg-info/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-05-30 11:23:42.000000 ango-1.0.6/ango.egg-info/SOURCES.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-05-30 11:23:42.000000 ango-1.0.6/ango.egg-info/dependency_links.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      130 2023-05-30 11:23:42.000000 ango-1.0.6/ango.egg-info/requires.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-05-30 11:23:42.000000 ango-1.0.6/ango.egg-info/top_level.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-05-30 11:23:42.908386 ango-1.0.6/setup.cfg
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      864 2023-05-30 11:23:40.000000 ango-1.0.6/setup.py
```

### Comparing `ango-1.0.5/PKG-INFO` & `ango-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.0.5
+Version: 1.0.6
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.0.5/README.md` & `ango-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ango-1.0.5/ango/models/label_category.py` & `ango-1.0.6/ango/models/label_category.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 import uuid
 import random
 from copy import deepcopy
 from typing import List
 
 
 class Tool(enum.Enum):
+    BoundingBox = "bounding-box"
     Segmentation = "segmentation"
     Polyline = "polyline"
     Polygon = "polygon"
-    Rotated_bounding_box = "rotated-bounding-box"
+    RotatedBoundingBox = "rotated-bounding-box"
     Ner = "ner"
     Point = "point"
     Pdf = "pdf"
 
 
 class Classification(enum.Enum):
     Multi_dropdown = "multi-dropdown"
```

### Comparing `ango-1.0.5/ango/plugin_logger.py` & `ango-1.0.6/ango/plugin_logger.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.5/ango/plugins.py` & `ango-1.0.6/ango/plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         logger = PluginLogger("logger", self.id, org_id, run_by, session, self)
         return logger
 
 
 class ExportPlugin(Plugin):
 
     def __init__(self, id: str, secret: str, callback: Callable[[str, dict], Tuple[str, BytesIO]],
-                 host="https://imerit.ango.ai"):
+                 host="https://imeritapi.ango.ai"):
         super().__init__(id, secret, callback)
         self.host = host
 
     def on_plugin(self, data):
         """
         :param data: {project_id: str, assignees: List[str] = None, completed_at: List[datetime.datetime] = None,
                updated_at: List[datetime.datetime = None, tags: List[str] = None}
```

### Comparing `ango-1.0.5/ango/sdk.py` & `ango-1.0.6/ango/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,17 +221,17 @@
 
         response = self.session.post(url, headers=headers, json=payload)
         return response.json()
 
     def get_assets(self, project_id, asset_id=None, external_id=None, page=1, limit=10):
         url = "%s/v2/project/%s/assets?page=%s&limit=%s" % (self.host, project_id, page, limit)
         if asset_id:
-            url += "?_id=" % asset_id
+            url += "?_id=%s" % asset_id
         if external_id:
-            url += "?externalId=" % external_id
+            url += "?externalId=%s" % external_id
 
         headers = {
             'apikey': self.api_key
         }
         response = self.session.get(url, headers=headers)
         return response.json()
```

### Comparing `ango-1.0.5/ango.egg-info/PKG-INFO` & `ango-1.0.6/ango.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.0.5
+Version: 1.0.6
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.0.5/setup.py` & `ango-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ango",
-    version="1.0.5",
+    version="1.0.6",
     author="Faruk Karakaya",
     author_email="<faruk@ango.ai>",
     description="Ango-Hub SDK",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

