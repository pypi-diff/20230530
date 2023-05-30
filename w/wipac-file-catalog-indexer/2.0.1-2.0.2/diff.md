# Comparing `tmp/wipac-file-catalog-indexer-2.0.1.tar.gz` & `tmp/wipac-file-catalog-indexer-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wipac-file-catalog-indexer-2.0.1.tar", last modified: Fri May  5 18:02:17 2023, max compression
+gzip compressed data, was "wipac-file-catalog-indexer-2.0.2.tar", last modified: Tue May 30 16:00:28 2023, max compression
```

## Comparing `wipac-file-catalog-indexer-2.0.1.tar` & `wipac-file-catalog-indexer-2.0.2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.705388 wipac-file-catalog-indexer-2.0.1/
--rw-r--r--   0 root         (0) root         (0)     1102 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8597 2023-05-05 18:02:17.705388 wipac-file-catalog-indexer-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7567 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.689387 wipac-file-catalog-indexer-2.0.1/indexer/
--rw-r--r--   0 root         (0) root         (0)      613 2023-05-05 18:02:14.000000 wipac-file-catalog-indexer-2.0.1/indexer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6001 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/client_auth.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/config.py
--rw-r--r--   0 root         (0) root         (0)      464 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/defaults.py
--rw-r--r--   0 root         (0) root         (0)     6095 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/delocate.py
--rw-r--r--   0 root         (0) root         (0)     2958 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/generate.py
--rwxr-xr-x   0 root         (0) root         (0)    14829 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/index.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.693387 wipac-file-catalog-indexer-2.0.1/indexer/metadata/
--rw-r--r--   0 root         (0) root         (0)      155 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/metadata/basic.py
--rw-r--r--   0 root         (0) root         (0)     2344 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/metadata/i3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.693387 wipac-file-catalog-indexer-2.0.1/indexer/metadata/real/
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/metadata/real/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7431 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/metadata/real/data_exp.py
--rw-r--r--   0 root         (0) root         (0)     6170 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/metadata/real/filename_patterns.py
--rw-r--r--   0 root         (0) root         (0)     4291 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/metadata/real/l2.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/metadata/real/pfdst.py
--rw-r--r--   0 root         (0) root         (0)      945 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/metadata/real/pffilt.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/metadata/real/pfraw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.693387 wipac-file-catalog-indexer-2.0.1/indexer/metadata/simulation/
--rw-r--r--   0 root         (0) root         (0)      118 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/metadata/simulation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11209 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/metadata/simulation/data_sim.py
--rw-r--r--   0 root         (0) root         (0)   102684 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/metadata/simulation/filename_patterns.py
--rw-r--r--   0 root         (0) root         (0)    17034 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/metadata/simulation/iceprod_tools.py
--rw-r--r--   0 root         (0) root         (0)     8259 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/metadata_manager.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.697387 wipac-file-catalog-indexer-2.0.1/indexer/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3776 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/utils/file_utils.py
--rw-r--r--   0 root         (0) root         (0)     2320 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/indexer/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.685387 wipac-file-catalog-indexer-2.0.1/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.697387 wipac-file-catalog-indexer-2.0.1/resources/filename_patterns/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/resources/filename_patterns/__init__.py
--rw-r--r--   0 root         (0) root         (0)      864 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/resources/filename_patterns/by_frequency.py
--rw-r--r--   0 root         (0) root         (0)      593 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/resources/filename_patterns/example_finder.py
--rw-r--r--   0 root         (0) root         (0)    15854 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/resources/filename_patterns/filename_pattern_finder.py
--rw-r--r--   0 root         (0) root         (0)     3151 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/resources/filename_patterns/filename_pattern_regexer.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/resources/filename_patterns/fpf_stage2.1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.697387 wipac-file-catalog-indexer-2.0.1/resources/find_nonindexed/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/resources/find_nonindexed/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3819 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/resources/find_nonindexed/get_nonindexed_files.py
--rw-r--r--   0 root         (0) root         (0)     2673 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/resources/find_nonindexed/make_condor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.701388 wipac-file-catalog-indexer-2.0.1/resources/path_collector/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/resources/path_collector/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2917 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/resources/path_collector/common_args.py
--rw-r--r--   0 root         (0) root         (0)      540 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/resources/path_collector/find_unfinished.py
--rw-r--r--   0 root         (0) root         (0)    13851 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/resources/path_collector/path_collector.py
--rw-r--r--   0 root         (0) root         (0)     5394 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/resources/path_collector/path_collector_make_condor.py
--rw-r--r--   0 root         (0) root         (0)     4401 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/resources/path_collector/traverser.py
--rw-r--r--   0 root         (0) root         (0)     2537 2023-05-05 18:02:17.709388 wipac-file-catalog-indexer-2.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.685387 wipac-file-catalog-indexer-2.0.1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.701388 wipac-file-catalog-indexer-2.0.1/tests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/integration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.701388 wipac-file-catalog-indexer-2.0.1/tests/integration/real/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/integration/real/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7480 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/integration/real/exp_data.py
--rw-r--r--   0 root         (0) root         (0)     3781 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/integration/real/test_data_exp_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.701388 wipac-file-catalog-indexer-2.0.1/tests/integration/resources/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/integration/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21005 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/integration/resources/test_path_collector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.701388 wipac-file-catalog-indexer-2.0.1/tests/integration/simulation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/integration/simulation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6084 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/integration/simulation/sim_data.py
--rw-r--r--   0 root         (0) root         (0)     4451 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/integration/simulation/test_data_sim_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.701388 wipac-file-catalog-indexer-2.0.1/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.701388 wipac-file-catalog-indexer-2.0.1/tests/unit/indexer/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/unit/indexer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2100 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/unit/indexer/test_metadata_manager.py
--rw-r--r--   0 root         (0) root         (0)     1692 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/unit/indexer/test_path_filtering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.701388 wipac-file-catalog-indexer-2.0.1/tests/unit/real/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/unit/real/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13503 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/unit/real/test_data_exp_filename_parsing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.705388 wipac-file-catalog-indexer-2.0.1/tests/unit/simulation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/unit/simulation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17291 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/unit/simulation/filepath_data.py
--rw-r--r--   0 root         (0) root         (0)     5541 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/unit/simulation/steering_param_data.py
--rw-r--r--   0 root         (0) root         (0)     3492 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/unit/simulation/test_data_sim_filename_parsing.py
--rw-r--r--   0 root         (0) root         (0)     2761 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/unit/simulation/test_iceprod_tools.py
--rw-r--r--   0 root         (0) root         (0)     1636 2023-05-05 18:02:13.000000 wipac-file-catalog-indexer-2.0.1/tests/unit/simulation/test_steering_parameter_parsing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:02:17.705388 wipac-file-catalog-indexer-2.0.1/wipac_file_catalog_indexer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8597 2023-05-05 18:02:17.000000 wipac-file-catalog-indexer-2.0.1/wipac_file_catalog_indexer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2571 2023-05-05 18:02:17.000000 wipac-file-catalog-indexer-2.0.1/wipac_file_catalog_indexer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 18:02:17.000000 wipac-file-catalog-indexer-2.0.1/wipac_file_catalog_indexer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      309 2023-05-05 18:02:17.000000 wipac-file-catalog-indexer-2.0.1/wipac_file_catalog_indexer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-05 18:02:17.000000 wipac-file-catalog-indexer-2.0.1/wipac_file_catalog_indexer.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.816404 wipac-file-catalog-indexer-2.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8597 2023-05-30 16:00:28.816404 wipac-file-catalog-indexer-2.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7567 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.808404 wipac-file-catalog-indexer-2.0.2/indexer/
+-rw-r--r--   0 root         (0) root         (0)      613 2023-05-30 16:00:26.000000 wipac-file-catalog-indexer-2.0.2/indexer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6001 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/client_auth.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/config.py
+-rw-r--r--   0 root         (0) root         (0)      464 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/defaults.py
+-rw-r--r--   0 root         (0) root         (0)     6095 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/delocate.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/generate.py
+-rwxr-xr-x   0 root         (0) root         (0)    14829 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/index.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.808404 wipac-file-catalog-indexer-2.0.2/indexer/metadata/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/metadata/basic.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/metadata/i3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.808404 wipac-file-catalog-indexer-2.0.2/indexer/metadata/real/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/metadata/real/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7431 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/metadata/real/data_exp.py
+-rw-r--r--   0 root         (0) root         (0)     6170 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/metadata/real/filename_patterns.py
+-rw-r--r--   0 root         (0) root         (0)     4291 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/metadata/real/l2.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/metadata/real/pfdst.py
+-rw-r--r--   0 root         (0) root         (0)      945 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/metadata/real/pffilt.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/metadata/real/pfraw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.808404 wipac-file-catalog-indexer-2.0.2/indexer/metadata/simulation/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/metadata/simulation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11209 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/metadata/simulation/data_sim.py
+-rw-r--r--   0 root         (0) root         (0)   102684 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/metadata/simulation/filename_patterns.py
+-rw-r--r--   0 root         (0) root         (0)    17034 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/metadata/simulation/iceprod_tools.py
+-rw-r--r--   0 root         (0) root         (0)     8259 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/metadata_manager.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.808404 wipac-file-catalog-indexer-2.0.2/indexer/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3776 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/utils/file_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/indexer/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.804403 wipac-file-catalog-indexer-2.0.2/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.808404 wipac-file-catalog-indexer-2.0.2/resources/filename_patterns/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/resources/filename_patterns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      864 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/resources/filename_patterns/by_frequency.py
+-rw-r--r--   0 root         (0) root         (0)      593 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/resources/filename_patterns/example_finder.py
+-rw-r--r--   0 root         (0) root         (0)    15854 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/resources/filename_patterns/filename_pattern_finder.py
+-rw-r--r--   0 root         (0) root         (0)     3151 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/resources/filename_patterns/filename_pattern_regexer.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/resources/filename_patterns/fpf_stage2.1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.812404 wipac-file-catalog-indexer-2.0.2/resources/find_nonindexed/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/resources/find_nonindexed/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3819 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/resources/find_nonindexed/get_nonindexed_files.py
+-rw-r--r--   0 root         (0) root         (0)     2673 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/resources/find_nonindexed/make_condor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.812404 wipac-file-catalog-indexer-2.0.2/resources/path_collector/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/resources/path_collector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/resources/path_collector/common_args.py
+-rw-r--r--   0 root         (0) root         (0)      540 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/resources/path_collector/find_unfinished.py
+-rw-r--r--   0 root         (0) root         (0)    13851 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/resources/path_collector/path_collector.py
+-rw-r--r--   0 root         (0) root         (0)     5394 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/resources/path_collector/path_collector_make_condor.py
+-rw-r--r--   0 root         (0) root         (0)     4401 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/resources/path_collector/traverser.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2023-05-30 16:00:28.816404 wipac-file-catalog-indexer-2.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.804403 wipac-file-catalog-indexer-2.0.2/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.812404 wipac-file-catalog-indexer-2.0.2/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.812404 wipac-file-catalog-indexer-2.0.2/tests/integration/real/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/integration/real/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/integration/real/exp_data.py
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/integration/real/test_data_exp_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.812404 wipac-file-catalog-indexer-2.0.2/tests/integration/resources/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/integration/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21005 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/integration/resources/test_path_collector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.812404 wipac-file-catalog-indexer-2.0.2/tests/integration/simulation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/integration/simulation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6084 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/integration/simulation/sim_data.py
+-rw-r--r--   0 root         (0) root         (0)     4451 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/integration/simulation/test_data_sim_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.812404 wipac-file-catalog-indexer-2.0.2/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.812404 wipac-file-catalog-indexer-2.0.2/tests/unit/indexer/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/unit/indexer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/unit/indexer/test_metadata_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/unit/indexer/test_path_filtering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.812404 wipac-file-catalog-indexer-2.0.2/tests/unit/real/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/unit/real/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13503 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/unit/real/test_data_exp_filename_parsing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.816404 wipac-file-catalog-indexer-2.0.2/tests/unit/simulation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/unit/simulation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17291 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/unit/simulation/filepath_data.py
+-rw-r--r--   0 root         (0) root         (0)     5541 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/unit/simulation/steering_param_data.py
+-rw-r--r--   0 root         (0) root         (0)     3492 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/unit/simulation/test_data_sim_filename_parsing.py
+-rw-r--r--   0 root         (0) root         (0)     2761 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/unit/simulation/test_iceprod_tools.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-05-30 16:00:25.000000 wipac-file-catalog-indexer-2.0.2/tests/unit/simulation/test_steering_parameter_parsing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:00:28.816404 wipac-file-catalog-indexer-2.0.2/wipac_file_catalog_indexer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8597 2023-05-30 16:00:28.000000 wipac-file-catalog-indexer-2.0.2/wipac_file_catalog_indexer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-05-30 16:00:28.000000 wipac-file-catalog-indexer-2.0.2/wipac_file_catalog_indexer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 16:00:28.000000 wipac-file-catalog-indexer-2.0.2/wipac_file_catalog_indexer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      309 2023-05-30 16:00:28.000000 wipac-file-catalog-indexer-2.0.2/wipac_file_catalog_indexer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-30 16:00:28.000000 wipac-file-catalog-indexer-2.0.2/wipac_file_catalog_indexer.egg-info/top_level.txt
```

### Comparing `wipac-file-catalog-indexer-2.0.1/LICENSE` & `wipac-file-catalog-indexer-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/PKG-INFO` & `wipac-file-catalog-indexer-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-file-catalog-indexer
-Version: 2.0.1
+Version: 2.0.2
 Summary: Indexing package and scripts for the File Catalog
 Home-page: https://github.com/WIPACrepo/file-catalog-indexer
 Download-URL: https://pypi.org/project/wipac-file-catalog-indexer/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/file-catalog-indexer/issues
