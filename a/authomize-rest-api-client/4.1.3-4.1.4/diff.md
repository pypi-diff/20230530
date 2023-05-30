# Comparing `tmp/authomize-rest-api-client-4.1.3.tar.gz` & `tmp/authomize-rest-api-client-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-4.1.3.tar", last modified: Mon May 29 21:32:33 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-4.1.4.tar", last modified: Tue May 30 14:06:16 2023, max compression
```

## Comparing `authomize-rest-api-client-4.1.3.tar` & `authomize-rest-api-client-4.1.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2194 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2538 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10358 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    13027 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75246 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35372 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   189364 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    87696 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-29 21:32:33.000000 authomize-rest-api-client-4.1.3/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-05-29 21:32:33.000000 authomize-rest-api-client-4.1.3/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 21:32:33.000000 authomize-rest-api-client-4.1.3/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-29 21:32:33.000000 authomize-rest-api-client-4.1.3/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-29 21:32:33.000000 authomize-rest-api-client-4.1.3/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-29 21:32:17.000000 authomize-rest-api-client-4.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.251852 authomize-rest-api-client-4.1.4/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-30 14:06:16.251852 authomize-rest-api-client-4.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.247852 authomize-rest-api-client-4.1.4/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.247852 authomize-rest-api-client-4.1.4/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.247852 authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2538 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10358 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    13027 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.247852 authomize-rest-api-client-4.1.4/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.247852 authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.247852 authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75246 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.247852 authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37380 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.247852 authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.247852 authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   189364 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.251852 authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89370 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.251852 authomize-rest-api-client-4.1.4/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-30 14:06:16.000000 authomize-rest-api-client-4.1.4/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-05-30 14:06:16.000000 authomize-rest-api-client-4.1.4/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 14:06:16.000000 authomize-rest-api-client-4.1.4/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-30 14:06:16.000000 authomize-rest-api-client-4.1.4/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-30 14:06:16.000000 authomize-rest-api-client-4.1.4/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-05-30 14:06:16.251852 authomize-rest-api-client-4.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-05-30 14:05:58.000000 authomize-rest-api-client-4.1.4/setup.py
```

### Comparing `authomize-rest-api-client-4.1.3/LICENSE.txt` & `authomize-rest-api-client-4.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.3/README.md` & `authomize-rest-api-client-4.1.4/README.md`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.3/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-4.1.4/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-05-23T14:21:16+00:00
+#   timestamp: 2023-05-30T13:55:35+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional
```

### Comparing `authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-05-25T09:00:40+00:00
+#   timestamp: 2023-05-30T13:58:26+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional, Union
 
@@ -363,15 +363,15 @@
     A_8_2_3 = 'A.8.2.3'
     A_7_3_1 = 'A.7.3.1'
     A_8_1_4 = 'A.8.1.4'
 
 
 class MeResponse(BaseModel):
     version: Optional[str] = Field(
-        default='4.1.2', description='**version**', title='Version'
+        default='4.1.3', description='**version**', title='Version'
     )
     id: str = Field(..., description='**id**', title='Id')
     tenant: str = Field(..., description='**tenant**', title='Tenant')
 
 
 class NonPaginatedResponseSchemaCommentSchema(BaseModel):
     class Config:
@@ -389,27 +389,35 @@
     )
 
 
 class PaginationRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    limit: Optional[int] = Field(default=None, description='Limit', title='Limit')
+    limit: Optional[int] = Field(
+        default=None,
+        description='Limit the number of identities per page',
+        title='Limit',
+    )
     nextPage: Optional[str] = Field(
-        default=None, description='Starting after', title='NextPage'
+        default=None, description='Token denoting start of next page', title='NextPage'
     )
 
 
 class PaginationResponseSchema(BaseModel):
-    limit: Optional[int] = Field(default=20, description='Limit', title='Limit')
+    limit: Optional[int] = Field(
+        default=20, description='Limit the number of identities per page', title='Limit'
+    )
     hasMore: Optional[bool] = Field(
-        default=None, description='Has more? `true` or `false`.', title='HasMore'
+        default=None,
+        description='Indicates that more data is available',
+        title='HasMore',
     )
     nextPage: Optional[str] = Field(
-        default=None, description='Starting after', title='NextPage'
+        default=None, description='Token denoting start of next page', title='NextPage'
     )
 
 
 class PermissionsExpansion(Enum):
     reviewer_user = 'reviewer.user'
 
 
@@ -436,18 +444,22 @@
 
 
 class SearchIdentitiesFilterBody(BaseModel):
     class Config:
         extra = Extra.forbid
 
     email: Optional[EmailFilter] = Field(
-        default=None, description='Email.', title='Email'
+        default=None,
+        description='Find identities by their email address',
+        title='Email',
     )
     authomizeId: Optional[IdFilter] = Field(
-        default=None, description='Authomize ID for the Identity', title='Authomizeid'
+        default=None,
+        description='Find identities by their Authomize ID',
+        title='Authomizeid',
     )
 
 
 class SearchIdentitiesSortFields(Enum):
     identity_name = 'identity.name'
 
 
