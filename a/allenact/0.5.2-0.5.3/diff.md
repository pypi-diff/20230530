# Comparing `tmp/allenact-0.5.2.tar.gz` & `tmp/allenact-0.5.3.tar.gz`

## Comparing `allenact-0.5.2.tar` & `allenact-0.5.3.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (121)     4376 2022-08-16 21:40:40.000000 allenact-0.5.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-16 21:40:40.000000 allenact-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact/
--rw-r--r--   0 runner    (1001) docker     (121)     4376 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact/algorithms/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact/algorithms/offpolicy_sync/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact/algorithms/offpolicy_sync/losses/
--rw-r--r--   0 runner    (1001) docker     (121)     1446 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/algorithms/offpolicy_sync/losses/abstract_offpolicy_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/algorithms/offpolicy_sync/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/algorithms/offpolicy_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact/algorithms/onpolicy_sync/
--rwxr-xr-x   0 runner    (1001) docker     (121)     7192 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/algorithms/onpolicy_sync/policy.py
--rw-r--r--   0 runner    (1001) docker     (121)    24843 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/algorithms/onpolicy_sync/storage.py
--rw-r--r--   0 runner    (1001) docker     (121)    85005 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/algorithms/onpolicy_sync/engine.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/algorithms/onpolicy_sync/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)    49634 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/algorithms/onpolicy_sync/vector_sampled_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact/algorithms/onpolicy_sync/losses/
--rw-r--r--   0 runner    (1001) docker     (121)     5198 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/algorithms/onpolicy_sync/losses/a2cacktr.py
--rw-r--r--   0 runner    (1001) docker     (121)     7597 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/algorithms/onpolicy_sync/losses/ppo.py
--rw-r--r--   0 runner    (1001) docker     (121)     8065 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/algorithms/onpolicy_sync/losses/imitation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2504 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/algorithms/onpolicy_sync/losses/grouped_action_imitation.py
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/algorithms/onpolicy_sync/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/algorithms/onpolicy_sync/losses/abstract_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/algorithms/onpolicy_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    60459 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/algorithms/onpolicy_sync/runner.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact/base_abstractions/
--rw-r--r--   0 runner    (1001) docker     (121)    13404 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/base_abstractions/distributions.py
--rw-r--r--   0 runner    (1001) docker     (121)    14726 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/base_abstractions/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)    11247 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/base_abstractions/experiment_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     6891 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/base_abstractions/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (121)    12653 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/base_abstractions/task.py
--rw-r--r--   0 runner    (1001) docker     (121)    14218 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/base_abstractions/sensor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/base_abstractions/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/base_abstractions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/_constants.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    18001 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact/embodiedai/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact/embodiedai/mapping/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact/embodiedai/mapping/mapping_utils/
--rw-r--r--   0 runner    (1001) docker     (121)    23116 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/mapping/mapping_utils/map_builders.py
--rw-r--r--   0 runner    (1001) docker     (121)    19996 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/mapping/mapping_utils/point_cloud_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/mapping/mapping_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact/embodiedai/mapping/mapping_models/
--rw-r--r--   0 runner    (1001) docker     (121)    29752 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/mapping/mapping_models/active_neural_slam.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/mapping/mapping_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6408 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/mapping/mapping_losses.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/mapping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact/embodiedai/models/
--rw-r--r--   0 runner    (1001) docker     (121)    12244 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     4009 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/models/fusion_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3647 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/models/aux_models.py
--rw-r--r--   0 runner    (1001) docker     (121)    10561 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/models/visual_nav_models.py
--rw-r--r--   0 runner    (1001) docker     (121)    25217 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/models/basic_models.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact/embodiedai/aux_losses/
--rw-r--r--   0 runner    (1001) docker     (121)    27794 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/aux_losses/losses.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/aux_losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact/embodiedai/preprocessors/
--rw-r--r--   0 runner    (1001) docker     (121)     3438 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/preprocessors/resnet.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/preprocessors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact/embodiedai/sensors/
--rw-r--r--   0 runner    (1001) docker     (121)    13273 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/sensors/vision_sensors.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/sensors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact/embodiedai/storage/
--rw-r--r--   0 runner    (1001) docker     (121)     7478 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/storage/vdr_storage.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/embodiedai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     5243 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (121)     8755 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/utils/spaces_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     9757 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2680 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/utils/cacheless_frcnn.py
--rw-r--r--   0 runner    (1001) docker     (121)     5772 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/utils/cache_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    16073 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/utils/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    41826 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/utils/experiment_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    45525 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/utils/viz_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7102 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (121)     7597 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4501 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/utils/multi_agent_viz_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-08-16 21:40:32.000000 allenact-0.5.2/allenact/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2860 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-08-16 21:40:40.000000 allenact-0.5.2/allenact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6098 2022-08-16 21:40:32.000000 allenact-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-08-16 21:40:40.000000 allenact-0.5.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:10.000000 allenact-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-05-30 17:11:58.000000 allenact-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    45635 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/utils/viz_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/utils/cacheless_frcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/utils/spaces_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16073 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/utils/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/utils/multi_agent_viz_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44726 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/utils/experiment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/utils/cache_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18001 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact/embodiedai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact/embodiedai/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    25217 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/models/basic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/models/fusion_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/models/visual_nav_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/models/aux_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact/embodiedai/preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/preprocessors/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact/embodiedai/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)    13335 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/sensors/vision_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/sensors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact/embodiedai/mapping/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact/embodiedai/mapping/mapping_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/mapping/mapping_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29752 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/mapping/mapping_models/active_neural_slam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/mapping/mapping_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/mapping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact/embodiedai/mapping/mapping_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/mapping/mapping_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26443 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/mapping/mapping_utils/map_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/mapping/mapping_utils/point_cloud_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact/embodiedai/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/storage/vdr_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact/embodiedai/aux_losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/aux_losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27796 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/embodiedai/aux_losses/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact/algorithms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact/algorithms/offpolicy_sync/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact/algorithms/offpolicy_sync/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/algorithms/offpolicy_sync/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/algorithms/offpolicy_sync/losses/abstract_offpolicy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/algorithms/offpolicy_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact/algorithms/onpolicy_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)    25168 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/algorithms/onpolicy_sync/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64292 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/algorithms/onpolicy_sync/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/algorithms/onpolicy_sync/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49637 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/algorithms/onpolicy_sync/vector_sampled_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact/algorithms/onpolicy_sync/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/algorithms/onpolicy_sync/losses/grouped_action_imitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/algorithms/onpolicy_sync/losses/abstract_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/algorithms/onpolicy_sync/losses/a2cacktr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/algorithms/onpolicy_sync/losses/imitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/algorithms/onpolicy_sync/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/algorithms/onpolicy_sync/losses/ppo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7192 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/algorithms/onpolicy_sync/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/algorithms/onpolicy_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100984 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/algorithms/onpolicy_sync/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact/base_abstractions/
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/base_abstractions/experiment_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14726 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/base_abstractions/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12653 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/base_abstractions/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/base_abstractions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/base_abstractions/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14218 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/base_abstractions/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/base_abstractions/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13360 2023-05-30 17:11:58.000000 allenact-0.5.3/allenact/base_abstractions/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-30 17:12:10.000000 allenact-0.5.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-30 17:12:10.000000 allenact-0.5.3/allenact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-30 17:12:10.000000 allenact-0.5.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 17:12:10.000000 allenact-0.5.3/setup.cfg
```

### Comparing `allenact-0.5.2/setup.py` & `allenact-0.5.3/allenact/setup.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/setup.py` & `allenact-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/algorithms/offpolicy_sync/losses/abstract_offpolicy_loss.py` & `allenact-0.5.3/allenact/algorithms/offpolicy_sync/losses/abstract_offpolicy_loss.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/algorithms/onpolicy_sync/policy.py` & `allenact-0.5.3/allenact/algorithms/onpolicy_sync/policy.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/algorithms/onpolicy_sync/storage.py` & `allenact-0.5.3/allenact/algorithms/onpolicy_sync/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import allenact.utils.spaces_utils as su
 from allenact.algorithms.onpolicy_sync.policy import (
     FullMemorySpecType,
     ObservationType,
     ActionType,
 )
 from allenact.base_abstractions.misc import Memory
+from allenact.utils.system import get_logger
 
 
 class ExperienceStorage(abc.ABC):
     @abc.abstractmethod
     def initialize(self, *, observations: ObservationType, **kwargs):
         raise NotImplementedError
 
@@ -365,23 +366,31 @@
                 self.flattened_to_unflattened[storage_name][flatten_name] = path + [
                     name
                 ]
                 self.unflattened_to_flattened[storage_name][
                     tuple(path + [name])
                 ] = flatten_name
 
-            if storage_name == "observations":
-                # current_data has a step dimension
-                assert time_step >= 0
-                storage[flatten_name][0][time_step : time_step + 1].copy_(current_data)
-            elif storage_name == "memory":
-                # current_data does not have a step dimension
-                storage[flatten_name][0][time_step].copy_(current_data)
-            else:
-                raise NotImplementedError
+            try:
+                if storage_name == "observations":
+                    # current_data has a step dimension
+                    assert time_step >= 0
+                    storage[flatten_name][0][time_step : time_step + 1].copy_(
+                        current_data
+                    )
+                elif storage_name == "memory":
+                    # current_data does not have a step dimension
+                    storage[flatten_name][0][time_step].copy_(current_data)
+                else:
+                    raise NotImplementedError
+            except:
+                get_logger().error(
+                    f"Error while inserting data in storage for name {flatten_name}"
+                )
+                raise
 
     def create_tensor_storage(
         self, num_steps: int, template: torch.Tensor
     ) -> torch.Tensor:
         return torch.cat([torch.zeros_like(template).to(self.device)] * num_steps)
 
     def _double_storage_size(self):
```

### Comparing `allenact-0.5.2/allenact/algorithms/onpolicy_sync/engine.py` & `allenact-0.5.3/allenact/algorithms/onpolicy_sync/engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -142,24 +142,28 @@
         self.results_queue = results_queue
         self.checkpoints_queue = checkpoints_queue
         self.mp_ctx = mp_ctx
         self.checkpoints_dir = checkpoints_dir
         self.worker_id = worker_id
         self.num_workers = num_workers
         self.device = torch.device("cpu") if device == -1 else torch.device(device)  # type: ignore
+
+        if self.device != torch.device("cpu"):
+            torch.cuda.set_device(device)
+
         self.distributed_ip = distributed_ip
         self.distributed_port = distributed_port
         self.try_restart_after_task_error = try_restart_after_task_error
 
         self.mode = mode.lower().strip()
         assert self.mode in [
             TRAIN_MODE_STR,
             VALID_MODE_STR,
             TEST_MODE_STR,
-        ], 'Only "train", "valid", "test" modes supported'
+        ], f"Only {TRAIN_MODE_STR}, {VALID_MODE_STR}, {TEST_MODE_STR}, modes supported"
 
         self.callback_sensors = callback_sensors
         self.deterministic_cudnn = deterministic_cudnn
         if self.deterministic_cudnn:
             set_deterministic_cudnn()
 
         self.seed = seed
@@ -185,28 +189,28 @@
 
         self._vector_tasks: Optional[
             Union[VectorSampledTasks, SingleProcessVectorSampledTasks]
         ] = None
 
         self.sensor_preprocessor_graph = None
         self.actor_critic: Optional[ActorCriticModel] = None
-        if self.num_samplers > 0:
-            create_model_kwargs = {}
-            if self.machine_params.sensor_preprocessor_graph is not None:
-                self.sensor_preprocessor_graph = self.machine_params.sensor_preprocessor_graph.to(
-                    self.device
-                )
-                create_model_kwargs[
-                    "sensor_preprocessor_graph"
-                ] = self.sensor_preprocessor_graph
-
-            set_seed(self.seed)
-            self.actor_critic = cast(
-                ActorCriticModel, self.config.create_model(**create_model_kwargs),
-            ).to(self.device)
+
+        create_model_kwargs = {}
+        if self.machine_params.sensor_preprocessor_graph is not None:
+            self.sensor_preprocessor_graph = self.machine_params.sensor_preprocessor_graph.to(
+                self.device
+            )
+            create_model_kwargs[
+                "sensor_preprocessor_graph"
+            ] = self.sensor_preprocessor_graph
+
+        set_seed(self.seed)
+        self.actor_critic = cast(
+            ActorCriticModel, self.config.create_model(**create_model_kwargs),
+        ).to(self.device)
 
         if initial_model_state_dict is not None:
             if isinstance(initial_model_state_dict, int):
                 assert (
                     md5_hash_of_state_dict(self.actor_critic.state_dict())
                     == initial_model_state_dict
                 ), (
@@ -267,19 +271,31 @@
         self.deterministic_agents = deterministic_agents
 
         self._is_closing: bool = (
             False  # Useful for letting the RL runner know if this is closing
         )
         self._is_closed: bool = False
 
-        self.training_pipeline: Optional[TrainingPipeline] = None
-
-        # Keeping track of metrics during training/inference
+        # Keeping track of metrics and losses during training/inference
         self.single_process_metrics: List = []
         self.single_process_task_callback_data: List = []
+        self.tracking_info_list: List[TrackingInfo] = []
+
+        # Variables that wil only be instantiated in the trainer
+        self.optimizer: Optional[optim.optimizer.Optimizer] = None
+        # noinspection PyProtectedMember
+        self.lr_scheduler: Optional[_LRScheduler] = None
+        self.insufficient_data_for_update: Optional[
+            torch.distributed.PrefixStore
+        ] = None
+
+        # Training pipeline will be instantiated during training and inference.
+        # During inference however, it will be instantiated anew on each run of `run_eval`
+        # and will be set to `None` after the eval run is complete.
+        self.training_pipeline: Optional[TrainingPipeline] = None
 
     @property
     def vector_tasks(
         self,
     ) -> Union[VectorSampledTasks, SingleProcessVectorSampledTasks]:
         if self._vector_tasks is None and self.num_samplers > 0:
             if self.is_distributed:
@@ -339,15 +355,15 @@
             fn = self.config.train_task_sampler_args
         elif self.mode == VALID_MODE_STR:
             fn = self.config.valid_task_sampler_args
         elif self.mode == TEST_MODE_STR:
             fn = self.config.test_task_sampler_args
         else:
             raise NotImplementedError(
-                "self.mode must be one of `train`, `valid` or `test`."
+                f"self.mode must be one of {TRAIN_MODE_STR}, {VALID_MODE_STR}, or {TEST_MODE_STR}."
             )
 
         if self.is_distributed:
             total_processes = sum(self.num_samplers_per_worker)
             process_offset = sum(self.num_samplers_per_worker[: self.worker_id])
         else:
             total_processes = self.num_samplers
@@ -370,29 +386,34 @@
                 devices=sampler_devices_as_ints,
                 seeds=seeds,
             )
             for it in range(self.num_samplers)
         ]
 
     def checkpoint_load(
-        self, ckpt: Union[str, Dict[str, Any]]
+        self, ckpt: Union[str, Dict[str, Any]], restart_pipeline: bool
     ) -> Dict[str, Union[Dict[str, Any], torch.Tensor, float, int, str, List]]:
         if isinstance(ckpt, str):
             get_logger().info(
                 f"[{self.mode} worker {self.worker_id}] Loading checkpoint from {ckpt}"
             )
             # Map location CPU is almost always better than mapping to a CUDA device.
             ckpt = torch.load(os.path.abspath(ckpt), map_location="cpu")
 
         ckpt = cast(
             Dict[str, Union[Dict[str, Any], torch.Tensor, float, int, str, List]], ckpt,
         )
 
         self.actor_critic.load_state_dict(ckpt["model_state_dict"])  # type:ignore
 
+        if "training_pipeline_state_dict" in ckpt and not restart_pipeline:
+            self.training_pipeline.load_state_dict(
+                cast(Dict[str, Any], ckpt["training_pipeline_state_dict"])
+            )
+
         return ckpt
 
     # aggregates task metrics currently in queue
     def aggregate_task_metrics(
         self, logging_pkg: LoggingPackage, num_tasks: int = -1,
     ) -> LoggingPackage:
         if num_tasks > 0:
@@ -448,22 +469,36 @@
         return len(paused), keep, batch
 
     def initialize_storage_and_viz(
         self,
         storage_to_initialize: Optional[Sequence[ExperienceStorage]],
         visualizer: Optional[VizSuite] = None,
     ):
-        observations = self.vector_tasks.get_observations()
 
-        npaused, keep, batch = self.remove_paused(observations)
-        observations = self._preprocess_observations(batch) if len(keep) > 0 else batch
+        keep: Optional[List] = None
+        if visualizer is not None or (
+            storage_to_initialize is not None
+            and any(isinstance(s, RolloutStorage) for s in storage_to_initialize)
+        ):
+            # No rollout storage, thus we are not
+            observations = self.vector_tasks.get_observations()
+
+            npaused, keep, batch = self.remove_paused(observations)
+            observations = (
+                self._preprocess_observations(batch) if len(keep) > 0 else batch
+            )
+
+            assert npaused == 0, f"{npaused} samplers are paused during initialization."
 
-        assert npaused == 0, f"{npaused} samplers are paused during initialization."
+            num_samplers = len(keep)
+        else:
+            observations = {}
+            num_samplers = 0
+            npaused = 0
 
-        num_samplers = len(keep)
         recurrent_memory_specification = (
             self.actor_critic.recurrent_memory_specification
         )
 
         if storage_to_initialize is not None:
             for s in storage_to_initialize:
                 s.to(self.device)
@@ -471,21 +506,23 @@
                 s.initialize(
                     observations=observations,
                     num_samplers=num_samplers,
                     recurrent_memory_specification=recurrent_memory_specification,
                     action_space=self.actor_critic.action_space,
                 )
 
-        if visualizer is not None and len(keep) > 0:
+        if visualizer is not None and num_samplers > 0:
             visualizer.collect(vector_task=self.vector_tasks, alive=keep)
 
         return npaused
 
     @property
     def num_active_samplers(self):
+        if self.vector_tasks is None:
+            return 0
         return self.vector_tasks.num_unpaused_tasks
 
     def act(
         self,
         rollout_storage: RolloutStorage,
         dist_wrapper_class: Optional[type] = None,
     ):
@@ -497,14 +534,60 @@
             if dist_wrapper_class is not None:
                 distr = dist_wrapper_class(distr=distr, obs=agent_input["observations"])
 
             actions = distr.sample() if not self.deterministic_agents else distr.mode()
 
         return actions, actor_critic_output, memory, agent_input["observations"]
 
