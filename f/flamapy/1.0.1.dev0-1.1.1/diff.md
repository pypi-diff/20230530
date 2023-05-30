# Comparing `tmp/flamapy-1.0.1.dev0.tar.gz` & `tmp/flamapy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamapy-1.0.1.dev0.tar", last modified: Sat Aug 13 17:00:47 2022, max compression
+gzip compressed data, was "flamapy-1.1.1.tar", last modified: Tue May 30 16:40:14 2023, max compression
```

## Comparing `flamapy-1.0.1.dev0.tar` & `flamapy-1.1.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:47.798804 flamapy-1.0.1.dev0/
--rw-r--r--   0 runner    (1001) docker     (121)     2007 2022-08-13 17:00:47.798804 flamapy-1.0.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:47.790804 flamapy-1.0.1.dev0/flamapy/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:47.790804 flamapy-1.0.1.dev0/flamapy/commands/
--rw-r--r--   0 runner    (1001) docker     (121)     2595 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:47.790804 flamapy-1.0.1.dev0/flamapy/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    10151 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/discover.py
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:47.794804 flamapy-1.0.1.dev0/flamapy/core/models/
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11605 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/models/ast.py
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/models/variability_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:47.794804 flamapy-1.0.1.dev0/flamapy/core/operations/
--rw-r--r--   0 runner    (1001) docker     (121)     1777 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/abstract_operation.py
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/atomic_sets.py
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/average_branching_factor.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/commonality.py
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/core_features.py
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/count_leafs.py
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/dead_features.py
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/error_detection.py
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/error_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/estimated_products_number.py
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/false_optional_features.py
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/filter.py
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/products.py
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/products_number.py
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/sampling.py
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/valid.py
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/valid_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/valid_product.py
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/operations/variability.py
--rw-r--r--   0 runner    (1001) docker     (121)     6538 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:47.794804 flamapy-1.0.1.dev0/flamapy/core/transformations/
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/transformations/abstract_transformation.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/transformations/model_to_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/transformations/model_to_text.py
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/transformations/text_to_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:47.794804 flamapy-1.0.1.dev0/flamapy/endpoint/
--rw-r--r--   0 runner    (1001) docker     (121)     2011 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/endpoint/diverso_lab.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:47.790804 flamapy-1.0.1.dev0/flamapy/metamodels/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:47.794804 flamapy-1.0.1.dev0/flamapy/metamodels/configuration_metamodel/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/metamodels/configuration_metamodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:47.794804 flamapy-1.0.1.dev0/flamapy/metamodels/configuration_metamodel/models/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/metamodels/configuration_metamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/metamodels/configuration_metamodel/models/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:47.798804 flamapy-1.0.1.dev0/flamapy/metamodels/configuration_metamodel/transformations/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/metamodels/configuration_metamodel/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/flamapy/metamodels/configuration_metamodel/transformations/configuration_basic_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:47.790804 flamapy-1.0.1.dev0/flamapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2007 2022-08-13 17:00:47.000000 flamapy-1.0.1.dev0/flamapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-08-13 17:00:47.000000 flamapy-1.0.1.dev0/flamapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-13 17:00:47.000000 flamapy-1.0.1.dev0/flamapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-08-13 17:00:47.000000 flamapy-1.0.1.dev0/flamapy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-08-13 17:00:47.000000 flamapy-1.0.1.dev0/flamapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-13 17:00:47.000000 flamapy-1.0.1.dev0/flamapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-13 17:00:47.798804 flamapy-1.0.1.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-08-13 17:00:34.000000 flamapy-1.0.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:40:14.543375 flamapy-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-30 16:40:14.543375 flamapy-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-30 16:39:55.000000 flamapy-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:40:14.531375 flamapy-1.1.1/flamapy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:40:14.535375 flamapy-1.1.1/flamapy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:40:14.535375 flamapy-1.1.1/flamapy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:40:14.535375 flamapy-1.1.1/flamapy/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/models/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/models/variability_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:40:14.539375 flamapy-1.1.1/flamapy/core/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/abstract_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/atomic_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/average_branching_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/commonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/core_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/count_leafs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/dead_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/error_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/error_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/estimated_products_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/false_optional_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/products.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/products_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/valid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/valid_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/valid_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/operations/variability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:40:14.539375 flamapy-1.1.1/flamapy/core/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/transformations/abstract_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/transformations/model_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/transformations/model_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/transformations/text_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:40:14.539375 flamapy-1.1.1/flamapy/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/endpoint/diverso_lab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:40:14.531375 flamapy-1.1.1/flamapy/metamodels/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:40:14.539375 flamapy-1.1.1/flamapy/metamodels/configuration_metamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/metamodels/configuration_metamodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:40:14.543375 flamapy-1.1.1/flamapy/metamodels/configuration_metamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/metamodels/configuration_metamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/metamodels/configuration_metamodel/models/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:40:14.543375 flamapy-1.1.1/flamapy/metamodels/configuration_metamodel/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/metamodels/configuration_metamodel/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-30 16:39:55.000000 flamapy-1.1.1/flamapy/metamodels/configuration_metamodel/transformations/configuration_basic_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:40:14.535375 flamapy-1.1.1/flamapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-30 16:40:14.000000 flamapy-1.1.1/flamapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-30 16:40:14.000000 flamapy-1.1.1/flamapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:40:14.000000 flamapy-1.1.1/flamapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-30 16:40:14.000000 flamapy-1.1.1/flamapy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-30 16:40:14.000000 flamapy-1.1.1/flamapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 16:40:14.000000 flamapy-1.1.1/flamapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 16:40:14.543375 flamapy-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-30 16:39:55.000000 flamapy-1.1.1/setup.py
```

### Comparing `flamapy-1.0.1.dev0/PKG-INFO` & `flamapy-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy
-Version: 1.0.1.dev0
+Version: 1.1.1
 Summary: Flamapy is a Python-based AAFM framework that takes into consideration previous AAFM tool designs and enables multi-solver and multi-metamodel support for the integration of AAFM tooling on the Python ecosystem.
 Home-page: https://github.com/flamapy/core
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -25,15 +25,15 @@
 
 ## Available plugins
 [flamapy-fm](https://github.com/flamapy/fm_metamodel)
 [flamapy-sat](https://github.com/flamapy/pysat_metamodel)
 
 ## Documentation
 
-All the proyect related documentation can be found in wiki format at [wiki](https://github.com/diverso-lab/core/wiki)
+All the proyect related documentation can be found in wiki format at [the tool website](https://flamapy.github.io/)
 
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/diverso-lab/core/releases)
 
 ## Contributing
 
 See [CONTRIBUTING.md](https://github.com/diverso-lab/core/blob/master/CONTRIBUTING.md)
```

### Comparing `flamapy-1.0.1.dev0/README.md` & `flamapy-1.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 ## Available plugins
 [flamapy-fm](https://github.com/flamapy/fm_metamodel)
 [flamapy-sat](https://github.com/flamapy/pysat_metamodel)
 
 ## Documentation
 
-All the proyect related documentation can be found in wiki format at [wiki](https://github.com/diverso-lab/core/wiki)
+All the proyect related documentation can be found in wiki format at [the tool website](https://flamapy.github.io/)
 
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/diverso-lab/core/releases)
 
 ## Contributing
 
 See [CONTRIBUTING.md](https://github.com/diverso-lab/core/blob/master/CONTRIBUTING.md)
```

### Comparing `flamapy-1.0.1.dev0/flamapy/commands/__init__.py` & `flamapy-1.1.1/flamapy/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `flamapy-1.0.1.dev0/flamapy/core/discover.py` & `flamapy-1.1.1/flamapy/core/discover.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 import logging
 from importlib import import_module
 from pkgutil import iter_modules
 from types import ModuleType
-from typing import Any, Optional, Protocol, Type, runtime_checkable
+from typing import Any, Optional, Protocol, Type, runtime_checkable, cast
 
 from flamapy.core.config import PLUGIN_PATHS
 from flamapy.core.exceptions import OperationNotFound
 from flamapy.core.exceptions import TransformationNotFound
 from flamapy.core.exceptions import ConfigurationNotFound
 from flamapy.core.models import VariabilityModel
 from flamapy.core.operations import Operation
@@ -166,14 +166,18 @@
         plugin = self.plugins.get_plugin_by_extension(dst)
         return plugin.use_transformation_t2m(src)
 
     def use_transformation_m2m(self, src: VariabilityModel, dst: str) -> VariabilityModel:
         plugin = self.plugins.get_plugin_by_extension(dst)
         return plugin.use_transformation_m2m(src, dst)
 
+    def get_operation(self, src: VariabilityModel, operation_name: str) -> Operation:
+        plugin = self.plugins.get_plugin_by_variability_model(src)
+        return plugin.get_operation(operation_name)
+
     def use_operation(self, src: VariabilityModel, operation_name: str) -> Operation:
         plugin = self.plugins.get_plugin_by_variability_model(src)
         operation = plugin.get_operation(operation_name)
         return plugin.use_operation(operation, src)
 
     def use_operation_from_file(
         self,
@@ -204,15 +208,15 @@
                     plugin = _plugin
 
         operation = plugin.get_operation(operation_name)
         if isinstance(operation, OperationWithConfiguration):
             if configuration_file is None:
                 raise ConfigurationNotFound()
             configuration = self.__transform_to_model_from_file(configuration_file)
-            operation.set_configuration(configuration)
+            operation.set_configuration(cast(Configuration, configuration))
 
         operation = plugin.use_operation(operation, vm_temp)
 
         return operation.get_result()
 
     def __transform_to_model_from_file(self, file: str) -> VariabilityModel:
         t2m_transformations = self.get_transformations_t2m()
@@ -271,8 +275,8 @@
 
         for _plugin in plugins_with_operation:
             output_extension = _plugin.get_extension()
             way = __search_recursive_way(input_extension, output_extension, [])
             if way and output_extension == way[-1][1]:
                 return way
 
-        raise NotImplementedError('Way to execute operation not found')
+        raise NotImplementedError('Way to execute operation not found')
```

### Comparing `flamapy-1.0.1.dev0/flamapy/core/models/ast.py` & `flamapy-1.1.1/flamapy/core/models/ast.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,19 +130,19 @@
     right = ast.root.right
     if logic_op in (ASTOperation.REQUIRES, ASTOperation.IMPLIES):
         # Replace P => Q with !P v Q.
         left = simplify_formula(AST(left)).root
         right = simplify_formula(AST(right)).root
         result = AST.create_binary_operation(ASTOperation.OR, Node(ASTOperation.NOT, left), right)
     elif logic_op == ASTOperation.EXCLUDES:
-        # Replace P EXCLUDES Q with P => !Q.
+        # Replace P EXCLUDES Q with !P v !Q.
         left = simplify_formula(AST(left)).root
         right = simplify_formula(AST(right)).root
-        result = AST.create_binary_operation(ASTOperation.IMPLIES,
-                                             left, Node(ASTOperation.NOT, right))
+        result = AST.create_binary_operation(ASTOperation.OR, Node(ASTOperation.NOT, left), 
+                                             Node(ASTOperation.NOT, right))
     elif logic_op == ASTOperation.EQUIVALENCE:
         # Replace P <=> Q with P => Q ∧ Q => P.
         left = simplify_formula(AST.create_binary_operation(ASTOperation.IMPLIES,
                                                             left, right)).root
         right = simplify_formula(AST.create_binary_operation(ASTOperation.IMPLIES,
                                                              right, left)).root
         result = AST.create_binary_operation(ASTOperation.AND, left, right)
```

### Comparing `flamapy-1.0.1.dev0/flamapy/core/operations/__init__.py` & `flamapy-1.1.1/flamapy/core/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `flamapy-1.0.1.dev0/flamapy/core/operations/atomic_sets.py` & `flamapy-1.1.1/flamapy/core/operations/atomic_sets.py`

 * *Files identical despite different names*

### Comparing `flamapy-1.0.1.dev0/flamapy/core/operations/false_optional_features.py` & `flamapy-1.1.1/flamapy/core/operations/false_optional_features.py`

 * *Files identical despite different names*

### Comparing `flamapy-1.0.1.dev0/flamapy/core/operations/sampling.py` & `flamapy-1.1.1/flamapy/core/operations/sampling.py`

 * *Files identical despite different names*

### Comparing `flamapy-1.0.1.dev0/flamapy/core/plugins.py` & `flamapy-1.1.1/flamapy/core/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,17 @@
             self.data
         )
 
         try:
             operation = next(candidates, None)
         except StopIteration:
             raise OperationNotFound from StopIteration
-        else:
-            if not operation:
-                raise OperationNotFound
+
+        if not operation:
+            raise OperationNotFound
         return operation
 
 
 class Plugin:
 
     def __init__(self, module: ModuleType) -> None:
         self.module: ModuleType = module
@@ -54,17 +54,17 @@
         filter_transformation: Callable[..., bool]
     ) -> Type[Transformation]:
         candidates = filter(filter_transformation, self.transformations)
         try:
             transformation = next(candidates, None)
         except StopIteration:
             raise TransformationNotFound from StopIteration
-        else:
-            if not transformation:
-                raise TransformationNotFound
+
+        if not transformation:
+            raise TransformationNotFound
         return transformation
 
     def append_operation(self, operation: Type[Operation]) -> None:
         self.operations.append(operation)
 
     def append_transformations(self, transformation: Type[Transformation]) -> None:
         self.transformations.append(transformation)
```

### Comparing `flamapy-1.0.1.dev0/flamapy/endpoint/diverso_lab.py` & `flamapy-1.1.1/flamapy/endpoint/diverso_lab.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,50 +13,47 @@
 
 PluginsType = NewType('PluginsType', dict[str, list[str]])
 OperationDict = NewType('OperationDict', dict[str, list[str]])
 OperationResult = NewType('OperationResult', dict[str, Any])
 
 
 @hug.cli()
-@hug.get('/get-plugins/', versions=1)
+@hug.get('/get-plugins/')
 def get_plugins() -> PluginsType:
     """ Get availables plugins """
     plugins = dm.get_plugins()
     return PluginsType({'plugins': plugins})
 
 
 @hug.cli()
 @hug.get('/get-operations/{plugin}/')
-def get_operations_name_by_plugin(plugin: str, versions: int = 1) -> OperationDict:
+def get_operations_name_by_plugin(plugin: str) -> OperationDict:
     """ Get availables operations gave a plugin name """
     operations = dm.get_name_operations_by_plugin(plugin)
     return OperationDict({'operations': operations})
 
 
 @hug.cli()
 @hug.get('/use-operation-from-file/{operation}/{filename}/')
 def use_operation_from_file(
     operation: str,
     filename: str,
     plugin: Optional[str] = None,
-    versions: int = 1
+    configuration_file: Optional[str] = None,
 ) -> OperationResult:
     """
     Execute an operation gave an operation and one input file. Optionally you
     can give a plugin as last parameter.
     """
     try:
-        result = dm.use_operation_from_file(operation, filename, plugin)
+        result = dm.use_operation_from_file(operation, filename, plugin, configuration_file)
+        return OperationResult({'result': result})
     except OperationNotFound:
         return OperationResult({'Error': 'Operation not found'})
     except PluginNotFound:
         return OperationResult({'Error': 'Plugin not found'})
     except TransformationNotFound:
         return OperationResult({'Error': 'Transformation not found'})
     except FileNotFoundError:
         return OperationResult({'Error': 'File not found'})
     except ConfigurationNotFound:
-        return OperationResult({'Error': 'Configuration file not found'})
-    except Exception:
-        return OperationResult({'Error': 'Unexpected error'})
-
-    return OperationResult({'result': result})
+        return OperationResult({'Error': 'Configuration file not found'})
```

### Comparing `flamapy-1.0.1.dev0/flamapy/metamodels/configuration_metamodel/models/configuration.py` & `flamapy-1.1.1/flamapy/metamodels/configuration_metamodel/models/configuration.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 
 
 class Configuration(VariabilityModel):
 
     @staticmethod
     def get_extension() -> str:
         return 'configuration'
-    """A configuration is a selection of elements in a variability model.
-
-    It is represented as a dictionary of elements of Any type -> bool.
-    """
 
     def __init__(self, elements: dict[Any, bool]) -> None:
         self.elements = elements
 
     def get_selected_elements(self) -> list[Any]:
         return [e for e in self.elements if self.elements[e]]
```

### Comparing `flamapy-1.0.1.dev0/flamapy/metamodels/configuration_metamodel/transformations/configuration_basic_reader.py` & `flamapy-1.1.1/flamapy/metamodels/configuration_metamodel/transformations/configuration_basic_reader.py`

 * *Files identical despite different names*

### Comparing `flamapy-1.0.1.dev0/flamapy.egg-info/PKG-INFO` & `flamapy-1.1.1/flamapy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy
-Version: 1.0.1.dev0
+Version: 1.1.1
 Summary: Flamapy is a Python-based AAFM framework that takes into consideration previous AAFM tool designs and enables multi-solver and multi-metamodel support for the integration of AAFM tooling on the Python ecosystem.
 Home-page: https://github.com/flamapy/core
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -25,15 +25,15 @@
 
 ## Available plugins
 [flamapy-fm](https://github.com/flamapy/fm_metamodel)
 [flamapy-sat](https://github.com/flamapy/pysat_metamodel)
 
 ## Documentation
 
-All the proyect related documentation can be found in wiki format at [wiki](https://github.com/diverso-lab/core/wiki)
+All the proyect related documentation can be found in wiki format at [the tool website](https://flamapy.github.io/)
 
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/diverso-lab/core/releases)
 
 ## Contributing
 
 See [CONTRIBUTING.md](https://github.com/diverso-lab/core/blob/master/CONTRIBUTING.md)
```

### Comparing `flamapy-1.0.1.dev0/flamapy.egg-info/SOURCES.txt` & `flamapy-1.1.1/flamapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flamapy-1.0.1.dev0/setup.py` & `flamapy-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="flamapy",
-    version="1.0.1.dev0",
+    version="1.1.1",
     author="Flamapy",
     author_email="flamapy@us.es",
     description="Flamapy is a Python-based AAFM framework that takes into consideration previous AAFM tool designs and enables multi-solver and multi-metamodel support for the integration of AAFM tooling on the Python ecosystem.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/flamapy/core",
     packages=setuptools.find_namespace_packages(include=['flamapy.*']),
```