@@ -478,60 +490,72 @@
 
 
 class SortSchemaFieldName(BaseModel):
     class Config:
         extra = Extra.forbid
 
     fieldName: FieldName = Field(
-        ..., description='Sort By Field Name', title='FieldName'
+        ..., description='Sort the results by field name', title='FieldName'
     )
     order: Optional[SortOrder] = Field(
-        default='ASC', description='Sort Order', title='Order'
+        default='ASC',
+        description='Sort by ascending or descending order (ascending is the default)',
+        title='Order',
     )
 
 
 class SortSchemaSearchAssetsSortFields(BaseModel):
     class Config:
         extra = Extra.forbid
 
     fieldName: SearchAssetsSortFields = Field(
-        ..., description='Sort By Field Name', title='FieldName'
+        ..., description='Sort the results by field name', title='FieldName'
     )
     order: Optional[SortOrder] = Field(
-        default='ASC', description='Sort Order', title='Order'
+        default='ASC',
+        description='Sort by ascending or descending order (ascending is the default)',
+        title='Order',
     )
 
 
 class SortSchemaSearchIdentitiesSortFields(BaseModel):
     class Config:
         extra = Extra.forbid
 
     fieldName: SearchIdentitiesSortFields = Field(
-        ..., description='Sort By Field Name', title='FieldName'
+        ..., description='Sort the results by field name', title='FieldName'
     )
     order: Optional[SortOrder] = Field(
-        default='ASC', description='Sort Order', title='Order'
+        default='ASC',
+        description='Sort by ascending or descending order (ascending is the default)',
+        title='Order',
     )
 
 
 class SortSchemaSearchIncidentsSortFields(BaseModel):
     class Config:
         extra = Extra.forbid
 
     fieldName: SearchIncidentsSortFields = Field(
-        ..., description='Sort By Field Name', title='FieldName'
+        ..., description='Sort the results by field name', title='FieldName'
     )
     order: Optional[SortOrder] = Field(
-        default='ASC', description='Sort Order', title='Order'
+        default='ASC',
+        description='Sort by ascending or descending order (ascending is the default)',
+        title='Order',
     )
 
 
 class SourceAppSchema(BaseModel):
-    id: str = Field(..., description='Unique ID', title='Id')
-    name: str = Field(..., description='Name', title='Name')
+    id: str = Field(..., description='Authomize ID of source application', title='Id')
+    name: str = Field(
+        ...,
+        description='Name of the asset (for example, application, virtual machine, file, etc.)',
+        title='Name',
+    )
 
 
 class TagSchema(BaseModel):
     id: str = Field(..., description='Authomize ID for the Tag', title='Id')
     name: str = Field(..., description='Name of the tag', title='Name')
     description: str = Field(
         ..., description='Description of the tag', title='Description'
@@ -586,49 +610,63 @@
     )
     name: Optional[str] = Field(
         default='SOC 2 (TSC 2017)', description='Name', title='Name'
     )
 
 
 class AssetSchema(BaseModel):
-    authomizeId: str = Field(..., description='Unique ID', title='Authomizeid')
-    name: str = Field(..., description='Name', title='Name')
-    type: str = Field(..., description='Type', title='Type')
+    authomizeId: str = Field(
+        ..., description='Authomize ID of source application', title='Authomizeid'
+    )
+    name: str = Field(
+        ...,
+        description='Name of the asset (for example, application, virtual machine, file, etc.)',
+        title='Name',
+    )
+    type: str = Field(..., description='Type of asset', title='Type')
     originType: Optional[str] = Field(
         default=None,
-        description='The asset type in the source system. The default is the canonical type (if not mentioned).\n',
+        description='The type of asset on the source system',
         title='Origintype',
     )
     sourceApp: Optional[SourceAppSchema] = Field(
-        default=None, description='Source App', title='Sourceapp'
+        default=None,
+        description='The source application of the asset',
+        title='Sourceapp',
     )
     createdAt: Optional[datetime] = Field(
         default=None,
-        description='The date (in ISO 8601 format) that the asset was created.\n',
+        description='The date (in ISO 8601 format) that the asset was created\n',
         title='Createdat',
     )
     lastUsedAt: Optional[str] = Field(
         default=None,
         description='The date (in ISO 8601 format) of the last time that the asset was in use.',
         title='Lastusedat',
     )
-    href: Optional[str] = Field(default=None, description='HREF', title='Href')
+    href: Optional[str] = Field(
+        default=None,
+        description='A link to the asset in the source application',
+        title='Href',
+    )
     uniqueId: Optional[str] = Field(
-        default=None, description='The Unique Identifier.', title='Uniqueid'
+        default=None,
+        description='The unique ID of the asset (as provided by the connector)',
+        title='Uniqueid',
     )
     originId: Optional[str] = Field(
         default=None,
-        description='The identifier of the asset from the origin system.',
+        description='The ID of the asset on the source system',
         title='Originid',
     )
     description: Optional[str] = Field(
-        default=None, description='Asset description', title='Description'
+        default=None, description='A description of the asset', title='Description'
     )
     tags: Optional[List[TagSchema]] = Field(
-        default=None, description='Expanded Tags', title='Tags'
+        default=None, description='List of tags associated with the asset', title='Tags'
     )
     incidentsCount: Optional[int] = Field(
         default=None,
         description='Number of associated incidents',
         title='Incidentscount',
     )
 