+    def aggregate_and_send_logging_package(
+        self,
+        tracking_info_list: List[TrackingInfo],
+        logging_pkg: Optional[LoggingPackage] = None,
+        send_logging_package: bool = True,
+    ):
+        if logging_pkg is None:
+            logging_pkg = LoggingPackage(
+                mode=self.mode,
+                training_steps=self.training_pipeline.total_steps,
+                pipeline_stage=self.training_pipeline.current_stage_index,
+                storage_uuid_to_total_experiences=self.training_pipeline.storage_uuid_to_total_experiences,
+            )
+
+        self.aggregate_task_metrics(logging_pkg=logging_pkg)
+
+        for callback_dict in self.single_process_task_callback_data:
+            logging_pkg.task_callback_data.append(callback_dict)
+        self.single_process_task_callback_data = []
+
+        for tracking_info in tracking_info_list:
+            if tracking_info.n < 0:
+                get_logger().warning(
+                    f"Obtained a train_info_dict with {tracking_info.n} elements."
+                    f" Full info: ({tracking_info.type}, {tracking_info.info}, {tracking_info.n})."
+                )
+            else:
+                tracking_info_dict = tracking_info.info
+
+                if tracking_info.type == TrackingInfoType.LOSS:
+                    tracking_info_dict = {
+                        f"losses/{k}": v for k, v in tracking_info_dict.items()
+                    }
+
+                logging_pkg.add_info_dict(
+                    info_dict=tracking_info_dict,
+                    n=tracking_info.n,
+                    stage_component_uuid=tracking_info.stage_component_uuid,
+                    storage_uuid=tracking_info.storage_uuid,
+                )
+
+        if send_logging_package:
+            self.results_queue.put(logging_pkg)
+
+        return logging_pkg
+
     @staticmethod
     def _active_memory(memory, keep):
         return memory.sampler_select(keep) if memory is not None else memory
 
     def probe(self, dones: List[bool], npaused, period=100000):
         """Debugging util. When called from
         self.collect_step_across_all_task_samplers(...), calls render for the
@@ -626,26 +709,26 @@
 
         npaused, keep, batch = self.remove_paused(observations)
 
         # TODO self.probe(...) can be useful for debugging (we might want to control it from main?)
         # self.probe(dones, npaused)
 
         if npaused > 0:
-            for s in uuid_to_storage.values():
-                if isinstance(s, RolloutStorage):
-                    s.sampler_select(keep)
-
             if self.mode == TRAIN_MODE_STR:
                 raise NotImplementedError(
                     "When trying to get a new task from a task sampler (using the `.next_task()` method)"
                     " the task sampler returned `None`. This is not currently supported during training"
                     " (and almost certainly a bug in the implementation of the task sampler or in the "
                     " initialization of the task sampler for training)."
                 )
 
+            for s in uuid_to_storage.values():
+                if isinstance(s, RolloutStorage):
+                    s.sampler_select(keep)
+
         to_add_to_storage = dict(
             observations=self._preprocess_observations(batch)
             if len(keep) > 0
             else batch,
             memory=self._active_memory(memory, keep),
             actions=flat_actions[0, keep],
             action_log_probs=actor_critic_output.distributions.log_prob(actions)[
@@ -668,14 +751,336 @@
                     actor_critic=actor_critic_output,
                 )
             else:
                 visualizer.collect(actor_critic=actor_critic_output)
 
         return npaused
 
+    def distributed_weighted_sum(
+        self,
+        to_share: Union[torch.Tensor, float, int],
+        weight: Union[torch.Tensor, float, int],
+    ):
+        """Weighted sum of scalar across distributed workers."""
+        if self.is_distributed:
+            aggregate = torch.tensor(to_share * weight).to(self.device)
+            dist.all_reduce(aggregate)
+            return aggregate.item()
+        else:
+            if abs(1 - weight) > 1e-5:
+                get_logger().warning(
+                    f"Scaling non-distributed value with weight {weight}"
+                )
+            return torch.tensor(to_share * weight).item()
+
+    def distributed_reduce(
+        self, to_share: Union[torch.Tensor, float, int], op: ReduceOp
+    ):
+        """Weighted sum of scalar across distributed workers."""
+        if self.is_distributed:
+            aggregate = torch.tensor(to_share).to(self.device)
+            dist.all_reduce(aggregate, op=op)
+            return aggregate.item()
+        else:
+            return torch.tensor(to_share).item()
+
+    def backprop_step(
+        self,
+        total_loss: torch.Tensor,
+        max_grad_norm: float,
+        local_to_global_batch_size_ratio: float = 1.0,
+    ):
+        raise NotImplementedError
+
+    def save_error_data(self, batch: Dict[str, Any]):
+        raise NotImplementedError
+
+    @property
+    def step_count(self) -> int:
+        if (
+            self.training_pipeline.current_stage is None
+        ):  # Might occur during testing when all stages are complete
+            return 0
+        return self.training_pipeline.current_stage.steps_taken_in_stage
+
+
+    def compute_losses_track_them_and_backprop(
+        self,
+        stage: PipelineStage,
+        stage_component: StageComponent,
+        storage: ExperienceStorage,
+        skip_backprop: bool = False,
+    ):
+        training = self.mode == TRAIN_MODE_STR
+
+        assert training or skip_backprop
+
+        if training and self.is_distributed:
+            self.insufficient_data_for_update.set(
+                "insufficient_data_for_update", str(0)
+            )
+            dist.barrier(
+                device_ids=None
+                if self.device == torch.device("cpu")
+                else [self.device.index]
+            )
+
+        training_settings = stage_component.training_settings
+
+        loss_names = stage_component.loss_names
+        losses = [self.training_pipeline.get_loss(ln) for ln in loss_names]
+        loss_weights = [stage.uuid_to_loss_weight[ln] for ln in loss_names]
+        loss_update_repeats_list = training_settings.update_repeats
+        if isinstance(loss_update_repeats_list, numbers.Integral):
+            loss_update_repeats_list = [loss_update_repeats_list] * len(loss_names)
+
+        if skip_backprop and isinstance(storage, MiniBatchStorageMixin):
+            if loss_update_repeats_list != [1] * len(loss_names):
+                loss_update_repeats_list = [1] * len(loss_names)
+                get_logger().warning(
+                    "Does not make sense to do multiple updates when"
+                    " skip_backprop is `True` and you are using a storage of type"
+                    " `MiniBatchStorageMixin`. This is likely a problem caused by"
+                    " using a custom valid/test stage component that is inheriting its"
+                    " TrainingSettings from the TrainingPipeline's TrainingSettings. We will override"
+                    " the requested number of updates repeats (which was"
+                    f" {dict(zip(loss_names, loss_update_repeats_list))}) to be 1 for all losses."
+                )
+
+        enough_data_for_update = True
+        for current_update_repeat_index in range(
+            max(loss_update_repeats_list, default=0)
+        ):
+            if isinstance(storage, MiniBatchStorageMixin):
+                batch_iterator = storage.batched_experience_generator(
+                    num_mini_batch=training_settings.num_mini_batch
+                )
+            elif isinstance(storage, StreamingStorageMixin):
+                assert (
+                    training_settings.num_mini_batch is None
+                    or training_settings.num_mini_batch == 1
+                )
+
+                def single_batch_generator(streaming_storage: StreamingStorageMixin):
+                    try:
+                        yield cast(
+                            StreamingStorageMixin, streaming_storage
+                        ).next_batch()
+                    except EOFError:
+                        if not training:
+                            raise
+
+                        if streaming_storage.empty():
+                            yield None
+                        else:
+                            cast(
+                                StreamingStorageMixin, streaming_storage
+                            ).reset_stream()
+                            stage.stage_component_uuid_to_stream_memory[
+                                stage_component.uuid
+                            ].clear()
+                            yield cast(
+                                StreamingStorageMixin, streaming_storage
+                            ).next_batch()
+
+                batch_iterator = single_batch_generator(streaming_storage=storage)
+            else:
+                raise NotImplementedError(
+                    f"Storage {storage} must be a subclass of `MiniBatchStorageMixin` or `StreamingStorageMixin`."
+                )
+
+            for batch in batch_iterator:
+                if batch is None:
+                    # This should only happen in a `StreamingStorageMixin` when it cannot
+                    # generate an initial batch or when we are in testing/validation and
+                    # we've reached the end of the dataset over which to test/validate.
+                    if training:
+                        assert isinstance(storage, StreamingStorageMixin)
+                        get_logger().warning(
+                            f"Worker {self.worker_id}: could not run update in {storage}, potentially because"
+                            f" not enough data has been accumulated to be able to fill an initial batch."
+                        )
+                    else:
+                        pass
+                    enough_data_for_update = False
+
+                if training and self.is_distributed:
+                    self.insufficient_data_for_update.add(
+                        "insufficient_data_for_update",
+                        1 * (not enough_data_for_update),
+                    )
+                    dist.barrier(
+                        device_ids=None
+                        if self.device == torch.device("cpu")
+                        else [self.device.index]
+                    )
+
+                    if (
+                        int(
+                            self.insufficient_data_for_update.get(
+                                "insufficient_data_for_update"
+                            )
+                        )
+                        != 0
+                    ):
+                        enough_data_for_update = False
+                        break
+
+                info: Dict[str, float] = {}
+
+                bsize: Optional[int] = None
+                total_loss: Optional[torch.Tensor] = None
+                actor_critic_output_for_batch: Optional[ActorCriticOutput] = None
+                batch_memory = Memory()
+
+                for loss, loss_name, loss_weight, max_update_repeats_for_loss in zip(
+                    losses, loss_names, loss_weights, loss_update_repeats_list
+                ):
+                    if current_update_repeat_index >= max_update_repeats_for_loss:
+                        continue
+
+                    if isinstance(loss, AbstractActorCriticLoss):
+                        bsize = batch["bsize"]
+
+                        if actor_critic_output_for_batch is None:
+
+                            try:
+                                actor_critic_output_for_batch, _ = self.actor_critic(
+                                    observations=batch["observations"],
+                                    memory=batch["memory"],
+                                    prev_actions=batch["prev_actions"],
+                                    masks=batch["masks"],
+                                )
+                            except ValueError:
+                                save_path = self.save_error_data(batch=batch)
+                                get_logger().error(
+                                    f"Encountered a value error! Likely because of nans in the output/input."
+                                    f" Saving all error information to {save_path}."
+                                )
+                                raise
+
+                        loss_return = loss.loss(
+                            step_count=self.step_count,
+                            batch=batch,
+                            actor_critic_output=actor_critic_output_for_batch,
+                        )
+
+                        per_epoch_info = {}
+                        if len(loss_return) == 2:
+                            current_loss, current_info = loss_return
+                        elif len(loss_return) == 3:
+                            current_loss, current_info, per_epoch_info = loss_return
+                        else:
+                            raise NotImplementedError
+
+                    elif isinstance(loss, GenericAbstractLoss):
+                        loss_output = loss.loss(
+                            model=self.actor_critic,
+                            batch=batch,
+                            batch_memory=batch_memory,
+                            stream_memory=stage.stage_component_uuid_to_stream_memory[
+                                stage_component.uuid
+                            ],
+                        )
+                        current_loss = loss_output.value
+                        current_info = loss_output.info
+                        per_epoch_info = loss_output.per_epoch_info
+                        batch_memory = loss_output.batch_memory
+                        stage.stage_component_uuid_to_stream_memory[
+                            stage_component.uuid
+                        ] = loss_output.stream_memory
+                        bsize = loss_output.bsize
+                    else:
+                        raise NotImplementedError(
+                            f"Loss of type {type(loss)} is not supported. Losses must be subclasses of"
+                            f" `AbstractActorCriticLoss` or `GenericAbstractLoss`."
+                        )
+
+                    if total_loss is None:
+                        total_loss = loss_weight * current_loss
+                    else:
+                        total_loss = total_loss + loss_weight * current_loss
+
+                    for key, value in current_info.items():
+                        info[f"{loss_name}/{key}"] = value
+
+                    if per_epoch_info is not None:
+                        for key, value in per_epoch_info.items():
+                            if max(loss_update_repeats_list, default=0) > 1:
+                                info[
+                                    f"{loss_name}/{key}_epoch{current_update_repeat_index:02d}"
+                                ] = value
+                                info[f"{loss_name}/{key}_combined"] = value
+                            else:
+                                info[f"{loss_name}/{key}"] = value
+
+                assert total_loss is not None, (
+                    f"No {stage_component.uuid} losses specified for training in stage"
+                    f" {self.training_pipeline.current_stage_index}"
+                )
+
+                total_loss_scalar = total_loss.item()
+                info[f"total_loss"] = total_loss_scalar
+
+                self.tracking_info_list.append(
+                    TrackingInfo(
+                        type=TrackingInfoType.LOSS,
+                        info=info,
+                        n=bsize,
+                        storage_uuid=stage_component.storage_uuid,
+                        stage_component_uuid=stage_component.uuid,
+                    )
+                )
+
+                to_track = {
+                    "rollout_epochs": max(loss_update_repeats_list, default=0),
+                    "worker_batch_size": bsize,
+                }
+
+                aggregate_bsize = None
+                if training:
+                    aggregate_bsize = self.distributed_weighted_sum(bsize, 1)
+                    to_track["global_batch_size"] = aggregate_bsize
+                    to_track["lr"] = self.optimizer.param_groups[0]["lr"]
+
+                if training_settings.num_mini_batch is not None:
+                    to_track[
+                        "rollout_num_mini_batch"
+                    ] = training_settings.num_mini_batch
+
+                for k, v in to_track.items():
+                    # We need to set the bsize to 1 for `worker_batch_size` below as we're trying to record the
+                    # average batch size per worker, not the average per worker weighted by the size of the batches
+                    # of those workers.
+                    self.tracking_info_list.append(
+                        TrackingInfo(
+                            type=TrackingInfoType.UPDATE_INFO,
+                            info={k: v},
+                            n=1 if k == "worker_batch_size" else bsize,
+                            storage_uuid=stage_component.storage_uuid,
+                            stage_component_uuid=stage_component.uuid,
+                        )
+                    )
+
+                if not skip_backprop:
+                    self.backprop_step(
+                        total_loss=total_loss,
+                        max_grad_norm=training_settings.max_grad_norm,
+                        local_to_global_batch_size_ratio=bsize / aggregate_bsize,
+                    )
+
+                stage.stage_component_uuid_to_stream_memory[
+                    stage_component.uuid
+                ] = detach_recursively(
+                    input=stage.stage_component_uuid_to_stream_memory[
+                        stage_component.uuid
+                    ],
+                    inplace=True,
+                )
+
     def close(self, verbose=True):
         self._is_closing = True
 
         if "_is_closed" in self.__dict__ and self._is_closed:
             return
 
         def logif(s: Union[str, Exception]):
@@ -817,15 +1222,14 @@
         else:
             self.num_workers_done = None
             self.num_workers_steps = None
             self.distributed_preemption_threshold = 1.0
             self.offpolicy_epoch_done = None
 
         # Keeping track of training state
-        self.tracking_info_list: List[TrackingInfo] = []
         self.former_steps: Optional[int] = None
         self.last_log: Optional[int] = None
         self.last_save: Optional[int] = None
         # The `self._last_aggregated_train_task_metrics` attribute defined
         # below is used for early stopping criterion computations
         self._last_aggregated_train_task_metrics: ScalarMeanTracker = (
             ScalarMeanTracker()
@@ -853,15 +1257,16 @@
 
     def deterministic_seeds(self) -> None:
         if self.seed is not None:
             set_seed(self.advance_seed(self.seed))  # known state for all workers
             seeds = self.worker_seeds(
                 self.num_samplers, None
             )  # use the latest seed for workers and update rng state
-            self.vector_tasks.set_seeds(seeds)
+            if self.vector_tasks is not None:
+                self.vector_tasks.set_seeds(seeds)
 
     def save_error_data(self, batch: Dict[str, Any]) -> str:
         model_path = os.path.join(
             self.checkpoints_dir,
             "error_for_exp_{}__stage_{:02d}__steps_{:012d}.pt".format(
                 self.experiment_name,
                 self.training_pipeline.current_stage_index,
@@ -885,14 +1290,36 @@
                     save_dict["scheduler_state"] = cast(
                         _LRScheduler, self.lr_scheduler
                     ).state_dict()
 
                 torch.save(save_dict, model_path)
         return model_path
 
+    def aggregate_and_send_logging_package(
+        self,
+        tracking_info_list: List[TrackingInfo],
+        logging_pkg: Optional[LoggingPackage] = None,
+        send_logging_package: bool = True,
+    ):
+        logging_pkg = super().aggregate_and_send_logging_package(
+            tracking_info_list=tracking_info_list,
+            logging_pkg=logging_pkg,
+            send_logging_package=send_logging_package,
+        )
+
+        if self.mode == TRAIN_MODE_STR:
+            # Technically self.mode should always be "train" here (as this is the training engine),
+            # this conditional is defensive
+            self._last_aggregated_train_task_metrics.add_scalars(
+                scalars=logging_pkg.metrics_tracker.means(),
+                n=logging_pkg.metrics_tracker.counts(),
+            )
+
+        return logging_pkg
+
     def checkpoint_save(self, pipeline_stage_index: Optional[int] = None) -> str:
         model_path = os.path.join(
             self.checkpoints_dir,
             "exp_{}__stage_{:02d}__steps_{:012d}.pt".format(
                 self.experiment_name,
                 self.training_pipeline.current_stage_index
                 if pipeline_stage_index is None
@@ -916,44 +1343,43 @@
 
         torch.save(save_dict, model_path)
         return model_path
 
     def checkpoint_load(
         self, ckpt: Union[str, Dict[str, Any]], restart_pipeline: bool = False
     ) -> Dict[str, Union[Dict[str, Any], torch.Tensor, float, int, str, List]]:
-        ckpt = super().checkpoint_load(ckpt)
+        if restart_pipeline:
+            if "training_pipeline_state_dict" in ckpt:
+                del ckpt["training_pipeline_state_dict"]
+
+        ckpt = super().checkpoint_load(ckpt, restart_pipeline=restart_pipeline)
 
-        self.training_pipeline.load_state_dict(
-            cast(Dict[str, Any], ckpt["training_pipeline_state_dict"])
-        )
         if restart_pipeline:
             self.training_pipeline.restart_pipeline()
         else:
             self.seed = cast(int, ckpt["trainer_seed"])
             self.optimizer.load_state_dict(ckpt["optimizer_state_dict"])  # type: ignore
-            if self.lr_scheduler is not None:
+            if self.lr_scheduler is not None and "scheduler_state" in ckpt:
                 self.lr_scheduler.load_state_dict(ckpt["scheduler_state"])  # type: ignore
 
         self.deterministic_seeds()
 
         return ckpt
 
     @property
     def step_count(self):
         return self.training_pipeline.current_stage.steps_taken_in_stage
 
     @step_count.setter
-    def step_count(self, val: int):
+    def step_count(self, val: int) -> None:
         self.training_pipeline.current_stage.steps_taken_in_stage = val
 
     @property
     def log_interval(self):
-        return (
-            self.training_pipeline.current_stage.training_settings.metric_accumulate_interval
-        )
+        return self.training_pipeline.current_stage.training_settings.metric_accumulate_interval
 
     @property
     def approx_steps(self):
         if self.is_distributed:
             # the actual number of steps gets synchronized after each rollout
             return (
                 self.step_count - self.former_steps
@@ -964,21 +1390,33 @@
     def act(
         self,
         rollout_storage: RolloutStorage,
         dist_wrapper_class: Optional[type] = None,
     ):
         if self.training_pipeline.current_stage.teacher_forcing is not None:
             assert dist_wrapper_class is None
+
+            def tracking_callback(type: TrackingInfoType, info: Dict[str, Any], n: int):
+                self.tracking_info_list.append(
+                    TrackingInfo(
+                        type=type,
+                        info=info,
+                        n=n,
+                        storage_uuid=self.training_pipeline.rollout_storage_uuid,
+                        stage_component_uuid=None,
+                    )
+                )
+
             dist_wrapper_class = partial(
                 TeacherForcingDistr,
                 action_space=self.actor_critic.action_space,
                 num_active_samplers=self.num_active_samplers,
                 approx_steps=self.approx_steps,
                 teacher_forcing=self.training_pipeline.current_stage.teacher_forcing,
-                tracking_info_list=self.tracking_info_list,
+                tracking_callback=tracking_callback,
             )
 
         actions, actor_critic_output, memory, step_observation = super().act(
             rollout_storage=rollout_storage, dist_wrapper_class=dist_wrapper_class,
         )
 
         self.step_count += self.num_active_samplers
@@ -1011,283 +1449,14 @@
             std = (summed_squares / (global_rollout_steps - 1)).sqrt()
         else:
             # noinspection PyArgumentList
             mean, std = advantages.mean(), advantages.std()
 
         return {"mean": mean, "std": std}
 
-    def distributed_weighted_sum(
-        self,
-        to_share: Union[torch.Tensor, float, int],
-        weight: Union[torch.Tensor, float, int],
-    ):
-        """Weighted sum of scalar across distributed workers."""
-        if self.is_distributed:
-            aggregate = torch.tensor(to_share * weight).to(self.device)
-            dist.all_reduce(aggregate)
-            return aggregate.item()
-        else:
-            if abs(1 - weight) > 1e-5:
-                get_logger().warning(
-                    f"Scaling non-distributed value with weight {weight}"
-                )
-            return torch.tensor(to_share * weight).item()
-
-    def distributed_reduce(
-        self, to_share: Union[torch.Tensor, float, int], op: ReduceOp
-    ):
-        """Weighted sum of scalar across distributed workers."""
-        if self.is_distributed:
-            aggregate = torch.tensor(to_share).to(self.device)
-            dist.all_reduce(aggregate, op=op)
-            return aggregate.item()
-        else:
-            return torch.tensor(to_share).item()
-
-    def update(
-        self,
-        stage: PipelineStage,
-        stage_component: StageComponent,
-        storage: ExperienceStorage,
-    ):
-        if self.is_distributed:
-            self.insufficient_data_for_update.set(
-                "insufficient_data_for_update", str(0)
-            )
-            dist.barrier(
-                device_ids=None
-                if self.device == torch.device("cpu")
-                else [self.device.index]
-            )
-
-        training_settings = stage_component.training_settings
-
-        loss_names = stage_component.loss_names
-        losses = [self.training_pipeline.get_loss(ln) for ln in loss_names]
-        loss_weights = [stage.uuid_to_loss_weight[ln] for ln in loss_names]
-        loss_update_repeats_list = training_settings.update_repeats
-        if isinstance(loss_update_repeats_list, numbers.Integral):
-            loss_update_repeats_list = [loss_update_repeats_list] * len(loss_names)
-
-        enough_data_for_update = True
-        for current_update_repeat_index in range(
-            max(loss_update_repeats_list, default=0)
-        ):
-            if isinstance(storage, MiniBatchStorageMixin):
-                batch_iterator = storage.batched_experience_generator(
-                    num_mini_batch=training_settings.num_mini_batch
-                )
-            elif isinstance(storage, StreamingStorageMixin):
-                assert (
-                    training_settings.num_mini_batch is None
-                    or training_settings.num_mini_batch == 1
-                )
-
-                def single_batch_generator(streaming_storage: StreamingStorageMixin):
-                    try:
-                        yield cast(
-                            StreamingStorageMixin, streaming_storage
-                        ).next_batch()
-                    except EOFError:
-                        if streaming_storage.empty():
-                            yield None
-                        else:
-                            cast(
-                                StreamingStorageMixin, streaming_storage
-                            ).reset_stream()
-                            stage.stage_component_uuid_to_stream_memory[
-                                stage_component.uuid
-                            ].clear()
-                            yield cast(
-                                StreamingStorageMixin, streaming_storage
-                            ).next_batch()
-
-                batch_iterator = single_batch_generator(streaming_storage=storage)
-            else:
-                raise NotImplementedError(
-                    f"Storage {storage} must be a subclass of `MiniBatchStorageMixin` or `StreamingStorageMixin`."
-                )
-
-            for batch in batch_iterator:
-                if batch is None:
-                    # This should only happen in a `StreamingStorageMixin` when it cannot
-                    # generate an initial batch.
-                    assert isinstance(storage, StreamingStorageMixin)
-                    get_logger().warning(
-                        f"Worker {self.worker_id}: could not run update in {storage}, potentially because"
-                        f" not enough data has been accumulated to be able to fill an initial batch."
-                    )
-                    enough_data_for_update = False
-
-                if self.is_distributed:
-                    self.insufficient_data_for_update.add(
-                        "insufficient_data_for_update",
-                        1 * (not enough_data_for_update),
-                    )
-                    dist.barrier(
-                        device_ids=None
-                        if self.device == torch.device("cpu")
-                        else [self.device.index]
-                    )
-
-                    if (
-                        int(
-                            self.insufficient_data_for_update.get(
-                                "insufficient_data_for_update"
-                            )
-                        )
-                        != 0
-                    ):
-                        enough_data_for_update = False
-                        break
-
-                info: Dict[str, float] = {}
-
-                bsize: Optional[int] = None
-                total_loss: Optional[torch.Tensor] = None
-                actor_critic_output_for_batch: Optional[ActorCriticOutput] = None
-                batch_memory = Memory()
-
-                for loss, loss_name, loss_weight, max_update_repeats_for_loss in zip(
-                    losses, loss_names, loss_weights, loss_update_repeats_list
-                ):
-                    if current_update_repeat_index >= max_update_repeats_for_loss:
-                        continue
-
-                    if isinstance(loss, AbstractActorCriticLoss):
-                        bsize = batch["bsize"]
-
-                        if actor_critic_output_for_batch is None:
-
-                            try:
-                                actor_critic_output_for_batch, _ = self.actor_critic(
-                                    observations=batch["observations"],
-                                    memory=batch["memory"],
-                                    prev_actions=batch["prev_actions"],
-                                    masks=batch["masks"],
-                                )
-                            except ValueError:
-                                save_path = self.save_error_data(batch=batch)
-                                get_logger().error(
-                                    f"Encountered a value error! Likely because of nans in the output/input."
-                                    f" Saving all error information to {save_path}."
-                                )
-                                raise
-
-                        loss_return = loss.loss(
-                            step_count=self.step_count,
-                            batch=batch,
-                            actor_critic_output=actor_critic_output_for_batch,
-                        )
-
-                        per_epoch_info = {}
-                        if len(loss_return) == 2:
-                            current_loss, current_info = loss_return
-                        elif len(loss_return) == 3:
-                            current_loss, current_info, per_epoch_info = loss_return
-                        else:
-                            raise NotImplementedError
-
-                    elif isinstance(loss, GenericAbstractLoss):
-                        loss_output = loss.loss(
-                            model=self.actor_critic,
-                            batch=batch,
-                            batch_memory=batch_memory,
-                            stream_memory=stage.stage_component_uuid_to_stream_memory[
-                                stage_component.uuid
-                            ],
-                        )
-                        current_loss = loss_output.value
-                        current_info = loss_output.info
-                        per_epoch_info = loss_output.per_epoch_info
-                        batch_memory = loss_output.batch_memory
-                        stage.stage_component_uuid_to_stream_memory[
-                            stage_component.uuid
-                        ] = loss_output.stream_memory
-                        bsize = loss_output.bsize
-                    else:
-                        raise NotImplementedError(
-                            f"Loss of type {type(loss)} is not supported. Losses must be subclasses of"
-                            f" `AbstractActorCriticLoss` or `GenericAbstractLoss`."
-                        )
-
-                    if total_loss is None:
-                        total_loss = loss_weight * current_loss
-                    else:
-                        total_loss = total_loss + loss_weight * current_loss
-
-                    for key, value in current_info.items():
-                        info[f"{loss_name}/{key}"] = value
-
-                    if per_epoch_info is not None:
-                        for key, value in per_epoch_info.items():
-                            if max(loss_update_repeats_list, default=0) > 1:
-                                info[
-                                    f"{loss_name}/{key}_epoch{current_update_repeat_index:02d}"
-                                ] = value
-                                info[f"{loss_name}/{key}_combined"] = value
-                            else:
-                                info[f"{loss_name}/{key}"] = value
-
-                assert total_loss is not None, (
-                    f"No {stage_component.uuid} losses specified for training in stage"
-                    f" {self.training_pipeline.current_stage_index}"
-                )
-
-                total_loss_scalar = total_loss.item()
-                info[f"total_loss"] = total_loss_scalar
-
-                self.tracking_info_list.append(
-                    TrackingInfo(
-                        type=TrackingInfoType.LOSS,
-                        info=info,
-                        n=bsize,
-                        storage_uuid=stage_component.storage_uuid,
-                        stage_component_uuid=stage_component.uuid,
-                    )
-                )
-
-                aggregate_bsize = self.distributed_weighted_sum(bsize, 1)
-                to_track = {
-                    "lr": self.optimizer.param_groups[0]["lr"],
-                    "rollout_epochs": max(loss_update_repeats_list, default=0),
-                    "global_batch_size": aggregate_bsize,
-                    "worker_batch_size": bsize,
-                }
-                if training_settings.num_mini_batch is not None:
-                    to_track[
-                        "rollout_num_mini_batch"
-                    ] = training_settings.num_mini_batch
-
-                for k, v in to_track.items():
-                    self.tracking_info_list.append(
-                        TrackingInfo(
-                            type=TrackingInfoType.UPDATE_INFO,
-                            info={k: v},
-                            n=bsize,
-                            storage_uuid=stage_component.storage_uuid,
-                            stage_component_uuid=stage_component.uuid,
-                        )
-                    )
-
-                self.backprop_step(
-                    total_loss=total_loss,
-                    max_grad_norm=training_settings.max_grad_norm,
-                    local_to_global_batch_size_ratio=bsize / aggregate_bsize,
-                )
-
-                stage.stage_component_uuid_to_stream_memory[
-                    stage_component.uuid
-                ] = detach_recursively(
-                    input=stage.stage_component_uuid_to_stream_memory[
-                        stage_component.uuid
-                    ],
-                    inplace=True,
-                )
-
     def backprop_step(
         self,
         total_loss: torch.Tensor,
         max_grad_norm: float,
         local_to_global_batch_size_ratio: float = 1.0,
     ):
         self.optimizer.zero_grad()  # type: ignore
@@ -1313,61 +1482,14 @@
 
         nn.utils.clip_grad_norm_(
             self.actor_critic.parameters(), max_norm=max_grad_norm,  # type: ignore
         )
 
         self.optimizer.step()  # type: ignore
 
-    def aggregate_and_send_logging_package(
-        self, tracking_info_list: List[TrackingInfo]
-    ):
-        logging_pkg = LoggingPackage(
-            mode=self.mode,
-            training_steps=self.training_pipeline.total_steps,
-            pipeline_stage=self.training_pipeline.current_stage_index,
-            storage_uuid_to_total_experiences=self.training_pipeline.storage_uuid_to_total_experiences,
-        )
-
-        self.aggregate_task_metrics(logging_pkg=logging_pkg)
-
-        for callback_dict in self.single_process_task_callback_data:
-            logging_pkg.task_callback_data.append(callback_dict)
-        self.single_process_task_callback_data = []
-
-        if self.mode == TRAIN_MODE_STR:
-            # Technically self.mode should always be "train" here (as this is the training engine),
-            # this conditional is defensive
-            self._last_aggregated_train_task_metrics.add_scalars(
-                scalars=logging_pkg.metrics_tracker.means(),
-                n=logging_pkg.metrics_tracker.counts(),
-            )
-
-        for tracking_info in tracking_info_list:
-            if tracking_info.n < 0:
-                get_logger().warning(
-                    f"Obtained a train_info_dict with {tracking_info.n} elements."
-                    f" Full info: ({tracking_info.type}, {tracking_info.info}, {tracking_info.n})."
-                )
-            else:
-                tracking_info_dict = tracking_info.info
-
-                if tracking_info.type == TrackingInfoType.LOSS:
-                    tracking_info_dict = {
-                        f"losses/{k}": v for k, v in tracking_info_dict.items()
-                    }
-
-                logging_pkg.add_train_info_dict(
-                    train_info_dict=tracking_info_dict,
-                    n=tracking_info.n,
-                    stage_component_uuid=tracking_info.stage_component_uuid,
-                    storage_uuid=tracking_info.storage_uuid,
-                )
-
-        self.results_queue.put(logging_pkg)
-
     def _save_checkpoint_then_send_checkpoint_for_validation_and_update_last_save_counter(
         self, pipeline_stage_index: Optional[int] = None
     ):
         self.deterministic_seeds()
         if self.worker_id == self.first_local_worker_id:
             model_path = self.checkpoint_save(pipeline_stage_index=pipeline_stage_index)
             if self.checkpoints_queue is not None:
@@ -1378,15 +1500,17 @@
         cur_stage_training_settings = (
             self.training_pipeline.current_stage.training_settings
         )
 
         rollout_storage = self.training_pipeline.rollout_storage
         uuid_to_storage = self.training_pipeline.current_stage_storage
         self.initialize_storage_and_viz(
-            storage_to_initialize=list(uuid_to_storage.values())
+            storage_to_initialize=cast(
+                List[ExperienceStorage], list(uuid_to_storage.values())
+            )
         )
         self.tracking_info_list.clear()
 
         self.last_log = self.training_pipeline.total_steps
 
         if self.last_save is None:
             self.last_save = self.training_pipeline.total_steps
@@ -1482,130 +1606,153 @@
 
             self.former_steps = self.step_count
             former_storage_experiences = {
                 k: v.total_experiences
                 for k, v in self.training_pipeline.current_stage_storage.items()
             }
 
-            vector_tasks_already_restarted = False
-            step = -1
-            while step < cur_stage_training_settings.num_steps - 1:
-                step += 1
+            if self.training_pipeline.rollout_storage_uuid is None:
+                # In this case we're not expecting to collect storage experiences, i.e. everything
+                # will be off-policy.
+
+                # self.step_count is normally updated by the `self.collect_step_across_all_task_samplers`
+                # call below, but since we're not collecting onpolicy experiences, we need to update
+                # it here. The step count here is now just effectively a count of the number of times
+                # we've called `compute_losses_track_them_and_backprop` below.
+                self.step_count += 1
+
+                before_update_info = dict(
+                    next_value=None,
+                    use_gae=cur_stage_training_settings.use_gae,
+                    gamma=cur_stage_training_settings.gamma,
+                    tau=cur_stage_training_settings.gae_lambda,
+                    adv_stats_callback=self.advantage_stats,
+                )
+            else:
+                vector_tasks_already_restarted = False
+                step = -1
+                while step < cur_stage_training_settings.num_steps - 1:
+                    step += 1
 
-                try:
-                    num_paused = self.collect_step_across_all_task_samplers(
-                        rollout_storage_uuid=self.training_pipeline.rollout_storage_uuid,
-                        uuid_to_storage=uuid_to_storage,
-                    )
-                except (TimeoutError, EOFError) as e:
-                    if (
-                        not self.try_restart_after_task_error
-                    ) or self.mode != TRAIN_MODE_STR:
-                        # Apparently you can just call `raise` here and doing so will just raise the exception as though
-                        # it was not caught (so the stacktrace isn't messed up)
-                        raise
-                    elif vector_tasks_already_restarted:
-                        raise RuntimeError(
-                            f"[{self.mode} worker {self.worker_id}] `vector_tasks` has timed out twice in the same"
-                            f" rollout. This suggests that this error was not recoverable. Timeout exception:\n{traceback.format_exc()}"
-                        )
-                    else:
-                        get_logger().warning(
-                            f"[{self.mode} worker {self.worker_id}] `vector_tasks` appears to have crashed during"
-                            f" training due to an {type(e).__name__} error. You have set"
-                            f" `try_restart_after_task_error` to `True` so we will attempt to restart these tasks from"
-                            f" the beginning. USE THIS FEATURE AT YOUR OWN"
-                            f" RISK. Exception:\n{traceback.format_exc()}."
+                    try:
+                        num_paused = self.collect_step_across_all_task_samplers(
+                            rollout_storage_uuid=self.training_pipeline.rollout_storage_uuid,
+                            uuid_to_storage=uuid_to_storage,
                         )
-                        self.vector_tasks.close()
-                        self._vector_tasks = None
+                    except (TimeoutError, EOFError) as e:
+                        if (
+                            not self.try_restart_after_task_error
+                        ) or self.mode != TRAIN_MODE_STR:
+                            # Apparently you can just call `raise` here and doing so will just raise the exception as though
+                            # it was not caught (so the stacktrace isn't messed up)
+                            raise
+                        elif vector_tasks_already_restarted:
+                            raise RuntimeError(
+                                f"[{self.mode} worker {self.worker_id}] `vector_tasks` has timed out twice in the same"
+                                f" rollout. This suggests that this error was not recoverable. Timeout exception:\n{traceback.format_exc()}"
+                            )
+                        else:
+                            get_logger().warning(
+                                f"[{self.mode} worker {self.worker_id}] `vector_tasks` appears to have crashed during"
+                                f" training due to an {type(e).__name__} error. You have set"
+                                f" `try_restart_after_task_error` to `True` so we will attempt to restart these tasks from"
+                                f" the beginning. USE THIS FEATURE AT YOUR OWN"
+                                f" RISK. Exception:\n{traceback.format_exc()}."
+                            )
+                            self.vector_tasks.close()
+                            self._vector_tasks = None
 
-                        vector_tasks_already_restarted = True
-                        for (
-                            storage
-                        ) in self.training_pipeline.current_stage_storage.values():
-                            storage.after_updates()
-                        self.initialize_storage_and_viz(
-                            storage_to_initialize=list(uuid_to_storage.values())
-                        )
-                        step = -1
-                        continue
+                            vector_tasks_already_restarted = True
+                            for (
+                                storage
+                            ) in self.training_pipeline.current_stage_storage.values():
+                                storage.after_updates()
+                            self.initialize_storage_and_viz(
+                                storage_to_initialize=cast(
+                                    List[ExperienceStorage],
+                                    list(uuid_to_storage.values()),
+                                )
+                            )
+                            step = -1
+                            continue
 
-                # A more informative error message should already have been thrown in be given in
-                # `collect_step_across_all_task_samplers` if `num_paused != 0` here but this serves
-                # as a sanity check.
-                assert num_paused == 0
+                    # A more informative error message should already have been thrown in be given in
+                    # `collect_step_across_all_task_samplers` if `num_paused != 0` here but this serves
+                    # as a sanity check.
+                    assert num_paused == 0
+
+                    if self.is_distributed:
+                        # Preempt stragglers
+                        # Each worker will stop collecting steps for the current rollout whenever a
+                        # 100 * distributed_preemption_threshold percentage of workers are finished collecting their
+                        # rollout steps, and we have collected at least 25% but less than 90% of the steps.
+                        num_done = int(self.num_workers_done.get("done"))
+                        if (
+                            num_done
+                            > self.distributed_preemption_threshold * self.num_workers
+                            and 0.25 * cur_stage_training_settings.num_steps
+                            <= step
+                            < 0.9 * cur_stage_training_settings.num_steps
+                        ):
+                            get_logger().debug(
+                                f"[{self.mode} worker {self.worker_id}] Preempted after {step}"
+                                f" steps (out of {cur_stage_training_settings.num_steps})"
+                                f" with {num_done} workers done"
+                            )
+                            break
 
-                if self.is_distributed:
-                    # Preempt stragglers
-                    # Each worker will stop collecting steps for the current rollout whenever a
-                    # 100 * distributed_preemption_threshold percentage of workers are finished collecting their
-                    # rollout steps, and we have collected at least 25% but less than 90% of the steps.
-                    num_done = int(self.num_workers_done.get("done"))
-                    if (
-                        num_done
-                        > self.distributed_preemption_threshold * self.num_workers
-                        and 0.25 * cur_stage_training_settings.num_steps
-                        <= step
-                        < 0.9 * cur_stage_training_settings.num_steps
-                    ):
-                        get_logger().debug(
-                            f"[{self.mode} worker {self.worker_id}] Preempted after {step}"
-                            f" steps (out of {cur_stage_training_settings.num_steps})"
-                            f" with {num_done} workers done"
-                        )
-                        break
+                with torch.no_grad():
+                    actor_critic_output, _ = self.actor_critic(
+                        **rollout_storage.agent_input_for_next_step()
+                    )
 
-            with torch.no_grad():
-                actor_critic_output, _ = self.actor_critic(
-                    **rollout_storage.agent_input_for_next_step()
-                )
+                self.training_pipeline.rollout_count += 1
 
-            self.training_pipeline.rollout_count += 1
+                if self.is_distributed:
+                    # Mark that a worker is done collecting experience
+                    self.num_workers_done.add("done", 1)
+                    self.num_workers_steps.add(
+                        "steps", self.step_count - self.former_steps
+                    )
 
-            if self.is_distributed:
-                # Mark that a worker is done collecting experience
-                self.num_workers_done.add("done", 1)
-                self.num_workers_steps.add("steps", self.step_count - self.former_steps)
+                    # Ensure all workers are done before updating step counter
+                    dist.barrier(
+                        device_ids=None
+                        if self.device == torch.device("cpu")
+                        else [self.device.index]
+                    )
 
-                # Ensure all workers are done before updating step counter
-                dist.barrier(
-                    device_ids=None
-                    if self.device == torch.device("cpu")
-                    else [self.device.index]
-                )
+                    ndone = int(self.num_workers_done.get("done"))
+                    assert (
+                        ndone == self.num_workers
+                    ), f"# workers done {ndone} != # workers {self.num_workers}"
 
-                ndone = int(self.num_workers_done.get("done"))
-                assert (
-                    ndone == self.num_workers
-                ), f"# workers done {ndone} != # workers {self.num_workers}"
+                    # get the actual step_count
+                    self.step_count = (
+                        int(self.num_workers_steps.get("steps")) + self.former_steps
+                    )
 
-                # get the actual step_count
-                self.step_count = (
-                    int(self.num_workers_steps.get("steps")) + self.former_steps
+                before_update_info = dict(
+                    next_value=actor_critic_output.values.detach(),
+                    use_gae=cur_stage_training_settings.use_gae,
+                    gamma=cur_stage_training_settings.gamma,
+                    tau=cur_stage_training_settings.gae_lambda,
+                    adv_stats_callback=self.advantage_stats,
                 )
 
-            before_update_info = dict(
-                next_value=actor_critic_output.values.detach(),
-                use_gae=cur_stage_training_settings.use_gae,
-                gamma=cur_stage_training_settings.gamma,
-                tau=cur_stage_training_settings.gae_lambda,
-                adv_stats_callback=self.advantage_stats,
-            )
-
             # Prepare storage for iteration during updates
             for storage in self.training_pipeline.current_stage_storage.values():
                 storage.before_updates(**before_update_info)
 
             for sc in self.training_pipeline.current_stage.stage_components:
                 component_storage = uuid_to_storage[sc.storage_uuid]
 
                 # before_update = time.time()
 
-                self.update(
+                self.compute_losses_track_them_and_backprop(
                     stage=self.training_pipeline.current_stage,
                     stage_component=sc,
                     storage=component_storage,
                 )
 
                 # after_update = time.time()
                 # delta = after_update - before_update
@@ -1632,14 +1779,15 @@
                     self.training_pipeline.current_stage_storage[k].total_experiences
                     - former_storage_experiences[k]
                 )
                 assert delta >= 0
                 change_in_storage_experiences[k] = self.distributed_weighted_sum(
                     to_share=delta, weight=1
                 )
+
             # Then we update `self.training_pipeline.current_stage.storage_uuid_to_steps_taken_in_stage` with the above
             # computed changes.
             for storage_uuid, delta in change_in_storage_experiences.items():
                 self.training_pipeline.current_stage.storage_uuid_to_steps_taken_in_stage[
                     storage_uuid
                 ] += delta
 
@@ -1674,15 +1822,17 @@
             ):
                 get_logger().info(
                     f"[{self.mode} worker {self.worker_id}] Force advance"
                     f" tasks with {self.training_pipeline.rollout_count} rollouts"
                 )
                 self.vector_tasks.next_task(force_advance_scene=True)
                 self.initialize_storage_and_viz(
-                    storage_to_initialize=list(uuid_to_storage.values())
+                    storage_to_initialize=cast(
+                        List[ExperienceStorage], list(uuid_to_storage.values())
+                    )
                 )
 
     def train(
         self,
         checkpoint_file_name: Optional[str] = None,
         restart_pipeline: bool = False,
         valid_on_initial_weights: bool = False,
@@ -1710,15 +1860,15 @@
             )
             get_logger().error(traceback.format_exc())
         finally:
             if training_completed_successfully:
                 if self.worker_id == 0:
                     self.results_queue.put(("train_stopped", 0))
                 get_logger().info(
-                    f"[{self.mode} worker {self.worker_id}]. Training finished successfully."
+                    f"[{self.mode} worker {self.worker_id}] Training finished successfully."
                 )
             else:
                 self.results_queue.put(("train_stopped", 1 + self.worker_id))
             self.close()
 
 
 class OnPolicyInference(OnPolicyRLEngine):
@@ -1764,40 +1914,85 @@
         self,
         checkpoint_file_path: str,
         rollout_steps: int = 100,
         visualizer: Optional[VizSuite] = None,
         update_secs: float = 20.0,
         verbose: bool = False,
     ) -> LoggingPackage:
-        assert self.actor_critic is not None, "called run_eval with no actor_critic"
+        assert self.actor_critic is not None, "called `run_eval` with no actor_critic"
+
+        # Sanity check that we haven't entered an invalid state. During eval the training_pipeline
+        # should be only set in this function and always unset at the end of it.
+        assert self.training_pipeline is None, (
+            "`training_pipeline` should be `None` before calling `run_eval`."
+            " This is necessary as we want to initialize new storages."
+        )
+        self.training_pipeline = self.config.training_pipeline()
 
-        ckpt = self.checkpoint_load(checkpoint_file_path)
+        ckpt = self.checkpoint_load(checkpoint_file_path, restart_pipeline=False)
         total_steps = cast(int, ckpt["total_steps"])
 
-        training_pipeline = self.config.training_pipeline()
-        rollout_storage = training_pipeline.rollout_storage
+        eval_pipeline_stage = cast(
+            PipelineStage,
+            getattr(self.training_pipeline, f"{self.mode}_pipeline_stage"),
+        )
+        assert (
+            len(eval_pipeline_stage.stage_components) <= 1
+        ), "Only one StageComponent is supported during inference."
+        uuid_to_storage = self.training_pipeline.get_stage_storage(eval_pipeline_stage)
+
+        assert len(uuid_to_storage) > 0, (
+            "No storage found for eval pipeline stage, this is a bug in AllenAct,"
+            " please submit an issue on GitHub (https://github.com/allenai/allenact/issues)."
+        )
+
+        uuid_to_rollout_storage = {
+            uuid: storage
+            for uuid, storage in uuid_to_storage.items()
+            if isinstance(storage, RolloutStorage)
+        }
+        uuid_to_non_rollout_storage = {
+            uuid: storage
+            for uuid, storage in uuid_to_storage.items()
+            if not isinstance(storage, RolloutStorage)
+        }
+
+        if len(uuid_to_rollout_storage) > 1 or len(uuid_to_non_rollout_storage) > 1:
+            raise NotImplementedError(
+                "Only one RolloutStorage and non-RolloutStorage object is allowed within an evaluation pipeline stage."
+                " If you'd like to evaluate against multiple storages please"
+                " submit an issue on GitHub (https://github.com/allenai/allenact/issues). For the moment you'll need"
+                " to evaluate against these storages separately."
+            )
+
+        rollout_storage = self.training_pipeline.rollout_storage
 
         if visualizer is not None:
             assert visualizer.empty()
 
         num_paused = self.initialize_storage_and_viz(
-            storage_to_initialize=[rollout_storage], visualizer=visualizer,
+            storage_to_initialize=cast(
+                List[ExperienceStorage], list(uuid_to_storage.values())
+            ),
+            visualizer=visualizer,
         )
         assert num_paused == 0, f"{num_paused} tasks paused when initializing eval"
 
-        num_tasks = sum(
-            self.vector_tasks.command(
-                "sampler_attr", ["length"] * self.num_active_samplers
-            )
-        ) + (  # We need to add this as the first tasks have already been sampled
-            self.num_active_samplers
-        )
-        # get_logger().debug(
-        #     "worker {} number of tasks {}".format(self.worker_id, num_tasks)
-        # )
+        if rollout_storage is not None:
+            num_tasks = sum(
+                self.vector_tasks.command(
+                    "sampler_attr", ["length"] * self.num_active_samplers
+                )
+            ) + (  # We need to add this as the first tasks have already been sampled
+                self.num_active_samplers
+            )
+        else:
+            num_tasks = 0
+
+        # get_logger().debug("worker {self.worker_id} number of tasks {num_tasks}")
         steps = 0
 
         self.actor_critic.eval()
 
         last_time: float = time.time()
         init_time: float = last_time
         frames: int = 0
@@ -1810,43 +2005,96 @@
         if self.enforce_expert:
             dist_wrapper_class = partial(
                 TeacherForcingDistr,
                 action_space=self.actor_critic.action_space,
                 num_active_samplers=None,
                 approx_steps=None,
                 teacher_forcing=None,
-                tracking_info_list=None,
+                tracking_callback=None,
                 always_enforce=True,
             )
         else:
             dist_wrapper_class = None
 
         logging_pkg = LoggingPackage(
             mode=self.mode,
             training_steps=total_steps,
-            storage_uuid_to_total_experiences={},
+            storage_uuid_to_total_experiences=self.training_pipeline.storage_uuid_to_total_experiences,
+        )
+        should_compute_onpolicy_losses = (
+            len(eval_pipeline_stage.loss_names) > 0
+            and eval_pipeline_stage.stage_components[0].storage_uuid
+            == self.training_pipeline.rollout_storage_uuid
         )
         while self.num_active_samplers > 0:
             frames += self.num_active_samplers
-            self.collect_step_across_all_task_samplers(
-                rollout_storage_uuid=training_pipeline.rollout_storage_uuid,
-                uuid_to_storage={
-                    training_pipeline.rollout_storage_uuid: rollout_storage
-                },
+            num_newly_paused = self.collect_step_across_all_task_samplers(
+                rollout_storage_uuid=self.training_pipeline.rollout_storage_uuid,
+                uuid_to_storage=uuid_to_rollout_storage,
                 visualizer=visualizer,
                 dist_wrapper_class=dist_wrapper_class,
             )
             steps += 1
 
-            if steps % rollout_steps == 0:
-                rollout_storage.after_updates()
+            if should_compute_onpolicy_losses and num_newly_paused > 0:
+                # The `collect_step_across_all_task_samplers` method will automatically drop
+                # parts of the rollout storage that correspond to paused tasks (namely by calling"
+                # `rollout_storage.sampler_select(UNPAUSED_TASK_INDS)`). This makes sense when you don't need to
+                # compute losses for tasks but is a bit limiting here as we're throwing away data before
+                # using it to compute losses. As changing this is non-trivial we'll just warn the user
+                # for now.
+                get_logger().warning(
+                    f"[{self.mode} worker {self.worker_id}] {num_newly_paused * rollout_storage.step} steps"
+                    f" will be dropped when computing losses in evaluation. This is a limitation of the current"
+                    f" implementation of rollout collection in AllenAct. If you'd like to see this"
+                    f" functionality improved please submit an issue on GitHub"
+                    f" (https://github.com/allenai/allenact/issues)."
+                )
+
+            if self.num_active_samplers == 0 or steps % rollout_steps == 0:
+                if should_compute_onpolicy_losses and self.num_active_samplers > 0:
+                    with torch.no_grad():
+                        actor_critic_output, _ = self.actor_critic(
+                            **rollout_storage.agent_input_for_next_step()
+                        )
+                        before_update_info = dict(
+                            next_value=actor_critic_output.values.detach(),
+                            use_gae=eval_pipeline_stage.training_settings.use_gae,
+                            gamma=eval_pipeline_stage.training_settings.gamma,
+                            tau=eval_pipeline_stage.training_settings.gae_lambda,
+                            adv_stats_callback=lambda advantages: {
+                                "mean": advantages.mean(),
+                                "std": advantages.std(),
+                            },
+                        )
+                    # Prepare storage for iteration during loss computation
+                    for storage in uuid_to_rollout_storage.values():
+                        storage.before_updates(**before_update_info)
+
+                    # Compute losses
+                    with torch.no_grad():
+                        for sc in eval_pipeline_stage.stage_components:
+                            self.compute_losses_track_them_and_backprop(
+                                stage=eval_pipeline_stage,
+                                stage_component=sc,
+                                storage=uuid_to_rollout_storage[sc.storage_uuid],
+                                skip_backprop=True,
+                            )
+
+                for storage in uuid_to_rollout_storage.values():
+                    storage.after_updates()
 
             cur_time = time.time()
             if self.num_active_samplers == 0 or cur_time - last_time >= update_secs:
-                self.aggregate_task_metrics(logging_pkg=logging_pkg)
+                logging_pkg = self.aggregate_and_send_logging_package(
+                    tracking_info_list=self.tracking_info_list,
+                    logging_pkg=logging_pkg,
+                    send_logging_package=False,
+                )
+                self.tracking_info_list.clear()
 
                 if verbose:
                     npending: int
                     lengths: List[int]
                     if self.num_active_samplers > 0:
                         lengths = self.vector_tasks.command(
                             "sampler_attr", ["length"] * self.num_active_samplers,
@@ -1879,37 +2127,132 @@
                                 [
                                     f"[{self.mode} worker {self.worker_id}]"
                                     f" num_{self.mode}_tasks_complete {logging_pkg.num_non_empty_metrics_dicts_added}",
                                     *[
                                         f"{k} {v:.3g}"
                                         for k, v in logging_pkg.metrics_tracker.means().items()
                                     ],
+                                    *[
+                                        f"{k0[1]}/{k1} {v1:.3g}"
+                                        for k0, v0 in logging_pkg.info_trackers.items()
+                                        for k1, v1 in v0.means().items()
+                                    ],
                                 ]
                             )
                         )
 
                     last_time = cur_time
 
         get_logger().info(
-            f"[{self.mode} worker {self.worker_id}] Evaluation complete, all task samplers paused."
+            f"[{self.mode} worker {self.worker_id}] Task evaluation complete, all task samplers paused."
         )
 
-        self.vector_tasks.resume_all()
-        self.vector_tasks.set_seeds(self.worker_seeds(self.num_samplers, self.seed))
-        self.vector_tasks.reset_all()
-
-        self.aggregate_task_metrics(logging_pkg=logging_pkg)
-
-        for callback_dict in self.single_process_task_callback_data:
-            logging_pkg.task_callback_data.append(callback_dict)
-        self.single_process_task_callback_data = []
+        if rollout_storage is not None:
+            self.vector_tasks.resume_all()
+            self.vector_tasks.set_seeds(self.worker_seeds(self.num_samplers, self.seed))
+            self.vector_tasks.reset_all()
+
+        logging_pkg = self.aggregate_and_send_logging_package(
+            tracking_info_list=self.tracking_info_list,
+            logging_pkg=logging_pkg,
+            send_logging_package=False,
+        )
+        self.tracking_info_list.clear()
 
         logging_pkg.viz_data = (
             visualizer.read_and_reset() if visualizer is not None else None
         )
+
+        should_compute_offpolicy_losses = (
+            len(eval_pipeline_stage.loss_names) > 0
+            and not should_compute_onpolicy_losses
+        )
+        if should_compute_offpolicy_losses:
+            # In this case we are evaluating a non-rollout storage, e.g. some off-policy data
+            get_logger().info(
+                f"[{self.mode} worker {self.worker_id}] Non-rollout storage detected, will now compute losses"
+                f" using this storage."
+            )
+
+            offpolicy_eval_done = False
+            while not offpolicy_eval_done:
+                before_update_info = dict(
+                    next_value=None,
+                    use_gae=eval_pipeline_stage.training_settings.use_gae,
+                    gamma=eval_pipeline_stage.training_settings.gamma,
+                    tau=eval_pipeline_stage.training_settings.gae_lambda,
+                    adv_stats_callback=lambda advantages: {
+                        "mean": advantages.mean(),
+                        "std": advantages.std(),
+                    },
+                )
+                # Prepare storage for iteration during loss computation
+                for storage in uuid_to_non_rollout_storage.values():
+                    storage.before_updates(**before_update_info)
+
+                # Compute losses
+                assert len(eval_pipeline_stage.stage_components) == 1
+                try:
+                    for sc in eval_pipeline_stage.stage_components:
+                        with torch.no_grad():
+                            self.compute_losses_track_them_and_backprop(
+                                stage=eval_pipeline_stage,
+                                stage_component=sc,
+                                storage=uuid_to_non_rollout_storage[sc.storage_uuid],
+                                skip_backprop=True,
+                            )
+                except EOFError:
+                    offpolicy_eval_done = True
+
+                for storage in uuid_to_non_rollout_storage.values():
+                    storage.after_updates()
+
+                total_bsize = sum(
+                    tif.info.get("worker_batch_size", 0)
+                    for tif in self.tracking_info_list
+                )
+                logging_pkg = self.aggregate_and_send_logging_package(
+                    tracking_info_list=self.tracking_info_list,
+                    logging_pkg=logging_pkg,
+                    send_logging_package=False,
+                )
+                self.tracking_info_list.clear()
+
+                cur_time = time.time()
+                if verbose and (cur_time - last_time >= update_secs):
+                    get_logger().info(
+                        f"[{self.mode} worker {self.worker_id}]"
+                        f" For ckpt {checkpoint_file_path}"
+                        f" {total_bsize / (cur_time - init_time):.1f} its/sec."
+                    )
+                    if logging_pkg.info_trackers != 0:
+                        get_logger().info(
+                            ", ".join(
+                                [
+                                    f"[{self.mode} worker {self.worker_id}]"
+                                    f" num_{self.mode}_iters_complete {total_bsize}",
+                                    *[
+                                        f"{'/'.join(k0)}/{k1} {v1:.3g}"
+                                        for k0, v0 in logging_pkg.info_trackers.items()
+                                        for k1, v1 in v0.means().items()
+                                    ],
+                                ]
+                            )
+                        )
+
+                    last_time = cur_time
+
+        # Call after_updates here to reset all storages
+        for storage in uuid_to_storage.values():
+            storage.after_updates()
+
+        # Set the training pipeline to `None` so that the storages do not
+        # persist across calls to `run_eval`
+        self.training_pipeline = None
+
         logging_pkg.checkpoint_file_name = checkpoint_file_path
 
         return logging_pkg
 
     @staticmethod
     def skip_to_latest(checkpoints_queue: mp.Queue, command: Optional[str], data):
         assert (
@@ -1968,50 +2311,41 @@
                 # get_logger().debug(
                 #     "{} {} command {} data {}".format(
                 #         self.mode, self.worker_id, command, data
                 #     )
                 # )
 
                 if command == "eval":
-                    if self.num_samplers > 0:
-                        if self.mode == VALID_MODE_STR:
-                            # skip to latest using
-                            # 1. there's only consumer in valid
-                            # 2. there's no quit/exit/close message issued by runner nor trainer
-                            ckp_file_path = self.skip_to_latest(
-                                checkpoints_queue=self.checkpoints_queue,
-                                command=command,
-                                data=ckp_file_path,
-                            )
+                    if self.mode == VALID_MODE_STR:
+                        # skip to latest using
+                        # 1. there's only consumer in valid
+                        # 2. there's no quit/exit/close message issued by runner nor trainer
+                        ckp_file_path = self.skip_to_latest(
+                            checkpoints_queue=self.checkpoints_queue,
+                            command=command,
+                            data=ckp_file_path,
+                        )
 
-                        if (
-                            visualizer is None
-                            and self.machine_params.visualizer is not None
-                        ):
-                            visualizer = self.machine_params.visualizer
+                    if (
+                        visualizer is None
+                        and self.machine_params.visualizer is not None
+                    ):
+                        visualizer = self.machine_params.visualizer
 
-                        eval_package = self.run_eval(
-                            checkpoint_file_path=ckp_file_path,
-                            visualizer=visualizer,
-                            verbose=True,
-                            update_secs=20 if self.mode == TEST_MODE_STR else 5 * 60,
-                        )
+                    eval_package = self.run_eval(
+                        checkpoint_file_path=ckp_file_path,
+                        visualizer=visualizer,
+                        verbose=True,
+                        update_secs=20 if self.mode == TEST_MODE_STR else 5 * 60,
+                    )
 
-                        self.results_queue.put(eval_package)
+                    self.results_queue.put(eval_package)
 
-                        if self.is_distributed:
-                            dist.barrier()
-                    else:
-                        self.results_queue.put(
-                            LoggingPackage(
-                                mode=self.mode,
-                                training_steps=None,
-                                storage_uuid_to_total_experiences={},
-                            )
-                        )
+                    if self.is_distributed:
+                        dist.barrier()
                 elif command in ["quit", "exit", "close"]:
                     finalized = True
                     break
                 else:
                     raise NotImplementedError()
         except KeyboardInterrupt:
             get_logger().info(
```

### Comparing `allenact-0.5.2/allenact/algorithms/onpolicy_sync/vector_sampled_tasks.py` & `allenact-0.5.3/allenact/algorithms/onpolicy_sync/vector_sampled_tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -730,15 +730,15 @@
             data_list = [None] * self.num_unpaused_tasks
 
         for write_fn, subcommands, subdata_list in zip(
             self._connection_write_fns,
             self._partition_to_processes(commands),
             self._partition_to_processes(data_list),
         ):
-            write_fn((subcommands, data_list))
+            write_fn((subcommands, subdata_list))
         results = []
         for read_fn in self._connection_read_fns:
             results.extend(read_fn())
         self._is_waiting = False
         return results
 
     def call(
```

### Comparing `allenact-0.5.2/allenact/algorithms/onpolicy_sync/losses/a2cacktr.py` & `allenact-0.5.3/allenact/algorithms/onpolicy_sync/losses/a2cacktr.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/algorithms/onpolicy_sync/losses/ppo.py` & `allenact-0.5.3/allenact/algorithms/onpolicy_sync/losses/ppo.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/algorithms/onpolicy_sync/losses/imitation.py` & `allenact-0.5.3/allenact/algorithms/onpolicy_sync/losses/imitation.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/algorithms/onpolicy_sync/losses/grouped_action_imitation.py` & `allenact-0.5.3/allenact/algorithms/onpolicy_sync/losses/grouped_action_imitation.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/algorithms/onpolicy_sync/losses/abstract_loss.py` & `allenact-0.5.3/allenact/algorithms/onpolicy_sync/losses/abstract_loss.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/algorithms/onpolicy_sync/runner.py` & `allenact-0.5.3/allenact/algorithms/onpolicy_sync/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         machine_id: int = 0,
         save_dir_fmt: SaveDirFormat = SaveDirFormat.FLAT,
         callbacks_paths: Optional[str] = None,
     ):
         self.config = config
         self.output_dir = output_dir
         self.loaded_config_src_files = loaded_config_src_files
-        self.seed = seed if seed is not None else random.randint(0, 2 ** 31 - 1)
+        self.seed = seed if seed is not None else random.randint(0, 2**31 - 1)
         self.deterministic_cudnn = deterministic_cudnn
         self.distributed_preemption_threshold = distributed_preemption_threshold
         if multiprocessing_start_method == "default":
             if torch.cuda.is_available():
                 multiprocessing_start_method = "forkserver"
             else:
                 # Spawn seems to play nicer with cpus and debugging
@@ -141,34 +141,43 @@
         self._collect_valid_results: bool = False
 
         self.distributed_ip_and_port = distributed_ip_and_port
         self.machine_id = machine_id
 
         self.save_dir_fmt = save_dir_fmt
 
-        self.callbacks = self.setup_callback_classes(callbacks_paths)
+        self.callbacks_paths = callbacks_paths
+
+    @lazy_property
+    def callbacks(self):
+        return self.setup_callback_classes(self.callbacks_paths)
 
     @property
     def local_start_time_str(self) -> str:
         if self._local_start_time_str is None:
             raise RuntimeError(
                 "Local start time string does not exist as neither `start_train()` or `start_test()`"
                 " has been called on this runner."
             )
         return self._local_start_time_str
 
     @property
     def running_validation(self):
+        pipeline = self.config.training_pipeline()
         return (
             sum(
                 MachineParams.instance_from(
                     self.config.machine_params(VALID_MODE_STR)
                 ).nprocesses
             )
             > 0
+            or (
+                pipeline.rollout_storage_uuid is None
+                and len(pipeline.valid_pipeline_stage.loss_names) > 0
+            )
         ) and self.machine_id == 0
 
     @staticmethod
     def init_context(
         mp_ctx: Optional[BaseContext] = None,
         multiprocessing_start_method: str = "forkserver",
         valid_start_methods: Tuple[str, ...] = ("forkserver", "spawn", "fork"),
@@ -185,44 +194,78 @@
                 f"ignoring multiprocessing_start_method '{multiprocessing_start_method}'"
                 f" and using given context with '{mp_ctx.get_start_method()}'"
             )
 
         return mp_ctx
 
     def setup_callback_classes(self, callbacks: Optional[str]) -> Set[Callback]:
-        """Get a list of Callback classes from a comma-separated list of
-        filenames."""
+        """Get a list of Callback classes from a comma-separated list of files,
+        paths, and/or functions.
+
+        After separating the `callbacks` into a list of strings, each string should either
+        be a:
+        1. Name of a function defined on the experiment config that, when called, returns an
+           object with of type `Callback`.
+        2. Path to a python file containing a single class that inherits from `Callback`.
+        3. Module path (e.g. `path.to.module`) where this module contains a single class that
+            inherits from `Callback`.
+        """
         if callbacks == "" or callbacks is None:
             return set()
 
-        setup_dict = dict(name=self.experiment_name, config=self.config, mode=self.mode)
-        callback_classes = set()
+        setup_dict = dict(
+            name=f"{self.experiment_name}/{self.local_start_time_str}",
+            config=self.config,
+            mode=self.mode,
+        )
+
+        callback_objects = set()
         files = callbacks.split(",")
         for filename in files:
+            # Check if the `filename` is a function on the config
+            if not any(k in filename for k in [".", "/"]):
+                callback_func = getattr(self.config, filename, None)
+                if callback_func is not None:
+                    callback = callback_func()
+                    callback.setup(**setup_dict)
+                    callback_objects.add(callback)
+                    continue
+
+            # Otherwise find the Callback class in the file or module
             module_path = filename.replace("/", ".")
             if module_path.endswith(".py"):
                 module_path = module_path[:-3]
             module = importlib.import_module(module_path)
             classes = inspect.getmembers(module, inspect.isclass)
 
-            for mod_class in classes:
-                if issubclass(mod_class[1], Callback) and mod_class[1] != Callback:
-                    # NOTE: initialize the callback class
-                    inst_class = mod_class[1]()
-                    inst_class.setup(**setup_dict)
-                    callback_classes.add(inst_class)
+            callback_classes = [
+                mod_class[1]
+                for mod_class in classes
+                if issubclass(mod_class[1], Callback)
+            ]
+
+            assert callback_classes == 1, (
+                f"Expected a single callback class in {filename}, but found {len(callback_classes)}."
+                f" These classes were found: {callback_classes}."
+            )
+
+            for mod_class in callback_classes:
+                # NOTE: initialize the callback class
+                callback = mod_class[1]()
+                callback.setup(**setup_dict)
+                callback_objects.add(callback)
 
-        return callback_classes
+        return callback_objects
 
     def _acquire_unique_local_start_time_string(self) -> str:
         """Creates a (unique) local start time string for this experiment.
 
         Ensures through file locks that the local start time string
         produced is unique. This implies that, if one has many
