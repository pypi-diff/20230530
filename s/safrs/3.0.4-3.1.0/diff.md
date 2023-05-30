# Comparing `tmp/safrs-3.0.4.tar.gz` & `tmp/safrs-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safrs-3.0.4.tar", last modified: Sun May  7 19:16:40 2023, max compression
+gzip compressed data, was "dist/safrs-3.1.0.tar", last modified: Tue May 30 18:29:19 2023, max compression
```

## Comparing `safrs-3.0.4.tar` & `safrs-3.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0 t         (1000) t         (1000)        0 2023-05-07 19:16:40.261346 safrs-3.0.4/
--rwxrwxrwx   0 t         (1000) t         (1000)    35120 2023-02-11 17:18:46.000000 safrs-3.0.4/LICENSE
--rwxrwxrwx   0 t         (1000) t         (1000)       90 2021-03-16 11:22:28.000000 safrs-3.0.4/MANIFEST.in
--rwxrwxrwx   0 t         (1000) t         (1000)     2665 2023-05-07 19:16:40.262343 safrs-3.0.4/PKG-INFO
--rwxrwxrwx   0 t         (1000) t         (1000)    16881 2023-02-18 08:57:06.000000 safrs-3.0.4/README.md
--rwxrwxrwx   0 t         (1000) t         (1000)     1374 2023-02-11 17:18:46.000000 safrs-3.0.4/README.rst
--rwxrwxrwx   0 t         (1000) t         (1000)     1422 2023-05-07 19:15:35.000000 safrs-3.0.4/pyproject.toml
--rwxrwxrwx   0 t         (1000) t         (1000)      433 2023-05-07 19:11:08.000000 safrs-3.0.4/requirements.txt
-drwxrwxrwx   0 t         (1000) t         (1000)        0 2023-05-07 19:16:40.249378 safrs-3.0.4/safrs/
--rwxrwxrwx   0 t         (1000) t         (1000)       93 2023-05-07 19:15:49.000000 safrs-3.0.4/safrs/__about__.py
--rwxrwxrwx   0 t         (1000) t         (1000)     1242 2023-02-11 17:18:47.000000 safrs-3.0.4/safrs/__init__.py
--rwxrwxrwx   0 t         (1000) t         (1000)     1980 2023-02-11 17:18:47.000000 safrs-3.0.4/safrs/_safrs_relationship.py
--rwxrwxrwx   0 t         (1000) t         (1000)     4082 2023-02-11 17:18:47.000000 safrs-3.0.4/safrs/api_methods.py
--rwxrwxrwx   0 t         (1000) t         (1000)     3349 2023-02-11 17:18:47.000000 safrs-3.0.4/safrs/attr_parse.py
--rwxrwxrwx   0 t         (1000) t         (1000)    49491 2023-05-01 07:36:38.000000 safrs-3.0.4/safrs/base.py
--rwxrwxrwx   0 t         (1000) t         (1000)     4047 2023-02-11 20:14:12.000000 safrs-3.0.4/safrs/config.py
--rwxrwxrwx   0 t         (1000) t         (1000)     3782 2023-02-11 17:18:47.000000 safrs-3.0.4/safrs/errors.py
--rwxrwxrwx   0 t         (1000) t         (1000)     1401 2023-02-11 17:18:47.000000 safrs-3.0.4/safrs/jabase.py
--rwxrwxrwx   0 t         (1000) t         (1000)     4531 2023-05-07 19:01:25.000000 safrs-3.0.4/safrs/json_encoder.py
--rwxrwxrwx   0 t         (1000) t         (1000)    41386 2023-02-18 08:46:45.000000 safrs-3.0.4/safrs/jsonapi.py
--rwxrwxrwx   0 t         (1000) t         (1000)     1682 2023-02-11 20:14:16.000000 safrs-3.0.4/safrs/jsonapi_attr.py
--rwxrwxrwx   0 t         (1000) t         (1000)     5857 2023-02-18 08:46:45.000000 safrs-3.0.4/safrs/jsonapi_filters.py
--rwxrwxrwx   0 t         (1000) t         (1000)     9866 2023-02-18 08:46:45.000000 safrs-3.0.4/safrs/jsonapi_formatting.py
--rwxrwxrwx   0 t         (1000) t         (1000)     6290 2023-05-07 19:03:35.000000 safrs-3.0.4/safrs/request.py
--rwxrwxrwx   0 t         (1000) t         (1000)      262 2023-02-11 17:18:47.000000 safrs-3.0.4/safrs/response.py
--rwxrwxrwx   0 t         (1000) t         (1000)    31273 2023-02-18 08:46:45.000000 safrs-3.0.4/safrs/safrs_api.py
--rwxrwxrwx   0 t         (1000) t         (1000)     6085 2023-05-07 19:00:53.000000 safrs-3.0.4/safrs/safrs_init.py
--rwxrwxrwx   0 t         (1000) t         (1000)     7458 2023-02-18 08:46:45.000000 safrs-3.0.4/safrs/safrs_types.py
--rwxrwxrwx   0 t         (1000) t         (1000)    26470 2023-02-18 08:46:45.000000 safrs-3.0.4/safrs/swagger_doc.py
--rwxrwxrwx   0 t         (1000) t         (1000)     1205 2023-02-18 08:46:44.000000 safrs-3.0.4/safrs/util.py
-drwxrwxrwx   0 t         (1000) t         (1000)        0 2023-05-07 19:16:40.260348 safrs-3.0.4/safrs.egg-info/
--rwxrwxrwx   0 t         (1000) t         (1000)     2665 2023-05-07 19:16:40.000000 safrs-3.0.4/safrs.egg-info/PKG-INFO
--rwxrwxrwx   0 t         (1000) t         (1000)      648 2023-05-07 19:16:40.000000 safrs-3.0.4/safrs.egg-info/SOURCES.txt
--rwxrwxrwx   0 t         (1000) t         (1000)        1 2023-05-07 19:16:40.000000 safrs-3.0.4/safrs.egg-info/dependency_links.txt
--rwxrwxrwx   0 t         (1000) t         (1000)      522 2023-05-07 19:16:40.000000 safrs-3.0.4/safrs.egg-info/requires.txt
--rwxrwxrwx   0 t         (1000) t         (1000)        6 2023-05-07 19:16:40.000000 safrs-3.0.4/safrs.egg-info/top_level.txt
--rwxrwxrwx   0 t         (1000) t         (1000)      263 2023-05-07 19:16:40.263340 safrs-3.0.4/setup.cfg
--rwxrwxrwx   0 t         (1000) t         (1000)     1687 2023-05-07 19:15:26.000000 safrs-3.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 18:29:19.000000 safrs-3.1.0/
+-rwxr-xr-x   0 root         (0) root         (0)     1687 2023-05-29 04:14:46.000000 safrs-3.1.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)      263 2023-05-30 18:29:19.000000 safrs-3.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 18:29:19.000000 safrs-3.1.0/safrs/
+-rwxr-xr-x   0 root         (0) root         (0)     4082 2022-10-24 17:17:14.000000 safrs-3.1.0/safrs/api_methods.py
+-rwxr-xr-x   0 root         (0) root         (0)     7458 2023-02-18 09:01:57.000000 safrs-3.1.0/safrs/safrs_types.py
+-rwxr-xr-x   0 root         (0) root         (0)     3349 2022-10-24 17:17:14.000000 safrs-3.1.0/safrs/attr_parse.py
+-rwxr-xr-x   0 root         (0) root         (0)     5843 2023-05-28 09:06:48.000000 safrs-3.1.0/safrs/safrs_init.py
+-rwxr-xr-x   0 root         (0) root         (0)    49467 2023-05-28 09:06:48.000000 safrs-3.1.0/safrs/base.py
+-rwxr-xr-x   0 root         (0) root         (0)    26470 2023-02-18 09:01:57.000000 safrs-3.1.0/safrs/swagger_doc.py
+-rwxr-xr-x   0 root         (0) root         (0)     3782 2022-10-24 17:17:14.000000 safrs-3.1.0/safrs/errors.py
+-rwxr-xr-x   0 root         (0) root         (0)     1401 2022-10-24 17:17:14.000000 safrs-3.1.0/safrs/jabase.py
+-rwxr-xr-x   0 root         (0) root         (0)     1682 2023-02-14 18:51:37.000000 safrs-3.1.0/safrs/jsonapi_attr.py
+-rwxr-xr-x   0 root         (0) root         (0)     5857 2023-02-18 09:01:57.000000 safrs-3.1.0/safrs/jsonapi_filters.py
+-rwxr-xr-x   0 root         (0) root         (0)     4047 2023-02-14 18:51:37.000000 safrs-3.1.0/safrs/config.py
+-rwxr-xr-x   0 root         (0) root         (0)     1205 2023-02-18 09:01:57.000000 safrs-3.1.0/safrs/util.py
+-rwxr-xr-x   0 root         (0) root         (0)    41404 2023-05-28 09:06:48.000000 safrs-3.1.0/safrs/jsonapi.py
+-rwxr-xr-x   0 root         (0) root         (0)    31418 2023-05-28 09:06:48.000000 safrs-3.1.0/safrs/safrs_api.py
+-rwxr-xr-x   0 root         (0) root         (0)     1980 2022-10-24 17:17:14.000000 safrs-3.1.0/safrs/_safrs_relationship.py
+-rwxr-xr-x   0 root         (0) root         (0)     4838 2023-05-30 18:27:13.000000 safrs-3.1.0/safrs/json_encoder.py
+-rwxr-xr-x   0 root         (0) root         (0)     1248 2023-05-28 09:06:48.000000 safrs-3.1.0/safrs/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      262 2022-10-24 17:17:14.000000 safrs-3.1.0/safrs/response.py
+-rwxr-xr-x   0 root         (0) root         (0)     9866 2023-02-18 09:01:57.000000 safrs-3.1.0/safrs/jsonapi_formatting.py
+-rwxr-xr-x   0 root         (0) root         (0)       93 2023-05-29 04:14:46.000000 safrs-3.1.0/safrs/__about__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6264 2023-05-28 09:06:48.000000 safrs-3.1.0/safrs/request.py
+-rwxr-xr-x   0 root         (0) root         (0)    35120 2023-02-11 18:54:12.000000 safrs-3.1.0/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 18:29:19.000000 safrs-3.1.0/safrs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-30 18:29:19.000000 safrs-3.1.0/safrs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 18:29:19.000000 safrs-3.1.0/safrs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      522 2023-05-30 18:29:19.000000 safrs-3.1.0/safrs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      648 2023-05-30 18:29:19.000000 safrs-3.1.0/safrs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     2665 2023-05-30 18:29:19.000000 safrs-3.1.0/safrs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1374 2022-10-24 17:17:13.000000 safrs-3.1.0/README.rst
+-rwxr-xr-x   0 root         (0) root         (0)    16881 2023-02-18 09:01:57.000000 safrs-3.1.0/README.md
+-rwxr-xr-x   0 root         (0) root         (0)     1422 2023-05-29 04:14:46.000000 safrs-3.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       90 2022-10-24 17:17:13.000000 safrs-3.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2665 2023-05-30 18:29:19.000000 safrs-3.1.0/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)      433 2023-05-28 09:06:48.000000 safrs-3.1.0/requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `safrs-3.0.4/LICENSE` & `safrs-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safrs-3.0.4/PKG-INFO` & `safrs-3.1.0/safrs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: safrs
-Version: 3.0.4
+Version: 3.1.0
 Summary: safrs : SqlAlchemy Flask-Restful Swagger2
 Home-page: https://github.com/thomaxxl/safrs
 Author: Thomas Pollet
 Author-email: thomas.pollet@gmail.com
 License: MIT
-Download-URL: https://github.com/thomaxxl/safrs/archive/3.0.4.tar.gz
+Download-URL: https://github.com/thomaxxl/safrs/archive/3.1.0.tar.gz
 Description: SAFRS: Python OpenAPI & JSON:API Framework
         ==========================================
         
         Please check the `GitHub Readme <https://github.com/thomaxxl/safrs>`__ for documentation.
         
         Overview
         --------
