# Comparing `tmp/fugue-warehouses-0.0.3.tar.gz` & `tmp/fugue-warehouses-0.0.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fugue-warehouses-0.0.3.tar", last modified: Tue May 30 05:46:37 2023, max compression
+gzip compressed data, was "fugue-warehouses-0.0.3.dev1.tar", last modified: Thu Mar 23 07:06:26 2023, max compression
```

## Comparing `fugue-warehouses-0.0.3.tar` & `fugue-warehouses-0.0.3.dev1.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:46:37.729663 fugue-warehouses-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-30 05:46:37.729663 fugue-warehouses-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:46:37.725664 fugue-warehouses-0.0.3/fugue_bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_bigquery/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_bigquery/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_bigquery/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_bigquery/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_bigquery/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_bigquery/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_bigquery/ray_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_bigquery/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:46:37.725664 fugue-warehouses-0.0.3/fugue_trino/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_trino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_trino/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_trino/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_trino/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_trino/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_trino/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_trino/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_trino/execution_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:46:37.725664 fugue-warehouses-0.0.3/fugue_trino/ibis_trino/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_trino/ibis_trino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_trino/ibis_trino/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_trino/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:46:37.725664 fugue-warehouses-0.0.3/fugue_warehouses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_warehouses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:46:37.725664 fugue-warehouses-0.0.3/fugue_warehouses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-30 05:46:37.000000 fugue-warehouses-0.0.3/fugue_warehouses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-30 05:46:37.000000 fugue-warehouses-0.0.3/fugue_warehouses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 05:46:37.000000 fugue-warehouses-0.0.3/fugue_warehouses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-30 05:46:37.000000 fugue-warehouses-0.0.3/fugue_warehouses.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-30 05:46:37.000000 fugue-warehouses-0.0.3/fugue_warehouses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-30 05:46:37.000000 fugue-warehouses-0.0.3/fugue_warehouses.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:46:37.729663 fugue-warehouses-0.0.3/fugue_warehouses_version/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/fugue_warehouses_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-30 05:46:37.729663 fugue-warehouses-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:46:37.729663 fugue-warehouses-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:46:37.729663 fugue-warehouses-0.0.3/tests/fugue_bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/tests/fugue_bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/tests/fugue_bigquery/mock_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/tests/fugue_bigquery/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/tests/fugue_bigquery/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/tests/fugue_bigquery/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/tests/fugue_bigquery/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/tests/fugue_bigquery/test_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:46:37.729663 fugue-warehouses-0.0.3/tests/fugue_trino/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/tests/fugue_trino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/tests/fugue_trino/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/tests/fugue_trino/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/tests/fugue_trino/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/tests/fugue_trino/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/tests/fugue_trino/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-30 05:45:27.000000 fugue-warehouses-0.0.3/tests/fugue_trino/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:06:26.908202 fugue-warehouses-0.0.3.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-23 07:06:26.908202 fugue-warehouses-0.0.3.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:06:26.904202 fugue-warehouses-0.0.3.dev1/fugue_bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_bigquery/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_bigquery/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_bigquery/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_bigquery/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_bigquery/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_bigquery/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_bigquery/ray_execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_bigquery/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:06:26.904202 fugue-warehouses-0.0.3.dev1/fugue_trino/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_trino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_trino/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_trino/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_trino/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_trino/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_trino/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_trino/execution_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:06:26.904202 fugue-warehouses-0.0.3.dev1/fugue_trino/ibis_trino/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_trino/ibis_trino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_trino/ibis_trino/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_trino/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:06:26.904202 fugue-warehouses-0.0.3.dev1/fugue_warehouses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_warehouses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:06:26.904202 fugue-warehouses-0.0.3.dev1/fugue_warehouses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-23 07:06:26.000000 fugue-warehouses-0.0.3.dev1/fugue_warehouses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-03-23 07:06:26.000000 fugue-warehouses-0.0.3.dev1/fugue_warehouses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 07:06:26.000000 fugue-warehouses-0.0.3.dev1/fugue_warehouses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-23 07:06:26.000000 fugue-warehouses-0.0.3.dev1/fugue_warehouses.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-23 07:06:26.000000 fugue-warehouses-0.0.3.dev1/fugue_warehouses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-23 07:06:26.000000 fugue-warehouses-0.0.3.dev1/fugue_warehouses.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:06:26.904202 fugue-warehouses-0.0.3.dev1/fugue_warehouses_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/fugue_warehouses_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-23 07:06:26.908202 fugue-warehouses-0.0.3.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:06:26.904202 fugue-warehouses-0.0.3.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:06:26.908202 fugue-warehouses-0.0.3.dev1/tests/fugue_bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/tests/fugue_bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/tests/fugue_bigquery/mock_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/tests/fugue_bigquery/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/tests/fugue_bigquery/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/tests/fugue_bigquery/test_execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/tests/fugue_bigquery/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/tests/fugue_bigquery/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:06:26.908202 fugue-warehouses-0.0.3.dev1/tests/fugue_trino/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/tests/fugue_trino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/tests/fugue_trino/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/tests/fugue_trino/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/tests/fugue_trino/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/tests/fugue_trino/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/tests/fugue_trino/test_execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-03-23 07:05:16.000000 fugue-warehouses-0.0.3.dev1/tests/fugue_trino/test_workflow.py
```

### Comparing `fugue-warehouses-0.0.3/LICENSE` & `fugue-warehouses-0.0.3.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `fugue-warehouses-0.0.3/PKG-INFO` & `fugue-warehouses-0.0.3.dev1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue-warehouses
-Version: 0.0.3
+Version: 0.0.3.dev1
 Summary: Fugue data warehouses integration
 Home-page: http://github.com/fugue-project/fugue-warehouses
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue Data Warehouses Integration
```