-        experiments starting in in parallel, at most one will be started
+        experiments starting in parallel, at most one will be started
         every second (as the local start time string only records the
         time up to the current second).
         """
         os.makedirs(self.output_dir, exist_ok=True)
         start_time_string_lock_path = os.path.abspath(
             os.path.join(self.output_dir, ".allenact_start_time_string.lock")
         )
@@ -517,28 +560,35 @@
                 else model_hash,
                 first_local_worker_id=worker_ids[0],
                 distributed_preemption_threshold=self.distributed_preemption_threshold,
                 valid_on_initial_weights=valid_on_initial_weights,
                 try_restart_after_task_error=try_restart_after_task_error,
             )
             train: BaseProcess = self.mp_ctx.Process(
-                target=self.train_loop, kwargs=training_kwargs,
+                target=self.train_loop,
+                kwargs=training_kwargs,
             )
             try:
                 train.start()
-            except ValueError as e:
+            except (ValueError, OSError, ConnectionRefusedError, EOFError) as e:
                 # If the `initial_model_state_dict` is too large we sometimes
                 # run into errors passing it with multiprocessing. In such cases
                 # we instead hash the state_dict and confirm, in each engine worker, that
                 # this hash equals the model the engine worker instantiates.
-                if e.args[0] == "too many fds":
+                if (
+                    (isinstance(e, ValueError) and e.args[0] == "too many fds")
+                    or (isinstance(e, OSError) and e.errno == 22)
+                    or (isinstance(e, ConnectionRefusedError) and e.errno == 111)
+                    or isinstance(e, EOFError)
+                ):
                     model_hash = md5_hash_of_state_dict(initial_model_state_dict)
                     training_kwargs["initial_model_state_dict"] = model_hash
                     train = self.mp_ctx.Process(
-                        target=self.train_loop, kwargs=training_kwargs,
+                        target=self.train_loop,
+                        kwargs=training_kwargs,
                     )
                     train.start()
                 else:
                     raise e
 
             self.processes[TRAIN_MODE_STR].append(train)
 
@@ -734,17 +784,25 @@
         path_parts = [
             self.config.tag()
             if self.extra_tag == ""
             else os.path.join(self.config.tag(), self.extra_tag),
             start_time_str or self.local_start_time_str,
         ]
         if self.save_dir_fmt == SaveDirFormat.NESTED:
-            folder = os.path.join(self.output_dir, *path_parts, "checkpoints",)
+            folder = os.path.join(
+                self.output_dir,
+                *path_parts,
+                "checkpoints",
+            )
         elif self.save_dir_fmt == SaveDirFormat.FLAT:
-            folder = os.path.join(self.output_dir, "checkpoints", *path_parts,)
+            folder = os.path.join(
+                self.output_dir,
+                "checkpoints",
+                *path_parts,
+            )
         else:
             raise NotImplementedError
         if create_if_none:
             os.makedirs(folder, exist_ok=True)
         return folder
 
     def log_writer_path(self, start_time_str: str) -> str:
@@ -779,15 +837,18 @@
             return path
         else:
             raise NotImplementedError
 
     def metric_path(self, start_time_str: str) -> str:
         if self.save_dir_fmt == SaveDirFormat.NESTED:
             return os.path.join(
-                self.output_dir, "test", self.config.tag(), start_time_str,
+                self.output_dir,
+                "test",
+                self.config.tag(),
+                start_time_str,
             )
         elif self.save_dir_fmt == SaveDirFormat.FLAT:
             return os.path.join(
                 self.output_dir,
                 "metrics",
                 self.config.tag()
                 if self.extra_tag == ""
@@ -801,17 +862,25 @@
         path_parts = [
             self.config.tag()
             if self.extra_tag == ""
             else os.path.join(self.config.tag(), self.extra_tag),
             self.local_start_time_str,
         ]
         if self.save_dir_fmt == SaveDirFormat.NESTED:
-            base_dir = os.path.join(self.output_dir, *path_parts, "used_configs",)
+            base_dir = os.path.join(
+                self.output_dir,
+                *path_parts,
+                "used_configs",
+            )
         elif self.save_dir_fmt == SaveDirFormat.FLAT:
-            base_dir = os.path.join(self.output_dir, "used_configs", *path_parts,)
+            base_dir = os.path.join(
+                self.output_dir,
+                "used_configs",
+                *path_parts,
+            )
         else:
             raise NotImplementedError
         os.makedirs(base_dir, exist_ok=True)
 
         # Saving current git diff
         try:
             sha, diff_str = get_git_diff_of_project()
@@ -825,15 +894,15 @@
                 f" Is it possible that {os.getcwd()} is not under version control?"
             )
 
         # Saving configs
         if self.loaded_config_src_files is not None:
             for src_path in self.loaded_config_src_files:
                 if src_path == CONFIG_KWARGS_STR:
-                    # We also save key-word arguments passed to to the experiment
+                    # We also save key-word arguments passed to the experiment
                     # initializer.
                     save_path = os.path.join(base_dir, "config_kwargs.json")
                     assert not os.path.exists(
                         save_path
                     ), f"{save_path} should not already exist."
                     with open(save_path, "w") as f:
                         json.dump(json.loads(self.loaded_config_src_files[src_path]), f)
@@ -846,15 +915,16 @@
                 # here until we find a prefix (if necessary) to prevent
                 # name collisions.
                 k = -1
                 while True:
                     prefix = "" if k == -1 else f"namecollision{k}__"
                     k += 1
                     dst_path = os.path.join(
-                        base_dir, f"{prefix}{os.path.basename(src_path)}",
+                        base_dir,
+                        f"{prefix}{os.path.basename(src_path)}",
                     )
                     if not os.path.exists(dst_path):
                         os.makedirs(os.path.dirname(dst_path), exist_ok=True)
                         with open(src_path, "r") as f:
                             file_contents = f.read()
                         with open(dst_path, "w") as f:
                             f.write(
@@ -862,328 +932,360 @@
                             )
                         break
 
         get_logger().info(f"Config files saved to {base_dir}")
         for callback in self.callbacks:
             callback.after_save_project_state(base_dir=base_dir)
 
-    def process_valid_package(
+    def _update_keys(
         self,
-        log_writer: Optional[SummaryWriter],
-        pkg: LoggingPackage,
-        all_results: Optional[List[Any]] = None,
-    ):
-        training_steps = pkg.training_steps
-        checkpoint_file_name = pkg.checkpoint_file_name
-        render = pkg.viz_data
-        task_outputs = pkg.metric_dicts
-
-        num_tasks = pkg.num_non_empty_metrics_dicts_added
-        metric_means = pkg.metrics_tracker.means()
-        callback_metric_means = dict()
-        tasks_callback_data = pkg.task_callback_data
-
-        mode = pkg.mode
-        assert mode == "valid"
-
-        num_tasks_key = f"{mode}-misc/num_tasks_evaled"
-        if log_writer is not None:
-            log_writer.add_scalar(num_tasks_key, num_tasks, training_steps)
-        callback_metric_means[num_tasks_key] = num_tasks
-
-        message = [f"{mode} {training_steps} steps:"]
-        for k in sorted(metric_means.keys()):
-            metrics_key = f"{mode}-metrics/{k}"
-            if log_writer is not None:
-                log_writer.add_scalar(metrics_key, metric_means[k], training_steps)
-            callback_metric_means[metrics_key] = metric_means[k]
-            message.append(f"{k} {metric_means[k]}")
-
-        results = copy.deepcopy(metric_means)
-        results.update({"training_steps": training_steps, "tasks": task_outputs})
-        if all_results is not None:
-            all_results.append(results)
-
-        message.append(f"tasks {num_tasks} checkpoint {checkpoint_file_name}")
-        get_logger().info(" ".join(message))
+        d: Union[Dict[str, Any], str],
+        tag_if_not_a_loss: str,
+        mode: str,
+        stage_component_uuid: Optional[str] = None,
+    ) -> Union[Dict[str, Any], str]:
+        midfix = "-" if stage_component_uuid is None else f"-{stage_component_uuid}-"
+
+        def _convert(key: str):
+            if key.startswith("losses/"):
+                return f"{mode}{midfix}{key}"
+            else:
+                return f"{mode}{midfix}{tag_if_not_a_loss}/{key}"
 
-        for callback in self.callbacks:
-            callback.on_valid_log(
-                metric_means=callback_metric_means,
-                metrics=results,
-                step=training_steps,
-                checkpoint_file_name=checkpoint_file_name,
-                tasks_data=tasks_callback_data,
-            )
+        if isinstance(d, str):
+            return _convert(d)
+        return {_convert(k): v for k, v in d.items()}
 
-        if self.visualizer is not None:
-            self.visualizer.log(
-                log_writer=log_writer,
-                task_outputs=task_outputs,
-                render=render,
-                num_steps=training_steps,
-            )
-
-    def process_train_packages(
+    def _process_logging_packages(
         self,
         log_writer: Optional[SummaryWriter],
-        pkgs: List[LoggingPackage],
-        last_steps: int,
-        last_storage_uuid_to_total_experiences: Dict[str, int],
-        last_time: float,
+        pkgs: Union[LoggingPackage, List[LoggingPackage]],
+        last_steps: Optional[int],
+        last_storage_uuid_to_total_experiences: Optional[Dict[str, int]],
+        last_time: Optional[float],
+        all_results: Optional[List[Any]] = None,
     ):
-        assert self.mode == TRAIN_MODE_STR
-        callback_metric_means = dict()
+        mode = pkgs[0].mode
+        assert all(
+            pkg.mode == mode for pkg in pkgs
+        ), "All logging packages must be the same mode."
+        assert mode == self.mode or (
+            mode == VALID_MODE_STR and self.mode == TRAIN_MODE_STR
+        ), (
+            "Logging package mode must match the logger mode except when training where the logging package may"
+            "be of mode 'valid'."
+        )
+        training = mode == TRAIN_MODE_STR  # Are we logging training packages
 
         current_time = time.time()
 
         training_steps = pkgs[0].training_steps
         storage_uuid_to_total_experiences = pkgs[0].storage_uuid_to_total_experiences
+        callback_metric_means = dict()
 
-        if log_writer is not None:
+        def update_keys_misc(
+            key_or_dict: Union[str, Dict[str, Any]],
+            stage_component_uuid: Optional[str] = None,
+        ):
+            # Important to use mode and not self.mode here
+            return self._update_keys(
+                d=key_or_dict,
+                tag_if_not_a_loss="misc",
+                mode=mode,
+                stage_component_uuid=stage_component_uuid,
+            )
+
+        def update_keys_metric(
+            key_or_dict: Union[str, Dict[str, Any]],
+            stage_component_uuid: Optional[str] = None,
+        ):
+            # Important to use mode and not self.mode here
+            return self._update_keys(
+                d=key_or_dict,
+                tag_if_not_a_loss="metrics",
+                mode=mode,
+                stage_component_uuid=stage_component_uuid,
+            )
+
+        if training and log_writer is not None:
             log_writer.add_scalar(
-                tag="train-misc/pipeline_stage",
+                tag=update_keys_misc("pipeline_stage"),
                 scalar_value=pkgs[0].pipeline_stage,
                 global_step=training_steps,
             )
-        callback_metric_means[f"train-misc/pipeline_stage"] = pkgs[0].pipeline_stage
+        callback_metric_means[update_keys_misc("pipeline_stage")] = pkgs[
+            0
+        ].pipeline_stage
 
+        storage_uuid_to_total_experiences_key = {}
         for storage_uuid, val in storage_uuid_to_total_experiences.items():
-            total_experiences_key = f"train-misc/{storage_uuid}_total_experiences"
-            if log_writer is not None:
+            total_experiences_key = update_keys_misc(
+                f"{storage_uuid}_total_experiences"
+            )
+            storage_uuid_to_total_experiences_key[storage_uuid] = total_experiences_key
+
+            if training and log_writer is not None:
                 log_writer.add_scalar(
                     tag=total_experiences_key,
                     scalar_value=val,
                     global_step=training_steps,
                 )
             callback_metric_means[total_experiences_key] = val
 
-        def add_prefix(
-            d: Union[Dict[str, Any], str],
-            tag_if_not_a_loss: str,
-            stage_component_uuid: Optional[str],
-        ) -> Union[Dict[str, Any], str]:
-            midfix = (
-                "-" if stage_component_uuid is None else f"-{stage_component_uuid}-"
-            )
-
-            def _convert(key: str):
-                if key.startswith("losses/"):
-                    return f"{self.mode}{midfix}{key}"
-                else:
-                    return f"{self.mode}{midfix}{tag_if_not_a_loss}/{key}"
-
-            if isinstance(d, str):
-                return _convert(d)
-            return {_convert(k): v for k, v in d.items()}
-
-        metrics_and_train_info_tracker = ScalarMeanTracker()
+        metrics_and_info_tracker = ScalarMeanTracker()
         scalar_name_to_total_storage_experience = {}
+        scalar_name_to_total_experiences_key = {}
         storage_uuid_to_stage_component_uuids = defaultdict(lambda: set())
+        metric_dicts_list, render, checkpoint_file_name = [], {}, []
         tasks_callback_data = []
+
         for pkg in pkgs:
-            metrics_and_train_info_tracker.add_scalars(
-                scalars=add_prefix(pkg.metrics_tracker.means(), "metrics", None),
-                n=add_prefix(pkg.metrics_tracker.counts(), "metrics", None),
+            metrics_and_info_tracker.add_scalars(
+                scalars=update_keys_metric(pkg.metrics_tracker.means()),
+                n=update_keys_metric(pkg.metrics_tracker.counts()),
             )
             tasks_callback_data.extend(pkg.task_callback_data)
+            metric_dicts_list.extend(pkg.metric_dicts)
+            if pkg.viz_data is not None:
+                render.update(pkg.viz_data)
+            checkpoint_file_name.append(pkg.checkpoint_file_name)
 
             for (
                 (stage_component_uuid, storage_uuid),
-                train_info_tracker,
-            ) in pkg.train_info_trackers.items():
+                info_tracker,
+            ) in pkg.info_trackers.items():
 
-                storage_uuid_to_stage_component_uuids[storage_uuid].add(
-                    stage_component_uuid
-                )
+                if stage_component_uuid is not None:
+                    storage_uuid_to_stage_component_uuids[storage_uuid].add(
+                        stage_component_uuid
+                    )
 
-                train_info_means = add_prefix(
-                    train_info_tracker.means(),
-                    tag_if_not_a_loss="misc",
-                    stage_component_uuid=stage_component_uuid,
+                info_means = update_keys_misc(
+                    info_tracker.means(),
+                    stage_component_uuid,
                 )
-                train_info_counts = add_prefix(
-                    train_info_tracker.counts(),
-                    tag_if_not_a_loss="misc",
-                    stage_component_uuid=stage_component_uuid,
+                info_counts = update_keys_misc(
+                    info_tracker.counts(),
+                    stage_component_uuid,
                 )
-                metrics_and_train_info_tracker.add_scalars(
-                    scalars=train_info_means, n=train_info_counts,
+                metrics_and_info_tracker.add_scalars(
+                    scalars=info_means,
+                    n=info_counts,
                 )
 
-                if storage_uuid is None:
-                    assert stage_component_uuid is None
-                    total_exp_for_storage = training_steps
-                else:
-                    total_exp_for_storage = pkg.storage_uuid_to_total_experiences[
-                        storage_uuid
-                    ]
-                for scalar_name in train_info_means:
+                total_exp_for_storage = pkg.storage_uuid_to_total_experiences[
+                    storage_uuid
+                ]
+
+                if stage_component_uuid is None:
+                    assert total_exp_for_storage == training_steps
+
+                for scalar_name in info_means:
                     if scalar_name in scalar_name_to_total_storage_experience:
                         assert (
                             total_exp_for_storage
                             == scalar_name_to_total_storage_experience[scalar_name]
                         ), (
                             f"For metric {scalar_name}: there is disagreement between the training steps parameter"
                             f" across different workers ({total_exp_for_storage} !="
                             f" {scalar_name_to_total_storage_experience[scalar_name]}). This suggests an error in "
                             f" AllenAct, please report this issue at https://github.com/allenai/allenact/issues."
                         )
                     else:
                         scalar_name_to_total_storage_experience[
                             scalar_name
                         ] = total_exp_for_storage
+                        scalar_name_to_total_experiences_key[
+                            scalar_name
+                        ] = storage_uuid_to_total_experiences_key[storage_uuid]
+
+        assert all_equal(
+            checkpoint_file_name
+        ), f"All {mode} logging packages must have the same checkpoint_file_name."
 
         message = [
-            f"TRAIN: {training_steps} rollout steps ({pkgs[0].storage_uuid_to_total_experiences})"
+            f"{mode.upper()}: {training_steps} rollout steps ({pkgs[0].storage_uuid_to_total_experiences})"
         ]
-        means = metrics_and_train_info_tracker.means()
-        callback_metric_means.update(means)
+        metrics_and_info_means = metrics_and_info_tracker.means()
+        callback_metric_means.update(metrics_and_info_means)
 
         for k in sorted(
-            means.keys(), key=lambda mean_key: (mean_key.count("/"), mean_key)
+            metrics_and_info_means.keys(),
+            key=lambda mean_key: (mean_key.count("/"), mean_key),
         ):
             if log_writer is not None:
                 log_writer.add_scalar(
                     tag=k,
-                    scalar_value=means[k],
+                    scalar_value=metrics_and_info_means[k],
                     global_step=scalar_name_to_total_storage_experience.get(
                         k, training_steps
                     ),
                 )
             short_key = (
-                "/".join(k.split("/")[1:]) if k.startswith("train-") and "/" in k else k
-            )
-            message.append(f"{short_key} {means[k]:.3g}")
-        message += [f"elapsed_time {(current_time - last_time):.3g}s"]
+                "/".join(k.split("/")[1:])
+                if k.startswith(f"{mode}-") and "/" in k
+                else k
+            )
+            message.append(f"{short_key} {metrics_and_info_means[k]:.3g}")
+
+        if training:
+            # Log information about FPS and EPS (experiences per second, for non-rollout storage).
+            # Not needed during testing or validation.
+            message += [f"elapsed_time {(current_time - last_time):.3g}s"]
+
+            if last_steps > 0:
+                fps = (training_steps - last_steps) / (current_time - last_time)
+                message += [f"approx_fps {fps:.3g}"]
+                approx_fps_key = update_keys_misc("approx_fps")
+                if log_writer is not None:
+                    log_writer.add_scalar(approx_fps_key, fps, training_steps)
+                callback_metric_means[approx_fps_key] = fps
 
-        if last_steps > 0:
-            fps = (training_steps - last_steps) / (current_time - last_time)
-            message += [f"approx_fps {fps:.3g}"]
-            approx_fps_key = add_prefix("approx_fps", "misc", None)
-            if log_writer is not None:
-                log_writer.add_scalar(approx_fps_key, fps, training_steps)
-            callback_metric_means[approx_fps_key] = fps
-
-        for (
-            storage_uuid,
-            last_total_exp,
-        ) in last_storage_uuid_to_total_experiences.items():
-            if storage_uuid in storage_uuid_to_total_experiences:
-                cur_total_exp = storage_uuid_to_total_experiences[storage_uuid]
-                eps = (cur_total_exp - last_total_exp) / (current_time - last_time)
-                message += [f"{storage_uuid}/approx_eps {eps:.3g}"]
-                for stage_component_uuid in storage_uuid_to_stage_component_uuids[
-                    storage_uuid
-                ]:
-                    approx_eps_key = add_prefix(
-                        f"approx_eps",
-                        "misc",
-                        stage_component_uuid=stage_component_uuid,
-                    )
-                    callback_metric_means[approx_eps_key] = eps
-                    if log_writer is not None:
-                        log_writer.add_scalar(
-                            approx_eps_key, eps, cur_total_exp,
+            for (
+                storage_uuid,
+                last_total_exp,
+            ) in last_storage_uuid_to_total_experiences.items():
+                if storage_uuid in storage_uuid_to_total_experiences:
+                    cur_total_exp = storage_uuid_to_total_experiences[storage_uuid]
+                    eps = (cur_total_exp - last_total_exp) / (current_time - last_time)
+                    message += [f"{storage_uuid}/approx_eps {eps:.3g}"]
+                    for stage_component_uuid in storage_uuid_to_stage_component_uuids[
+                        storage_uuid
+                    ]:
+                        approx_eps_key = update_keys_misc(
+                            f"approx_eps",
+                            stage_component_uuid,
                         )
+                        callback_metric_means[approx_eps_key] = eps
+                        scalar_name_to_total_experiences_key[
+                            approx_eps_key
+                        ] = storage_uuid_to_total_experiences_key[storage_uuid]
+
+                        if log_writer is not None:
+                            log_writer.add_scalar(
+                                approx_eps_key,
+                                eps,
+                                cur_total_exp,
+                            )
 
-        get_logger().info(" ".join(message))
-
-        metrics = []
-        for pkg in pkgs:
-            metrics.extend(pkg.metric_dicts)
-
-        for callback in self.callbacks:
-            callback.on_train_log(
-                metrics=metrics,
-                metric_means=callback_metric_means,
-                step=training_steps,
-                tasks_data=tasks_callback_data,
-            )
-
-        return training_steps, storage_uuid_to_total_experiences, current_time
-
-    def process_test_packages(
-        self,
-        log_writer: Optional[SummaryWriter],
-        pkgs: List[LoggingPackage],
-        all_results: Optional[List[Any]] = None,
-    ):
-        mode = pkgs[0].mode
-        assert mode == TEST_MODE_STR
-
-        training_steps = pkgs[0].training_steps
-
-        all_metrics_tracker = ScalarMeanTracker()
-        metric_dicts_list, render, checkpoint_file_name = [], {}, []
-        tasks_callback_data = []
-        for pkg in pkgs:
-            all_metrics_tracker.add_scalars(
-                scalars=pkg.metrics_tracker.means(), n=pkg.metrics_tracker.counts()
-            )
-            tasks_callback_data.extend(pkg.task_callback_data)
-            metric_dicts_list.extend(pkg.metric_dicts)
-            if pkg.viz_data is not None:
-                render.update(pkg.viz_data)
-            checkpoint_file_name.append(pkg.checkpoint_file_name)
-
-        assert all_equal(checkpoint_file_name)
-
-        message = [f"{mode} {training_steps} steps:"]
-
-        metric_means = all_metrics_tracker.means()
-        callback_metric_means = dict()
-        for k in sorted(metric_means.keys()):
-            metrics_key = f"{mode}-metrics/{k}"
-            if log_writer is not None:
-                log_writer.add_scalar(metrics_key, metric_means[k], training_steps)
-            callback_metric_means[metrics_key] = metric_means[k]
-            message.append(k + f" {metric_means[k]:.3g}")
-
+        metrics_and_info_means_with_metrics_dicts_list = copy.deepcopy(
+            metrics_and_info_means
+        )
+        metrics_and_info_means_with_metrics_dicts_list.update(
+            {"training_steps": training_steps, "tasks": metric_dicts_list}
+        )
         if all_results is not None:
-            results = copy.deepcopy(metric_means)
-            results.update(
-                {"training_steps": training_steps, "tasks": metric_dicts_list}
-            )
-            all_results.append(results)
+            all_results.append(metrics_and_info_means_with_metrics_dicts_list)
 
         num_tasks = sum([pkg.num_non_empty_metrics_dicts_added for pkg in pkgs])
-
-        num_tasks_evaled_key = f"{mode}-misc/num_tasks_evaled"
+        num_tasks_completed_key = update_keys_misc("num_tasks_completed_since_last_log")
         if log_writer is not None:
-            log_writer.add_scalar(num_tasks_evaled_key, num_tasks, training_steps)
-        callback_metric_means[num_tasks_evaled_key] = num_tasks
+            log_writer.add_scalar(num_tasks_completed_key, num_tasks, training_steps)
+        callback_metric_means[num_tasks_completed_key] = num_tasks
+
+        message.append(f"new_tasks_completed {num_tasks}")
+        if not training:
+            message.append(f"checkpoint {checkpoint_file_name[0]}")
 
-        message.append(f"tasks {num_tasks} checkpoint {checkpoint_file_name[0]}")
         get_logger().info(" ".join(message))
 
         for callback in self.callbacks:
-            callback.on_test_log(
-                metric_means=callback_metric_means,
-                metrics=all_results[-1],
-                step=training_steps,
-                checkpoint_file_name=checkpoint_file_name[0],
-                tasks_data=tasks_callback_data,
-            )
+            if mode == TRAIN_MODE_STR:
+                callback.on_train_log(
+                    metrics=metric_dicts_list,
+                    metric_means=callback_metric_means,
+                    step=training_steps,
+                    tasks_data=tasks_callback_data,
+                    scalar_name_to_total_experiences_key=scalar_name_to_total_experiences_key,
+                )
+
+            if mode == VALID_MODE_STR:
+                callback.on_valid_log(
+                    metrics=metrics_and_info_means_with_metrics_dicts_list,
+                    metric_means=callback_metric_means,
+                    step=training_steps,
+                    checkpoint_file_name=checkpoint_file_name[0],
+                    tasks_data=tasks_callback_data,
+                    scalar_name_to_total_experiences_key=scalar_name_to_total_experiences_key,
+                )
+
+            if mode == TEST_MODE_STR:
+                callback.on_test_log(
+                    metrics=metrics_and_info_means_with_metrics_dicts_list,
+                    metric_means=callback_metric_means,
+                    step=training_steps,
+                    checkpoint_file_name=checkpoint_file_name[0],
+                    tasks_data=tasks_callback_data,
+                    scalar_name_to_total_experiences_key=scalar_name_to_total_experiences_key,
+                )
 
         if self.visualizer is not None:
             self.visualizer.log(
                 log_writer=log_writer,
                 task_outputs=metric_dicts_list,
                 render=render,
                 num_steps=training_steps,
             )
 
+        return training_steps, storage_uuid_to_total_experiences, current_time
+
+    def process_valid_package(
+        self,
+        log_writer: Optional[SummaryWriter],
+        pkg: LoggingPackage,
+        all_results: Optional[List[Any]] = None,
+    ):
+        return self._process_logging_packages(
+            log_writer=log_writer,
+            pkgs=[pkg],
+            last_steps=None,
+            last_storage_uuid_to_total_experiences=None,
+            last_time=None,
+            all_results=all_results,
+        )
+
+    def process_train_packages(
+        self,
+        log_writer: Optional[SummaryWriter],
+        pkgs: List[LoggingPackage],
+        last_steps: int,
+        last_storage_uuid_to_total_experiences: Dict[str, int],
+        last_time: float,
+    ):
+        return self._process_logging_packages(
+            log_writer=log_writer,
+            pkgs=pkgs,
+            last_steps=last_steps,
+            last_storage_uuid_to_total_experiences=last_storage_uuid_to_total_experiences,
+            last_time=last_time,
+        )
+
+    def process_test_packages(
+        self,
+        log_writer: Optional[SummaryWriter],
+        pkgs: List[LoggingPackage],
+        all_results: Optional[List[Any]] = None,
+    ):
+        return self._process_logging_packages(
+            log_writer=log_writer,
+            pkgs=pkgs,
+            last_steps=None,
+            last_storage_uuid_to_total_experiences=None,
+            last_time=None,
+            all_results=all_results,
+        )
+
     def log_and_close(
         self,
         start_time_str: str,
         nworkers: int,
         test_steps: Sequence[int] = (),
         metrics_file: Optional[str] = None,
     ) -> List[Dict]:
+        ptitle(f"AllenAct-Logging-{self.local_start_time_str}")
         finalized = False
 
         log_writer: Optional[SummaryWriter] = None
         if not self.disable_tensorboard:
             log_writer = SummaryWriter(
                 log_dir=self.log_writer_path(start_time_str),
                 filename_suffix=f"__{self.mode}_{self.local_start_time_str}",
```

### Comparing `allenact-0.5.2/allenact/base_abstractions/distributions.py` & `allenact-0.5.3/allenact/base_abstractions/distributions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import abc
 from collections import OrderedDict
-from typing import Any, Union, Callable, TypeVar, Dict, Optional, cast, List
+from typing import Any, Union, Callable, TypeVar, Dict, Optional, cast, Protocol
 
 import gym
 import torch
 import torch.nn as nn
 from torch.distributions.utils import lazy_property
 
-from allenact.algorithms.onpolicy_sync.misc import TrackingInfoType, TrackingInfo
+from allenact.algorithms.onpolicy_sync.misc import TrackingInfoType
 from allenact.base_abstractions.sensor import AbstractExpertActionSensor as Expert
 from allenact.utils import spaces_utils as su
 from allenact.utils.misc_utils import all_unique
 
 TeacherForcingAnnealingType = TypeVar("TeacherForcingAnnealingType")
 
 """