@@ -705,21 +743,23 @@
     class Config:
         extra = Extra.forbid
 
     originId: Optional[OriginIdFilter] = Field(
         default=None, description='Origin ID of the Asset.', title='Originid'
     )
     appId: Optional[AppIdFilter] = Field(
-        default=None, description='ID of the Application.', title='Appid'
+        default=None, description='Find assets by their app ID', title='Appid'
     )
     uniqueId: Optional[UniqueIdFilter] = Field(
-        default=None, description='Unique ID of the Asset.', title='Uniqueid'
+        default=None, description='Find assets by their unique ID', title='Uniqueid'
     )
     authomizeId: Optional[AssetIdFilter] = Field(
-        default=None, description='Authomize ID for the Asset', title='Authomizeid'
+        default=None,
+        description='Find assets by their Authomize ID',
+        title='Authomizeid',
     )
 
 
 class HTTPValidationError(BaseModel):
     detail: Optional[List[ValidationError]] = Field(default=None, title='Detail')
 
 
@@ -787,28 +827,34 @@
         ..., description='List of Actual Data', title='Data'
     )
 
 
 class RawIdentitySchema(BaseModel):
     authomizeId: str = Field(..., description='Unique ID', title='Authomizeid')
     name: Optional[str] = Field(
-        default=None, description='Name of Identity', title='Name'
+        default=None, description='Name of the identity', title='Name'
+    )
+    title: Optional[str] = Field(
+        default=None, description='Title of the identity', title='Title'
     )
-    title: Optional[str] = Field(default=None, description='Title', title='Title')
     department: Optional[str] = Field(
-        default=None, description='Department', title='Department'
+        default=None,
+        description='The department in which the identity works',
+        title='Department',
     )
     accountIds: Optional[List[str]] = Field(
-        default=[], description='List of associated account IDs', title='Accountids'
+        default=[],
+        description='The account IDs associated with the identity',
+        title='Accountids',
     )
     email: Optional[str] = Field(
-        default=None, description="User's work email address.\n", title='Email'
+        default=None, description='The email of the identity', title='Email'
     )
     tags: Optional[List[TagSchema]] = Field(
-        default=None, description='Expanded Tags', title='Tags'
+        default=None, description='The tags provided for the identity', title='Tags'
     )
     terminatedAt: Optional[str] = Field(
         default=None, description='Time of termination', title='Terminatedat'
     )
     hiredAt: Optional[str] = Field(
         default=None, description='Hired At', title='Hiredat'
     )
@@ -838,33 +884,37 @@
 
 
 class SearchAssetsRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     sort: Optional[List[SortSchemaSearchAssetsSortFields]] = Field(
-        default=None, description='Sort', title='Sort'
+        default=None,
+        description='Sort the results by identity name in ascending or descending order',
+        title='Sort',
     )
     pagination: Optional[PaginationRequestSchema] = Field(
-        default=None, description='Pagination', title='Pagination'
+        default=None, description='Pagination metadata', title='Pagination'
     )
     expand: Optional[List[AssetExpansion]] = Field(
-        default=None, description='Expand Fields'
+        default=None, description='Expand fields (to show additional information)'
     )
     filter: Optional[Chainable] = Field(
-        default=None, description='Search Assets Filter', title='Filter'
+        default=None,
+        description='Find assets by their ID on the source system',
+        title='Filter',
     )
 
 
 class SearchCampaignPermissionsRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     pagination: Optional[PaginationRequestSchema] = Field(
-        default=None, description='Pagination', title='Pagination'
+        default=None, description='Pagination metadata', title='Pagination'
     )
     filter: Optional[CampaignPermissionsSearchFilterBody] = Field(
         default=None, description='Filter by the reviewer decisions. \n', title='Filter'
     )
     expand: Optional[List[PermissionsExpansion]] = Field(
         default=None, description='Fields to expand.\n'
     )
@@ -877,36 +927,41 @@
     filter: Optional[CampaignSearchFilterBody] = Field(
         default=None, description='Status filter', title='Filter'
     )
     expand: Optional[List[CampaignExpansion]] = Field(
         default=None, description='Expand Fields'
     )
     pagination: Optional[PaginationRequestSchema] = Field(
-        default=None, description='Pagination', title='Pagination'
+        default=None, description='Pagination metadata', title='Pagination'
     )
     sort: Optional[List[SortSchemaFieldName]] = Field(
-        default=None, description='Sort', title='Sort'
+        default=None,
+        description='Sort the results by identity name in ascending or descending order',
+        title='Sort',
     )
 
 
 class SearchIdentitiesRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     sort: Optional[List[SortSchemaSearchIdentitiesSortFields]] = Field(
-        default=None, description='Sort', title='Sort'
+        default=None,
+        description='Sort the results by identity name in ascending or descending order',
+        title='Sort',
     )
     pagination: Optional[PaginationRequestSchema] = Field(
-        default=None, description='Pagination', title='Pagination'
+        default=None, description='Pagination metadata', title='Pagination'
     )
     expand: Optional[List[IdentityExpansion]] = Field(
-        default=None, description='Expand Fields'
+        default=None,
+        description='Expand the account or tag fields to get additional data on related accounts or related tags',
     )
     filter: Optional[SearchIdentitiesFilterBody] = Field(
-        default=None, description='Search Identities Filter', title='Filter'
+        default=None, description='Search filter options', title='Filter'
     )
 
 
 class SearchIncidentsFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
