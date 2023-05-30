# Comparing `tmp/openedx-ledger-0.4.1.tar.gz` & `tmp/openedx-ledger-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-ledger-0.4.1.tar", last modified: Wed May 24 15:52:21 2023, max compression
+gzip compressed data, was "openedx-ledger-1.0.0.tar", last modified: Tue May 30 20:48:33 2023, max compression
```

## Comparing `openedx-ledger-0.4.1.tar` & `openedx-ledger-1.0.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.979185 openedx-ledger-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8581 2023-05-24 15:52:21.979185 openedx-ledger-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.975185 openedx-ledger-0.4.1/openedx_ledger/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3884 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5394 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.975185 openedx-ledger-0.4.1/openedx_ledger/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     6005 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py
--rw-r--r--   0 runner    (1001) docker     (122)     4294 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/migrations/0003_field_updates_20230216_1605.py
--rw-r--r--   0 runner    (1001) docker     (122)      638 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py
--rw-r--r--   0 runner    (1001) docker     (122)    12708 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/migrations/0005_help_text_and_more_indices.py
--rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/migrations/0006_auto_20230404_1744.py
--rw-r--r--   0 runner    (1001) docker     (122)      468 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/migrations/0007_alter_externalfulfillmentprovider_name.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15825 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.975185 openedx-ledger-0.4.1/openedx_ledger/signals/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      246 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/signals/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.971185 openedx-ledger-0.4.1/openedx_ledger/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.975185 openedx-ledger-0.4.1/openedx_ledger/templates/edx_ledger/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.979185 openedx-ledger-0.4.1/openedx_ledger/templates/edx_ledger/admin/
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/templates/edx_ledger/base.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.979185 openedx-ledger-0.4.1/openedx_ledger/test_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/test_utils/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.975185 openedx-ledger-0.4.1/openedx_ledger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8581 2023-05-24 15:52:21.000000 openedx-ledger-0.4.1/openedx_ledger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-05-24 15:52:21.000000 openedx-ledger-0.4.1/openedx_ledger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 15:52:21.000000 openedx-ledger-0.4.1/openedx_ledger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 15:52:21.000000 openedx-ledger-0.4.1/openedx_ledger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      197 2023-05-24 15:52:21.000000 openedx-ledger-0.4.1/openedx_ledger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-24 15:52:21.000000 openedx-ledger-0.4.1/openedx_ledger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.979185 openedx-ledger-0.4.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-24 15:52:21.979185 openedx-ledger-0.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5100 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.979185 openedx-ledger-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     7504 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8698 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/openedx_ledger/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3884 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5394 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/openedx_ledger/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6005 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4294 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/migrations/0003_field_updates_20230216_1605.py
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12708 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/migrations/0005_help_text_and_more_indices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/migrations/0006_auto_20230404_1744.py
+-rw-r--r--   0 runner    (1001) docker     (122)      468 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/migrations/0007_alter_externalfulfillmentprovider_name.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15825 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/openedx_ledger/signals/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/signals/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.502779 openedx-ledger-1.0.0/openedx_ledger/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/openedx_ledger/templates/edx_ledger/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/openedx_ledger/templates/edx_ledger/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/templates/edx_ledger/base.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/openedx_ledger/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/test_utils/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1463 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/openedx_ledger/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/openedx_ledger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8698 2023-05-30 20:48:33.000000 openedx-ledger-1.0.0/openedx_ledger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-05-30 20:48:33.000000 openedx-ledger-1.0.0/openedx_ledger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 20:48:33.000000 openedx-ledger-1.0.0/openedx_ledger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 20:48:33.000000 openedx-ledger-1.0.0/openedx_ledger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-05-30 20:48:33.000000 openedx-ledger-1.0.0/openedx_ledger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-30 20:48:33.000000 openedx-ledger-1.0.0/openedx_ledger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-30 20:48:33.510779 openedx-ledger-1.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5100 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:48:33.506779 openedx-ledger-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7504 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-05-30 20:48:29.000000 openedx-ledger-1.0.0/tests/test_utils.py
```

### Comparing `openedx-ledger-0.4.1/CHANGELOG.rst` & `openedx-ledger-1.0.0/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 
+[1.0.0]
+*******
+* Look for an ``lms_user_id`` key when generating transaction idempotency keys, not ``learner_id``.
+
 [0.4.0]
 *******
 * include only non-failed transactions in ledger balance calculation by default
 
 [0.3.3]
 *******
 * drop `ExternalFulfillmentProvider` name constraints