@@ -205,35 +205,40 @@
                 res = res + current_log_prob
             else:
                 res[cd.action_group_name] = current_log_prob
 
         return res
 
 
+class TrackingCallback(Protocol):
+    def __call__(self, type: TrackingInfoType, info: Dict[str, Any], n: int):
+        ...
+
+
 class TeacherForcingDistr(Distr):
     def __init__(
         self,
         distr: Distr,
         obs: Dict[str, Any],
         action_space: gym.spaces.Space,
         num_active_samplers: Optional[int],
         approx_steps: Optional[int],
         teacher_forcing: Optional[TeacherForcingAnnealingType],
-        tracking_info_list: Optional[List[TrackingInfo]],
+        tracking_callback: Optional[TrackingCallback],
         always_enforce: bool = False,
     ):
         self.distr = distr
         self.is_sequential = isinstance(self.distr, SequentialDistr)
 
         # action_space is a gym.spaces.Dict for SequentialDistr, or any gym.Space for other Distr
         self.action_space = action_space
         self.num_active_samplers = num_active_samplers
         self.approx_steps = approx_steps
         self.teacher_forcing = teacher_forcing
-        self.tracking_info_list = tracking_info_list
+        self.tracking_callback = tracking_callback
         self.always_enforce = always_enforce
 
         assert (
             "expert_action" in obs
         ), "When using teacher forcing, obs must contain an `expert_action` uuid"
 
         obs_space = Expert.flagged_space(
@@ -332,23 +337,19 @@
             res = self.enforce(
                 self.distr.sample(sample_shape),
                 self.action_space,
                 self.expert,
                 teacher_force_info,
             )
 
-        if self.tracking_info_list is not None and self.num_active_samplers is not None:
-            self.tracking_info_list.append(
-                TrackingInfo(
-                    type=TrackingInfoType.TEACHER_FORCING,
-                    info=teacher_force_info,
-                    n=self.num_active_samplers,
-                    storage_uuid=None,
-                    stage_component_uuid=None,
-                )
+        if self.tracking_callback is not None and self.num_active_samplers is not None:
+            self.tracking_callback(
+                type=TrackingInfoType.TEACHER_FORCING,
+                info=teacher_force_info,
+                n=self.num_active_samplers,
             )
 
         return res
 
 
 class AddBias(nn.Module):
     """Adding bias parameters to input values."""
```

### Comparing `allenact-0.5.2/allenact/base_abstractions/misc.py` & `allenact-0.5.3/allenact/base_abstractions/misc.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/base_abstractions/experiment_config.py` & `allenact-0.5.3/allenact/base_abstractions/experiment_config.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/base_abstractions/preprocessor.py` & `allenact-0.5.3/allenact/base_abstractions/preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
                 uuid: obs_spaces[uuid]
                 for uuid in obs_spaces
                 if uuid in additional_output_uuids or g.out_degree(uuid) == 0
             }
         )
 
         # ensure dependencies are precomputed
