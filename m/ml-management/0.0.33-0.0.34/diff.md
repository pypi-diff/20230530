# Comparing `tmp/ml-management-0.0.33.tar.gz` & `tmp/ml-management-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-management-0.0.33.tar", last modified: Mon May 29 06:00:27 2023, max compression
+gzip compressed data, was "ml-management-0.0.34.tar", last modified: Tue May 30 12:44:33 2023, max compression
```

## Comparing `ml-management-0.0.33.tar` & `ml-management-0.0.34.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.799593 ml-management-0.0.33/
--rw-rw-r--   0 denis     (1000) denis     (1000)       18 2023-04-17 13:42:26.000000 ml-management-0.0.33/MANIFEST.in
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.795593 ml-management-0.0.33/ML_management/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2022-10-04 18:14:32.000000 ml-management-0.0.33/ML_management/__init__.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.795593 ml-management-0.0.33/ML_management/collectors/
--rw-rw-r--   0 denis     (1000) denis     (1000)      120 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1092 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/collector_pattern.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      456 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/collector_pattern_to_methods_map.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      509 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/collectors.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.795593 ml-management-0.0.33/ML_management/collectors/dummy/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/dummy/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      463 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/dummy/dummy_collector.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.795593 ml-management-0.0.33/ML_management/collectors/s3/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/s3/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)    10557 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/s3/s3collector.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.795593 ml-management-0.0.33/ML_management/collectors/topic_markers/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/topic_markers/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)   331440 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/topic_markers/api_schema.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     3167 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/topic_markers/topic_markers_collector.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.795593 ml-management-0.0.33/ML_management/dataset_loader_template/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/dataset_loader_template/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2407 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/dataset_loader_template/dataset_loader_pattern.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      457 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.795593 ml-management-0.0.33/ML_management/executor_template/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/executor_template/__init__.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.795593 ml-management-0.0.33/ML_management/executor_template/default_executors/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/executor_template/default_executors/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      895 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/executor_template/default_executors/finetune_executor.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      843 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/executor_template/default_executors/test_executor.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      869 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/executor_template/default_executors/train_executor.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     4566 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/executor_template/executor_pattern.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      402 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/executor_template/executor_pattern_to_methods_map.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      334 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/executor_template/upload_model_mode.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.795593 ml-management-0.0.33/ML_management/mlmanagement/
--rw-rw-r--   0 denis     (1000) denis     (1000)      581 2023-04-26 06:58:05.000000 ml-management-0.0.33/ML_management/mlmanagement/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     3392 2023-05-11 13:44:22.000000 ml-management-0.0.33/ML_management/mlmanagement/jsonschema_exceptions.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     5054 2023-05-11 13:44:22.000000 ml-management-0.0.33/ML_management/mlmanagement/jsonschema_inference.py
--rw-rw-r--   0 denis     (1000) denis     (1000)    12327 2023-05-26 08:34:53.000000 ml-management-0.0.33/ML_management/mlmanagement/mlmanagement.py
--rw-rw-r--   0 denis     (1000) denis     (1000)    10262 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/mlmanagement/mlmanager.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      201 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/mlmanagement/model_type.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     5001 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/mlmanagement/server_mlmanager_exceptions.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      316 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/mlmanagement/utils.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.799593 ml-management-0.0.33/ML_management/models/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2022-10-04 18:14:32.000000 ml-management-0.0.33/ML_management/models/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      949 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/models/model_type_to_methods_map.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.799593 ml-management-0.0.33/ML_management/models/patterns/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/models/patterns/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     4202 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/models/patterns/model_pattern.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      561 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/models/patterns/retrainable_model.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      445 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/models/patterns/torch_model.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      457 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/models/patterns/trainable_model.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.799593 ml-management-0.0.33/ML_management/registry/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2022-10-04 18:14:32.000000 ml-management-0.0.33/ML_management/registry/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2566 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/registry/exceptions.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     7556 2023-05-15 06:26:40.000000 ml-management-0.0.33/ML_management/registry/registry_manager.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.799593 ml-management-0.0.33/ML_management/tests/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-04-17 13:42:26.000000 ml-management-0.0.33/ML_management/tests/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     3361 2023-04-17 13:42:26.000000 ml-management-0.0.33/ML_management/tests/test_jsonschema_inference.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     9298 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/tests/test_s3_dataset.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.799593 ml-management-0.0.33/ML_management/uploader_data/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/uploader_data/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1582 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/uploader_data/s3_uploader.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      312 2023-05-29 06:00:27.799593 ml-management-0.0.33/PKG-INFO
--rw-rw-r--   0 denis     (1000) denis     (1000)       56 2022-11-02 13:55:55.000000 ml-management-0.0.33/README.md
--rw-rw-r--   0 denis     (1000) denis     (1000)        7 2023-05-29 06:00:26.000000 ml-management-0.0.33/VERSION
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.799593 ml-management-0.0.33/ml_management.egg-info/
--rw-rw-r--   0 denis     (1000) denis     (1000)      312 2023-05-29 06:00:27.000000 ml-management-0.0.33/ml_management.egg-info/PKG-INFO
--rw-rw-r--   0 denis     (1000) denis     (1000)     2449 2023-05-29 06:00:27.000000 ml-management-0.0.33/ml_management.egg-info/SOURCES.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)        1 2023-05-29 06:00:27.000000 ml-management-0.0.33/ml_management.egg-info/dependency_links.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)      142 2023-05-29 06:00:27.000000 ml-management-0.0.33/ml_management.egg-info/requires.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)       14 2023-05-29 06:00:27.000000 ml-management-0.0.33/ml_management.egg-info/top_level.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)       38 2023-05-29 06:00:27.799593 ml-management-0.0.33/setup.cfg
--rw-rw-r--   0 denis     (1000) denis     (1000)     1030 2023-05-15 06:26:38.000000 ml-management-0.0.33/setup.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.677273 ml-management-0.0.34/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       18 2023-02-15 13:35:59.000000 ml-management-0.0.34/MANIFEST.in
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.673273 ml-management-0.0.34/ML_management/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-02-15 13:35:59.000000 ml-management-0.0.34/ML_management/__init__.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.673273 ml-management-0.0.34/ML_management/collectors/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      120 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1092 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/collector_pattern.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      456 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/collector_pattern_to_methods_map.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1318 2023-05-30 12:24:50.000000 ml-management-0.0.34/ML_management/collectors/collectors.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.673273 ml-management-0.0.34/ML_management/collectors/dummy/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/dummy/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      463 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/dummy/dummy_collector.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.673273 ml-management-0.0.34/ML_management/collectors/s3/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/s3/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)    10557 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/s3/s3collector.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.673273 ml-management-0.0.34/ML_management/collectors/topic_markers/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/topic_markers/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)   331440 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/topic_markers/api_schema.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3167 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/topic_markers/topic_markers_collector.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.673273 ml-management-0.0.34/ML_management/dataset_loader_template/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/dataset_loader_template/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2407 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/dataset_loader_template/dataset_loader_pattern.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      457 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.673273 ml-management-0.0.34/ML_management/executor_template/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/executor_template/__init__.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.677273 ml-management-0.0.34/ML_management/executor_template/default_executors/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/executor_template/default_executors/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      895 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/executor_template/default_executors/finetune_executor.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      843 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/executor_template/default_executors/test_executor.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      869 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/executor_template/default_executors/train_executor.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     4566 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/executor_template/executor_pattern.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      402 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/executor_template/executor_pattern_to_methods_map.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      334 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/executor_template/upload_model_mode.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.677273 ml-management-0.0.34/ML_management/mlmanagement/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      581 2023-03-13 10:54:54.000000 ml-management-0.0.34/ML_management/mlmanagement/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3392 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/mlmanagement/jsonschema_exceptions.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     5054 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/mlmanagement/jsonschema_inference.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)    12327 2023-05-30 12:24:50.000000 ml-management-0.0.34/ML_management/mlmanagement/mlmanagement.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)    10262 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/mlmanagement/mlmanager.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      201 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/mlmanagement/model_type.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     5001 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/mlmanagement/server_mlmanager_exceptions.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      316 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/mlmanagement/utils.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.677273 ml-management-0.0.34/ML_management/models/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-02-15 13:35:59.000000 ml-management-0.0.34/ML_management/models/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      949 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/models/model_type_to_methods_map.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.677273 ml-management-0.0.34/ML_management/models/patterns/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/models/patterns/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     4202 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/models/patterns/model_pattern.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      561 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/models/patterns/retrainable_model.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      445 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/models/patterns/torch_model.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      457 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/models/patterns/trainable_model.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.677273 ml-management-0.0.34/ML_management/registry/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-02-15 13:35:59.000000 ml-management-0.0.34/ML_management/registry/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2566 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/registry/exceptions.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     7556 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/registry/registry_manager.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.677273 ml-management-0.0.34/ML_management/tests/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-02-15 13:35:59.000000 ml-management-0.0.34/ML_management/tests/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3361 2023-02-15 13:35:59.000000 ml-management-0.0.34/ML_management/tests/test_jsonschema_inference.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     9298 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/tests/test_s3_dataset.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.677273 ml-management-0.0.34/ML_management/uploader_data/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/uploader_data/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1582 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/uploader_data/s3_uploader.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      312 2023-05-30 12:44:33.677273 ml-management-0.0.34/PKG-INFO
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       56 2023-02-15 13:35:59.000000 ml-management-0.0.34/README.md
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        7 2023-05-30 12:44:18.000000 ml-management-0.0.34/VERSION
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.677273 ml-management-0.0.34/ml_management.egg-info/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      312 2023-05-30 12:44:33.000000 ml-management-0.0.34/ml_management.egg-info/PKG-INFO
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2449 2023-05-30 12:44:33.000000 ml-management-0.0.34/ml_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        1 2023-05-30 12:44:33.000000 ml-management-0.0.34/ml_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      154 2023-05-30 12:44:33.000000 ml-management-0.0.34/ml_management.egg-info/requires.txt
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       14 2023-05-30 12:44:33.000000 ml-management-0.0.34/ml_management.egg-info/top_level.txt
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       38 2023-05-30 12:44:33.677273 ml-management-0.0.34/setup.cfg
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1053 2023-05-30 12:24:50.000000 ml-management-0.0.34/setup.py
```

### Comparing `ml-management-0.0.33/ML_management/collectors/collector_pattern.py` & `ml-management-0.0.34/ML_management/collectors/collector_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/collectors/s3/s3collector.py` & `ml-management-0.0.34/ML_management/collectors/s3/s3collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/collectors/topic_markers/api_schema.py` & `ml-management-0.0.34/ML_management/collectors/topic_markers/api_schema.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/collectors/topic_markers/topic_markers_collector.py` & `ml-management-0.0.34/ML_management/collectors/topic_markers/topic_markers_collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/dataset_loader_template/dataset_loader_pattern.py` & `ml-management-0.0.34/ML_management/dataset_loader_template/dataset_loader_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/executor_template/default_executors/finetune_executor.py` & `ml-management-0.0.34/ML_management/executor_template/default_executors/finetune_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/executor_template/default_executors/test_executor.py` & `ml-management-0.0.34/ML_management/executor_template/default_executors/test_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/executor_template/default_executors/train_executor.py` & `ml-management-0.0.34/ML_management/executor_template/default_executors/train_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/executor_template/executor_pattern.py` & `ml-management-0.0.34/ML_management/executor_template/executor_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/mlmanagement/__init__.py` & `ml-management-0.0.34/ML_management/mlmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/mlmanagement/jsonschema_exceptions.py` & `ml-management-0.0.34/ML_management/mlmanagement/jsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/mlmanagement/jsonschema_inference.py` & `ml-management-0.0.34/ML_management/mlmanagement/jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/mlmanagement/mlmanagement.py` & `ml-management-0.0.34/ML_management/mlmanagement/mlmanagement.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/mlmanagement/mlmanager.py` & `ml-management-0.0.34/ML_management/mlmanagement/mlmanager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/mlmanagement/server_mlmanager_exceptions.py` & `ml-management-0.0.34/ML_management/mlmanagement/server_mlmanager_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/models/model_type_to_methods_map.py` & `ml-management-0.0.34/ML_management/models/model_type_to_methods_map.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/models/patterns/model_pattern.py` & `ml-management-0.0.34/ML_management/models/patterns/model_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/models/patterns/retrainable_model.py` & `ml-management-0.0.34/ML_management/models/patterns/retrainable_model.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/registry/exceptions.py` & `ml-management-0.0.34/ML_management/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/registry/registry_manager.py` & `ml-management-0.0.34/ML_management/registry/registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/tests/test_jsonschema_inference.py` & `ml-management-0.0.34/ML_management/tests/test_jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/tests/test_s3_dataset.py` & `ml-management-0.0.34/ML_management/tests/test_s3_dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ML_management/uploader_data/s3_uploader.py` & `ml-management-0.0.34/ML_management/uploader_data/s3_uploader.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/ml_management.egg-info/SOURCES.txt` & `ml-management-0.0.34/ml_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.33/setup.py` & `ml-management-0.0.34/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     author="ISPRAS MODIS",
     author_email="modis@ispras.ru",
     maintainer="Maxim Ryndin",
     packages=find_packages(include=["ML_management", "ML_management.*"]),
     include_package_data=True,
     # jsonschema 2.6.0 is the last one to support python 3.6
     install_requires=[
+        "sgqlc==16.1",
         "mlflow==1.21.0",
         "pandas>=0.20.1,<=1.5.2",
         "numpy>=1.8.1,<=1.23.5",
         "jsonschema==2.6.0",
         "requests_toolbelt>=0.9.1,<=0.10.1",
         "boto3==1.21.21",
         "protobuf<4.0.0",
```