```

### Comparing `safrs-3.0.4/README.md` & `safrs-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `safrs-3.0.4/README.rst` & `safrs-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `safrs-3.0.4/pyproject.toml` & `safrs-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "safrs"
 
-version = "3.0.4"
+version = "3.1.0"
 
 description="SAFRS : SqlAlchemy Flask-Restful Swagger"
 
 readme = "README.md"
 
 requires-python = ">=3.7"
```

### Comparing `safrs-3.0.4/safrs/__init__.py` & `safrs-3.1.0/safrs/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa: F401
 #
 # The code implements some seemingly awkward constructs and redundant functionality
 # This is however required for backwards compatibility, we'll get rid of it eventually
 #
 from .safrs_init import DB, log, SAFRS, dict_merge, test_decorator, SAFRSRequest
 from .errors import ValidationError, GenericError, UnAuthorizedError, NotFoundError
-from .json_encoder import SAFRSJSONEncoder, SAFRSFormattedResponse
+from .json_encoder import DefaultJSONProvider, SAFRSFormattedResponse
 from .safrs_api import SAFRSAPI
 from .base import SAFRSBase
 from .jabase import JABase
 from .jsonapi_attr import jsonapi_attr
 from .jsonapi import jsonapi_format_response, paginate
 from .api_methods import search, startswith
 from .swagger_doc import jsonapi_rpc