-        self.compute_order = [n for n in nx.dfs_postorder_nodes(g)]
+        self.compute_order = [n for n in nx.dfs_preorder_nodes(g)]
 
     def get(self, uuid: str) -> Preprocessor:
         """Return preprocessor with the given `uuid`.
 
         # Parameters
 
         uuid : The unique id of the preprocessor.
```

### Comparing `allenact-0.5.2/allenact/base_abstractions/task.py` & `allenact-0.5.3/allenact/base_abstractions/task.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/base_abstractions/sensor.py` & `allenact-0.5.3/allenact/base_abstractions/sensor.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/base_abstractions/callbacks.py` & `allenact-0.5.3/allenact/base_abstractions/callbacks.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,63 @@
+import abc
 from typing import List, Dict, Any, Sequence, Optional
 
 from allenact.base_abstractions.experiment_config import ExperimentConfig
 from allenact.base_abstractions.sensor import Sensor
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 
-class Callback:
+class Callback(abc.ABC):
     def setup(
         self,
         name: str,
         config: ExperimentConfig,
         mode: Literal["train", "valid", "test"],
         **kwargs,
     ) -> None:
         """Called once before training begins."""
 
     def on_train_log(
         self,
+        *,
         metrics: List[Dict[str, Any]],
         metric_means: Dict[str, float],
-        step: int,
         tasks_data: List[Any],
+        step: int,
+        scalar_name_to_total_experiences_key: Dict[str, str],
         **kwargs,
     ) -> None:
         """Called once train is supposed to log."""
 
     def on_valid_log(
         self,
+        *,
         metrics: Dict[str, Any],
         metric_means: Dict[str, float],
-        checkpoint_file_name: str,
         tasks_data: List[Any],
         step: int,
+        scalar_name_to_total_experiences_key: Dict[str, str],
+        checkpoint_file_name: str,
         **kwargs,
     ) -> None:
         """Called after validation ends."""
 
     def on_test_log(
         self,
-        checkpoint_file_name: str,
+        *,
         metrics: Dict[str, Any],
         metric_means: Dict[str, float],
         tasks_data: List[Any],
         step: int,
+        scalar_name_to_total_experiences_key: Dict[str, str],
+        checkpoint_file_name: str,
         **kwargs,
     ) -> None:
         """Called after test ends."""
 
     def after_save_project_state(self, base_dir: str) -> None:
         """Called after saving the project state in base_dir."""
```

### Comparing `allenact-0.5.2/allenact/main.py` & `allenact-0.5.3/allenact/main.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/embodiedai/mapping/mapping_utils/map_builders.py` & `allenact-0.5.3/allenact/embodiedai/mapping/mapping_utils/map_builders.py`

 * *Files 15% similar despite different names*

```diff
@@ -71,24 +71,26 @@
     def __init__(
         self,
         fov: float,
         vision_range_in_cm: int,
         map_size_in_cm: int,
         resolution_in_cm: int,
         height_bins: Sequence[float],
+        return_egocentric_local_context: bool = False,
         device: torch.device = torch.device("cpu"),
     ):
         assert vision_range_in_cm % resolution_in_cm == 0
 
         self.fov = fov
         self.vision_range_in_map_units = vision_range_in_cm // resolution_in_cm
         self.map_size_in_cm = map_size_in_cm
         self.resolution_in_cm = resolution_in_cm
         self.height_bins = height_bins
         self.device = device
+        self.return_egocentric_local_context = return_egocentric_local_context
 
         self.binned_point_cloud_map = np.zeros(
             (
                 self.map_size_in_cm // self.resolution_in_cm,
                 self.map_size_in_cm // self.resolution_in_cm,
                 len(self.height_bins) + 1,
             ),
@@ -131,15 +133,19 @@
         with torch.no_grad():
             assert self.min_xyz is not None, "Please call `reset` before `update`."
 
             camera_xyz = (
                 torch.from_numpy(camera_xyz - self.min_xyz).float().to(self.device)
             )
 
-            depth_frame = torch.from_numpy(depth_frame).to(self.device)
+            try:
+                depth_frame = torch.from_numpy(depth_frame).to(self.device)
+            except ValueError:
+                depth_frame = torch.from_numpy(depth_frame.copy()).to(self.device)
+
             depth_frame[
                 depth_frame
                 > self.vision_range_in_map_units * self.resolution_in_cm / 100
             ] = np.NaN
 
             world_space_point_cloud = depth_frame_to_world_space_xyz(
                 depth_frame=depth_frame,
@@ -197,20 +203,96 @@
             vr = self.vision_range_in_map_units
             vr_div_2 = self.vision_range_in_map_units // 2
             width_div_2 = agent_centric_binned_map.shape[1] // 2
             agent_centric_binned_map = agent_centric_binned_map[
                 :vr, (width_div_2 - vr_div_2) : (width_div_2 + vr_div_2), :
             ]
 
-            return {
+            to_return = {
                 "egocentric_update": agent_centric_binned_map.cpu().numpy(),
                 "allocentric_update": allocentric_update_numpy,
                 "map": self.binned_point_cloud_map,
             }
 
+            if self.return_egocentric_local_context:
+                # See the update function of the semantic map sensor for in depth comments regarding the below
+                # Essentially we are simply rotating the full map into the orientation of the agent and then
+                # selecting a smaller region around the agent.
+                theta = -np.pi * camera_rotation / 180
+                cos_theta = np.cos(theta)
+                sin_theta = np.sin(theta)
+                rot_mat = torch.FloatTensor(
+                    [[cos_theta, -sin_theta], [sin_theta, cos_theta]]
+                ).to(self.device)
+
+                move_back_offset = (
+                    -0.5
+                    * (self.vision_range_in_map_units * self.resolution_in_cm / 100)
+                ) * (
+                    rot_mat
+                    @ torch.tensor(
+                        [0, 1], dtype=torch.float, device=self.device
+                    ).unsqueeze(-1)
+                )
+
+                map_size = self.binned_point_cloud_map.shape[0]
+                scaler = 2 * (100 / (self.resolution_in_cm * map_size))
+                offset_to_center_the_agent = (
+                    scaler
+                    * (
+                        torch.tensor(
+                            [camera_xyz[0], camera_xyz[2],],
+                            dtype=torch.float,
+                            device=self.device,
+                        ).unsqueeze(-1)
+                        + move_back_offset
+                    )
+                    - 1
+                )
+                offset_to_top_of_image = rot_mat @ torch.FloatTensor(
+                    [0, 1.0]
+                ).unsqueeze(1).to(self.device)
+                rotation_and_translate_mat = torch.cat(
+                    (rot_mat, offset_to_top_of_image + offset_to_center_the_agent,),
+                    dim=1,
+                )
+
+                full_map_tensor = (
+                    torch.tensor(
+                        self.binned_point_cloud_map,
+                        dtype=torch.float,
+                        device=self.device,
+                    )
+                    .unsqueeze(0)
+                    .permute(0, 3, 1, 2)
+                )
+                full_ego_map = (
+                    F.grid_sample(
+                        full_map_tensor,
+                        F.affine_grid(
+                            rotation_and_translate_mat.to(self.device).unsqueeze(0),
+                            full_map_tensor.shape,
+                            align_corners=False,
+                        ),
+                        align_corners=False,
+                    )
+                    .squeeze(0)
+                    .permute(1, 2, 0)
+                )
+
+                egocentric_local_context = full_ego_map[
+                    :vr, (width_div_2 - vr_div_2) : (width_div_2 + vr_div_2), :
+                ]
+
+                to_return[
+                    "egocentric_local_context"
+                ] = egocentric_local_context.cpu().numpy()
+
+            return to_return
+
     def reset(self, min_xyz: np.ndarray):
         """Reset the map.
 
         Resets the internally stored map.
 
         # Parameters
         min_xyz : An array of size (3,) corresponding to the minimum possible x, y, and z values that will be observed