### Comparing `fugue-warehouses-0.0.3/fugue_bigquery/_utils.py` & `fugue-warehouses-0.0.3.dev1/fugue_bigquery/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-warehouses-0.0.3/fugue_bigquery/api.py` & `fugue-warehouses-0.0.3.dev1/fugue_bigquery/api.py`

 * *Files identical despite different names*

### Comparing `fugue-warehouses-0.0.3/fugue_bigquery/client.py` & `fugue-warehouses-0.0.3.dev1/fugue_bigquery/client.py`

 * *Files identical despite different names*

### Comparing `fugue-warehouses-0.0.3/fugue_bigquery/dataframe.py` & `fugue-warehouses-0.0.3.dev1/fugue_bigquery/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-warehouses-0.0.3/fugue_bigquery/execution_engine.py` & `fugue-warehouses-0.0.3.dev1/fugue_bigquery/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-warehouses-0.0.3/fugue_bigquery/ray_execution_engine.py` & `fugue-warehouses-0.0.3.dev1/fugue_bigquery/ray_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-warehouses-0.0.3/fugue_bigquery/registry.py` & `fugue-warehouses-0.0.3.dev1/fugue_bigquery/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-warehouses-0.0.3/fugue_trino/_constants.py` & `fugue-warehouses-0.0.3.dev1/fugue_trino/_constants.py`

 * *Files identical despite different names*

### Comparing `fugue-warehouses-0.0.3/fugue_trino/_utils.py` & `fugue-warehouses-0.0.3.dev1/fugue_trino/_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import re
 from typing import Any, List, Optional
 
 import fugue.api as fa
-import ibis
-import ibis.expr.datatypes as dt
 import pyarrow as pa
 from fugue.extensions import namespace_candidate
 from fugue_ibis import IbisSchema, IbisTable