@@ -24,15 +24,15 @@
     "SAFRSAPI",
     "SafrsApi",
     # db:
     "SAFRSBase",
     "jsonapi_attr",
     "jsonapi_rpc",
     # jsonapi:
-    "SAFRSJSONEncoder",
+    "DefaultJSONProvider",
     "paginate",
     "jsonapi_format_response",
     "SAFRSFormattedResponse",
     "JABase",
     # api_methods:
     "search",
     "startswith",
```

### Comparing `safrs-3.0.4/safrs/_safrs_relationship.py` & `safrs-3.1.0/safrs/_safrs_relationship.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.4/safrs/api_methods.py` & `safrs-3.1.0/safrs/api_methods.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.4/safrs/attr_parse.py` & `safrs-3.1.0/safrs/attr_parse.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.4/safrs/base.py` & `safrs-3.1.0/safrs/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # base.py: implements the SAFRSBase SQLAlchemy db Mixin and related operations
 #
 # pylint: disable=logging-format-interpolation,no-self-argument,no-member,line-too-long,fixme,protected-access
 #
 from __future__ import annotations
 import inspect
 import datetime
-from subprocess import list2cmdline
 import sqlalchemy
 import json
 import operator
 from http import HTTPStatus
 from urllib.parse import urljoin
 from flask import request, url_for, has_request_context, current_app, g
 from flask_sqlalchemy import Model