```

### Comparing `allenact-0.5.2/allenact/embodiedai/mapping/mapping_utils/point_cloud_utils.py` & `allenact-0.5.3/allenact/embodiedai/mapping/mapping_utils/point_cloud_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 
 import math
 from typing import Optional, Sequence, cast
 
 import numpy as np
 import torch
 
+from allenact_plugins.ithor_plugin.ithor_util import vertical_to_horizontal_fov
+
 
 def camera_space_xyz_to_world_xyz(
     camera_space_xyzs: torch.Tensor,
     camera_world_xyz: torch.Tensor,
     rotation: float,
     horizon: float,
 ) -> torch.Tensor:
@@ -119,36 +121,36 @@
     fov: The field of view of the camera.
 
     # Returns
 
     A 3xN matrix with entry [:, i] equalling a the xyz coordinates (in the camera's coordinate
     frame) of a point in the point cloud corresponding to the input depth frame.
     """
-    assert (
-        len(depth_frame.shape) == 2 and depth_frame.shape[0] == depth_frame.shape[1]
-    ), f"depth has shape {depth_frame.shape}, we only support (N, N) shapes for now."
-
-    resolution = depth_frame.shape[0]
+    h, w = depth_frame.shape[:2]
     if mask is None:
         mask = torch.ones_like(depth_frame, dtype=torch.bool)
 
     # pixel centers
     camera_space_yx_offsets = (
         torch.stack(torch.where(mask))
         + 0.5  # Offset by 0.5 so that we are in the middle of the pixel
     )
 
     # Subtract center
-    camera_space_yx_offsets -= resolution / 2.0
+    camera_space_yx_offsets[:1] -= h / 2.0
+    camera_space_yx_offsets[1:] -= w / 2.0
 
     # Make "up" in y be positive
     camera_space_yx_offsets[0, :] *= -1
 
     # Put points on the clipping plane
-    camera_space_yx_offsets *= (2.0 / resolution) * math.tan((fov / 2) / 180 * math.pi)
+    camera_space_yx_offsets[:1] *= (2.0 / h) * math.tan((fov / 2) / 180 * math.pi)
+    camera_space_yx_offsets[1:] *= (2.0 / w) * math.tan(
+        (vertical_to_horizontal_fov(fov, height=h, width=w) / 2) / 180 * math.pi
+    )
 
     # noinspection PyArgumentList
     camera_space_xyz = torch.cat(
         [
             camera_space_yx_offsets[1:, :],  # This is x
             camera_space_yx_offsets[:1, :],  # This is y
             torch.ones_like(camera_space_yx_offsets[:1, :]),
```

### Comparing `allenact-0.5.2/allenact/embodiedai/mapping/mapping_models/active_neural_slam.py` & `allenact-0.5.3/allenact/embodiedai/mapping/mapping_models/active_neural_slam.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/embodiedai/mapping/mapping_losses.py` & `allenact-0.5.3/allenact/embodiedai/mapping/mapping_losses.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/embodiedai/models/resnet.py` & `allenact-0.5.3/allenact/embodiedai/models/resnet.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/embodiedai/models/fusion_models.py` & `allenact-0.5.3/allenact/embodiedai/models/fusion_models.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/embodiedai/models/aux_models.py` & `allenact-0.5.3/allenact/embodiedai/models/aux_models.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,64 +33,79 @@
         cpca_softmax_dim: int = 128,
     ):
         super().__init__()
         self.aux_uuid = aux_uuid
         self.action_dim = action_dim
         self.obs_embed_dim = obs_embed_dim
         self.belief_dim = belief_dim
-
-        if self.aux_uuid == InverseDynamicsLoss.UUID:
-            self.decoder = nn.Linear(
-                2 * self.obs_embed_dim + self.belief_dim, self.action_dim
-            )
-        elif self.aux_uuid == TemporalDistanceLoss.UUID:
-            self.decoder = nn.Linear(2 * self.obs_embed_dim + self.belief_dim, 1)
-        elif CPCALoss.UUID in self.aux_uuid:  # the CPCA family with various k
-            ## Auto-regressive model to predict future context
-            self.action_embedder = FeatureEmbedding(
-                self.action_dim + 1, action_embed_size
-            )
-            # NOTE: add extra 1 in embedding dict cuz we will pad zero actions?
-            self.context_model = nn.GRU(action_embed_size, self.belief_dim)
-
-            ## Classifier to estimate mutual information
-            self.classifier = nn.Sequential(
-                nn.Linear(
-                    self.belief_dim + self.obs_embed_dim, cpca_classifier_hidden_dim
-                ),
-                nn.ReLU(),
-                nn.Linear(cpca_classifier_hidden_dim, 1),
-            )
-
-        elif CPCASoftMaxLoss.UUID in self.aux_uuid:
-            ###
-            # same as CPCA with extra MLP for contrastive losses.
-            ###
-            self.action_embedder = FeatureEmbedding(
-                self.action_dim + 1, action_embed_size
-            )
-            # NOTE: add extra 1 in embedding dict cuz we will pad zero actions?
-            self.context_model = nn.GRU(action_embed_size, self.belief_dim)
-
-            ## Classifier to estimate mutual information
-            self.visual_mlp = nn.Sequential(
-                nn.Linear(obs_embed_dim, cpca_classifier_hidden_dim),
-                nn.ReLU(),
-                nn.Linear(cpca_classifier_hidden_dim, cpca_softmax_dim),
-            )
-
-            self.belief_mlp = nn.Sequential(
-                nn.Linear(self.belief_dim, cpca_classifier_hidden_dim),
-                nn.ReLU(),
-                nn.Linear(cpca_classifier_hidden_dim, cpca_softmax_dim),
-            )
-
+        self.action_embed_size = action_embed_size
+        self.cpca_classifier_hidden_dim = cpca_classifier_hidden_dim
+        self.cpca_softmax_dim = cpca_softmax_dim
+
+        self.initialize_model_given_aux_uuid(self.aux_uuid)
+
+    def initialize_model_given_aux_uuid(self, aux_uuid: str):
+        if aux_uuid == InverseDynamicsLoss.UUID:
+            self.init_inverse_dynamics()
+        elif aux_uuid == TemporalDistanceLoss.UUID:
+            self.init_temporal_distance()
+        elif CPCALoss.UUID in aux_uuid:  # the CPCA family with various k
+            self.init_cpca()
+        elif CPCASoftMaxLoss.UUID in aux_uuid:
+            self.init_cpca_softmax()
         else:
             raise ValueError("Unknown Auxiliary Loss UUID")
 
+    def init_inverse_dynamics(self):
+        self.decoder = nn.Linear(
+            2 * self.obs_embed_dim + self.belief_dim, self.action_dim
+        )
+
+    def init_temporal_distance(self):
+        self.decoder = nn.Linear(2 * self.obs_embed_dim + self.belief_dim, 1)
+
+    def init_cpca(self):
+        ## Auto-regressive model to predict future context
+        self.action_embedder = FeatureEmbedding(
+            self.action_dim + 1, self.action_embed_size
+        )
+        # NOTE: add extra 1 in embedding dict cuz we will pad zero actions?
+        self.context_model = nn.GRU(self.action_embed_size, self.belief_dim)
+
+        ## Classifier to estimate mutual information
+        self.classifier = nn.Sequential(
+            nn.Linear(
+                self.belief_dim + self.obs_embed_dim, self.cpca_classifier_hidden_dim
+            ),
+            nn.ReLU(),
+            nn.Linear(self.cpca_classifier_hidden_dim, 1),
+        )
+
+    def init_cpca_softmax(self):
+        # same as CPCA with extra MLP for contrastive losses.
+        ###
+        self.action_embedder = FeatureEmbedding(
+            self.action_dim + 1, self.action_embed_size
+        )
+        # NOTE: add extra 1 in embedding dict cuz we will pad zero actions?
+        self.context_model = nn.GRU(self.action_embed_size, self.belief_dim)
+
+        ## Classifier to estimate mutual information
+        self.visual_mlp = nn.Sequential(
+            nn.Linear(self.obs_embed_dim, self.cpca_classifier_hidden_dim),
+            nn.ReLU(),
+            nn.Linear(self.cpca_classifier_hidden_dim, self.cpca_softmax_dim),
+        )
+
+        self.belief_mlp = nn.Sequential(
+            nn.Linear(self.belief_dim, self.cpca_classifier_hidden_dim),
+            nn.ReLU(),
+            nn.Linear(self.cpca_classifier_hidden_dim, self.cpca_softmax_dim),
+        )
+
     def forward(self, features: torch.FloatTensor):
         if self.aux_uuid in [InverseDynamicsLoss.UUID, TemporalDistanceLoss.UUID]:
             return self.decoder(features)
         else:
             raise NotImplementedError(
                 f"Auxiliary model with UUID {self.aux_uuid} does not support `forward` call."
             )
```

### Comparing `allenact-0.5.2/allenact/embodiedai/models/visual_nav_models.py` & `allenact-0.5.3/allenact/embodiedai/models/visual_nav_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         self,
         action_space: gym.spaces.Discrete,
         observation_space: SpaceDict,
         hidden_size=512,
         multiple_beliefs=False,
         beliefs_fusion: Optional[FusionType] = None,
         auxiliary_uuids: Optional[List[str]] = None,
+        auxiliary_model_class=AuxiliaryModel,
     ):
         super().__init__(action_space=action_space, observation_space=observation_space)
         self._hidden_size = hidden_size
         assert multiple_beliefs == (beliefs_fusion is not None)
         self.multiple_beliefs = multiple_beliefs
         self.beliefs_fusion = beliefs_fusion
         self.auxiliary_uuids = auxiliary_uuids
@@ -58,14 +59,15 @@
         self.aux_models: Optional[nn.ModuleDict] = None
         self.actor: Optional[LinearActorHead] = None
         self.critic: Optional[LinearCriticHead] = None
         self.prev_action_embedder: Optional[FeatureEmbedding] = None
 
         self.fusion_model: Optional[nn.Module] = None
         self.belief_names: Optional[Sequence[str]] = None
+        self.auxiliary_model_class = auxiliary_model_class
 
     def create_state_encoders(
         self,
         obs_embed_size: int,
         prev_action_embed_size: int,
         num_rnn_layers: int,
         rnn_type: str,
@@ -137,15 +139,15 @@
         self.critic = LinearCriticHead(self._hidden_size)
 
     def create_aux_models(self, obs_embed_size: int, action_embed_size: int):
         if self.auxiliary_uuids is None:
             return
         aux_models = OrderedDict()
         for aux_uuid in self.auxiliary_uuids:
-            aux_models[aux_uuid] = AuxiliaryModel(
+            aux_models[aux_uuid] = self.auxiliary_model_class(
                 aux_uuid=aux_uuid,
                 action_dim=self.action_space.n,
                 obs_embed_dim=obs_embed_size,
                 belief_dim=self._hidden_size,
                 action_embed_size=action_embed_size,
             )
```

### Comparing `allenact-0.5.2/allenact/embodiedai/models/basic_models.py` & `allenact-0.5.3/allenact/embodiedai/models/basic_models.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/embodiedai/aux_losses/losses.py` & `allenact-0.5.3/allenact/embodiedai/aux_losses/losses.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,15 @@
         # sample valid pairs: sampled_pairs shape (M, num_pairs, 3)
         # where M is the num of total episodes in the batch
         locs = locs_batch.cpu().numpy()  # as torch.randint only support int, not tensor
         sampled_pairs = np.random.randint(
             np.repeat(locs[:, [1]], 2 * self.num_pairs, axis=-1),  # (M, 2*k)
             np.repeat(locs[:, [2]] + 1, 2 * self.num_pairs, axis=-1),  # (M, 2*k)
         ).reshape(
-            -1, self.num_pairs, 2
+            (-1, self.num_pairs, 2)
         )  # (M, k, 2)
         sampled_pairs_batch = torch.from_numpy(sampled_pairs).to(
             locs_batch
         )  # (M, k, 2)
 
         num_sampler_batch = locs_batch[:, [0]].expand(
             -1, 2 * self.num_pairs
```

### Comparing `allenact-0.5.2/allenact/embodiedai/preprocessors/resnet.py` & `allenact-0.5.3/allenact/embodiedai/preprocessors/resnet.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/embodiedai/sensors/vision_sensors.py` & `allenact-0.5.3/allenact/embodiedai/sensors/vision_sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,17 @@
         output_channels : Optional observation space number of channels (alternative to `output_shape`).
         unnormalized_infimum : Lower limit(s) for the observation space range.
         unnormalized_supremum : Upper limit(s) for the observation space range.
         scale_first : Whether to scale image before normalization (if needed).
         kwargs : Extra kwargs. Currently unused.
         """
 