```

### Comparing `wipac-file-catalog-indexer-2.0.1/README.md` & `wipac-file-catalog-indexer-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/__init__.py` & `wipac-file-catalog-indexer-2.0.2/indexer/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "2.0.1"
+__version__ = "2.0.2"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/client_auth.py` & `wipac-file-catalog-indexer-2.0.2/indexer/client_auth.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/config.py` & `wipac-file-catalog-indexer-2.0.2/indexer/config.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/delocate.py` & `wipac-file-catalog-indexer-2.0.2/indexer/delocate.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/generate.py` & `wipac-file-catalog-indexer-2.0.2/indexer/generate.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/index.py` & `wipac-file-catalog-indexer-2.0.2/indexer/index.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/metadata/basic.py` & `wipac-file-catalog-indexer-2.0.2/indexer/metadata/basic.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/metadata/i3.py` & `wipac-file-catalog-indexer-2.0.2/indexer/metadata/i3.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/metadata/real/data_exp.py` & `wipac-file-catalog-indexer-2.0.2/indexer/metadata/real/data_exp.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/metadata/real/filename_patterns.py` & `wipac-file-catalog-indexer-2.0.2/indexer/metadata/real/filename_patterns.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/metadata/real/l2.py` & `wipac-file-catalog-indexer-2.0.2/indexer/metadata/real/l2.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/metadata/real/pfdst.py` & `wipac-file-catalog-indexer-2.0.2/indexer/metadata/real/pfdst.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/metadata/real/pffilt.py` & `wipac-file-catalog-indexer-2.0.2/indexer/metadata/real/pffilt.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/metadata/real/pfraw.py` & `wipac-file-catalog-indexer-2.0.2/indexer/metadata/real/pfraw.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/metadata/simulation/data_sim.py` & `wipac-file-catalog-indexer-2.0.2/indexer/metadata/simulation/data_sim.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/metadata/simulation/filename_patterns.py` & `wipac-file-catalog-indexer-2.0.2/indexer/metadata/simulation/filename_patterns.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/metadata/simulation/iceprod_tools.py` & `wipac-file-catalog-indexer-2.0.2/indexer/metadata/simulation/iceprod_tools.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/metadata_manager.py` & `wipac-file-catalog-indexer-2.0.2/indexer/metadata_manager.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/utils/file_utils.py` & `wipac-file-catalog-indexer-2.0.2/indexer/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/indexer/utils/utils.py` & `wipac-file-catalog-indexer-2.0.2/indexer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/resources/filename_patterns/by_frequency.py` & `wipac-file-catalog-indexer-2.0.2/resources/filename_patterns/by_frequency.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/resources/filename_patterns/example_finder.py` & `wipac-file-catalog-indexer-2.0.2/resources/filename_patterns/example_finder.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/resources/filename_patterns/filename_pattern_finder.py` & `wipac-file-catalog-indexer-2.0.2/resources/filename_patterns/filename_pattern_finder.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/resources/filename_patterns/filename_pattern_regexer.py` & `wipac-file-catalog-indexer-2.0.2/resources/filename_patterns/filename_pattern_regexer.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/resources/filename_patterns/fpf_stage2.1.py` & `wipac-file-catalog-indexer-2.0.2/resources/filename_patterns/fpf_stage2.1.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/resources/find_nonindexed/get_nonindexed_files.py` & `wipac-file-catalog-indexer-2.0.2/resources/find_nonindexed/get_nonindexed_files.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/resources/find_nonindexed/make_condor.py` & `wipac-file-catalog-indexer-2.0.2/resources/find_nonindexed/make_condor.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/resources/path_collector/common_args.py` & `wipac-file-catalog-indexer-2.0.2/resources/path_collector/common_args.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/resources/path_collector/find_unfinished.py` & `wipac-file-catalog-indexer-2.0.2/resources/path_collector/find_unfinished.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/resources/path_collector/path_collector.py` & `wipac-file-catalog-indexer-2.0.2/resources/path_collector/path_collector.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/resources/path_collector/path_collector_make_condor.py` & `wipac-file-catalog-indexer-2.0.2/resources/path_collector/path_collector_make_condor.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/resources/path_collector/traverser.py` & `wipac-file-catalog-indexer-2.0.2/resources/path_collector/traverser.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/setup.cfg` & `wipac-file-catalog-indexer-2.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/tests/integration/real/exp_data.py` & `wipac-file-catalog-indexer-2.0.2/tests/integration/real/exp_data.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/tests/integration/real/test_data_exp_metadata.py` & `wipac-file-catalog-indexer-2.0.2/tests/integration/real/test_data_exp_metadata.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/tests/integration/resources/test_path_collector.py` & `wipac-file-catalog-indexer-2.0.2/tests/integration/resources/test_path_collector.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/tests/integration/simulation/sim_data.py` & `wipac-file-catalog-indexer-2.0.2/tests/integration/simulation/sim_data.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/tests/integration/simulation/test_data_sim_metadata.py` & `wipac-file-catalog-indexer-2.0.2/tests/integration/simulation/test_data_sim_metadata.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/tests/unit/indexer/test_metadata_manager.py` & `wipac-file-catalog-indexer-2.0.2/tests/unit/indexer/test_metadata_manager.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/tests/unit/indexer/test_path_filtering.py` & `wipac-file-catalog-indexer-2.0.2/tests/unit/indexer/test_path_filtering.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/tests/unit/real/test_data_exp_filename_parsing.py` & `wipac-file-catalog-indexer-2.0.2/tests/unit/real/test_data_exp_filename_parsing.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/tests/unit/simulation/filepath_data.py` & `wipac-file-catalog-indexer-2.0.2/tests/unit/simulation/filepath_data.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/tests/unit/simulation/steering_param_data.py` & `wipac-file-catalog-indexer-2.0.2/tests/unit/simulation/steering_param_data.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/tests/unit/simulation/test_data_sim_filename_parsing.py` & `wipac-file-catalog-indexer-2.0.2/tests/unit/simulation/test_data_sim_filename_parsing.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/tests/unit/simulation/test_iceprod_tools.py` & `wipac-file-catalog-indexer-2.0.2/tests/unit/simulation/test_iceprod_tools.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/tests/unit/simulation/test_steering_parameter_parsing.py` & `wipac-file-catalog-indexer-2.0.2/tests/unit/simulation/test_steering_parameter_parsing.py`

 * *Files identical despite different names*

### Comparing `wipac-file-catalog-indexer-2.0.1/wipac_file_catalog_indexer.egg-info/PKG-INFO` & `wipac-file-catalog-indexer-2.0.2/wipac_file_catalog_indexer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-file-catalog-indexer
-Version: 2.0.1
+Version: 2.0.2
 Summary: Indexing package and scripts for the File Catalog
 Home-page: https://github.com/WIPACrepo/file-catalog-indexer
 Download-URL: https://pypi.org/project/wipac-file-catalog-indexer/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/file-catalog-indexer/issues
```

### Comparing `wipac-file-catalog-indexer-2.0.1/wipac_file_catalog_indexer.egg-info/SOURCES.txt` & `wipac-file-catalog-indexer-2.0.2/wipac_file_catalog_indexer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