-from fugue_ibis._utils import ibis_to_pa_type, pa_to_ibis_type
+from fugue_ibis._utils import ibis_to_pa_type
 from ibis.backends.trino import Backend
 from triad import ParamDict, Schema
 from triad.utils.pyarrow import TRIAD_DEFAULT_TIMESTAMP
 
 from ._constants import (
     FUGUE_TRINO_CONF_TEMP_SCHEMA,
     FUGUE_TRINO_CONF_TEMP_SCHEMA_DEFAULT_NAME,
@@ -44,29 +42,16 @@
         ptp = ibis_to_pa_type(tp)
         if _is_default_timestamp(ptp):
             ptp = TRIAD_DEFAULT_TIMESTAMP
         fields.append(pa.field(n, ptp))
     return Schema(fields)
 
 
-def to_ibis_schema(schema: Schema) -> ibis.Schema:
-    fields = [(f.name, _pa_to_ibis_type(f.type)) for f in schema.fields]
-    return ibis.schema(fields)
-
-
 def is_select_query(s: str) -> bool:
     return (
         re.match(r"^\s*select\s", s, re.IGNORECASE) is not None
         or re.match(r"^\s*with\s", s, re.IGNORECASE) is not None
     )
 
 
 def _is_default_timestamp(tp: pa.DataType) -> bool:
     return pa.types.is_timestamp(tp) and str(tp.tz).lower() == "utc"
-
-
-def _pa_to_ibis_type(tp: pa.DataType) -> dt.DataType:
-    if pa.types.is_timestamp(tp):
-        if tp.tz is None:
-            return dt.Timestamp(scale=6)
-        return dt.Timestamp(scale=6, timezone=str(tp.tz))
-    return pa_to_ibis_type(tp)
```

### Comparing `fugue-warehouses-0.0.3/fugue_trino/client.py` & `fugue-warehouses-0.0.3.dev1/fugue_trino/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from uuid import uuid4
 
 import fugue.api as fa
 import ibis
 import numpy as np
 from fugue import AnyDataFrame
 from fugue_ibis import IbisDataFrame, IbisTable
+from fugue_ibis._utils import to_ibis_schema
 from ibis import BaseBackend
 from sqlalchemy import exc as sa_exc
 from triad import ParamDict, SerializableRLock, assert_or_throw
 from trino.auth import BasicAuthentication
 from trino.dbapi import Connection as TrinoConnection
 from trino.dbapi import Cursor as TrinoCursor
 from trino.dbapi import connect
@@ -22,20 +23,15 @@
     FUGUE_TRINO_CONF_CATALOG,
     FUGUE_TRINO_CONF_HOST,
     FUGUE_TRINO_CONF_PASSWORD,
     FUGUE_TRINO_CONF_PORT,
     FUGUE_TRINO_CONF_USER,
     FUGUE_TRINO_ENV_PASSWORD,
 )
-from ._utils import (
-    get_temp_schema,
-    is_select_query,
-    is_trino_ibis_table,
-    to_ibis_schema,
-)
+from ._utils import get_temp_schema, is_trino_ibis_table, is_select_query
 from .collections import TableName
 
 _FUGUE_TRINO_CLIENT_CONTEXT = ContextVar("_FUGUE_TRINO_CLIENT_CONTEXT", default=None)
 
 _CONTEXT_LOCK = SerializableRLock()
 
 
@@ -104,16 +100,14 @@
                 auth=BasicAuthentication(user, password),
                 http_scheme="https",
             )
         else:
             self._trino_con = connect(host=host, port=port, user=user)
         self._con_lock = SerializableRLock()
         self._schema_backends: Dict[str, BaseBackend] = {}
-        self.sql(f"CREATE SCHEMA IF NOT EXISTS {catalog}.{self._temp_schema}")
-        self.sql(f"USE {catalog}.{self._temp_schema}")
 
     @property
     def catalog(self) -> str:
         return self._catalog
 
     @property
     def connection(self) -> TrinoConnection:
@@ -154,28 +148,26 @@
         fdf = fa.as_fugue_df(df)
         con = self.connect_to_schema(tb.schema)
         try:
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore", category=sa_exc.SAWarning)
                 if isinstance(fdf, IbisDataFrame) and is_trino_ibis_table(fdf.native):
                     obj: Any = fdf.native
-                    query = f"CREATE OR REPLACE VIEW {tb} AS " + fdf.to_sql()
-                    self.sql(query)
                 else:
                     obj = fdf.as_pandas().replace({np.nan: None})
                     if len(obj) == 0:
                         obj = None
                     else:
                         obj = ibis.memtable(obj, schema=to_ibis_schema(fdf.schema))