@@ -92,15 +91,15 @@
 
     db_commit = True  # commit instances automatically, see also _s_auto_commit property below
     url_prefix = ""
     allow_client_generated_ids = False  # Indicates whether the client is allowed to create the id
     exclude_attrs = []  # list of attribute names that should not be serialized
     exclude_rels = []  # list of relationship names that should not be serialized
     supports_includes = True  # Set to False if you don't want this class to return included items
-    
+
     # The swagger models are kept here, this lookup table will be used when the api swagger is generated
     # on startup
     swagger_models = {"instance": None, "collection": None}
     _s_expose = True  # indicates we want to expose this (see _s_check_perms)
     jsonapi_filter = jsonapi_filter  # filtering implementation
 
     # Cached lookup tables
@@ -114,17 +113,16 @@
     _rpc_api = safrs.jsonapi.SAFRSJSONRPCAPI
 
     _s_upsert = True  # indicates we want to lookup and use existing objects
     _s_allow_add_rels = True  # allow relationships to be added in post requests
 
     _s_pk_delimiter = "_"
 
-    _s_url_root = None # url prefix shown in the "links" field, if not set, request.url_root will be 
+    _s_url_root = None  # url prefix shown in the "links" field, if not set, request.url_root will be
 
-    
     included_list = None
 
     def __new__(cls, *args, **kwargs):
         """
         If an object with given arguments already exists, this object is instantiated
         """
         if "id" not in kwargs or not cls._s_upsert:
@@ -915,25 +913,27 @@
 
     @classmethod
     def _s_count(cls):
         """
         returning None will cause our jsonapi to perform a count() on the result
         this can be overridden with a cached value for performance on large tables (>1G)
         """
-        max_table_count =  get_config("MAX_TABLE_COUNT")
-        
+        max_table_count = get_config("MAX_TABLE_COUNT")
+
         try:
             count = cls.jsonapi_filter().count()
         except Exception as exc:
             # May happen for custom types, for ex. the psycopg2 extension
             safrs.log.warning(f"Can't get count for {cls} ({exc})")
             count = -1
 
         if count > max_table_count:
-            safrs.log.warning(f"Large table count detected ({count}>{max_table_count}), performance may be impacted, consider '{cls.__name__}._s_count' override")
+            safrs.log.warning(
+                f"Large table count detected ({count}>{max_table_count}), performance may be impacted, consider '{cls.__name__}._s_count' override"
+            )
 
         return count
 
     #
     # Following methods are used to create the swagger2 API documentation
     #
     @classmethod
```

### Comparing `safrs-3.0.4/safrs/config.py` & `safrs-3.1.0/safrs/config.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.4/safrs/errors.py` & `safrs-3.1.0/safrs/errors.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.4/safrs/jabase.py` & `safrs-3.1.0/safrs/jabase.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.4/safrs/json_encoder.py` & `safrs-3.1.0/safrs/json_encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # safrs to json encoding
 
 import datetime
 import decimal
 import json
-from flask.json import JSONEncoder
+from flask.json.provider import DefaultJSONProvider
 from sqlalchemy.ext.declarative import DeclarativeMeta
 from uuid import UUID
 import safrs
 from .config import is_debug
 from .base import SAFRSBase, Included
 from .jsonapi_formatting import jsonapi_format_response
 
@@ -47,17 +47,18 @@
 
         if self.result is not None:
             return {"meta": {"result": self.result}}
 
         return None
 
 
-class SAFRSJSONEncoder(JSONEncoder):
+
+class _SAFRSJSONEncoder():
     """
-    Encodes safrs objs (SAFRSBase subclasses)
+    JSON encoding for safrs objects (SAFRSBase subclasses and common types)
     """
 
     # pylint: disable=too-many-return-statements,logging-format-interpolation
     # pylint: disable=arguments-differ,protected-access,method-hidden
     def default(self, obj, **kwargs):
         """
         override the default json encoding
@@ -139,7 +140,21 @@
                 # this will raise an exception if the data can't be serialized
                 fields[field] = json.dumps(data)
             except TypeError:
                 fields[field] = str(data)
 
         # a json-encodable dict
         return fields
+
+
+class SAFRSJSONProvider(_SAFRSJSONEncoder, DefaultJSONProvider):
+    """
+        Flask JSON encoding
+    """
+    mimetype = "application/vnd.api+json"
+
+
+class SAFRSJSONEncoder(_SAFRSJSONEncoder, json.JSONEncoder):
+    """
+        Common JSON encoding
+    """
+    pass
```

### Comparing `safrs-3.0.4/safrs/jsonapi.py` & `safrs-3.1.0/safrs/jsonapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,15 +273,16 @@
             # retrieve a collection, filter and sort
             instances = self.SAFRSObject._s_get()
             instances = jsonapi_sort(instances, self.SAFRSObject)
             links, data, count = paginate(instances, self.SAFRSObject)
 
         # format the response: add the included objects
         result = jsonapi_format_response(data, meta, links, errors, count)
-        return make_response(jsonify(result))
+        return jsonify(result)
+        return make_response({})
 
     def patch(self, **kwargs):
         """
         summary : Update {class_name}
         description: Update {class_name} attributes
         responses:
             200 :
```

### Comparing `safrs-3.0.4/safrs/jsonapi_attr.py` & `safrs-3.1.0/safrs/jsonapi_attr.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.4/safrs/jsonapi_filters.py` & `safrs-3.1.0/safrs/jsonapi_filters.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.4/safrs/jsonapi_formatting.py` & `safrs-3.1.0/safrs/jsonapi_formatting.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.4/safrs/request.py` & `safrs-3.1.0/safrs/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,31 +80,31 @@
             page_size = self.args.get("page[size]", type=int)
             page_number = self.args.get("page[number]", type=int) - 1
             page_offset = page_number * page_size
         return page_offset
 
     def get_page_offset(self, rel_name):
         """
-            get the page offset for the included relationship resource 
-            :param rel_name: name of the relationship
-            :return: page offset for included resources
+        get the page offset for the included relationship resource
+        :param rel_name: name of the relationship
+        :return: page offset for included resources
         """
         page_offset = self.args.get(f"page[{rel_name}][offset]", 0, type=int)
         if page_offset == 0 and "page[{rel_name}][number]" in self.args and "page[{rel_name}][size]" in self.args:
             page_size = self.args.get("page[{rel_name}][size]", type=int)
             page_number = self.args.get("page[{rel_name}][number]", type=int) - 1
             page_offset = page_number * page_size
         return page_offset
 
     @property
     def page_limit(self):
         """
-            get the page limit for the included relationship resource 
-            :param rel_name: name of the relationship
-            :return: page limit for included resources
+        get the page limit for the included relationship resource
+        :param rel_name: name of the relationship
+        :return: page limit for included resources
         """
         page_limit = self.args.get("page[limit]", get_config("DEFAULT_PAGE_LIMIT"), type=int)
         if "page[number]" in self.args and "page[size]" in self.args:
             return self.args.get("page[size]", type=int)
         return page_limit
 
     def get_page_limit(self, rel_name):