@@ -940,51 +995,61 @@
     filter: Optional[SearchIncidentsFilter] = Field(
         default=None, description='Filter', title='Filter'
     )
     expand: Optional[List[IncidentExpansion]] = Field(
         default=None, description='Expend'
     )
     sort: Optional[List[SortSchemaSearchIncidentsSortFields]] = Field(
-        default=None, description='Sort', title='Sort'
+        default=None,
+        description='Sort the results by identity name in ascending or descending order',
+        title='Sort',
     )
     pagination: Optional[PaginationRequestSchema] = Field(
-        default=None, description='Pagination', title='Pagination'
+        default=None, description='Pagination metadata', title='Pagination'
     )
 
 
 class AccountSchema(BaseModel):
     authomizeId: str = Field(..., description='Unique ID', title='Authomizeid')
     originId: Optional[str] = Field(
         default=None,
-        description='The identifier of the account from the origin system.',
+        description='The identifier of the account from the source system.',
         title='Originid',
     )
     uniqueId: Optional[str] = Field(
         default=None,
-        description='Unique ID is an identifier coming from the connector that is guaranteed to be unique across all accounts coming from that connector.',
+        description='Unique ID is an identifier coming from the connector that is unique across all accounts coming from that connector',
         title='Uniqueid',
     )
-    name: Optional[str] = Field(default=None, description='Name', title='Name')
-    type: str = Field(..., description='Type', title='Type')
-    isExternal: bool = Field(..., description='Is External', title='Isexternal')
-    email: Optional[str] = Field(default=None, description='Email', title='Email')
+    name: Optional[str] = Field(
+        default=None, description='Name of account', title='Name'
+    )
+    type: str = Field(..., description='Type of account', title='Type')
+    isExternal: bool = Field(
+        ..., description='Is account external (Yes or No)', title='Isexternal'
+    )
+    email: Optional[str] = Field(
+        default=None, description='Email address of account', title='Email'
+    )
     identityId: Optional[str] = Field(
-        default=None, description='Associated Identity ID ', title='Identityid'
+        default=None, description='ID of identitiy', title='Identityid'
     )
     identity: Optional[RawIdentitySchema] = Field(
         default=None, description='Associated Identity', title='Identity'
     )
     sourceApp: Optional[SourceAppSchema] = Field(
-        default=None, description='Source App', title='Sourceapp'
+        default=None, description='Associated source app ', title='Sourceapp'
     )
     isAdmin: Optional[bool] = Field(
-        default=None, description='Is Admin', title='Isadmin'
+        default=None,
+        description='Is the account an admin account (Yes or No)',
+        title='Isadmin',
     )
     tags: Optional[List[TagSchema]] = Field(
-        default=None, description='Expanded Tags', title='Tags'
+        default=None, description='List of tags associated with the asset', title='Tags'
     )
 
 
 class CampaignsPermissionSchema(BaseModel):
     id: str = Field(..., description='Campaign ID (unique). \n', title='Id')
     campaignId: str = Field(
         ..., description='ID of the Campaign.\n', title='Campaignid'
@@ -1024,42 +1089,50 @@
         title='Decisionreason',
     )
 
 
 class IdentitySchema(BaseModel):
     authomizeId: str = Field(..., description='Unique ID', title='Authomizeid')
     name: Optional[str] = Field(
-        default=None, description='Name of Identity', title='Name'
+        default=None, description='Name of the identity', title='Name'
+    )
+    title: Optional[str] = Field(
+        default=None, description='Title of the identity', title='Title'
     )
