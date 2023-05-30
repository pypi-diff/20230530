# Comparing `tmp/jsa-0.1.0.tar.gz` & `tmp/jsa-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsa-0.1.0.tar", max compression
+gzip compressed data, was "jsa-0.2.0.tar", max compression
```

## Comparing `jsa-0.1.0.tar` & `jsa-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0        0 2023-05-30 13:12:38.341368 jsa-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-30 13:12:38.341309 jsa-0.1.0/jsa/__init__.py
--rw-r--r--   0        0        0     2438 2023-05-30 13:12:38.725159 jsa-0.1.0/jsa/api_client.py
--rw-r--r--   0        0        0     2450 2023-05-30 13:12:38.720372 jsa-0.1.0/jsa/apis/apis_request_builder.py
--rw-r--r--   0        0        0     2347 2023-05-30 13:12:38.724254 jsa-0.1.0/jsa/apis/beta/acs/acs_request_builder.py
--rw-r--r--   0        0        0     4188 2023-05-30 13:12:38.723424 jsa-0.1.0/jsa/apis/beta/acs/v1/item/with_client_item_request_builder.py
--rw-r--r--   0        0        0     4909 2023-05-30 13:12:38.723891 jsa-0.1.0/jsa/apis/beta/acs/v1/v1_request_builder.py
--rw-r--r--   0        0        0     1596 2023-05-30 13:12:38.724465 jsa-0.1.0/jsa/apis/beta/beta_request_builder.py
--rw-r--r--   0        0        0     2307 2023-05-30 13:12:38.720090 jsa-0.1.0/jsa/apis/organizations/organizations_request_builder.py
--rw-r--r--   0        0        0     6794 2023-05-30 13:12:38.718860 jsa-0.1.0/jsa/apis/organizations/v1/item/authentication_policy/authentication_policy_request_builder.py
--rw-r--r--   0        0        0     1811 2023-05-30 13:12:38.719474 jsa-0.1.0/jsa/apis/organizations/v1/item/v1_item_request_builder.py
--rw-r--r--   0        0        0     1285 2023-05-30 13:12:38.712809 jsa-0.1.0/jsa/apis/organizations/v1/v1_request_builder.py
--rw-r--r--   0        0        0     2322 2023-05-30 13:12:38.722891 jsa-0.1.0/jsa/apis/service_accounts/service_accounts_request_builder.py
--rw-r--r--   0        0        0     4349 2023-05-30 13:12:38.721943 jsa-0.1.0/jsa/apis/service_accounts/v1/item/reset_secret/reset_secret_request_builder.py
--rw-r--r--   0        0        0     9985 2023-05-30 13:12:38.721267 jsa-0.1.0/jsa/apis/service_accounts/v1/item/v1_item_request_builder.py
--rw-r--r--   0        0        0     8123 2023-05-30 13:12:38.722561 jsa-0.1.0/jsa/apis/service_accounts/v1/v1_request_builder.py
--rw-r--r--   0        0        0     1109 2023-05-30 13:12:38.743716 jsa-0.1.0/jsa/kiota-lock.json
--rw-r--r--   0        0        0     4723 2023-05-30 13:12:38.735882 jsa-0.1.0/jsa/models/acs_client_request_data.py
--rw-r--r--   0        0        0     5331 2023-05-30 13:12:38.730930 jsa-0.1.0/jsa/models/acs_client_response_data.py
--rw-r--r--   0        0        0     3298 2023-05-30 13:12:38.729328 jsa-0.1.0/jsa/models/authentication_factors.py
--rw-r--r--   0        0        0     3813 2023-05-30 13:12:38.729658 jsa-0.1.0/jsa/models/authentication_policy.py
--rw-r--r--   0        0        0     3196 2023-05-30 13:12:38.730481 jsa-0.1.0/jsa/models/error.py
--rw-r--r--   0        0        0     3197 2023-05-30 13:12:38.727806 jsa-0.1.0/jsa/models/otp.py
--rw-r--r--   0        0        0     4579 2023-05-30 13:12:38.735398 jsa-0.1.0/jsa/models/red_hat_error_representation.py
--rw-r--r--   0        0        0      865 2023-05-30 13:12:38.728229 jsa-0.1.0/jsa/models/red_hat_error_representation_error.py
--rw-r--r--   0        0        0     4019 2023-05-30 13:12:38.728921 jsa-0.1.0/jsa/models/service_account_create_request_data.py
--rw-r--r--   0        0        0     7558 2023-05-30 13:12:38.734848 jsa-0.1.0/jsa/models/service_account_data.py
--rw-r--r--   0        0        0     3989 2023-05-30 13:12:38.731347 jsa-0.1.0/jsa/models/service_account_request_data.py
--rw-r--r--   0        0        0     5226 2023-05-30 13:12:38.730095 jsa-0.1.0/jsa/models/validation_exception_data.py
--rw-r--r--   0        0        0     2622 2023-05-30 13:12:38.728496 jsa-0.1.0/jsa/models/validation_exception_data_fields.py
--rw-r--r--   0        0        0      455 2023-05-30 13:12:41.450626 jsa-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 jsa-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-30 13:12:38.341368 jsa-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 13:12:38.341309 jsa-0.2.0/jsa/__init__.py
+-rw-r--r--   0        0        0     2438 2023-05-30 13:12:38.725159 jsa-0.2.0/jsa/api_client.py
+-rw-r--r--   0        0        0     2450 2023-05-30 13:12:38.720372 jsa-0.2.0/jsa/apis/apis_request_builder.py
+-rw-r--r--   0        0        0     2347 2023-05-30 13:12:38.724254 jsa-0.2.0/jsa/apis/beta/acs/acs_request_builder.py
+-rw-r--r--   0        0        0     4188 2023-05-30 13:12:38.723424 jsa-0.2.0/jsa/apis/beta/acs/v1/item/with_client_item_request_builder.py
+-rw-r--r--   0        0        0     4909 2023-05-30 13:12:38.723891 jsa-0.2.0/jsa/apis/beta/acs/v1/v1_request_builder.py
+-rw-r--r--   0        0        0     1596 2023-05-30 13:12:38.724465 jsa-0.2.0/jsa/apis/beta/beta_request_builder.py
+-rw-r--r--   0        0        0     2307 2023-05-30 13:12:38.720090 jsa-0.2.0/jsa/apis/organizations/organizations_request_builder.py
+-rw-r--r--   0        0        0     6794 2023-05-30 13:12:38.718860 jsa-0.2.0/jsa/apis/organizations/v1/item/authentication_policy/authentication_policy_request_builder.py
+-rw-r--r--   0        0        0     1811 2023-05-30 13:12:38.719474 jsa-0.2.0/jsa/apis/organizations/v1/item/v1_item_request_builder.py
+-rw-r--r--   0        0        0     1285 2023-05-30 13:12:38.712809 jsa-0.2.0/jsa/apis/organizations/v1/v1_request_builder.py
+-rw-r--r--   0        0        0     2322 2023-05-30 13:12:38.722891 jsa-0.2.0/jsa/apis/service_accounts/service_accounts_request_builder.py
+-rw-r--r--   0        0        0     4349 2023-05-30 13:12:38.721943 jsa-0.2.0/jsa/apis/service_accounts/v1/item/reset_secret/reset_secret_request_builder.py
+-rw-r--r--   0        0        0     9985 2023-05-30 13:12:38.721267 jsa-0.2.0/jsa/apis/service_accounts/v1/item/v1_item_request_builder.py
+-rw-r--r--   0        0        0     8123 2023-05-30 13:12:38.722561 jsa-0.2.0/jsa/apis/service_accounts/v1/v1_request_builder.py
+-rw-r--r--   0        0        0     1109 2023-05-30 13:12:38.743716 jsa-0.2.0/jsa/kiota-lock.json
+-rw-r--r--   0        0        0     4723 2023-05-30 13:12:38.735882 jsa-0.2.0/jsa/models/acs_client_request_data.py
+-rw-r--r--   0        0        0     5331 2023-05-30 13:12:38.730930 jsa-0.2.0/jsa/models/acs_client_response_data.py
+-rw-r--r--   0        0        0     3298 2023-05-30 13:12:38.729328 jsa-0.2.0/jsa/models/authentication_factors.py
+-rw-r--r--   0        0        0     3813 2023-05-30 13:12:38.729658 jsa-0.2.0/jsa/models/authentication_policy.py
+-rw-r--r--   0        0        0     3196 2023-05-30 13:12:38.730481 jsa-0.2.0/jsa/models/error.py
+-rw-r--r--   0        0        0     3197 2023-05-30 13:12:38.727806 jsa-0.2.0/jsa/models/otp.py
+-rw-r--r--   0        0        0     4579 2023-05-30 13:12:38.735398 jsa-0.2.0/jsa/models/red_hat_error_representation.py
+-rw-r--r--   0        0        0      865 2023-05-30 13:12:38.728229 jsa-0.2.0/jsa/models/red_hat_error_representation_error.py
+-rw-r--r--   0        0        0     4019 2023-05-30 13:12:38.728921 jsa-0.2.0/jsa/models/service_account_create_request_data.py
+-rw-r--r--   0        0        0     7558 2023-05-30 13:12:38.734848 jsa-0.2.0/jsa/models/service_account_data.py
+-rw-r--r--   0        0        0     3989 2023-05-30 13:12:38.731347 jsa-0.2.0/jsa/models/service_account_request_data.py
+-rw-r--r--   0        0        0     5226 2023-05-30 13:12:38.730095 jsa-0.2.0/jsa/models/validation_exception_data.py
+-rw-r--r--   0        0        0     2622 2023-05-30 13:12:38.728496 jsa-0.2.0/jsa/models/validation_exception_data_fields.py
+-rw-r--r--   0        0        0      454 2023-05-30 13:16:35.490687 jsa-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 jsa-0.2.0/PKG-INFO
```

### Comparing `jsa-0.1.0/jsa/api_client.py` & `jsa-0.2.0/jsa/api_client.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/apis/apis_request_builder.py` & `jsa-0.2.0/jsa/apis/apis_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/apis/beta/acs/acs_request_builder.py` & `jsa-0.2.0/jsa/apis/beta/acs/acs_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/apis/beta/acs/v1/item/with_client_item_request_builder.py` & `jsa-0.2.0/jsa/apis/beta/acs/v1/item/with_client_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/apis/beta/acs/v1/v1_request_builder.py` & `jsa-0.2.0/jsa/apis/beta/acs/v1/v1_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/apis/beta/beta_request_builder.py` & `jsa-0.2.0/jsa/apis/beta/beta_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/apis/organizations/organizations_request_builder.py` & `jsa-0.2.0/jsa/apis/organizations/organizations_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/apis/organizations/v1/item/authentication_policy/authentication_policy_request_builder.py` & `jsa-0.2.0/jsa/apis/organizations/v1/item/authentication_policy/authentication_policy_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/apis/organizations/v1/item/v1_item_request_builder.py` & `jsa-0.2.0/jsa/apis/organizations/v1/item/v1_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/apis/organizations/v1/v1_request_builder.py` & `jsa-0.2.0/jsa/apis/organizations/v1/v1_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/apis/service_accounts/service_accounts_request_builder.py` & `jsa-0.2.0/jsa/apis/service_accounts/service_accounts_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/apis/service_accounts/v1/item/reset_secret/reset_secret_request_builder.py` & `jsa-0.2.0/jsa/apis/service_accounts/v1/item/reset_secret/reset_secret_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/apis/service_accounts/v1/item/v1_item_request_builder.py` & `jsa-0.2.0/jsa/apis/service_accounts/v1/item/v1_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/apis/service_accounts/v1/v1_request_builder.py` & `jsa-0.2.0/jsa/apis/service_accounts/v1/v1_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/kiota-lock.json` & `jsa-0.2.0/jsa/kiota-lock.json`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/models/acs_client_request_data.py` & `jsa-0.2.0/jsa/models/acs_client_request_data.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/models/acs_client_response_data.py` & `jsa-0.2.0/jsa/models/acs_client_response_data.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/models/authentication_factors.py` & `jsa-0.2.0/jsa/models/authentication_factors.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/models/authentication_policy.py` & `jsa-0.2.0/jsa/models/authentication_policy.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/models/error.py` & `jsa-0.2.0/jsa/models/error.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/models/otp.py` & `jsa-0.2.0/jsa/models/otp.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/models/red_hat_error_representation.py` & `jsa-0.2.0/jsa/models/red_hat_error_representation.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/models/red_hat_error_representation_error.py` & `jsa-0.2.0/jsa/models/red_hat_error_representation_error.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/models/service_account_create_request_data.py` & `jsa-0.2.0/jsa/models/service_account_create_request_data.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/models/service_account_data.py` & `jsa-0.2.0/jsa/models/service_account_data.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/models/service_account_request_data.py` & `jsa-0.2.0/jsa/models/service_account_request_data.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/models/validation_exception_data.py` & `jsa-0.2.0/jsa/models/validation_exception_data.py`

 * *Files identical despite different names*

### Comparing `jsa-0.1.0/jsa/models/validation_exception_data_fields.py` & `jsa-0.2.0/jsa/models/validation_exception_data_fields.py`

 * *Files identical despite different names*

