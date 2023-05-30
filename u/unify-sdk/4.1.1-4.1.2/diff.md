# Comparing `tmp/unify-sdk-4.1.1.tar.gz` & `tmp/unify-sdk-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unify-sdk-4.1.1.tar", last modified: Thu May 11 16:30:06 2023, max compression
+gzip compressed data, was "dist/unify-sdk-4.1.2.tar", last modified: Tue May 30 20:44:58 2023, max compression
```

## Comparing `unify-sdk-4.1.1.tar` & `unify-sdk-4.1.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2747 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2331 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1897 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2581 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3881 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/disable_test_connectors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3811 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/disable_test_connectors_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7017 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_aa_permissions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4821 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_api_manager.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4416 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_api_manager_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1481 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_asset_access.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2600 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_graph_v2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2080 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_graph_v2_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1852 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_hierarchies.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1747 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_hierarchies_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2142 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_org_admin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2958 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_org_admin_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8643 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_pipelines.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8064 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_pipelines_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2388 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_properties.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10038 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_sources.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6669 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_sources_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3616 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_templates.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3390 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_templates_default_org.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/Unify.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4376 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/WaitingLibrary.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    44927 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/apimanager.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8167 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/apirequestsmng.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2950 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/apiutils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3609 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/assetaccess.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1480 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/clusters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11459 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/connectors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3057 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/generalutils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5142 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/graph.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify/helpers/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify/helpers/Permissions/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      864 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/Permissions/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      450 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/SingleOrg.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify/helpers/datasets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/datasets/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2084 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/datasets/column.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify/helpers/graph_ql/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/graph_ql/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2559 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/graph_ql/dataset_gql.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10009 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/graph_ql/graphql.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7479 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/graph_ql/permissions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5401 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/graph_ql/pipeline_gql.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify/helpers/pipeline/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/pipeline/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      449 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/pipeline/flow_column.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      551 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/pipeline/schema.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      894 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/staticsql.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify/helpers/unify_objects/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1001 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/unify_objects/Template.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/unify_objects/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5399 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/hierarchies.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17684 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/orgadmin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8738 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/permissions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    30555 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/pipelines.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14043 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/properties.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    52295 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/sources.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21586 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/templates.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3803 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/users.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify_sdk.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2747 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify_sdk.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1728 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       70 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify_sdk.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-30 20:44:58.000000 unify-sdk-4.1.2/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2747 2023-05-30 20:44:58.000000 unify-sdk-4.1.2/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2331 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-05-30 20:44:58.000000 unify-sdk-4.1.2/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1897 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-30 20:44:58.000000 unify-sdk-4.1.2/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2581 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3881 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/disable_test_connectors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3811 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/disable_test_connectors_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7017 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/test_aa_permissions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4821 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/test_api_manager.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4416 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/test_api_manager_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1481 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/test_asset_access.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2600 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/test_graph_v2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2080 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/test_graph_v2_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1852 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/test_hierarchies.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1747 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/test_hierarchies_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2142 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/test_org_admin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2958 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/test_org_admin_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8643 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/test_pipelines.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8064 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/test_pipelines_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2388 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/test_properties.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10038 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/test_sources.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6669 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/test_sources_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3616 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/test_templates.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3390 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/tests/test_templates_default_org.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-30 20:44:58.000000 unify-sdk-4.1.2/unify/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/Unify.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4376 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/WaitingLibrary.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    45309 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/apimanager.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8167 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/apirequestsmng.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2950 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/apiutils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3609 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/assetaccess.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1480 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/clusters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11459 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/connectors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3057 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/generalutils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5142 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/graph.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-30 20:44:58.000000 unify-sdk-4.1.2/unify/helpers/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-30 20:44:58.000000 unify-sdk-4.1.2/unify/helpers/Permissions/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      864 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/helpers/Permissions/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      450 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/helpers/SingleOrg.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/helpers/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-30 20:44:58.000000 unify-sdk-4.1.2/unify/helpers/datasets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/helpers/datasets/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2084 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/helpers/datasets/column.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-30 20:44:58.000000 unify-sdk-4.1.2/unify/helpers/graph_ql/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/helpers/graph_ql/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2559 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/helpers/graph_ql/dataset_gql.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10009 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/helpers/graph_ql/graphql.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7479 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/helpers/graph_ql/permissions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6099 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/helpers/graph_ql/pipeline_gql.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-30 20:44:58.000000 unify-sdk-4.1.2/unify/helpers/pipeline/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/helpers/pipeline/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      449 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/helpers/pipeline/flow_column.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      551 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/helpers/pipeline/schema.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      894 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/helpers/staticsql.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-30 20:44:58.000000 unify-sdk-4.1.2/unify/helpers/unify_objects/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1001 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/helpers/unify_objects/Template.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/helpers/unify_objects/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5399 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/hierarchies.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17684 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/orgadmin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8738 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/permissions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    31127 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/pipelines.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14043 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/properties.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    52295 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/sources.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21586 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/templates.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3803 2023-05-30 20:44:51.000000 unify-sdk-4.1.2/unify/users.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-30 20:44:58.000000 unify-sdk-4.1.2/unify_sdk.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2747 2023-05-30 20:44:57.000000 unify-sdk-4.1.2/unify_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1728 2023-05-30 20:44:57.000000 unify-sdk-4.1.2/unify_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-30 20:44:57.000000 unify-sdk-4.1.2/unify_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       70 2023-05-30 20:44:57.000000 unify-sdk-4.1.2/unify_sdk.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2023-05-30 20:44:57.000000 unify-sdk-4.1.2/unify_sdk.egg-info/top_level.txt
```

### Comparing `unify-sdk-4.1.1/LICENSE` & `unify-sdk-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/PKG-INFO` & `unify-sdk-4.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unify-sdk
-Version: 4.1.1
+Version: 4.1.2
 Summary: Unify Python SDK
 Home-page: https://github.com/ElementAnalytics/unify-python-sdk
 Author: Element Analytics
 Author-email: platform@ean.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `unify-sdk-4.1.1/README.md` & `unify-sdk-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/setup.py` & `unify-sdk-4.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/__init__.py` & `unify-sdk-4.1.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/disable_test_connectors.py` & `unify-sdk-4.1.2/tests/disable_test_connectors.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/disable_test_connectors_default_org.py` & `unify-sdk-4.1.2/tests/disable_test_connectors_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/test_aa_permissions.py` & `unify-sdk-4.1.2/tests/test_aa_permissions.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/test_api_manager.py` & `unify-sdk-4.1.2/tests/test_api_manager.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/test_api_manager_default_org.py` & `unify-sdk-4.1.2/tests/test_api_manager_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/test_asset_access.py` & `unify-sdk-4.1.2/tests/test_asset_access.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/test_graph_v2.py` & `unify-sdk-4.1.2/tests/test_graph_v2.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/test_graph_v2_default_org.py` & `unify-sdk-4.1.2/tests/test_graph_v2_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/test_hierarchies.py` & `unify-sdk-4.1.2/tests/test_hierarchies.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/test_hierarchies_default_org.py` & `unify-sdk-4.1.2/tests/test_hierarchies_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/test_org_admin.py` & `unify-sdk-4.1.2/tests/test_org_admin.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/test_org_admin_default_org.py` & `unify-sdk-4.1.2/tests/test_org_admin_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/test_pipelines.py` & `unify-sdk-4.1.2/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/test_pipelines_default_org.py` & `unify-sdk-4.1.2/tests/test_pipelines_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/test_properties.py` & `unify-sdk-4.1.2/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/test_sources.py` & `unify-sdk-4.1.2/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/test_sources_default_org.py` & `unify-sdk-4.1.2/tests/test_sources_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/test_templates.py` & `unify-sdk-4.1.2/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/tests/test_templates_default_org.py` & `unify-sdk-4.1.2/tests/test_templates_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/WaitingLibrary.py` & `unify-sdk-4.1.2/unify/WaitingLibrary.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/apimanager.py` & `unify-sdk-4.1.2/unify/apimanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,44 +216,48 @@
         return self.sources.append_dataset(
             org_id=orgid,
             data_set_id=dataset_id,
             content=content
         )
 
     @single_org
-    def dataset_list(self, org_id=None):
+    def dataset_list(self, org_id=None, page_num=1, page_size=1000):
         """
-        Retrieves metadata for all datasets on a given org
+        Retrieves metadata for all datasets on a given org, as long as there
+        are 1000 or less. For more than 1k, page through the results by
+        incrementing page_num (or increasing page_size)
 
         :param org_id: ORG id to be queried
         :type org_id: ORG id to be queried
+        :param page_num: page number of results
+        :param page_size: number of results per page
         :return:
         """
         try:
-            sources = self.sources.get_sources(org_id=org_id)
+            sources = self.sources.get_sources(org_id=org_id, page_num=page_num, page_size=page_size)
 
             for source in sources:
                 if "schema" in source:
                     del source["schema"]
 
             return sources
         except Exception as error:
             raise error
 
     @single_org
-    def pipeline_list(self, org_id=None):
+    def pipeline_list(self, org_id=None, page_num=1, page_size=100):
         """
         Retrieves metadata for all pipelines on a given org
 
         :param org_id: ORG id to be queried
         :type org_id: ORG id to be queried
         :return:
         """
         try:
-            return self.pipelines.get_pipelines_v2(org_id=org_id)
+            return self.pipelines.get_pipelines_v2(org_id=org_id, page_num=page_num, page_size=page_size)
 
         except Exception as error:
             raise error
 
     def execute_query(self, query, orgid, format):
         """
         Executes the given sql query through Unify Access on a given org
```