-    title: Optional[str] = Field(default=None, description='Title', title='Title')
     department: Optional[str] = Field(
-        default=None, description='Department', title='Department'
+        default=None,
+        description='The department in which the identity works',
+        title='Department',
     )
     accountIds: Optional[List[str]] = Field(
-        default=[], description='List of associated account IDs', title='Accountids'
+        default=[],
+        description='The account IDs associated with the identity',
+        title='Accountids',
     )
     email: Optional[str] = Field(
-        default=None, description="User's work email address.\n", title='Email'
+        default=None, description='The email of the identity', title='Email'
     )
     tags: Optional[List[TagSchema]] = Field(
-        default=None, description='Expanded Tags', title='Tags'
+        default=None, description='The tags provided for the identity', title='Tags'
     )
     terminatedAt: Optional[str] = Field(
         default=None, description='Time of termination', title='Terminatedat'
     )
     hiredAt: Optional[str] = Field(
         default=None, description='Hired At', title='Hiredat'
     )
     incidentsCount: Optional[int] = Field(
         default=None,
         description='Number of associated incidents',
         title='Incidentscount',
     )
     accounts: Optional[List[AccountSchema]] = Field(
-        default=[], description='List of associated accounts', title='Accounts'
+        default=[],
+        description='List of associated user or service accounts',
+        title='Accounts',
     )
 
 
 class IncidentSchema(BaseModel):
     id: str = Field(..., description='Unique id', title='Id')
     createdAt: Optional[datetime] = Field(
         default=None,
```

### Comparing `authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9874970238095238%*

 * *Differences: {"'info'": "{'version': '4.1.3'}",*

 * * "'paths'": "{'/v2/apps/{appId}/data': {'delete': {'parameters': {1: {'example': "*

 * *            "'2023-05-30T13:53:04.594383+00:00'}}}}}"}*

```diff
@@ -3764,15 +3764,15 @@
                 "type": "apiKey"
             }
         }
     },
     "info": {
         "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "4.1.1",
+        "version": "4.1.3",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
@@ -5571,15 +5571,15 @@
                         "schema": {
                             "title": "Appid",
                             "type": "string"
                         }
                     },
                     {
                         "description": "Delete all the app data lastly updated before the given date.",
-                        "example": "2023-05-23T09:23:41.791121+00:00",
+                        "example": "2023-05-30T13:53:04.594383+00:00",
                         "in": "query",
                         "name": "modifiedBefore",
                         "required": false,
                         "schema": {
                             "description": "Delete all the app data lastly updated before the given date.",
                             "format": "date-time",
                             "title": "Modifiedbefore",
```

### Comparing `authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9809347392474648%*

 * *Differences: {"'components'": "{'schemas': {'AccountSchema': {'properties': {'originId': {'description': 'The "*

 * *                 "identifier of the account from the source system.'}, 'uniqueId': {'description': "*

 * *                 "'Unique ID is an identifier coming from the connector that is unique across all "*

 * *                 "accounts coming from that connector'}, 'name': {'description': 'Name of "*

 * *                 "account'}, 'type': {'description': 'Type of account'}, 'isExternal': "*

 * *                 "{'description […]*

```diff
@@ -23,76 +23,76 @@
                 "properties": {
                     "authomizeId": {
                         "description": "Unique ID",
                         "title": "Authomizeid",
                         "type": "string"
                     },
                     "email": {
-                        "description": "Email",
+                        "description": "Email address of account",
                         "title": "Email",
                         "type": "string"
                     },
                     "identity": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/RawIdentitySchema"
                             }
                         ],
                         "description": "Associated Identity",
                         "title": "Identity"
                     },
                     "identityId": {
-                        "description": "Associated Identity ID ",
+                        "description": "ID of identitiy",
                         "title": "Identityid",
                         "type": "string"
                     },
                     "isAdmin": {
-                        "description": "Is Admin",
+                        "description": "Is the account an admin account (Yes or No)",
                         "title": "Isadmin",
                         "type": "boolean"
                     },
                     "isExternal": {
-                        "description": "Is External",
+                        "description": "Is account external (Yes or No)",
                         "title": "Isexternal",
                         "type": "boolean"
                     },
                     "name": {
-                        "description": "Name",
+                        "description": "Name of account",
                         "title": "Name",
                         "type": "string"
                     },
                     "originId": {
-                        "description": "The identifier of the account from the origin system.",
+                        "description": "The identifier of the account from the source system.",
                         "title": "Originid",
                         "type": "string"
                     },
                     "sourceApp": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/SourceAppSchema"
                             }
                         ],
-                        "description": "Source App",
+                        "description": "Associated source app ",
                         "title": "Sourceapp"
                     },
                     "tags": {
-                        "description": "Expanded Tags",
+                        "description": "List of tags associated with the asset",
                         "items": {
                             "$ref": "#/components/schemas/TagSchema"
                         },
                         "title": "Tags",
                         "type": "array"
                     },
                     "type": {
-                        "description": "Type",
+                        "description": "Type of account",
                         "title": "Type",
                         "type": "string"
                     },
                     "uniqueId": {
-                        "description": "Unique ID is an identifier coming from the connector that is guaranteed to be unique across all accounts coming from that connector.",
+                        "description": "Unique ID is an identifier coming from the connector that is unique across all accounts coming from that connector",
                         "title": "Uniqueid",
                         "type": "string"
                     }
                 },
                 "required": [
                     "authomizeId",
                     "type",
@@ -224,83 +224,83 @@
                 },
                 "title": "AssetIdFilter",
                 "type": "object"
             },
             "AssetSchema": {
                 "properties": {
                     "authomizeId": {
-                        "description": "Unique ID",
+                        "description": "Authomize ID of source application",
                         "title": "Authomizeid",
                         "type": "string"
                     },
                     "createdAt": {
-                        "description": "The date (in ISO 8601 format) that the asset was created.\n",
+                        "description": "The date (in ISO 8601 format) that the asset was created\n",
                         "format": "date-time",
                         "title": "Createdat",
                         "type": "string"
                     },
                     "description": {
-                        "description": "Asset description",
+                        "description": "A description of the asset",
                         "title": "Description",
                         "type": "string"
                     },
                     "href": {
-                        "description": "HREF",
+                        "description": "A link to the asset in the source application",
                         "title": "Href",
                         "type": "string"
                     },
                     "incidentsCount": {
                         "description": "Number of associated incidents",
                         "title": "Incidentscount",
                         "type": "integer"
                     },
                     "lastUsedAt": {
                         "description": "The date (in ISO 8601 format) of the last time that the asset was in use.",
                         "title": "Lastusedat",
                         "type": "string"
                     },
                     "name": {
-                        "description": "Name",
+                        "description": "Name of the asset (for example, application, virtual machine, file, etc.)",
                         "title": "Name",
                         "type": "string"
                     },
                     "originId": {
-                        "description": "The identifier of the asset from the origin system.",
+                        "description": "The ID of the asset on the source system",
                         "title": "Originid",
                         "type": "string"
                     },
                     "originType": {
-                        "description": "The asset type in the source system. The default is the canonical type (if not mentioned).\n",
+                        "description": "The type of asset on the source system",
                         "title": "Origintype",
                         "type": "string"
                     },
                     "sourceApp": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/SourceAppSchema"
                             }
                         ],
-                        "description": "Source App",
+                        "description": "The source application of the asset",
                         "title": "Sourceapp"
                     },
                     "tags": {
-                        "description": "Expanded Tags",
+                        "description": "List of tags associated with the asset",
                         "items": {
                             "$ref": "#/components/schemas/TagSchema"
                         },
                         "title": "Tags",
                         "type": "array"
                     },
                     "type": {
-                        "description": "Type",
+                        "description": "Type of asset",
                         "title": "Type",
                         "type": "string"
                     },
                     "uniqueId": {
-                        "description": "The Unique Identifier.",
+                        "description": "The unique ID of the asset (as provided by the connector)",
                         "title": "Uniqueid",
                         "type": "string"
                     }
                 },
                 "required": [
                     "authomizeId",
                     "name",
@@ -676,24 +676,24 @@
                 "properties": {
                     "appId": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/AppIdFilter"
                             }
                         ],
-                        "description": "ID of the Application.",
+                        "description": "Find assets by their app ID",
                         "title": "Appid"
                     },
                     "authomizeId": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/AssetIdFilter"
                             }
                         ],
-                        "description": "Authomize ID for the Asset",
+                        "description": "Find assets by their Authomize ID",
                         "title": "Authomizeid"
                     },
                     "originId": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/OriginIdFilter"
                             }
@@ -703,15 +703,15 @@
                     },
                     "uniqueId": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/UniqueIdFilter"
                             }
                         ],
-                        "description": "Unique ID of the Asset.",
+                        "description": "Find assets by their unique ID",
                         "title": "Uniqueid"
                     }
                 },
                 "title": "Chainable",
                 "type": "object"
             },
             "CisV8Standard": {
@@ -863,75 +863,75 @@
                 "title": "IdentityExpansion",
                 "type": "string"
             },
             "IdentitySchema": {
                 "properties": {
                     "accountIds": {
                         "default": [],
-                        "description": "List of associated account IDs",
+                        "description": "The account IDs associated with the identity",
                         "items": {
                             "type": "string"
                         },
                         "title": "Accountids",
                         "type": "array"
                     },
                     "accounts": {
                         "default": [],
-                        "description": "List of associated accounts",
+                        "description": "List of associated user or service accounts",
                         "items": {
                             "$ref": "#/components/schemas/AccountSchema"
                         },
                         "title": "Accounts",
                         "type": "array"
                     },
                     "authomizeId": {
                         "description": "Unique ID",
                         "title": "Authomizeid",
                         "type": "string"
                     },
                     "department": {
-                        "description": "Department",
+                        "description": "The department in which the identity works",
                         "title": "Department",
                         "type": "string"
                     },
                     "email": {
-                        "description": "User's work email address.\n",
+                        "description": "The email of the identity",
                         "title": "Email",
                         "type": "string"
                     },
                     "hiredAt": {
                         "description": "Hired At",
                         "title": "Hiredat",
                         "type": "string"
                     },
                     "incidentsCount": {
                         "description": "Number of associated incidents",
                         "title": "Incidentscount",
                         "type": "integer"
                     },
                     "name": {
-                        "description": "Name of Identity",
+                        "description": "Name of the identity",
                         "title": "Name",
                         "type": "string"
                     },
                     "tags": {
-                        "description": "Expanded Tags",
+                        "description": "The tags provided for the identity",
                         "items": {
                             "$ref": "#/components/schemas/TagSchema"
                         },
                         "title": "Tags",
                         "type": "array"
                     },
                     "terminatedAt": {
                         "description": "Time of termination",
                         "title": "Terminatedat",
                         "type": "string"
                     },
                     "title": {
-                        "description": "Title",
+                        "description": "Title of the identity",
                         "title": "Title",
                         "type": "string"
                     }
                 },
                 "required": [
                     "authomizeId"
                 ],
@@ -1372,15 +1372,15 @@
                     },
                     "tenant": {
                         "description": "**tenant**",
                         "title": "Tenant",
                         "type": "string"
                     },
                     "version": {
-                        "default": "4.1.2",
+                        "default": "4.1.3",
                         "description": "**version**",
                         "title": "Version",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
@@ -1617,43 +1617,43 @@
                 "type": "object"
             },
             "PaginationRequestSchema": {
                 "additionalProperties": false,
                 "description": "Base schema for all incoming API requests.",
                 "properties": {
                     "limit": {
-                        "description": "Limit",
+                        "description": "Limit the number of identities per page",
                         "title": "Limit",
                         "type": "integer"
                     },
                     "nextPage": {
-                        "description": "Starting after",
+                        "description": "Token denoting start of next page",
                         "title": "NextPage",
                         "type": "string"
                     }
                 },
                 "title": "PaginationRequestSchema",
                 "type": "object"
             },
             "PaginationResponseSchema": {
                 "description": "Common pagination model that has been used across services.",
                 "properties": {
                     "hasMore": {
-                        "description": "Has more? `true` or `false`.",
+                        "description": "Indicates that more data is available",
                         "title": "HasMore",
                         "type": "boolean"
                     },
                     "limit": {
                         "default": 20,
-                        "description": "Limit",
+                        "description": "Limit the number of identities per page",
                         "title": "Limit",
                         "type": "integer"
                     },
                     "nextPage": {
-                        "description": "Starting after",
+                        "description": "Token denoting start of next page",
                         "title": "NextPage",
                         "type": "string"
                     }
                 },
                 "title": "PaginationResponseSchema",
                 "type": "object"
             },
@@ -1691,66 +1691,66 @@
                 "title": "PolicySchema",
                 "type": "object"
             },
             "RawIdentitySchema": {
                 "properties": {
                     "accountIds": {
                         "default": [],
-                        "description": "List of associated account IDs",
+                        "description": "The account IDs associated with the identity",
                         "items": {
                             "type": "string"
                         },
                         "title": "Accountids",
                         "type": "array"
                     },
                     "authomizeId": {
                         "description": "Unique ID",
                         "title": "Authomizeid",
                         "type": "string"
                     },
                     "department": {
-                        "description": "Department",
+                        "description": "The department in which the identity works",
                         "title": "Department",
                         "type": "string"
                     },
                     "email": {
-                        "description": "User's work email address.\n",
+                        "description": "The email of the identity",
                         "title": "Email",
                         "type": "string"
                     },
                     "hiredAt": {
                         "description": "Hired At",
                         "title": "Hiredat",
                         "type": "string"
                     },
                     "incidentsCount": {
                         "description": "Number of associated incidents",
                         "title": "Incidentscount",
                         "type": "integer"
                     },
                     "name": {
-                        "description": "Name of Identity",
+                        "description": "Name of the identity",
                         "title": "Name",
                         "type": "string"
                     },
                     "tags": {
-                        "description": "Expanded Tags",
+                        "description": "The tags provided for the identity",
                         "items": {
                             "$ref": "#/components/schemas/TagSchema"
                         },
                         "title": "Tags",
                         "type": "array"
                     },
                     "terminatedAt": {
                         "description": "Time of termination",
                         "title": "Terminatedat",
                         "type": "string"
                     },
                     "title": {
-                        "description": "Title",
+                        "description": "Title of the identity",
                         "title": "Title",
                         "type": "string"
                     }
                 },
                 "required": [
                     "authomizeId"
                 ],
@@ -1839,40 +1839,40 @@
                 "type": "object"
             },
             "SearchAssetsRequestSchema": {
                 "additionalProperties": false,
                 "description": "Base schema for all incoming API requests.",
                 "properties": {
                     "expand": {
-                        "description": "Expand Fields",
+                        "description": "Expand fields (to show additional information)",
                         "items": {
                             "$ref": "#/components/schemas/AssetExpansion"
                         },
                         "type": "array"
                     },
                     "filter": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/Chainable"
                             }
                         ],
-                        "description": "Search Assets Filter",
+                        "description": "Find assets by their ID on the source system",
                         "title": "Filter"
                     },
                     "pagination": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/PaginationRequestSchema"
                             }
                         ],
-                        "description": "Pagination",
+                        "description": "Pagination metadata",
                         "title": "Pagination"
                     },
                     "sort": {
-                        "description": "Sort",
+                        "description": "Sort the results by identity name in ascending or descending order",
                         "items": {
                             "$ref": "#/components/schemas/SortSchema_SearchAssetsSortFields_"
                         },
                         "title": "Sort",
                         "type": "array"
                     }
                 },
@@ -1909,15 +1909,15 @@
                     },
                     "pagination": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/PaginationRequestSchema"
                             }
                         ],
-                        "description": "Pagination",
+                        "description": "Pagination metadata",
                         "title": "Pagination"
                     }
                 },
                 "title": "SearchCampaignPermissionsRequestSchema",
                 "type": "object"
             },
             "SearchCampaignsRequestSchema": {
@@ -1942,19 +1942,19 @@
                     },
                     "pagination": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/PaginationRequestSchema"
                             }
                         ],
-                        "description": "Pagination",
+                        "description": "Pagination metadata",
                         "title": "Pagination"
                     },
                     "sort": {
-                        "description": "Sort",
+                        "description": "Sort the results by identity name in ascending or descending order",
                         "items": {
                             "$ref": "#/components/schemas/SortSchema_FieldName_"
                         },
                         "title": "Sort",
                         "type": "array"
                     }
                 },
@@ -1967,61 +1967,61 @@
                 "properties": {
                     "authomizeId": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/IdFilter"
                             }
                         ],
-                        "description": "Authomize ID for the Identity",
+                        "description": "Find identities by their Authomize ID",
                         "title": "Authomizeid"
                     },
                     "email": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/EmailFilter"
                             }
                         ],
-                        "description": "Email.",
+                        "description": "Find identities by their email address",
                         "title": "Email"
                     }
                 },
                 "title": "SearchIdentitiesFilterBody",
                 "type": "object"
             },
             "SearchIdentitiesRequestSchema": {
                 "additionalProperties": false,
                 "description": "Base schema for all incoming API requests.",
                 "properties": {
                     "expand": {
-                        "description": "Expand Fields",
+                        "description": "Expand the account or tag fields to get additional data on related accounts or related tags",
                         "items": {
                             "$ref": "#/components/schemas/IdentityExpansion"
                         },
                         "type": "array"
                     },
                     "filter": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/SearchIdentitiesFilterBody"
                             }
                         ],
-                        "description": "Search Identities Filter",
+                        "description": "Search filter options",
                         "title": "Filter"
                     },
                     "pagination": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/PaginationRequestSchema"
                             }
                         ],
-                        "description": "Pagination",
+                        "description": "Pagination metadata",
                         "title": "Pagination"
                     },
                     "sort": {
-                        "description": "Sort",
+                        "description": "Sort the results by identity name in ascending or descending order",
                         "items": {
                             "$ref": "#/components/schemas/SortSchema_SearchIdentitiesSortFields_"
                         },
                         "title": "Sort",
                         "type": "array"
                     }
                 },
@@ -2129,19 +2129,19 @@
                     },
                     "pagination": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/PaginationRequestSchema"
                             }
                         ],
-                        "description": "Pagination",
+                        "description": "Pagination metadata",
                         "title": "Pagination"
                     },
                     "sort": {
-                        "description": "Sort",
+                        "description": "Sort the results by identity name in ascending or descending order",
                         "items": {
                             "$ref": "#/components/schemas/SortSchema_SearchIncidentsSortFields_"
                         },
                         "title": "Sort",
                         "type": "array"
                     }
                 },
@@ -2193,25 +2193,25 @@
                 "properties": {
                     "fieldName": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/FieldName"
                             }
                         ],
-                        "description": "Sort By Field Name",
+                        "description": "Sort the results by field name",
                         "title": "FieldName"
                     },
                     "order": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/SortOrder"
                             }
                         ],
                         "default": "ASC",
-                        "description": "Sort Order",
+                        "description": "Sort by ascending or descending order (ascending is the default)",
                         "title": "Order"
                     }
                 },
                 "required": [
                     "fieldName"
                 ],
                 "title": "SortSchema[FieldName]",
@@ -2222,25 +2222,25 @@
                 "properties": {
                     "fieldName": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/SearchAssetsSortFields"
                             }
                         ],
-                        "description": "Sort By Field Name",
+                        "description": "Sort the results by field name",
                         "title": "FieldName"
                     },
                     "order": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/SortOrder"
                             }
                         ],
                         "default": "ASC",
-                        "description": "Sort Order",
+                        "description": "Sort by ascending or descending order (ascending is the default)",
                         "title": "Order"
                     }
                 },
                 "required": [
                     "fieldName"
                 ],
                 "title": "SortSchema[SearchAssetsSortFields]",
@@ -2251,25 +2251,25 @@
                 "properties": {
                     "fieldName": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/SearchIdentitiesSortFields"
                             }
                         ],
-                        "description": "Sort By Field Name",
+                        "description": "Sort the results by field name",
                         "title": "FieldName"
                     },
                     "order": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/SortOrder"
                             }
                         ],
                         "default": "ASC",
-                        "description": "Sort Order",
+                        "description": "Sort by ascending or descending order (ascending is the default)",
                         "title": "Order"
                     }
                 },
                 "required": [
                     "fieldName"
                 ],
                 "title": "SortSchema[SearchIdentitiesSortFields]",
@@ -2280,43 +2280,43 @@
                 "properties": {
                     "fieldName": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/SearchIncidentsSortFields"
                             }
                         ],
-                        "description": "Sort By Field Name",
+                        "description": "Sort the results by field name",
                         "title": "FieldName"
                     },
                     "order": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/SortOrder"
                             }
                         ],
                         "default": "ASC",
-                        "description": "Sort Order",
+                        "description": "Sort by ascending or descending order (ascending is the default)",
                         "title": "Order"
                     }
                 },
                 "required": [
                     "fieldName"
                 ],
                 "title": "SortSchema[SearchIncidentsSortFields]",
                 "type": "object"
             },
             "SourceAppSchema": {
                 "properties": {
                     "id": {
-                        "description": "Unique ID",
+                        "description": "Authomize ID of source application",
                         "title": "Id",
                         "type": "string"
                     },
                     "name": {
-                        "description": "Name",
+                        "description": "Name of the asset (for example, application, virtual machine, file, etc.)",
                         "title": "Name",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
                     "name"
@@ -2461,15 +2461,15 @@
                 "type": "apiKey"
             }
         }
     },
     "info": {
         "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "4.1.2",
+        "version": "4.1.3",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
@@ -3030,15 +3030,15 @@
                 "tags": [
                     "Incident"
                 ]
             }
         },
         "/v2/inventory/assets/search": {
             "post": {
-                "description": "Search Assets",
+                "description": "Find specific assets on Authomize and get related data (as found on the asset\u2019s Single Entity page)",
                 "operationId": "search_assets_v2_inventory_assets_search_post",
                 "requestBody": {
                     "content": {
                         "application/json": {
                             "schema": {
                                 "$ref": "#/components/schemas/SearchAssetsRequestSchema"
                             }
@@ -3077,15 +3077,15 @@
                 "tags": [
                     "Inventory"
                 ]
             }
         },
         "/v2/inventory/identities/search": {
             "post": {
-                "description": "Search Identities",
+                "description": "Find specific identities on Authomize and get related data (as found on Identity Single Entity page). Search by email address or AuthomizeID.",
                 "operationId": "search_identities_v2_inventory_identities_search_post",
                 "requestBody": {
                     "content": {
                         "application/json": {
                             "schema": {
                                 "$ref": "#/components/schemas/SearchIdentitiesRequestSchema"
                             }
@@ -3137,12 +3137,12 @@
             "name": "Incident"
         },
         {
             "description": "Campaign APIs enable you to pull all the decisions from the campaign (keep or revoke) and to automate the revocation process to remove unnecessary permissions.\nCampaign APIs also enable you to pull basic details on the campaigns and to pull a list of all campaigns.\n",
             "name": "Campaign"
         },
         {
-            "description": "Inventory APIs",
+            "description": "Inventory APIs can be used to find identities and assets",
             "name": "Inventory"
         }
     ]
 }
```

### Comparing `authomize-rest-api-client-4.1.3/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-4.1.4/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.3/setup.py` & `authomize-rest-api-client-4.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='4.1.3',
+        version='4.1.4',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