```

### Comparing `openedx-ledger-0.4.1/LICENSE.txt` & `openedx-ledger-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.1/PKG-INFO` & `openedx-ledger-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-ledger
-Version: 0.4.1
+Version: 1.0.0
 Summary: Records transactions against a ledger, denominated in units of value.
 Home-page: https://github.com/openedx/openedx-ledger
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -206,14 +206,18 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 
+[1.0.0]
+*******
+* Look for an ``lms_user_id`` key when generating transaction idempotency keys, not ``learner_id``.
+
 [0.4.0]
 *******
 * include only non-failed transactions in ledger balance calculation by default
 
 [0.3.3]
 *******
 * drop `ExternalFulfillmentProvider` name constraints
```

### Comparing `openedx-ledger-0.4.1/README.rst` & `openedx-ledger-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.1/openedx_ledger/admin.py` & `openedx-ledger-1.0.0/openedx_ledger/admin.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.1/openedx_ledger/api.py` & `openedx-ledger-1.0.0/openedx_ledger/api.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.1/openedx_ledger/migrations/0001_initial.py` & `openedx-ledger-1.0.0/openedx_ledger/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.1/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py` & `openedx-ledger-1.0.0/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.1/openedx_ledger/migrations/0003_field_updates_20230216_1605.py` & `openedx-ledger-1.0.0/openedx_ledger/migrations/0003_field_updates_20230216_1605.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.1/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py` & `openedx-ledger-1.0.0/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.1/openedx_ledger/migrations/0005_help_text_and_more_indices.py` & `openedx-ledger-1.0.0/openedx_ledger/migrations/0005_help_text_and_more_indices.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.1/openedx_ledger/migrations/0006_auto_20230404_1744.py` & `openedx-ledger-1.0.0/openedx_ledger/migrations/0006_auto_20230404_1744.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.1/openedx_ledger/models.py` & `openedx-ledger-1.0.0/openedx_ledger/models.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.1/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html` & `openedx-ledger-1.0.0/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.1/openedx_ledger/templates/edx_ledger/base.html` & `openedx-ledger-1.0.0/openedx_ledger/templates/edx_ledger/base.html`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.1/openedx_ledger/test_utils/factories.py` & `openedx-ledger-1.0.0/openedx_ledger/test_utils/factories.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.1/openedx_ledger/utils.py` & `openedx-ledger-1.0.0/openedx_ledger/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .constants import (
     INITIAL_DEPOSIT_TRANSACTION_SLUG,
     LEDGER_DEFAULT_IDEMPOTENCY_KEY_PREFIX,
     LEDGERED_SUBSIDY_IDEMPOTENCY_KEY_PREFIX,
 )
 
 TRANSACTION_METADATA_KEYS = {
-    'learner_id',
+    'lms_user_id',
     'content_key',
     'subsidy_access_policy_uuid',
 }
 
 
 def create_idempotency_key_for_ledger(subsidy_uuid=None):
     """
```

### Comparing `openedx-ledger-0.4.1/openedx_ledger/views.py` & `openedx-ledger-1.0.0/openedx_ledger/views.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.1/openedx_ledger.egg-info/PKG-INFO` & `openedx-ledger-1.0.0/openedx_ledger.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-ledger
-Version: 0.4.1
+Version: 1.0.0
 Summary: Records transactions against a ledger, denominated in units of value.
 Home-page: https://github.com/openedx/openedx-ledger
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -206,14 +206,18 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 
+[1.0.0]
+*******
+* Look for an ``lms_user_id`` key when generating transaction idempotency keys, not ``learner_id``.
+
 [0.4.0]
 *******
 * include only non-failed transactions in ledger balance calculation by default
 
 [0.3.3]
 *******
 * drop `ExternalFulfillmentProvider` name constraints
```

### Comparing `openedx-ledger-0.4.1/openedx_ledger.egg-info/SOURCES.txt` & `openedx-ledger-1.0.0/openedx_ledger.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,8 +32,9 @@
 openedx_ledger/templates/edx_ledger/base.html
 openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html
 openedx_ledger/test_utils/__init__.py
 openedx_ledger/test_utils/factories.py
 requirements/base.in
 requirements/constraints.txt
 tests/test_api.py
-tests/test_models.py
+tests/test_models.py
+tests/test_utils.py
```

### Comparing `openedx-ledger-0.4.1/requirements/constraints.txt` & `openedx-ledger-1.0.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.1/setup.py` & `openedx-ledger-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.1/tests/test_api.py` & `openedx-ledger-1.0.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.1/tests/test_models.py` & `openedx-ledger-1.0.0/tests/test_models.py`

 * *Files identical despite different names*

