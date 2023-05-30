# Comparing `tmp/ds_caselaw_marklogic_api_client-7.0.0.tar.gz` & `tmp/ds_caselaw_marklogic_api_client-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds_caselaw_marklogic_api_client-7.0.0.tar", max compression
+gzip compressed data, was "ds_caselaw_marklogic_api_client-8.0.0.tar", max compression
```

## Comparing `ds_caselaw_marklogic_api_client-7.0.0.tar` & `ds_caselaw_marklogic_api_client-8.0.0.tar`

### file list

```diff
@@ -1,47 +1,52 @@
--rw-r--r--   0        0        0     1108 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/LICENSE.md
--rw-r--r--   0        0        0     3128 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/README.md
--rw-r--r--   0        0        0      926 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/pyproject.toml
--rw-r--r--   0        0        0    28845 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/Client.py
--rw-r--r--   0        0        0        0 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/__init__.py
--rw-r--r--   0        0        0     2236 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/content_hash.py
--rw-r--r--   0        0        0     2526 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/errors.py
--rw-r--r--   0        0        0        0 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/models/__init__.py
--rw-r--r--   0        0        0     6376 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/models/judgments.py
--rw-r--r--   0        0        0     1341 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/models/utilities/__init__.py
--rw-r--r--   0        0        0     4098 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/models/utilities/aws.py
--rw-r--r--   0        0        0        0 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/py.typed
--rw-r--r--   0        0        0     3821 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xml_tools.py
--rw-r--r--   0        0        0      220 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/break_judgment_checkout.xqy
--rw-r--r--   0        0        0      197 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/checkin_judgment.xqy
--rw-r--r--   0        0        0      385 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/checkout_judgment.xqy
--rw-r--r--   0        0        0      318 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/copy_judgment.xqy
--rw-r--r--   0        0        0      302 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/delete_judgment.xqy
--rw-r--r--   0        0        0      715 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_judgment.xqy
--rw-r--r--   0        0        0      193 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_judgment_checkout_status.xqy
--rw-r--r--   0        0        0      292 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_judgment_version.xqy
--rw-r--r--   0        0        0      172 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_last_modified.xqy
--rw-r--r--   0        0        0      338 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_metadata_citation.xqy
--rw-r--r--   0        0        0      339 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_metadata_court.xqy
--rw-r--r--   0        0        0      221 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_metadata_name.xqy
--rw-r--r--   0        0        0      358 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_metadata_work_date.xqy
--rw-r--r--   0        0        0      594 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_properties_for_search_results.xqy
--rw-r--r--   0        0        0      209 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_property.xqy
--rw-r--r--   0        0        0      326 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/insert_judgment.xqy
--rw-r--r--   0        0        0       95 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/judgment_exists.xqy
--rw-r--r--   0        0        0      190 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/list_judgment_versions.xqy
--rw-r--r--   0        0        0      355 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_boolean_property.xqy
--rw-r--r--   0        0        0      659 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_citation.xqy
--rw-r--r--   0        0        0     1013 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_court.xqy
--rw-r--r--   0        0        0      756 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_name.xqy
--rw-r--r--   0        0        0     1762 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_this_uri.xqy
--rw-r--r--   0        0        0      939 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_work_expression_date.xqy
--rw-r--r--   0        0        0      343 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_property.xqy
--rw-r--r--   0        0        0      420 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/update_judgment.xqy
--rw-r--r--   0        0        0      556 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/update_locked_judgment.xqy
--rw-r--r--   0        0        0      371 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/user_has_privilege.xqy
--rw-r--r--   0        0        0      246 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/user_has_role.xqy
--rw-r--r--   0        0        0      156 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/validate_all_documents.xqy
--rw-r--r--   0        0        0      199 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/xslt.xqy
--rw-r--r--   0        0        0     1381 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/xslt_transform.xqy
--rw-r--r--   0        0        0     3536 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery_type_dicts.py
--rw-r--r--   0        0        0     4182 1970-01-01 00:00:00.000000 ds_caselaw_marklogic_api_client-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/LICENSE.md
+-rw-r--r--   0        0        0     3128 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/README.md
+-rw-r--r--   0        0        0      937 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/pyproject.toml
+-rw-r--r--   0        0        0    27558 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/Client.py
+-rw-r--r--   0        0        0        0 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/__init__.py
+-rw-r--r--   0        0        0     2236 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/content_hash.py
+-rw-r--r--   0        0        0     2526 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/errors.py
+-rw-r--r--   0        0        0        0 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/models/__init__.py
+-rw-r--r--   0        0        0     6376 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/models/judgments.py
+-rw-r--r--   0        0        0     1341 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/models/utilities/__init__.py
+-rw-r--r--   0        0        0     4098 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/models/utilities/aws.py
+-rw-r--r--   0        0        0        0 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/py.typed
+-rw-r--r--   0        0        0        0 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/responses/__init__.py
+-rw-r--r--   0        0        0     1697 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/responses/search_response.py
+-rw-r--r--   0        0        0     6999 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/responses/search_result.py
+-rw-r--r--   0        0        0      918 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/responses/xsl/search_match.xsl
+-rw-r--r--   0        0        0     3001 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/search_parameters.py
+-rw-r--r--   0        0        0     3821 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xml_tools.py
+-rw-r--r--   0        0        0      220 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/break_judgment_checkout.xqy
+-rw-r--r--   0        0        0      197 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/checkin_judgment.xqy
+-rw-r--r--   0        0        0      385 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/checkout_judgment.xqy
+-rw-r--r--   0        0        0      318 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/copy_judgment.xqy
+-rw-r--r--   0        0        0      302 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/delete_judgment.xqy
+-rw-r--r--   0        0        0      715 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_judgment.xqy
+-rw-r--r--   0        0        0      193 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_judgment_checkout_status.xqy
+-rw-r--r--   0        0        0      292 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_judgment_version.xqy
+-rw-r--r--   0        0        0      172 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_last_modified.xqy
+-rw-r--r--   0        0        0      338 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_metadata_citation.xqy
+-rw-r--r--   0        0        0      339 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_metadata_court.xqy
+-rw-r--r--   0        0        0      221 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_metadata_name.xqy
+-rw-r--r--   0        0        0      358 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_metadata_work_date.xqy
+-rw-r--r--   0        0        0      594 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_properties_for_search_results.xqy
+-rw-r--r--   0        0        0      209 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_property.xqy
+-rw-r--r--   0        0        0      326 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/insert_judgment.xqy
+-rw-r--r--   0        0        0       95 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/judgment_exists.xqy
+-rw-r--r--   0        0        0      190 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/list_judgment_versions.xqy
+-rw-r--r--   0        0        0      355 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_boolean_property.xqy
+-rw-r--r--   0        0        0      659 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_citation.xqy
+-rw-r--r--   0        0        0     1013 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_court.xqy
+-rw-r--r--   0        0        0      756 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_name.xqy
+-rw-r--r--   0        0        0     1762 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_this_uri.xqy
+-rw-r--r--   0        0        0      939 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_work_expression_date.xqy
+-rw-r--r--   0        0        0      343 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_property.xqy
+-rw-r--r--   0        0        0      420 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/update_judgment.xqy
+-rw-r--r--   0        0        0      556 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/update_locked_judgment.xqy
+-rw-r--r--   0        0        0      371 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/user_has_privilege.xqy
+-rw-r--r--   0        0        0      246 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/user_has_role.xqy
+-rw-r--r--   0        0        0      156 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/validate_all_documents.xqy
+-rw-r--r--   0        0        0      199 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/xslt.xqy
+-rw-r--r--   0        0        0     1381 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/xslt_transform.xqy
+-rw-r--r--   0        0        0     3536 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery_type_dicts.py
+-rw-r--r--   0        0        0     4182 1970-01-01 00:00:00.000000 ds_caselaw_marklogic_api_client-8.0.0/PKG-INFO
```

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/LICENSE.md` & `ds_caselaw_marklogic_api_client-8.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/README.md` & `ds_caselaw_marklogic_api_client-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/pyproject.toml` & `ds_caselaw_marklogic_api_client-8.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "ds-caselaw-marklogic-api-client"
-version = "7.0.0"
+version = "8.0.0"
 description = "An API client for interacting with the underlying data in Find Caselaw."
 authors = ["The National Archives"]
 homepage = "https://github.com/nationalarchives/ds-caselaw-custom-api-client"
 keywords = ["national archives", "caselaw"]
 readme = "README.md"
 packages = [
     { include = "caselawclient", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-certifi = "^2022.12.7"
+certifi = ">=2022.12.7,<2024.0.0"
 charset-normalizer = "^2.1.1"
 django-environ = "^0.10.0"
 idna = "^3.4"
 requests = "^2.28.2"
 requests-toolbelt = ">=0.10.1,<1.1.0"
 urllib3 = "^1.26.15"
 memoization = "^0.4.0"
```

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/Client.py` & `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/Client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import json
 import logging
 import os
 import re
 import warnings
 from datetime import datetime, time, timedelta
 from pathlib import Path
