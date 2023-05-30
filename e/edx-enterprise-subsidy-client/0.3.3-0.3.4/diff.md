# Comparing `tmp/edx-enterprise-subsidy-client-0.3.3.tar.gz` & `tmp/edx-enterprise-subsidy-client-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-enterprise-subsidy-client-0.3.3.tar", last modified: Thu May 18 20:04:32 2023, max compression
+gzip compressed data, was "edx-enterprise-subsidy-client-0.3.4.tar", last modified: Tue May 30 15:52:52 2023, max compression
```

## Comparing `edx-enterprise-subsidy-client-0.3.3.tar` & `edx-enterprise-subsidy-client-0.3.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:04:32.123772 edx-enterprise-subsidy-client-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8909 2023-05-18 20:04:32.123772 edx-enterprise-subsidy-client-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6341 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:04:32.123772 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client/
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10533 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:04:32.123772 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8909 2023-05-18 20:04:32.000000 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      544 2023-05-18 20:04:32.000000 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-18 20:04:32.000000 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-18 20:04:32.000000 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-18 20:04:32.000000 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-18 20:04:32.000000 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:04:32.123772 edx-enterprise-subsidy-client-0.3.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-18 20:04:32.123772 edx-enterprise-subsidy-client-0.3.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5111 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:04:32.123772 edx-enterprise-subsidy-client-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3178 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 15:52:52.456090 edx-enterprise-subsidy-client-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1998 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9022 2023-05-30 15:52:52.456090 edx-enterprise-subsidy-client-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6341 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 15:52:52.456090 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10723 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 15:52:52.456090 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9022 2023-05-30 15:52:52.000000 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2023-05-30 15:52:52.000000 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 15:52:52.000000 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 15:52:52.000000 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-30 15:52:52.000000 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-30 15:52:52.000000 edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 15:52:52.456090 edx-enterprise-subsidy-client-0.3.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-30 15:52:52.456090 edx-enterprise-subsidy-client-0.3.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5111 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 15:52:52.456090 edx-enterprise-subsidy-client-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3275 2023-05-30 15:52:44.000000 edx-enterprise-subsidy-client-0.3.4/tests/test_client.py
```

### Comparing `edx-enterprise-subsidy-client-0.3.3/CHANGELOG.rst` & `edx-enterprise-subsidy-client-0.3.4/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
 [0.3.3]
 *******
+* allow additional query params, like ``page_size``, to be passed through to listing endpoints.
+
+[0.3.3]
+*******
 * admin-list transactions will also be filtered by ``created`` state by default.
 * Adds an ADR explaining the default states for which this client filters transactions.
 
 [0.3.2]
 *******
 * admin-list transactions will ask to be filtered for only `committed` and `pending` states by default.
   Caller may specify other valid states (e.g. `failed` or `created`).
```

### Comparing `edx-enterprise-subsidy-client-0.3.3/LICENSE` & `edx-enterprise-subsidy-client-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.3/LICENSE.txt` & `edx-enterprise-subsidy-client-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.3/PKG-INFO` & `edx-enterprise-subsidy-client-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.3.3
+Version: 0.3.4
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -225,14 +225,18 @@
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
 [0.3.3]
 *******
+* allow additional query params, like ``page_size``, to be passed through to listing endpoints.
+
+[0.3.3]
+*******
 * admin-list transactions will also be filtered by ``created`` state by default.
 * Adds an ADR explaining the default states for which this client filters transactions.
 
 [0.3.2]
 *******
 * admin-list transactions will ask to be filtered for only `committed` and `pending` states by default.
   Caller may specify other valid states (e.g. `failed` or `created`).
```

### Comparing `edx-enterprise-subsidy-client-0.3.3/README.rst` & `edx-enterprise-subsidy-client-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client/client.py` & `edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             logger.exception(
                 f'Subsidy client failed to fetch content metadata for {content_identifier} '
                 f'in customer {enterprise_customer_uuid}'
             )
             raise exc
         return response_data.json()
 
-    def list_subsidies(self, enterprise_customer_uuid):
+    def list_subsidies(self, enterprise_customer_uuid, **kwargs):
         """
         Client method to list enterprise subsidy records for the given enterprise_customer_uuid.
 
         Args:
             enterprise_customer_uuid (str): Enterprise customer UUID
         Returns:
             Paginated response of serialized Subsidy records:
@@ -133,17 +133,19 @@
                     "reference_type": "opportunity_product_id",
                     "current_balance": "string"
                   }
                 ]
               }
             ```
         """