-                    con.create_table(
-                        tb.table,
-                        obj,
-                        schema=to_ibis_schema(fdf.schema),
-                        overwrite=overwrite,
-                    )
+                con.create_table(
+                    tb.table,
+                    obj,
+                    schema=to_ibis_schema(fdf.schema),
+                    overwrite=overwrite,
+                )
         except HttpError:  # pragma: no cover
             pass
         return tb
 
     def query_to_ibis(self, query: Any) -> IbisTable:
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", category=sa_exc.SAWarning)
```

### Comparing `fugue-warehouses-0.0.3/fugue_trino/collections.py` & `fugue-warehouses-0.0.3.dev1/fugue_trino/collections.py`

 * *Files identical despite different names*

### Comparing `fugue-warehouses-0.0.3/fugue_trino/dataframe.py` & `fugue-warehouses-0.0.3.dev1/fugue_trino/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-warehouses-0.0.3/fugue_trino/execution_engine.py` & `fugue-warehouses-0.0.3.dev1/fugue_trino/execution_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     def backend(self) -> ibis.BaseBackend:
         return self.client.ibis
 
     def encode_column_name(self, name: str) -> str:
         return '"' + name.replace('"', '\\"') + '"'
 
     def get_temp_table_name(self) -> str:
-        return str(self.client.to_table_name(None))
+        return str(self.client.to_table_name(super().get_temp_table_name()))
 
     def to_df(self, df: Any, schema: Any = None) -> IbisDataFrame:
         if isinstance(df, TrinoDataFrame):
             assert_or_throw(
                 schema is None,
                 ValueError("schema must be None when df is TrinoDataFrame"),
             )
```

### Comparing `fugue-warehouses-0.0.3/fugue_trino/ibis_trino/backend.py` & `fugue-warehouses-0.0.3.dev1/fugue_trino/ibis_trino/backend.py`

 * *Files identical despite different names*

### Comparing `fugue-warehouses-0.0.3/fugue_trino/registry.py` & `fugue-warehouses-0.0.3.dev1/fugue_trino/registry.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,43 @@
 from typing import Any, Optional, Tuple
 
 import fugue.plugins as fp
-import fugue.api as fa
 from fugue import DataFrame, ExecutionEngine, SQLEngine, is_pandas_or
-from triad import ParamDict, Schema
-from fugue_ibis import IbisTable
-from ._utils import is_trino_ibis_table, is_trino_repr, to_schema
+from triad import ParamDict
+
+from ._utils import is_trino_ibis_table, is_trino_repr
 from .client import TrinoClient
 from .dataframe import TrinoDataFrame
 from .execution_engine import TrinoExecutionEngine, TrinoSQLEngine
 
 
 @fp.as_fugue_dataset.candidate(lambda query, **kwargs: is_trino_repr(query))
 def _trino_to_df(query: Tuple[str, str], **kwargs: Any) -> DataFrame:
     return TrinoDataFrame(TrinoClient.get_current().query_to_ibis(query[1]))
 
 
-@fp.is_df.candidate(lambda df: is_trino_ibis_table(df) or is_trino_repr(df))
-def _is_trino_df(df: Any):
-    return True
-
-
-@fp.get_schema.candidate(lambda df: is_trino_ibis_table(df) or is_trino_repr(df))
-def _trino_get_schema(df: Any) -> Schema:
-    """Get the schema of certain query or table
-
-    :param query_or_table: the table name or query string
-    :return: the schema of the output
-    """
-    if isinstance(df, IbisTable):
-        return to_schema(df.schema())
-    client = TrinoClient.get_or_create(fa.get_current_conf())
-    return to_schema(client.query_to_ibis(df[1]).schema())
+@fp.parse_creator.candidate(is_trino_repr)
+def _parse_trino_creator(query: Tuple[str, str]):
+    def _creator() -> DataFrame:
+        return _trino_to_df(query)
+
+    return _creator
 
 
 @fp.parse_execution_engine.candidate(
     matcher=lambda engine, conf, **kwargs: isinstance(engine, str)
     and engine == "trino",
     priority=2.5,
 )
 def _parse_trino(engine: str, conf: Any, **kwargs) -> ExecutionEngine:
     _conf = ParamDict(conf)
     client = TrinoClient.get_or_create(_conf)
     return TrinoExecutionEngine(client, _conf)
 
 