### Comparing `unify-sdk-4.1.1/unify/apirequestsmng.py` & `unify-sdk-4.1.2/unify/apirequestsmng.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/apiutils.py` & `unify-sdk-4.1.2/unify/apiutils.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/assetaccess.py` & `unify-sdk-4.1.2/unify/assetaccess.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/clusters.py` & `unify-sdk-4.1.2/unify/clusters.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/connectors.py` & `unify-sdk-4.1.2/unify/connectors.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/generalutils.py` & `unify-sdk-4.1.2/unify/generalutils.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/graph.py` & `unify-sdk-4.1.2/unify/graph.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/helpers/Permissions/__init__.py` & `unify-sdk-4.1.2/unify/helpers/Permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/helpers/datasets/column.py` & `unify-sdk-4.1.2/unify/helpers/datasets/column.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/helpers/graph_ql/dataset_gql.py` & `unify-sdk-4.1.2/unify/helpers/graph_ql/dataset_gql.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/helpers/graph_ql/graphql.py` & `unify-sdk-4.1.2/unify/helpers/graph_ql/graphql.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/helpers/graph_ql/permissions.py` & `unify-sdk-4.1.2/unify/helpers/graph_ql/permissions.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/helpers/graph_ql/pipeline_gql.py` & `unify-sdk-4.1.2/unify/helpers/graph_ql/pipeline_gql.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,59 @@
 import json
 from unify.helpers.graph_ql.graphql import GraphQLBuilder
 
 
 class PipelineGrapql(GraphQLBuilder):
 