-        self._norm_means = np.array(mean)
-        self._norm_sds = np.array(stdev)
+        self._norm_means = np.array(mean) if mean is not None else None
+        self._norm_sds = np.array(stdev) if stdev is not None else None
+
         assert (self._norm_means is None) == (self._norm_sds is None), (
             "In VisionSensor's config, "
             "either both mean/stdev must be None or neither."
         )
         self._should_normalize = self._norm_means is not None
 
         self._height = height
```

### Comparing `allenact-0.5.2/allenact/embodiedai/storage/vdr_storage.py` & `allenact-0.5.3/allenact/embodiedai/storage/vdr_storage.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/utils/inference.py` & `allenact-0.5.3/allenact/utils/inference.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/utils/spaces_utils.py` & `allenact-0.5.3/allenact/utils/spaces_utils.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/utils/misc_utils.py` & `allenact-0.5.3/allenact/utils/misc_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import copy
 import functools
 import hashlib
 import inspect
 import json
 import math
 import os
+import pdb
 import random
 import subprocess
+import sys
 import urllib
 import urllib.request
 from collections import Counter
 from contextlib import contextmanager
 from typing import Sequence, List, Optional, Tuple, Hashable
 
 import filelock
@@ -327,7 +329,19 @@
     v = v.lower().strip()
     if v in ("yes", "true", "t", "y", "1"):
         return True
     elif v in ("no", "false", "f", "n", "0"):
         return False
     else:
         raise ValueError(f"{v} cannot be converted to a bool")