-@fp.parse_execution_engine.candidate(
-    lambda engine, conf, **kwargs: isinstance(engine, TrinoClient)
-)
-def _parse_trino_client(engine: TrinoClient, conf: Any, **kwargs) -> ExecutionEngine:
-    return TrinoExecutionEngine(engine, conf)
-
-
 @fp.infer_execution_engine.candidate(
     lambda objs: is_pandas_or(objs, TrinoDataFrame)
     or any(
         is_trino_ibis_table(x)
         or (isinstance(x, str) and x == "force_trino")
         or is_trino_repr(x)
         for x in objs
```

### Comparing `fugue-warehouses-0.0.3/fugue_warehouses.egg-info/PKG-INFO` & `fugue-warehouses-0.0.3.dev1/fugue_warehouses.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue-warehouses
-Version: 0.0.3
+Version: 0.0.3.dev1
 Summary: Fugue data warehouses integration
 Home-page: http://github.com/fugue-project/fugue-warehouses
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue Data Warehouses Integration
```

### Comparing `fugue-warehouses-0.0.3/fugue_warehouses.egg-info/SOURCES.txt` & `fugue-warehouses-0.0.3.dev1/fugue_warehouses.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 fugue_bigquery/dataframe.py
 fugue_bigquery/execution_engine.py
 fugue_bigquery/ray_execution_engine.py
 fugue_bigquery/registry.py
 fugue_trino/__init__.py
 fugue_trino/_constants.py
 fugue_trino/_utils.py
-fugue_trino/api.py
 fugue_trino/client.py
 fugue_trino/collections.py
 fugue_trino/dataframe.py
 fugue_trino/execution_engine.py
 fugue_trino/registry.py
 fugue_trino/ibis_trino/__init__.py
 fugue_trino/ibis_trino/backend.py
```

### Comparing `fugue-warehouses-0.0.3/setup.py` & `fugue-warehouses-0.0.3.dev1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,26 +28,26 @@
     author="The Fugue Development Team",
     author_email="hello@fugue.ai",
     keywords="fugue data warehouses bigquery trino sql",
     url="http://github.com/fugue-project/fugue-warehouses",
     install_requires=[],
     extras_require={
         "bigquery": [
-            "fugue[ibis]>=0.8.4",
+            "fugue[ibis]>=0.8.1",
             "fs-gcsfs",
             "pandas-gbq",
             "google-auth",
             "db-dtypes",
             "ibis-framework[bigquery]",
         ],
         "trino": [
-            "fugue[ibis]>=0.8.4",
+            "fugue[ibis]>=0.8.1",
             "ibis-framework[trino]",
         ],
-        "ray": ["fugue[ray]>=0.8.4"],
+        "ray": ["fugue[ray]>=0.8.1"],
     },
     classifiers=[
         # "3 - Alpha", "4 - Beta" or "5 - Production/Stable"
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `fugue-warehouses-0.0.3/tests/fugue_bigquery/mock_engine.py` & `fugue-warehouses-0.0.3.dev1/tests/fugue_bigquery/mock_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-warehouses-0.0.3/tests/fugue_bigquery/test_api.py` & `fugue-warehouses-0.0.3.dev1/tests/fugue_bigquery/test_api.py`

 * *Files identical despite different names*

### Comparing `fugue-warehouses-0.0.3/tests/fugue_bigquery/test_dataframe.py` & `fugue-warehouses-0.0.3.dev1/tests/fugue_bigquery/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-warehouses-0.0.3/tests/fugue_bigquery/test_execution_engine.py` & `fugue-warehouses-0.0.3.dev1/tests/fugue_bigquery/test_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-warehouses-0.0.3/tests/fugue_bigquery/test_workflow.py` & `fugue-warehouses-0.0.3.dev1/tests/fugue_bigquery/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-warehouses-0.0.3/tests/fugue_trino/_utils.py` & `fugue-warehouses-0.0.3.dev1/tests/fugue_trino/_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Optional
 
 from fugue import DataFrame
+from triad import to_uuid
 
 from fugue_trino import TrinoClient, TrinoExecutionEngine
 from fugue_trino._constants import FUGUE_TRINO_CONF_TEMP_SCHEMA_DEFAULT_NAME
 
 
 def get_testing_client():
     client = TrinoClient.get_or_create(
@@ -24,8 +25,16 @@
 
 class MockTrinoExecutionEngine(TrinoExecutionEngine):
     def __init__(self, client: Optional[TrinoClient] = None, conf: Any = None):
         super().__init__(client, conf)
         self._cache = {}
 
     def to_df(self, df: Any, schema: Any = None) -> DataFrame:
-        return super().sql_engine.to_df(df, schema)
+        if isinstance(df, list):
+            key = to_uuid(df, schema)
+        else:
+            key = to_uuid(id(df), schema)
+        if key in self._cache:
+            return self._cache[key]
+        res = super().sql_engine.to_df(df, schema)
+        self._cache[key] = res
+        return res
```

### Comparing `fugue-warehouses-0.0.3/tests/fugue_trino/test_api.py` & `fugue-warehouses-0.0.3.dev1/tests/fugue_trino/test_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,22 @@
 import fugue.api as fa
-import pandas as pd
-from fugue_ibis import IbisTable
-
-import fugue_trino.api as fta
-from fugue_trino import TrinoDataFrame
-
 from ._utils import get_testing_client
-import ray
-from fugue_ray import RayDataFrame
-import ray.data as rd
+import pandas as pd
 
 
-def test_fugue_api():
+def test_api():
     def tr(df: pd.DataFrame) -> pd.DataFrame:
         return df
 
     with get_testing_client() as client:
         df1 = fa.as_fugue_df([["a", 1], ["b", 2]], schema="x:str,b:long")
         tb1 = str(client.df_to_table(df1))
-        assert fa.get_schema(("trino", tb1)) == "x:str,b:long"
-        assert fa.get_schema(client.query_to_ibis(tb1)) == "x:str,b:long"
         df2 = fa.as_fugue_df([["a", True], ["c", False]], schema="x:str,c:bool")
         tb2 = str(client.df_to_table(df2))
         fa.show(("trino", tb1))
         res = fa.inner_join(("trino", tb1), ("trino", tb2), as_fugue=True)
         assert [["a", 1, True]] == res.as_array()
         assert [["b", 2]] == fa.as_array(("trino", f"SELECT * FROM {tb1} WHERE b=2"))
         assert 1 == fa.count(("trino", f"SELECT * FROM {tb1} WHERE b=2"))
         res = fa.transform(res, tr, schema="*")
         assert [["a", 1, True]] == res.as_array()
         assert 2 == fa.count(fa.transform(("trino", tb1), tr, schema="*"))
-
-
-def test_load():
-    with get_testing_client() as client:
-        df1 = fa.as_fugue_df([["a", 1], ["b", 2]], schema="x:str,b:long")
-        tb1 = str(client.df_to_table(df1))
-        with fa.engine_context(client):
-            df = fta.load(tb1)
-            assert isinstance(df, IbisTable)
-            df = fta.load(tb1, as_fugue=True)
-            assert isinstance(df, TrinoDataFrame)
-
-        with ray.init():
-            with fa.engine_context("ray"):
-                df = fta.load(tb1, parallelism=5)
-                assert isinstance(df, rd.Dataset)
-                df = fta.load(tb1, parallelism=5, as_fugue=True)
-                assert isinstance(df, RayDataFrame)
-                assert df.num_partitions == 5
```

### Comparing `fugue-warehouses-0.0.3/tests/fugue_trino/test_collections.py` & `fugue-warehouses-0.0.3.dev1/tests/fugue_trino/test_collections.py`

 * *Files identical despite different names*

### Comparing `fugue-warehouses-0.0.3/tests/fugue_trino/test_dataframe.py` & `fugue-warehouses-0.0.3.dev1/tests/fugue_trino/test_dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from fugue_trino import TrinoDataFrame
 
 from ._utils import MockTrinoExecutionEngine, get_testing_client
 
 
 @pytest.mark.skipif(sys.version_info < (3, 8), reason="< 3.8")
-class TrinoDataFrameTests(DataFrameTests.Tests):
+class BigQueryDataFrameTests(DataFrameTests.Tests):
     @classmethod
     def setUpClass(cls):
         cls._client = get_testing_client()
         cls._engine = MockTrinoExecutionEngine(cls._client)
         cls._cache = {}
 
     @classmethod
```

### Comparing `fugue-warehouses-0.0.3/tests/fugue_trino/test_execution_engine.py` & `fugue-warehouses-0.0.3.dev1/tests/fugue_trino/test_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-warehouses-0.0.3/tests/fugue_trino/test_workflow.py` & `fugue-warehouses-0.0.3.dev1/tests/fugue_trino/test_workflow.py`

 * *Files identical despite different names*