+        query_params = {'enterprise_customer_uuid': enterprise_customer_uuid}
+        query_params.update(kwargs)
         response = self.client.get(
             self.SUBSIDIES_ENDPOINT,
-            params={'enterprise_customer_uuid': enterprise_customer_uuid}
+            params=query_params,
         )
         response.raise_for_status()
         return response.json()
 
     def retrieve_subsidy(self, subsidy_uuid):
         """
         TODO: add docstring.
@@ -154,19 +156,21 @@
         response.raise_for_status()
         return response.json()
 
     def list_subsidy_transactions(
         self, subsidy_uuid, include_aggregates=True,
         lms_user_id=None, content_key=None,
         subsidy_access_policy_uuid=None,
+        **kwargs
     ):
         """
         TODO: add docstring.
         """
         query_params = {'subsidy_uuid': subsidy_uuid}
+        query_params.update(kwargs)
         if include_aggregates:
             query_params['include_aggregates'] = include_aggregates
         if lms_user_id:
             query_params['lms_user_id'] = lms_user_id
         if content_key:
             query_params['content_key'] = content_key
         if subsidy_access_policy_uuid:
@@ -243,25 +247,27 @@
     V2_BASE_URL = EnterpriseSubsidyAPIClient.API_BASE_URL + 'v2/'
     TRANSACTIONS_LIST_ENDPOINT = V2_BASE_URL + 'subsidies/{subsidy_uuid}/admin/transactions/'
 
     def list_subsidy_transactions(
         self, subsidy_uuid, include_aggregates=True,
         lms_user_id=None, content_key=None,
         subsidy_access_policy_uuid=None, transaction_states=None,
+        **kwargs,
     ):
         """
         List transactions in a subsidy with admin- or operator-level permissions.
         """
         query_params = {
             'state': [
                 TransactionStateChoices.COMMITTED,
                 TransactionStateChoices.PENDING,
                 TransactionStateChoices.CREATED,
             ],
         }
+        query_params.update(kwargs)
         if include_aggregates:
             query_params['include_aggregates'] = include_aggregates
         if lms_user_id:
             query_params['lms_user_id'] = lms_user_id
         if content_key:
             query_params['content_key'] = content_key
         if subsidy_access_policy_uuid:
```

### Comparing `edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client.egg-info/PKG-INFO` & `edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.3.3
+Version: 0.3.4
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -225,14 +225,18 @@
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
 [0.3.3]
 *******
+* allow additional query params, like ``page_size``, to be passed through to listing endpoints.
+
+[0.3.3]
+*******
 * admin-list transactions will also be filtered by ``created`` state by default.
 * Adds an ADR explaining the default states for which this client filters transactions.
 
 [0.3.2]
 *******
 * admin-list transactions will ask to be filtered for only `committed` and `pending` states by default.
   Caller may specify other valid states (e.g. `failed` or `created`).
```

### Comparing `edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client.egg-info/SOURCES.txt` & `edx-enterprise-subsidy-client-0.3.4/edx_enterprise_subsidy_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.3/requirements/constraints.txt` & `edx-enterprise-subsidy-client-0.3.4/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.3/setup.py` & `edx-enterprise-subsidy-client-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.3/tests/test_client.py` & `edx-enterprise-subsidy-client-0.3.4/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,35 +60,39 @@
     content_key = 'the-best-content'
     subsidy_access_policy_uuid = uuid.uuid4()
 
     subsidy_service_client = EnterpriseSubsidyAPIClientV2()
 
     data_driven_test = [
         (
-            {'transaction_states': ['committed', 'pending', 'district-of-columbia']},
+            {
+                'page_size': 1,
+                'transaction_states': ['committed', 'pending', 'district-of-columbia'],
+            },
             ['committed', 'pending'],
         ),
         (
-            {},
+            {'page_size': 1},
             ['committed', 'pending', 'created'],
         ),
     ]
-    for state_kwargs, expected_state_call_param in data_driven_test:
+    for kwargs, expected_state_call_param in data_driven_test:
         response = subsidy_service_client.list_subsidy_transactions(
             subsidy_uuid=subsidy_uuid,
             lms_user_id=lms_user_id,
             content_key=content_key,
             subsidy_access_policy_uuid=subsidy_access_policy_uuid,
-            **state_kwargs,
+            **kwargs,
         )
 
         assert response == mocked_response_data
         mock_oauth_client.return_value.get.assert_called_with(
             f'enterprise-subsidy-service-base-url/api/v2/subsidies/{subsidy_uuid}/admin/transactions/',
             params={
                 'state': expected_state_call_param,
                 'include_aggregates': True,
                 'lms_user_id': 123,
                 'content_key': 'the-best-content',
                 'subsidy_access_policy_uuid': str(subsidy_access_policy_uuid),
+                'page_size': 1,
             },
         )
```