-    def get_non_deleted_pipelines(self, pipeline_type="standard"):
+    def get_non_deleted_pipelines(self, pipeline_type="standard", page_num=1, page_size=100):
         """
         Creates graphql query to retrieve all non deleted pipelines
 
         :param pipeline_type: function or standard
         :return:
         """
-        return self.build_pipeline_query(is_deleted=False, pipeline_type=pipeline_type)
+        return self.build_pipeline_query(is_deleted=False,
+                                         pipeline_type=pipeline_type,
+                                         page_num=page_num,
+                                         page_size=page_size)
 
-    def get_deleted_pipelines(self, pipeline_type="standard"):
+    def get_deleted_pipelines(self, pipeline_type="standard", page_num=1, page_size=100):
         """
         Creates graphql query to retrieve all deleted pipelines
 
         :param pipeline_type:
         :return:
         """
-        return self.build_pipeline_query(is_deleted=True, pipeline_type=pipeline_type)
+        return self.build_pipeline_query(is_deleted=True,
+                                         pipeline_type=pipeline_type,
+                                         page_num=page_num,
+                                         page_size=page_size)
 
-    def get_pipelines_query(self, pipeline_type="standard"):
+
+    def get_pipelines_query(self, pipeline_type="standard", page_num=1, page_size=100):
         """
         Creates graphql query to retrieve all non deleted standard pipelines
 
         :param pipeline_type:
         :return:
         """
-        return self.build_pipeline_query(is_deleted=None, pipeline_type=pipeline_type)
+        return self.build_pipeline_query(is_deleted=None,
+                                         pipeline_type=pipeline_type,
+                                         page_num=page_num,
+                                         page_size=page_size)
 
-    def get_functions_query(self):
+    def get_functions_query(self, page_num=1, page_size=100):
         """
         Creates graphql query to retrieve all non deleted function pipelines
 
         :return:
         """