```

### Comparing `safrs-3.0.4/safrs/safrs_api.py` & `safrs-3.1.0/safrs/safrs_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from flask import request
 from functools import wraps
 import safrs
 from .swagger_doc import swagger_doc, swagger_method_doc, default_paging_parameters
 from .swagger_doc import parse_object_doc, swagger_relationship_doc, get_http_methods
 from .errors import JsonapiError, SystemValidationError, GenericError
 from .config import get_config
-from .json_encoder import SAFRSJSONEncoder
+from .json_encoder import SAFRSJSONProvider, SAFRSJSONEncoder
 from ._safrs_relationship import SAFRSRelationshipObject
 from sqlalchemy.orm.interfaces import MANYTOONE
 from flask import current_app, Response
 import json
 import yaml
 from flask.app import Flask
 from typing import Callable, Type
@@ -44,15 +44,15 @@
     def __init__(
         self,
         app: Flask,
         host: str = "localhost",
         port: int = 5000,
         prefix: str = "",
         description: str = "SAFRSAPI",
-        json_encoder: Type[SAFRSJSONEncoder] = SAFRSJSONEncoder,
+        json_encoder: Type[SAFRSJSONProvider] = None,
         swaggerui_blueprint: bool = True,
         **kwargs,
     ) -> None:
         """
         http://jsonapi.org/format/#content-negotiation-servers
         Servers MUST send all JSON:API data in response documents with
         the header Content-Type: application/vnd.api+json without any media type parameters.
@@ -81,14 +81,16 @@
             api_spec_url=kwargs.pop("api_spec_url", "/swagger"),
             host=host,
             description=description,
             prefix=prefix,
             base_path=prefix,
             **kwargs,
         )
+        app.json = SAFRSJSONProvider(app)
+        app.json_encoder = SAFRSJSONEncoder  # deprecated, but used by the swaggerui blueprint
         self.init_app(app)
         self.representations = OrderedDict(DEFAULT_REPRESENTATIONS)
         self.update_spec()
 
     def update_spec(self) -> None:
         """
         :param custom_swagger: swagger spec to be added to the swagger.json
```

### Comparing `safrs-3.0.4/safrs/safrs_init.py` & `safrs-3.1.0/safrs/safrs_init.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import logging
 import os
 import sys
 from flask_swagger_ui import get_swaggerui_blueprint
 from flask import Flask, g
-from flask.json import JSONEncoder
 from flask_sqlalchemy import SQLAlchemy
 from .request import SAFRSRequest
 from .response import SAFRSResponse
-from .json_encoder import SAFRSJSONEncoder
 from .jsonapi_filters import FilteringStrategy
 from functools import wraps
 import safrs
 import flask.app
 from typing import Any, Dict, Type, Union
 
 
@@ -57,44 +55,41 @@
     def init_app(
         self,
         app: flask.app.Flask,
         host: str = "localhost",
         port: int = 5000,
         prefix: str = "",
         app_db: None = None,
-        json_encoder: Type[SAFRSJSONEncoder] = SAFRSJSONEncoder,
         swaggerui_blueprint: bool = True,
         **kwargs,
     ) -> None:
         """
         API and application initialization
         """
         if not isinstance(app, Flask):  # pragma: no cover
             raise TypeError("'app' should be Flask.")
 
         if app_db is None:
             app_db = app.extensions["sqlalchemy"]
 
         safrs.DB = self.db = app_db
 