-from typing import Any, Optional, Set, Type, Union
+from typing import Any, Optional, Type, Union
 from xml.etree import ElementTree
 from xml.etree.ElementTree import Element
 
 import environ
 import requests
 from requests.auth import HTTPBasicAuth
 from requests.structures import CaseInsensitiveDict
 from requests_toolbelt.multipart import decoder
 
+from caselawclient.search_parameters import SearchParameters
+
 from . import xml_tools
 from . import xquery_type_dicts as query_dicts
 from .content_hash import validate_content_hash
 from .errors import MarklogicAPIError  # noqa: F401
 from .errors import (
     MarklogicBadRequestError,
     MarklogicCheckoutConflictError,
@@ -29,15 +31,14 @@
     MarklogicResourceNotFoundError,
     MarklogicResourceUnmanagedError,
     MarklogicUnauthorizedError,
     MarklogicValidationFailedError,
 )
 
 env = environ.Env()
-RESULTS_PER_PAGE = 10
 ROOT_DIR = os.path.dirname(os.path.realpath(__file__))
 DEFAULT_XSL_TRANSFORM = "accessible-html.xsl"
 
 
 def decode_multipart(response: requests.Response) -> str:
     """Decode a multipart response and return just the text inside it.
     Note that it is possible for multiple responses to be returned, if
@@ -53,14 +54,17 @@
     if part_count > 1:
         logging.warning(
             f"Throwing away multipart data ({part_count} items, expected 1)"
         )
     return str(multipart_data.parts[0].text)
 
 
+JUDGMENT_COLLECTION_URI = "judgment"
+
+
 class MarklogicApiClient:
     http_error_classes: dict[int, Type[MarklogicAPIError]] = {
         400: MarklogicBadRequestError,
         401: MarklogicUnauthorizedError,
         403: MarklogicNotPermittedError,
         404: MarklogicResourceNotFoundError,
     }
@@ -96,33 +100,14 @@
                 return error
         print(f"No error code match found for {error_code}")
         return self.default_http_error_class
 
     def _path_to_request_url(self, path: str) -> str:
         return f"{self.base_url}/{path.lstrip('/')}"
 
-    def _court_list_splitter(self, court_text: str) -> Set[str]:
-        return set(court_text.lower().replace(" ", "").split(","))
-
-    def _court_list(self, court_text: str) -> Optional[list[str]]:
-        if not court_text.strip():
-            return None
-        alt_names = {
-            "ewhc/qb": "ewhc/kb",
-            "ewhc/kb": "ewhc/qb",
-            "ewhc/scco": "ewhc/costs",
-            "ewhc/costs": "ewhc/scco",
-        }
-        new_names = set()
-        courts = self._court_list_splitter(court_text)
-        for primary_name, secondary_name in alt_names.items():
-            if primary_name in courts and secondary_name not in courts:
-                new_names.add(secondary_name)
-        return list(courts | new_names)
-
     def _raise_for_status(self, response: requests.Response) -> None:
         try:
             response.raise_for_status()
         except requests.exceptions.HTTPError as e:
             status_code = e.response.status_code
             new_error_class = self.http_error_classes.get(
                 status_code, self.default_http_error_class
@@ -444,30 +429,15 @@
         response = self.session.request(
             "POST", url=self._path_to_request_url(path), headers=headers, data=data
         )
         # Raise relevant exception for an erroneous response
         self._raise_for_status(response)
         return response
 
-    def advanced_search(
-        self,
-        q: Optional[str] = None,
-        court: Optional[str] = None,
-        judge: Optional[str] = None,
-        party: Optional[str] = None,
-        neutral_citation: Optional[str] = None,
-        specific_keyword: Optional[str] = None,
-        order: Optional[str] = None,
-        date_from: Optional[str] = None,
-        date_to: Optional[str] = None,
-        page: int = 1,
-        page_size: int = RESULTS_PER_PAGE,
-        show_unpublished: bool = False,
-        only_unpublished: bool = False,
-    ) -> requests.Response:
+    def advanced_search(self, search_parameters: SearchParameters) -> requests.Response:
         """
         Performs a search on the entire document set.
 
         :param q:
         :param court:
         :param judge:
         :param party:
@@ -476,35 +446,22 @@
         :param order:
         :param date_from:
         :param date_to:
         :param page:
         :param page_size:
         :param show_unpublished: If True, both published and unpublished documents will be returned
         :param only_unpublished: If True, will only return published documents. Ignores the value of show_unpublished
+        :param collections:
         :return:
         """
         module = "/judgments/search/search-v2.xqy"  # as stored on Marklogic
-        show_unpublished = self.verify_show_unpublished(show_unpublished)
-        vars = json.dumps(
-            {
-                "court": self._court_list(court or ""),
-                "judge": str(judge or ""),
-                "page": max(1, int(page)),
-                "page-size": int(page_size),
-                "q": str(q or ""),
-                "party": str(party or ""),
-                "neutral_citation": str(neutral_citation or ""),
-                "specific_keyword": str(specific_keyword or ""),
-                "order": str(order or ""),
-                "from": str(date_from or ""),
-                "to": str(date_to or ""),
-                "show_unpublished": str(show_unpublished).lower(),
-                "only_unpublished": str(only_unpublished).lower(),
-            }
+        search_parameters.show_unpublished = self.verify_show_unpublished(
+            search_parameters.show_unpublished
         )
+        vars = json.dumps(search_parameters.as_marklogic_payload())
         return self.invoke(module, vars)
 
     def eval_xslt(
         self,
         judgment_uri: str,
         version_uri: Optional[str] = None,
         show_unpublished: bool = False,
@@ -744,14 +701,24 @@
             self._format_uri_for_marklogic(judgment_uri)
             for judgment_uri in judgment_uris
         ]
         vars: query_dicts.GetPropertiesForSearchResultsDict = {"uris": uris}
         response = self._send_to_eval(vars, "get_properties_for_search_results.xqy")
         return decode_multipart(response)
 
+    def search_and_decode_response(self, search_parameters: SearchParameters) -> str:
+        response = self.advanced_search(search_parameters)
+        return decode_multipart(response)
+
+    def search_judgments_and_decode_response(
+        self, search_parameters: SearchParameters
+    ) -> str:
+        search_parameters.collections = [JUDGMENT_COLLECTION_URI]
+        return self.search_and_decode_response(search_parameters)
+
 
 api_client = MarklogicApiClient(
     host=env("MARKLOGIC_HOST", default=None),
     username=env("MARKLOGIC_USER", default=None),
     password=env("MARKLOGIC_PASSWORD", default=None),
     use_https=env("MARKLOGIC_USE_HTTPS", default=False),
 )
```

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/content_hash.py` & `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/content_hash.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/errors.py` & `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/errors.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/models/judgments.py` & `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/models/judgments.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/models/utilities/__init__.py` & `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/models/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/models/utilities/aws.py` & `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/models/utilities/aws.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xml_tools.py` & `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xml_tools.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_judgment.xqy` & `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_judgment.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_properties_for_search_results.xqy` & `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_properties_for_search_results.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_citation.xqy` & `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_citation.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_court.xqy` & `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_court.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_name.xqy` & `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_name.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_this_uri.xqy` & `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_this_uri.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_work_expression_date.xqy` & `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_work_expression_date.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/update_locked_judgment.xqy` & `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/update_locked_judgment.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/xslt_transform.xqy` & `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/xslt_transform.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery_type_dicts.py` & `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery_type_dicts.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-7.0.0/PKG-INFO` & `ds_caselaw_marklogic_api_client-8.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ds-caselaw-marklogic-api-client
-Version: 7.0.0
+Version: 8.0.0
 Summary: An API client for interacting with the underlying data in Find Caselaw.
 Home-page: https://github.com/nationalarchives/ds-caselaw-custom-api-client
 Keywords: national archives,caselaw
 Author: The National Archives
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.112,<2.0.0)
-Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
+Requires-Dist: certifi (>=2022.12.7,<2024.0.0)
 Requires-Dist: charset-normalizer (>=2.1.1,<3.0.0)
 Requires-Dist: django-environ (>=0.10.0,<0.11.0)
 Requires-Dist: ds-caselaw-utils (>=1.0.0,<2.0.0)
 Requires-Dist: idna (>=3.4,<4.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: memoization (>=0.4.0,<0.5.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
```