-        return self.build_pipeline_query(
-            pipeline_type="function"
-        )
+        return self.build_pipeline_query(pipeline_type="function",
+                                         page_num=page_num,
+                                         page_size=page_size)
 
     def build_pipeline_query(
             self,
             count=True,
             page_num: int = 1,
             page_size: int = 100,
             facets=None,
```

### Comparing `unify-sdk-4.1.1/unify/helpers/pipeline/schema.py` & `unify-sdk-4.1.2/unify/helpers/pipeline/schema.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/helpers/staticsql.py` & `unify-sdk-4.1.2/unify/helpers/staticsql.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/helpers/unify_objects/Template.py` & `unify-sdk-4.1.2/unify/helpers/unify_objects/Template.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/hierarchies.py` & `unify-sdk-4.1.2/unify/hierarchies.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/orgadmin.py` & `unify-sdk-4.1.2/unify/orgadmin.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/permissions.py` & `unify-sdk-4.1.2/unify/permissions.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/pipelines.py` & `unify-sdk-4.1.2/unify/pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -566,57 +566,63 @@
 
         if result.status_code == 200:
             return json.loads(result.content)
 
         raise Exception(repr(result.content))
 
     @single_org
-    def get_pipelines_v2(self, org_id=None, deleted=False, pipeline_type="standard"):
+    def get_pipelines_v2(self, org_id=None, deleted=False, pipeline_type="standard", page_num=1, page_size=100):
         """
         Retrieves the pipeline list from the given org
 
         :param org_id: Org id to be queried
         :type org_id: int or str
         :param deleted: Deletion status fo pipeliens to be queried
         :type deleted: bool or None
         :param pipeline_type: Pipeline type standard or function
         :type pipeline_type: str
         :return:
         """
 
         if deleted is True:
-            query = self.gql_builder.get_deleted_pipelines(pipeline_type=pipeline_type)
+            query = self.gql_builder.get_deleted_pipelines(pipeline_type=pipeline_type,
+                                                           page_num=page_num,
+                                                           page_size=page_size)
         elif deleted is False:
-            query = self.gql_builder.get_non_deleted_pipelines(pipeline_type=pipeline_type)
+            query = self.gql_builder.get_non_deleted_pipelines(pipeline_type=pipeline_type,
+                                                               page_num=page_num,
+                                                               page_size=page_size)
         else:
-            query = self.gql_builder.get_pipelines_query(pipeline_type=pipeline_type)
+            query = self.gql_builder.get_pipelines_query(pipeline_type=pipeline_type,
+                                                         page_num=page_num,
+                                                         page_size=page_size)
 
         get_pipelines_request = self.graph_ql_query(org_id=org_id, query=query)
 
         if get_pipelines_request.status_code in range(200, 202):
             data = json.loads(get_pipelines_request.content)
             if "data" in data:
                 if "artifacts" in data["data"]:
                     return data["data"]["artifacts"]
 
             return []
         raise Exception(repr(get_pipelines_request.content))
 
     @single_org
-    def get_pipelines_functions(self, org_id=None, deleted=False):
+    def get_pipelines_functions(self, org_id=None, deleted=False, page_num=1, page_size=100):
         """
         Retrieves the pipeline list from the given org
 
         :param org_id: Org id to be queried
         :type org_id: int or str
         :param deleted: Deletion status fo pipeliens to be queried
         :type deleted: bool or None
         :return:
         """
-        return self.get_pipelines_v2(org_id=org_id, deleted=deleted, pipeline_type="function")
+        return self.get_pipelines_v2(org_id=org_id, deleted=deleted, pipeline_type="function", page_num=page_num, page_size=page_size)
 
     @single_org
     def verify_if_pipeline_exists_and_get_id(self, org_id=None, *, pipeline_name):
         """
         Verifies that the pipeline name exists on the given org. Returns pipeline id.
 
         :param org_id: Org id of pipeline
```

### Comparing `unify-sdk-4.1.1/unify/properties.py` & `unify-sdk-4.1.2/unify/properties.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/sources.py` & `unify-sdk-4.1.2/unify/sources.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/templates.py` & `unify-sdk-4.1.2/unify/templates.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify/users.py` & `unify-sdk-4.1.2/unify/users.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.1/unify_sdk.egg-info/PKG-INFO` & `unify-sdk-4.1.2/unify_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unify-sdk
-Version: 4.1.1
+Version: 4.1.2
 Summary: Unify Python SDK
 Home-page: https://github.com/ElementAnalytics/unify-python-sdk
 Author: Element Analytics
 Author-email: platform@ean.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `unify-sdk-4.1.1/unify_sdk.egg-info/SOURCES.txt` & `unify-sdk-4.1.2/unify_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

