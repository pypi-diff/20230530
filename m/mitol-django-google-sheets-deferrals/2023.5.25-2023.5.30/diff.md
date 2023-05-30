# Comparing `tmp/mitol-django-google-sheets-deferrals-2023.5.25.tar.gz` & `tmp/mitol-django-google-sheets-deferrals-2023.5.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitol-django-google-sheets-deferrals-2023.5.25.tar", last modified: Thu May 25 10:53:11 2023, max compression
+gzip compressed data, was "mitol-django-google-sheets-deferrals-2023.5.30.tar", last modified: Tue May 30 13:53:51 2023, max compression
```

## Comparing `mitol-django-google-sheets-deferrals-2023.5.25.tar` & `mitol-django-google-sheets-deferrals-2023.5.30.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:11.146418 mitol-django-google-sheets-deferrals-2023.5.25/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4652 2023-05-25 10:53:11.146418 mitol-django-google-sheets-deferrals-2023.5.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:11.146418 mitol-django-google-sheets-deferrals-2023.5.25/mitol/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:11.146418 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     4105 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4958 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      511 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      276 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:11.142418 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/management/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:11.146418 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/management/commands/process_deferral_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:11.146418 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/models.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:11.146418 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/settings/
--rw-r--r--   0 runner    (1001) docker     (122)     1942 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/settings/google_sheets_deferrals.py
--rw-r--r--   0 runner    (1001) docker     (122)     4433 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:11.146418 mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4652 2023-05-25 10:53:11.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-05-25 10:53:11.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 10:53:11.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-25 10:53:11.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-25 10:53:11.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-25 10:53:11.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 10:53:11.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 10:53:11.146418 mitol-django-google-sheets-deferrals-2023.5.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5673 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:51.293285 mitol-django-google-sheets-deferrals-2023.5.30/
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4652 2023-05-30 13:53:51.293285 mitol-django-google-sheets-deferrals-2023.5.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:51.289285 mitol-django-google-sheets-deferrals-2023.5.30/mitol/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:51.289285 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/
+-rw-r--r--   0 runner    (1001) docker     (122)      882 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     4105 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6038 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:51.289285 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/management/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:51.293285 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/management/commands/process_deferral_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:51.293285 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:51.293285 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)     1942 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/settings/google_sheets_deferrals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4433 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:53:51.293285 mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4652 2023-05-30 13:53:51.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-05-30 13:53:51.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 13:53:51.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-30 13:53:51.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-30 13:53:51.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-30 13:53:51.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 13:53:51.000000 mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-30 13:53:51.293285 mitol-django-google-sheets-deferrals-2023.5.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5673 2023-05-30 13:53:50.000000 mitol-django-google-sheets-deferrals-2023.5.30/setup.py
```

### Comparing `mitol-django-google-sheets-deferrals-2023.5.25/PKG-INFO` & `mitol-django-google-sheets-deferrals-2023.5.30/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitol-django-google-sheets-deferrals
-Version: 2023.5.25
+Version: 2023.5.30
 Summary: Library to handle Deferral requests using Google Sheets integrations in Django
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mitol-django-google-sheets-deferrals-2023.5.25/backend_shim.py` & `mitol-django-google-sheets-deferrals-2023.5.30/backend_shim.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/CHANGELOG.md` & `mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/CHANGELOG.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,23 @@
 
+<a id='changelog-2023.5.30'></a>
+## [2023.5.30] - 2023-05-30
+
+### Added
+
+- Added the `mitol-django-google-sheets-deferrals` app
+
+- Added implementation of filter_ignored_rows to request handler
+
+### Changed
+
+- Updated release version format
+
+- Set default_auto_field in app config
+
 <a id='changelog-2023.5.25'></a>
 ## [2023.5.25] - 2023-05-25
 
 ### Added
 
 - Added the `mitol-django-google-sheets-deferrals` app
```

### Comparing `mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/README.md` & `mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/README.md`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/api.py` & `mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Enrollment deferral API"""
 import logging
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
 
+from mitol.common.utils.collections import item_at_index_or_none
 from mitol.common.utils.config import get_missing_settings
 from mitol.common.utils.datetime import now_in_utc
+from mitol.google_sheets.constants import GOOGLE_API_TRUE_VAL
 from mitol.google_sheets.exceptions import SheetRowParsingException
 from mitol.google_sheets.sheet_handler_api import GoogleSheetsChangeRequestHandler
 from mitol.google_sheets.utils import ResultType, RowResult
 from mitol.google_sheets_deferrals.constants import (
     REQUIRED_GOOGLE_SHEETS_DEFERRALS_SETTINGS,
 )
 from mitol.google_sheets_deferrals.hooks import get_plugin_manager
@@ -130,7 +132,29 @@
         return RowResult(
             row_index=row_index,
             row_db_record=deferral_request,
             row_object=deferral_req_row,
             result_type=result_type,
             message=message,
         )
+
+    def filter_ignored_rows(self, enumerated_rows):
+        """
+        Takes an iterable of enumerated rows, and returns an iterable of those rows without the ones that should be
+        ignored. The row is ignored if Deferral Complete Date is entered or Ignore? column has TRUE
+
+        Args:
+            enumerated_rows (Iterable[Tuple[int, List[str]]]): Row indices paired with a list of strings
+                representing the data in each row
+
+        Returns:
+            Iterable[Tuple[int, List[str]]]: Iterable of data rows without the ones that should be ignored.
+        """
+        for row_index, row_data in enumerated_rows:
+            if item_at_index_or_none(
+                row_data, self.sheet_metadata.SKIP_ROW_COL
+            ).strip() == GOOGLE_API_TRUE_VAL or item_at_index_or_none(
+                row_data, self.sheet_metadata.COMPLETED_DATE_COL
+            ):
+                continue
+
+            yield row_index, row_data
```

### Comparing `mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/hooks.py` & `mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/hooks.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/management/commands/process_deferral_requests.py` & `mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/management/commands/process_deferral_requests.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/migrations/0001_initial.py` & `mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/settings/google_sheets_deferrals.py` & `mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/settings/google_sheets_deferrals.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/utils.py` & `mitol-django-google-sheets-deferrals-2023.5.30/mitol/google_sheets_deferrals/utils.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/PKG-INFO` & `mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitol-django-google-sheets-deferrals
-Version: 2023.5.25
+Version: 2023.5.30
 Summary: Library to handle Deferral requests using Google Sheets integrations in Django
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/SOURCES.txt` & `mitol-django-google-sheets-deferrals-2023.5.30/mitol_django_google_sheets_deferrals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.25/setup.py` & `mitol-django-google-sheets-deferrals-2023.5.30/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,10 +152,10 @@
         'mitol',
         'mitol.google_sheets_deferrals',
         'mitol.google_sheets_deferrals.management.commands',
         'mitol.google_sheets_deferrals.migrations',
         'mitol.google_sheets_deferrals.settings',
     ),
     'python_requires': '>=3.8',
-    'version': '2023.5.25',
+    'version': '2023.5.30',
     'zip_safe': True,
 })
```