+
+
+class ForkedPdb(pdb.Pdb):
+    """A Pdb subclass that may be used from a forked multiprocessing child."""
+
+    def interaction(self, *args, **kwargs):
+        _stdin = sys.stdin
+        try:
+            sys.stdin = open("/dev/stdin")
+            pdb.Pdb.interaction(self, *args, **kwargs)
+        finally:
+            sys.stdin = _stdin
```

### Comparing `allenact-0.5.2/allenact/utils/cacheless_frcnn.py` & `allenact-0.5.3/allenact/utils/cacheless_frcnn.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/utils/cache_utils.py` & `allenact-0.5.3/allenact/utils/cache_utils.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/utils/tensor_utils.py` & `allenact-0.5.3/allenact/utils/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/utils/experiment_utils.py` & `allenact-0.5.3/allenact/utils/experiment_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,15 +250,15 @@
         self.training_steps: int = training_steps
         self.storage_uuid_to_total_experiences: Dict[
             str, int
         ] = storage_uuid_to_total_experiences
         self.pipeline_stage = pipeline_stage
 
         self.metrics_tracker = ScalarMeanTracker()
-        self.train_info_trackers: Dict[Tuple[str, str], ScalarMeanTracker] = {}
+        self.info_trackers: Dict[Tuple[str, str], ScalarMeanTracker] = {}
 
         self.metric_dicts: List[Any] = []
         self.viz_data: Optional[Dict[str, List[Dict[str, Any]]]] = None
         self.checkpoint_file_name: Optional[str] = None
         self.task_callback_data: List[Any] = []
 
         self.num_empty_metrics_dicts_added: int = 0
@@ -292,27 +292,27 @@
 
         self.metric_dicts.append(single_task_metrics_dict)
         self.metrics_tracker.add_scalars(
             {k: v for k, v in single_task_metrics_dict.items() if k != "task_info"}
         )
         return True
 
-    def add_train_info_dict(
+    def add_info_dict(
         self,
-        train_info_dict: Dict[str, Union[int, float]],
+        info_dict: Dict[str, Union[int, float]],
         n: int,
         stage_component_uuid: str,
         storage_uuid: str,
     ):
         key = (stage_component_uuid, storage_uuid)
-        if key not in self.train_info_trackers:
-            self.train_info_trackers[key] = ScalarMeanTracker()
+        if key not in self.info_trackers:
+            self.info_trackers[key] = ScalarMeanTracker()
 
         assert n >= 0
-        self.train_info_trackers[key].add_scalars(scalars=train_info_dict, n=n)
+        self.info_trackers[key].add_scalars(scalars=info_dict, n=n)
 
 
 class LinearDecay(object):
     """Linearly decay between two values over some number of steps.
 
     Obtain the value corresponding to the `i`-th step by calling
     an instance of this class with the value `i`.
@@ -555,16 +555,16 @@
             return val
         else:
             super(TrainingSettings, self).__getattribute__(item)
 
 
 @attr.s(kw_only=True)
 class StageComponent:
-    """An custom component for a PipelineStage, possibly including overrides to
-    the `TrainingSettings` in from the `TrainingPipeline` and `PipelineStage`.
+    """A custom component for a PipelineStage, possibly including overrides to
+    the `TrainingSettings` from the `TrainingPipeline` and `PipelineStage`.
 
     # Attributes
 
     uuid: the name of this component
     storage_uuid: the name of the `ExperienceStorage` that will be used with this component.
     loss_names: list of unique names assigned to off-policy losses
     training_settings: Instance of `TrainingSettings`
@@ -615,15 +615,15 @@
     teacher_forcing : If applicable, defines the probability an agent will take the
         expert action (as opposed to its own sampled action) at a given time point.
     early_stopping_criterion: An `EarlyStoppingCriterion` object which determines if
         training in this stage should be stopped early. If `None` then no early stopping
         occurs. If `early_stopping_criterion` is not `None` then we do not guarantee
         reproducibility when restarting a model from a checkpoint (as the
         `EarlyStoppingCriterion` object may store internal state which is not
-        saved in the checkpoint). Currently AllenAct only supports using early stopping
+        saved in the checkpoint). Currently, AllenAct only supports using early stopping
         criterion when **not** using distributed training.
     training_settings: Instance of `TrainingSettings`.
     training_settings_kwargs: For backwards compatability: arguments to instantiate TrainingSettings when
      `training_settings` is `None`.
     """
 
     def __init__(
@@ -794,14 +794,16 @@
         named_storages: Optional[
             Dict[str, Union[ExperienceStorage, Builder[ExperienceStorage]]]
         ] = None,
         rollout_storage_uuid: Optional[str] = None,
         should_log: bool = True,
         lr_scheduler_builder: Optional[Builder[_LRScheduler]] = None,  # type: ignore
         training_settings: Optional[TrainingSettings] = None,
+        valid_pipeline_stage: Optional[PipelineStage] = None,
+        test_pipeline_stage: Optional[PipelineStage] = None,
         **training_settings_kwargs,
     ):
         """Initializer.
 
         See class docstring for parameter definitions.
         """
 
@@ -827,80 +829,111 @@
         self._named_storages = self._initialize_named_storages(
             named_storages=named_storages
         )
         self.rollout_storage_uuid = self._initialize_rollout_storage_uuid(
             rollout_storage_uuid
         )
 
+        if self.rollout_storage_uuid is None:
+            get_logger().warning(
+                f"No rollout storage was specified in the TrainingPipeline. This need not be an issue"
+                f" if you are performing off-policy training but, otherwise, please ensure you have"
+                f" defined a rollout storage in the `named_storages` argument of the TrainingPipeline."
+            )
+
         self.should_log = should_log
 
         self.pipeline_stages = pipeline_stages
-        assert len(self.pipeline_stages) == len(
-            set(id(ps) for ps in pipeline_stages)
+
+        def if_none_then_empty_stage(stage: Optional[PipelineStage]) -> PipelineStage:
+            return (
+                stage
+                if stage is not None
+                else PipelineStage(max_stage_steps=-1, loss_names=[])
+            )
+
+        self.valid_pipeline_stage = if_none_then_empty_stage(valid_pipeline_stage)
+        self.test_pipeline_stage = if_none_then_empty_stage(test_pipeline_stage)
+
+        assert (
+            len(self.pipeline_stages) == len(set(id(ps) for ps in pipeline_stages))
+            and self.valid_pipeline_stage not in self.pipeline_stages
+            and self.test_pipeline_stage not in self.pipeline_stages
         ), (
             "Duplicate `PipelineStage` object instances found in the pipeline stages input"
             " to `TrainingPipeline`. `PipelineStage` objects are not immutable, if you'd"
             " like to have multiple pipeline stages of the same type, please instantiate"
             " multiple separate instances."
         )
 
-        self._ensure_pipeline_stages_all_have_at_least_one_valid_stage_component()
+        self._ensure_pipeline_stages_all_have_at_least_one_stage_component()
 
         self._current_stage: Optional[PipelineStage] = None
         self.rollout_count = 0
         self._refresh_current_stage(force_stage_search_from_start=True)
 
     def _initialize_rollout_storage_uuid(
         self, rollout_storage_uuid: Optional[str]
     ) -> str:
         if rollout_storage_uuid is None:
             rollout_storage_uuids = self._get_uuids_of_rollout_storages(
                 self._named_storages
             )
-            assert len(rollout_storage_uuids) == 1, (
+            assert len(rollout_storage_uuids) <= 1, (
                 f"`rollout_storage_uuid` cannot be automatically inferred as there are multiple storages defined"
                 f" (ids: {rollout_storage_uuids}) of type `RolloutStorage`."
             )
-            rollout_storage_uuid = rollout_storage_uuids[0]
-        assert rollout_storage_uuid in self._named_storages
+            rollout_storage_uuid = next(iter(rollout_storage_uuids), None)
+        assert (
+            rollout_storage_uuid is None or rollout_storage_uuid in self._named_storages
+        )
         return rollout_storage_uuid
 
-    def _ensure_pipeline_stages_all_have_at_least_one_valid_stage_component(self):
+    def _ensure_pipeline_stages_all_have_at_least_one_stage_component(self):
         rollout_storages_uuids = self._get_uuids_of_rollout_storages(
             self._named_storages
         )
 
-        for sit, stage in enumerate(self.pipeline_stages):
+        named_pipeline_stages = {
+            f"{i}th": ps for i, ps in enumerate(self.pipeline_stages)
+        }
+
+        named_pipeline_stages["valid"] = self.valid_pipeline_stage
+        named_pipeline_stages["test"] = self.test_pipeline_stage
+
+        for stage_name, stage in named_pipeline_stages.items():
             # Forward default `TrainingSettings` to all `PipelineStage`s settings:
             stage.training_settings.set_defaults(defaults=self.training_settings)
 
             if len(stage.stage_components) == 0:
-                assert len(rollout_storages_uuids) == 1, (
-                    f"In {sit}th pipeline stage: you have several storages specified ({rollout_storages_uuids}) which"
+                assert len(rollout_storages_uuids) <= 1, (
+                    f"In {stage_name} pipeline stage: you have several storages specified ({rollout_storages_uuids}) which"
                     f" are subclasses of `RolloutStorage`. This is only allowed when stage components are explicitly"
                     f" defined in every `PipelineStage` instance. You have `PipelineStage`s for which stage components"
                     f" are not specified."
                 )
-                stage.add_stage_component(
-                    StageComponent(
-                        uuid=rollout_storages_uuids[0],
-                        storage_uuid=rollout_storages_uuids[0],
-                        loss_names=stage.loss_names,
-                        training_settings=TrainingSettings(),
+                if len(rollout_storages_uuids) > 0:
+                    stage.add_stage_component(
+                        StageComponent(
+                            uuid=rollout_storages_uuids[0],
+                            storage_uuid=rollout_storages_uuids[0],
+                            loss_names=stage.loss_names,
+                            training_settings=TrainingSettings(),
+                        )
                     )
-                )
 
             for sc in stage.stage_components:
                 assert sc.storage_uuid in self._named_storages, (
-                    f"In {sit}th pipeline stage: storage with name '{sc.storage_uuid}' not found in collection of"
+                    f"In {stage_name} pipeline stage: storage with name '{sc.storage_uuid}' not found in collection of"
                     f" defined storages names: {list(self._named_storages.keys())}"
                 )
 
             if (
-                self.rollout_storage_uuid
+                self.rollout_storage_uuid is not None
+                and self.rollout_storage_uuid
                 not in stage.storage_uuid_to_steps_taken_in_stage
             ):
                 stage.storage_uuid_to_steps_taken_in_stage[
                     self.rollout_storage_uuid
                 ] = 0
 
     @classmethod
@@ -924,15 +957,15 @@
         named_storages: Optional[
             Dict[str, Union[Builder[ExperienceStorage], ExperienceStorage]]
         ],
     ) -> Dict[str, Union[Builder[ExperienceStorage], ExperienceStorage]]:
         named_storages = {} if named_storages is None else {**named_storages}
 
         rollout_storages_uuids = cls._get_uuids_of_rollout_storages(named_storages)
-        if len(rollout_storages_uuids) == 0:
+        if len(named_storages) == 0:
             assert (
                 _DEFAULT_ONPOLICY_UUID not in named_storages
             ), f"Storage uuid '{_DEFAULT_ONPOLICY_UUID}' is reserved, please pick a different uuid."
             named_storages[_DEFAULT_ONPOLICY_UUID] = Builder(RolloutBlockStorage)
             rollout_storages_uuids.append(_DEFAULT_ONPOLICY_UUID)
         return named_storages
 
@@ -962,14 +995,27 @@
     @property
     def storage_uuid_to_total_experiences(self) -> Dict[str, int]:
         totals = {k: 0 for k in self._named_storages}
         for ps in self.pipeline_stages:
             for k in ps.storage_uuid_to_steps_taken_in_stage:
                 totals[k] += ps.storage_uuid_to_steps_taken_in_stage[k]
 
+        for k in totals:
+            split = k.split("__")
+            if len(split) == 2 and split[1] in ["valid", "test"]:
+                assert totals[k] == 0, (
+                    "Total experiences should be 0 for validation/test storages, i.e."
+                    " storages who have `__valid` or `__test` as their suffix. These storages"
+                    " will copy their `total_experiences` from the corresponding training"
+                    " storage i.e.:\n"
+                    " 1. the storage without the above suffix if it exists, else\n"
+                    " 2. the total number of steps."
+                )
+                totals[k] = totals.get(split[0], self.total_steps)
+
         return totals
 
     @property
     def current_stage(self) -> Optional[PipelineStage]:
         return self._current_stage
 
     @property
@@ -996,14 +1042,21 @@
         return self.current_stage is not self._refresh_current_stage(
             force_stage_search_from_start=False
         )
 
     def restart_pipeline(self):
         for ps in self.pipeline_stages:
             ps.reset()
+
+        if self.valid_pipeline_stage:
+            self.valid_pipeline_stage.reset()
+
+        if self.test_pipeline_stage:
+            self.test_pipeline_stage.reset()
+
         self._current_stage = None
         self._refresh_current_stage(force_stage_search_from_start=True)
 
     def state_dict(self):
         return dict(
             stage_info_list=[
                 {
@@ -1038,39 +1091,54 @@
                 ps.rollout_count = stage_info["rollout_count"]
 
         self.rollout_count = state_dict["rollout_count"]
 
         self._refresh_current_stage(force_stage_search_from_start=True)
 
     @property
-    def rollout_storage(self) -> RolloutStorage:
-        return cast(
-            RolloutStorage, self.current_stage_storage[self.rollout_storage_uuid]
-        )
+    def rollout_storage(self) -> Optional[RolloutStorage]:
+        if self.rollout_storage_uuid is None:
+            return None
+
+        rs = self._named_storages[self.rollout_storage_uuid]
+        if isinstance(rs, Builder):
+            rs = rs()
+            self._named_storages[self.rollout_storage_uuid] = rs
+
+        return cast(RolloutStorage, rs)
+
+    def get_stage_storage(
+        self, stage: PipelineStage
+    ) -> "OrderedDict[str, ExperienceStorage]":
+        storage_uuids_for_current_stage_set = set(
+            sc.storage_uuid for sc in stage.stage_components
+        )
+
+        # Always include self.rollout_storage_uuid in the current stage storage (when the uuid is defined)
+        if self.rollout_storage_uuid is not None:
+            storage_uuids_for_current_stage_set.add(self.rollout_storage_uuid)
 
-    @property
-    def current_stage_storage(self) -> "OrderedDict[str, ExperienceStorage]":
         storage_uuids_for_current_stage = sorted(
-            list(
-                set(sc.storage_uuid for sc in self.current_stage.stage_components)
-                | {
-                    self.rollout_storage_uuid
-                }  # Always include self.rollout_storage_uuid
-            )
+            list(storage_uuids_for_current_stage_set)
         )
+
         for storage_uuid in storage_uuids_for_current_stage:
             if isinstance(self._named_storages[storage_uuid], Builder):
                 self._named_storages[storage_uuid] = cast(
                     Builder["ExperienceStorage"], self._named_storages[storage_uuid],
                 )()
 
         return OrderedDict(
             (k, self._named_storages[k]) for k in storage_uuids_for_current_stage
         )
 
+    @property
+    def current_stage_storage(self) -> "OrderedDict[str, ExperienceStorage]":
+        return self.get_stage_storage(self.current_stage)
+
     def get_loss(self, uuid: str):
         if isinstance(self._named_losses[uuid], Builder):
             self._named_losses[uuid] = cast(
                 Builder[Union["AbstractActorCriticLoss", "GenericAbstractLoss"]],
                 self._named_losses[uuid],
             )()
         return self._named_losses[uuid]
```

### Comparing `allenact-0.5.2/allenact/utils/viz_utils.py` & `allenact-0.5.3/allenact/utils/viz_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -552,15 +552,15 @@
 
         return fig
 
 
 class TensorViz2D(AbstractTensorViz):
     def __init__(
         self,
-        rollout_source: Union[str, Sequence[str]] = ("memory", "rnn"),
+        rollout_source: Union[str, Sequence[str]] = ("memory_first_last", "rnn"),
         label: Optional[str] = None,
         figsize: Tuple[float, float] = (10, 10),
         fontsize: float = 5,
         **other_base_kwargs,
     ):
         super().__init__(rollout_source, label, figsize, **other_base_kwargs)
         self.fontsize = fontsize
@@ -880,14 +880,17 @@
 
                 # Access storage
                 res = getattr(rollout, storage)
                 episode_dim = rollout.dim_names.index("sampler")
 
                 # Access sub-storage if path not empty
                 if len(path) > 0:
+                    if storage == "memory_first_last":
+                        storage = "memory"
+
                     flattened_name = rollout.unflattened_to_flattened[storage][
                         tuple(path)
                     ]
                     # for path_step in path:
                     #     res = res[path_step]
                     res = res[flattened_name]
                     res, episode_dim = res
```

### Comparing `allenact-0.5.2/allenact/utils/system.py` & `allenact-0.5.3/allenact/utils/system.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/utils/model_utils.py` & `allenact-0.5.3/allenact/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact/utils/multi_agent_viz_utils.py` & `allenact-0.5.3/allenact/utils/multi_agent_viz_utils.py`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact.egg-info/SOURCES.txt` & `allenact-0.5.3/allenact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/allenact.egg-info/PKG-INFO` & `allenact-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allenact
-Version: 0.5.2
+Version: 0.5.3
 Summary: AllenAct framework
 Home-page: https://github.com/allenai/allenact
 Author: Allen Institute for Artificial Intelligence
 Author-email: lucaw@allenai.org
 License: MIT
 Description: AllenAct is a modular and flexible learning framework designed with a focus on the unique requirements of Embodied-AI research.
 Keywords: reinforcement learning,embodied-AI,AI,RL,SLAM
```

### Comparing `allenact-0.5.2/README.md` & `allenact-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `allenact-0.5.2/PKG-INFO` & `allenact-0.5.3/allenact.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allenact
-Version: 0.5.2
+Version: 0.5.3
 Summary: AllenAct framework
 Home-page: https://github.com/allenai/allenact
 Author: Allen Institute for Artificial Intelligence
 Author-email: lucaw@allenai.org
 License: MIT
 Description: AllenAct is a modular and flexible learning framework designed with a focus on the unique requirements of Embodied-AI research.
 Keywords: reinforcement learning,embodied-AI,AI,RL,SLAM
```