-        app.json_encoder = json_encoder
         app.request_class = SAFRSRequest
         app.response_class = SAFRSResponse
         app.url_map.strict_slashes = False
 
         if app.config.get("DEBUG", False):
             log.setLevel(logging.DEBUG)
 
         # Register the API blueprint
         if swaggerui_blueprint is True:
             swaggerui_blueprint = get_swaggerui_blueprint(
                 prefix, f"{prefix}/swagger.json", config={"docExpansion": "none", "defaultModelsExpandDepth": -1}
             )
             app.register_blueprint(swaggerui_blueprint, url_prefix=prefix)
-            swaggerui_blueprint.json_encoder = JSONEncoder
 
         for conf_name, conf_val in kwargs.items():
             setattr(SAFRS, conf_name, conf_val)
 
         for conf_name, conf_val in app.config.items():
             setattr(SAFRS, conf_name, conf_val)
```

### Comparing `safrs-3.0.4/safrs/safrs_types.py` & `safrs-3.1.0/safrs/safrs_types.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.4/safrs/swagger_doc.py` & `safrs-3.1.0/safrs/swagger_doc.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.4/safrs/util.py` & `safrs-3.1.0/safrs/util.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.4/safrs.egg-info/PKG-INFO` & `safrs-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: safrs
-Version: 3.0.4
+Version: 3.1.0
 Summary: safrs : SqlAlchemy Flask-Restful Swagger2
 Home-page: https://github.com/thomaxxl/safrs
 Author: Thomas Pollet
 Author-email: thomas.pollet@gmail.com
 License: MIT
-Download-URL: https://github.com/thomaxxl/safrs/archive/3.0.4.tar.gz
+Download-URL: https://github.com/thomaxxl/safrs/archive/3.1.0.tar.gz
 Description: SAFRS: Python OpenAPI & JSON:API Framework
         ==========================================
         
         Please check the `GitHub Readme <https://github.com/thomaxxl/safrs>`__ for documentation.
         
         Overview
         --------
```

### Comparing `safrs-3.0.4/safrs.egg-info/SOURCES.txt` & `safrs-3.1.0/safrs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safrs-3.0.4/safrs.egg-info/requires.txt` & `safrs-3.1.0/safrs.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-Flask-Cors>=3.0.10
-Flask-RESTful>=0.3.9
-Flask-SQLAlchemy>=3.0.3
-Flask==2.2.5
-Jinja2>=3.1.2
-MarkupSafe>=2.1.2
-PyYAML>=6.0
-SQLAlchemy>=2.0.3
-Werkzeug>=2.2.2
 aniso8601>=9.0.1
 build>=0.10.0
 click>=8.1.3
+Flask>=2.3.2
+Flask-Cors>=3.0.10
+Flask-RESTful>=0.3.9
 flask-restful-swagger-2>=0.35
+Flask-SQLAlchemy>=3.0.3
 flask-swagger-ui>=4.11.1
 greenlet>=2.0.2
 importlib-metadata>=6.0.0
 itsdangerous>=2.1.2
+Jinja2>=3.1.2
+MarkupSafe>=2.1.2
 packaging>=23.0
 pyproject-hooks>=1.0.0
 pytz>=2022.7.1
+PyYAML>=6.0
 six>=1.16.0
+SQLAlchemy>=2.0.3
 tomli>=2.0.1
 typing-extensions>=4.4.0
+Werkzeug>=2.2.2
 zipp>=3.13.0
 
 [admin]
 Flask-Admin>=1.5.8
 Flask-Cors>=3.0.9
 
 [db2api]
-Flask-Cors>=3.0.9
 inflect==5.0.2
+Flask-Cors>=3.0.9
```

### Comparing `safrs-3.0.4/setup.py` & `safrs-3.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup, find_packages
 
 
 def safrs_setup():
     with open("requirements.txt", "rt") as fp:
         install_requires = fp.read().strip().split("\n")
 
-    version = "3.0.4"
+    version = "3.1.0"
 
     setup(
         name="safrs",
         packages=find_packages(exclude=['test']),
         version=version,
         license="MIT",
         description="safrs : SqlAlchemy Flask-Restful Swagger2",
```

