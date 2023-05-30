# Comparing `tmp/allenact_plugins-0.5.2.tar.gz` & `tmp/allenact_plugins-0.5.3.tar.gz`

## Comparing `allenact_plugins-0.5.2.tar` & `allenact_plugins-0.5.3.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (121)     4667 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5063 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins.egg-info/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)     4667 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/navigation_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/navigation_plugin/pointnav/
--rw-r--r--   0 runner    (1001) docker     (121)     4927 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/navigation_plugin/pointnav/models.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/navigation_plugin/pointnav/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/navigation_plugin/objectnav/
--rw-r--r--   0 runner    (1001) docker     (121)    20609 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/navigation_plugin/objectnav/models.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/navigation_plugin/objectnav/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/navigation_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/
--rw-r--r--   0 runner    (1001) docker     (121)     4596 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/arm_calculation_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1740 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/manipulathor_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    20432 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/manipulathor_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)    15032 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/manipulathor_viz.py
--rw-r--r--   0 runner    (1001) docker     (121)    10508 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/manipulathor_sensors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2391 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/manipulathor_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    19507 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/manipulathor_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/armpointnav_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    18342 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/manipulathor_task_samplers.py
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/lighthouse_plugin/
--rw-r--r--   0 runner    (1001) docker     (121)     2841 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/lighthouse_plugin/lighthouse_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/lighthouse_plugin/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/lighthouse_plugin/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/lighthouse_plugin/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/lighthouse_plugin/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/lighthouse_plugin/configs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/lighthouse_plugin/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10100 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/lighthouse_plugin/lighthouse_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/lighthouse_plugin/lighthouse_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    14337 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/lighthouse_plugin/lighthouse_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     9042 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/lighthouse_plugin/lighthouse_sensors.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/lighthouse_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/gym_plugin/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/gym_plugin/gym_distributions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4157 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/gym_plugin/gym_sensors.py
--rw-r--r--   0 runner    (1001) docker     (121)      811 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/gym_plugin/gym_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     2599 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/gym_plugin/gym_models.py
--rw-r--r--   0 runner    (1001) docker     (121)    10428 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/gym_plugin/gym_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/gym_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/
--rw-r--r--   0 runner    (1001) docker     (121)     6233 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/minigrid_environments.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/configs/
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/configs/minigrid_nomemory.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8211 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/minigrid_models.py
--rw-r--r--   0 runner    (1001) docker     (121)    11576 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/minigrid_offpolicy.py
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19216 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/minigrid_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     4281 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/minigrid_sensors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/
--rw-r--r--   0 runner    (1001) docker     (121)     6552 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/ithor_task_samplers.py
--rw-r--r--   0 runner    (1001) docker     (121)    15676 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/ithor_viz.py
--rw-r--r--   0 runner    (1001) docker     (121)    43142 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/ithor_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     9983 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/ithor_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/scripts/make_objectnav_debug_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/scripts/make_pointnav_debug_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5611 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/ithor_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2940 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/ithor_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    18614 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/ithor_sensors.py
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/
--rw-r--r--   0 runner    (1001) docker     (121)     5293 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/habitat_sensors.py
--rw-r--r--   0 runner    (1001) docker     (121)    15168 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/habitat_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/habitat_preprocessors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/scripts/make_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/scripts/agent_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/habitat_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     8327 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/habitat_task_samplers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8181 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/habitat_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2629 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/habitat_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/clip_plugin/
--rw-r--r--   0 runner    (1001) docker     (121)     8119 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/clip_plugin/clip_preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/clip_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/babyai_plugin/
--rw-r--r--   0 runner    (1001) docker     (121)     7768 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/babyai_plugin/babyai_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/babyai_plugin/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/babyai_plugin/scripts/get_instr_length_percentiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     3758 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/babyai_plugin/scripts/download_babyai_expert_demos.py
--rw-r--r--   0 runner    (1001) docker     (121)      846 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/babyai_plugin/scripts/truncate_expert_demos.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/babyai_plugin/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/babyai_plugin/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/babyai_plugin/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/babyai_plugin/configs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/babyai_plugin/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/babyai_plugin/babyai_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    24194 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/babyai_plugin/babyai_models.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/babyai_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/
--rw-r--r--   0 runner    (1001) docker     (121)    19722 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/robothor_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)    19345 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/robothor_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     2612 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/scripts/make_objectnav_debug_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/scripts/make_pointnav_debug_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3698 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/robothor_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     6804 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/robothor_sensors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/configs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/robothor_distributions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8719 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/robothor_preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (121)    39301 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/robothor_task_samplers.py
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/robothor_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    15438 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/robothor_viz.py
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/allenact_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6098 2022-08-16 21:40:32.000000 allenact_plugins-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-08-16 21:40:40.000000 allenact_plugins-0.5.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/robothor_distributions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/robothor_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19722 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/robothor_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/scripts/make_pointnav_debug_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/scripts/make_objectnav_debug_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39301 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/robothor_task_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19328 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/robothor_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/robothor_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/robothor_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/robothor_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/robothor_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/babyai_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/babyai_plugin/babyai_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24194 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/babyai_plugin/babyai_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/babyai_plugin/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/babyai_plugin/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/babyai_plugin/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/babyai_plugin/scripts/truncate_expert_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/babyai_plugin/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/babyai_plugin/scripts/get_instr_length_percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/babyai_plugin/scripts/download_babyai_expert_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/babyai_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/babyai_plugin/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/babyai_plugin/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/babyai_plugin/babyai_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/gym_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/gym_plugin/gym_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/gym_plugin/gym_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/gym_plugin/gym_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/gym_plugin/gym_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/gym_plugin/gym_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/gym_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/habitat_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/habitat_sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/scripts/make_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/scripts/agent_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/habitat_preprocessors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15168 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/habitat_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/habitat_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/habitat_task_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/habitat_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)    20098 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/ithor_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/ithor_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/ithor_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/ithor_task_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43142 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/ithor_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15676 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/ithor_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/scripts/make_pointnav_debug_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/scripts/make_objectnav_debug_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/ithor_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/armpointnav_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/manipulathor_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/manipulathor_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19507 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/manipulathor_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/arm_calculation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18342 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/manipulathor_task_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/manipulathor_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/manipulathor_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/manipulathor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/clip_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/clip_plugin/clip_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/clip_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/navigation_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/navigation_plugin/pointnav/
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/navigation_plugin/pointnav/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/navigation_plugin/pointnav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/navigation_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/navigation_plugin/objectnav/
+-rw-r--r--   0 runner    (1001) docker     (123)    20689 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/navigation_plugin/objectnav/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/navigation_plugin/objectnav/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/lighthouse_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/lighthouse_plugin/lighthouse_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/lighthouse_plugin/lighthouse_sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/lighthouse_plugin/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/lighthouse_plugin/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/lighthouse_plugin/lighthouse_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/lighthouse_plugin/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/lighthouse_plugin/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/lighthouse_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/lighthouse_plugin/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/lighthouse_plugin/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14337 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/lighthouse_plugin/lighthouse_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/lighthouse_plugin/lighthouse_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/minigrid_environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/minigrid_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/configs/minigrid_nomemory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19216 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/minigrid_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/minigrid_sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-05-30 17:11:58.000000 allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/minigrid_offpolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 17:12:11.000000 allenact_plugins-0.5.3/setup.cfg
```

### Comparing `allenact_plugins-0.5.2/setup.py` & `allenact_plugins-0.5.3/allenact_plugins/setup.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins.egg-info/SOURCES.txt` & `allenact_plugins-0.5.3/allenact_plugins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins.egg-info/requires.txt` & `allenact_plugins-0.5.3/allenact_plugins.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 gym<0.20.0,>=0.17.0
 torch!=1.8.0,<2.0.0,>=1.6.0
 torchvision>=0.7.0
 numpy>=1.19.1
 wheel>=0.36.2
-allenact==0.5.2
+allenact==0.5.3
 
 [all]
-patsy>=0.5.1
-gym-minigrid>=1.0.1
-gym[box2d]<0.20.0,>=0.17.0
-patsy>=0.5.1
-gym-minigrid>=1.0.1
-pickle5
 ai2thor>=2.5.3
 numpy-quaternion
 pyquaternion>=0.9.9
 colour
 numba
 packaging
 python-xlib
+networkx
+gym[box2d]<0.20.0,>=0.17.0
 numpy-quaternion
 pyquaternion>=0.9.9
 numba
-torch>=1.7.1
-torchvision
-ftfy
-regex
-tqdm
-networkx
 ai2thor>=2.5.3
 numpy-quaternion
 pyquaternion>=0.9.9
 colour
 numba
 packaging
 python-xlib
+torch>=1.7.1
+torchvision
+ftfy
+regex
+tqdm
+patsy>=0.5.1
+gym-minigrid>=1.0.1
+patsy>=0.5.1
+gym-minigrid>=1.0.1
+pickle5
 
 [babyai]
 networkx
 
 [clip]
 torch>=1.7.1
 torchvision
```

### Comparing `allenact_plugins-0.5.2/allenact_plugins.egg-info/PKG-INFO` & `allenact_plugins-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: allenact-plugins
-Version: 0.5.2
+Name: allenact_plugins
+Version: 0.5.3
 Summary: Plugins for the AllenAct framework
 Home-page: https://github.com/allenai/allenact
 Author: Allen Institute for Artificial Intelligence
 Author-email: lucaw@allenai.org
 License: MIT
 Description: A collection of plugins/extensions for use within the AllenAct framework.
 Keywords: reinforcement learning,embodied-AI,AI,RL,SLAM
@@ -15,16 +15,16 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Provides-Extra: lighthouse
+Provides-Extra: robothor
+Provides-Extra: babyai
 Provides-Extra: gym
-Provides-Extra: minigrid
-Provides-Extra: ithor
 Provides-Extra: habitat
+Provides-Extra: ithor
 Provides-Extra: clip
-Provides-Extra: babyai
-Provides-Extra: robothor
+Provides-Extra: lighthouse
+Provides-Extra: minigrid
 Provides-Extra: all
```

### Comparing `allenact_plugins-0.5.2/allenact_plugins/setup.py` & `allenact_plugins-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/navigation_plugin/pointnav/models.py` & `allenact_plugins-0.5.3/allenact_plugins/navigation_plugin/pointnav/models.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/navigation_plugin/objectnav/models.py` & `allenact_plugins-0.5.3/allenact_plugins/navigation_plugin/objectnav/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,22 +216,24 @@
         auxiliary_uuids: Optional[List[str]] = None,
         # custom params
         rgb_resnet_preprocessor_uuid: Optional[str] = None,
         depth_resnet_preprocessor_uuid: Optional[str] = None,
         goal_dims: int = 32,
         resnet_compressor_hidden_out_dims: Tuple[int, int] = (128, 32),
         combiner_hidden_out_dims: Tuple[int, int] = (128, 32),
+        **kwargs,
     ):
         super().__init__(
             action_space=action_space,
             observation_space=observation_space,
             hidden_size=hidden_size,
             multiple_beliefs=multiple_beliefs,
             beliefs_fusion=beliefs_fusion,
             auxiliary_uuids=auxiliary_uuids,
+            **kwargs,
         )
 
         if (
             rgb_resnet_preprocessor_uuid is None
             or depth_resnet_preprocessor_uuid is None
         ):
             resnet_preprocessor_uuid = (
@@ -362,14 +364,15 @@
     def distribute_target(self, observations):
         target_emb = self.embed_goal(observations[self.goal_uuid])
         return target_emb.view(-1, self.goal_embed_dims, 1, 1).expand(
             -1, -1, self.resnet_tensor_shape[-2], self.resnet_tensor_shape[-1]
         )
 
     def adapt_input(self, observations):
+        observations = {**observations}
         resnet = observations[self.resnet_uuid]
         goal = observations[self.goal_uuid]
 
         use_agent = False
         nagent = 1
 
         if len(resnet.shape) == 6:
```

### Comparing `allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/arm_calculation_utils.py` & `allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/arm_calculation_utils.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/manipulathor_constants.py` & `allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/manipulathor_constants.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/manipulathor_tasks.py` & `allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/manipulathor_tasks.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/manipulathor_viz.py` & `allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/manipulathor_viz.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/manipulathor_sensors.py` & `allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/manipulathor_sensors.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/manipulathor_utils.py` & `allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/manipulathor_utils.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/manipulathor_environment.py` & `allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/manipulathor_environment.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/armpointnav_constants.py` & `allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/armpointnav_constants.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/manipulathor_plugin/manipulathor_task_samplers.py` & `allenact_plugins-0.5.3/allenact_plugins/manipulathor_plugin/manipulathor_task_samplers.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/lighthouse_plugin/lighthouse_models.py` & `allenact_plugins-0.5.3/allenact_plugins/lighthouse_plugin/lighthouse_models.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/lighthouse_plugin/lighthouse_environment.py` & `allenact_plugins-0.5.3/allenact_plugins/lighthouse_plugin/lighthouse_environment.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/lighthouse_plugin/lighthouse_util.py` & `allenact_plugins-0.5.3/allenact_plugins/lighthouse_plugin/lighthouse_util.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/lighthouse_plugin/lighthouse_tasks.py` & `allenact_plugins-0.5.3/allenact_plugins/lighthouse_plugin/lighthouse_tasks.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/lighthouse_plugin/lighthouse_sensors.py` & `allenact_plugins-0.5.3/allenact_plugins/lighthouse_plugin/lighthouse_sensors.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/gym_plugin/gym_sensors.py` & `allenact_plugins-0.5.3/allenact_plugins/gym_plugin/gym_sensors.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/gym_plugin/gym_environment.py` & `allenact_plugins-0.5.3/allenact_plugins/gym_plugin/gym_environment.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/gym_plugin/gym_models.py` & `allenact_plugins-0.5.3/allenact_plugins/gym_plugin/gym_models.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/gym_plugin/gym_tasks.py` & `allenact_plugins-0.5.3/allenact_plugins/gym_plugin/gym_tasks.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/minigrid_environments.py` & `allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/minigrid_environments.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/configs/minigrid_nomemory.py` & `allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/configs/minigrid_nomemory.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/minigrid_models.py` & `allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/minigrid_models.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/minigrid_offpolicy.py` & `allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/minigrid_offpolicy.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/minigrid_tasks.py` & `allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/minigrid_tasks.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/minigrid_plugin/minigrid_sensors.py` & `allenact_plugins-0.5.3/allenact_plugins/minigrid_plugin/minigrid_sensors.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/ithor_task_samplers.py` & `allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/ithor_task_samplers.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/ithor_viz.py` & `allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/ithor_viz.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/ithor_environment.py` & `allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/ithor_environment.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/ithor_tasks.py` & `allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/ithor_tasks.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/scripts/make_objectnav_debug_dataset.py` & `allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/scripts/make_objectnav_debug_dataset.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/scripts/make_pointnav_debug_dataset.py` & `allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/scripts/make_pointnav_debug_dataset.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/ithor_constants.py` & `allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/ithor_constants.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/ithor_util.py` & `allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/ithor_util.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/ithor_plugin/ithor_sensors.py` & `allenact_plugins-0.5.3/allenact_plugins/ithor_plugin/ithor_sensors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+from functools import reduce
 from typing import Any, Dict, Optional, Union, Sequence
 
 import ai2thor.controller
 import gym
 import gym.spaces
 import numpy as np
 import torch
@@ -28,17 +29,15 @@
 THOR_TASK_TYPE = Union[
     Task[ai2thor.controller.Controller],
     Task[IThorEnvironment],
     Task[RoboThorEnvironment],
 ]
 
 
-class RGBSensorThor(
-    RGBSensor[THOR_ENV_TYPE, THOR_TASK_TYPE]
-):
+class RGBSensorThor(RGBSensor[THOR_ENV_TYPE, THOR_TASK_TYPE]):
     """Sensor for RGB images in THOR.
 
     Returns from a running IThorEnvironment instance, the current RGB
     frame corresponding to the agent's egocentric view.
     """
 
     def frame_from_env(
@@ -265,18 +264,23 @@
     def get_observation(
         self,
         env: RoboThorEnvironment,
         task: Optional[Task[RoboThorEnvironment]],
         *args: Any,
         **kwargs: Any,
     ) -> Any:
-        scene_name = env.controller.last_event.metadata["sceneName"]
+        if isinstance(env, ai2thor.controller.Controller):
+            controller = env
+        else:
+            controller = env.controller
+
+        scene_name = controller.last_event.metadata["sceneName"]
         if scene_name not in self._bounds_cache:
             self._bounds_cache[scene_name] = self.get_bounds(
-                controller=env.controller, margin=self.margin
+                controller=controller, margin=self.margin
             )
 
         return copy.deepcopy(self._bounds_cache[scene_name])
 
 
 class SceneBoundsTHORSensor(Sensor[RoboThorEnvironment, Task[RoboThorEnvironment]]):
     def __init__(self, uuid: str = "scene_bounds", **kwargs: Any):
@@ -322,52 +326,70 @@
 class BinnedPointCloudMapTHORSensor(
     Sensor[RoboThorEnvironment, Task[RoboThorEnvironment]]
 ):
     observation_space = gym.spaces.Dict
 
     def __init__(
         self,
-        fov: float,
+        fov: Optional[float],
         vision_range_in_cm: int,
         map_size_in_cm: int,
         resolution_in_cm: int,
         map_range_sensor: Sensor,
+        return_egocentric_local_context: bool = False,
         height_bins: Sequence[float] = (0.02, 2),
         ego_only: bool = True,
+        exclude_agent: bool = False,
         uuid: str = "binned_pc_map",
+        device: torch.device = torch.device("cpu"),
         **kwargs: Any,
     ):
         self.fov = fov
         self.vision_range_in_cm = vision_range_in_cm
         self.map_size_in_cm = map_size_in_cm
         self.resolution_in_cm = resolution_in_cm
         self.height_bins = height_bins
         self.ego_only = ego_only
+        self.return_egocentric_local_context = return_egocentric_local_context
+        self.exclude_agent = exclude_agent
 
         self.binned_pc_map_builder = BinnedPointCloudMapBuilder(
             fov=fov,
             vision_range_in_cm=vision_range_in_cm,
             map_size_in_cm=map_size_in_cm,
             resolution_in_cm=resolution_in_cm,
             height_bins=height_bins,
+            return_egocentric_local_context=return_egocentric_local_context,
         )
+        self.device = device
 
-        map_space = gym.spaces.Box(
+        big_map_space = gym.spaces.Box(
             low=0,
             high=np.inf,
             shape=self.binned_pc_map_builder.binned_point_cloud_map.shape,
             dtype=np.float32,
         )
+        local_map_space = gym.spaces.Box(
+            low=0,
+            high=np.inf,
+            shape=(self.binned_pc_map_builder.vision_range_in_map_units,) * 2
+            + self.binned_pc_map_builder.binned_point_cloud_map.shape[-1:],
+            dtype=np.float32,
+        )
 
         space_dict = {
-            "egocentric_update": map_space,
+            "egocentric_update": local_map_space,
         }
+        if self.return_egocentric_local_context:
+            space_dict = {
+                "egocentric_local_context": copy.deepcopy(local_map_space),
+            }
         if not ego_only:
-            space_dict["allocentric_update"] = copy.deepcopy(map_space)
-            space_dict["map"] = copy.deepcopy(map_space)
+            space_dict["allocentric_update"] = copy.deepcopy(big_map_space)
+            space_dict["map"] = copy.deepcopy(big_map_space)
 
         observation_space = gym.spaces.Dict(space_dict)
         super().__init__(**prepare_locals_for_super(locals()))
 
         self.map_range_sensor = map_range_sensor
 
     @property
@@ -381,31 +403,45 @@
     def get_observation(
         self,
         env: RoboThorEnvironment,
         task: Optional[Task[RoboThorEnvironment]],
         *args: Any,
         **kwargs: Any,
     ) -> Any:
-        e = env.controller.last_event
+        if isinstance(env, ai2thor.controller.Controller):
+            controller = env
+        else:
+            controller = env.controller
+
+        e = controller.last_event
         metadata = e.metadata
 
         if task.num_steps_taken() == 0:
             xz_ranges_dict = self.map_range_sensor.get_observation(env=env, task=task)
+            if self.fov is None:
+                self.binned_pc_map_builder.fov = e.metadata["fov"]
             self.binned_pc_map_builder.reset(
                 min_xyz=np.array(
                     [
                         xz_ranges_dict["x_range"][0],
                         0,  # TODO: Should y be different per scene?
                         xz_ranges_dict["z_range"][0],
                     ]
                 )
             )
 
+        depth_frame = e.depth_frame
+
+        if self.exclude_agent:
+            depth_frame = depth_frame.copy()
+            assert len(e.instance_masks) > 0
+            depth_frame[~reduce(np.logical_or, e.instance_masks.values())] = np.nan
+
         map_dict = self.binned_pc_map_builder.update(
-            depth_frame=e.depth_frame,
+            depth_frame=depth_frame,
             camera_xyz=np.array(
                 [metadata["cameraPosition"][k] for k in ["x", "y", "z"]]
             ),
             camera_rotation=metadata["agent"]["rotation"]["y"],
             camera_horizon=metadata["agent"]["cameraHorizon"],
         )
         return {k: map_dict[k] for k in self.observation_space.spaces.keys()}
```

### Comparing `allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/habitat_sensors.py` & `allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/habitat_sensors.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/habitat_tasks.py` & `allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/habitat_tasks.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/scripts/make_map.py` & `allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/scripts/make_map.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/scripts/agent_demo.py` & `allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/scripts/agent_demo.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/habitat_constants.py` & `allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/habitat_constants.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/habitat_task_samplers.py` & `allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/habitat_task_samplers.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/habitat_utils.py` & `allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/habitat_utils.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/habitat_plugin/habitat_environment.py` & `allenact_plugins-0.5.3/allenact_plugins/habitat_plugin/habitat_environment.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """A wrapper for interacting with the Habitat environment."""
 import os
 from typing import Dict, Union, List, Optional
 
-import habitat
 import numpy as np
+
+import habitat
+from allenact.utils.cache_utils import DynamicDistanceCache
+from allenact.utils.system import get_logger
 from habitat.config import Config
 from habitat.core.dataset import Dataset
 from habitat.core.simulator import Observations, AgentState, ShortestPathPoint
 from habitat.tasks.nav.nav import NavigationEpisode as HabitatNavigationEpisode
 
-from allenact.utils.cache_utils import DynamicDistanceCache
-from allenact.utils.system import get_logger
-
 
 class HabitatEnvironment:
     def __init__(self, config: Config, dataset: Dataset, verbose: bool = False) -> None:
         self.env = habitat.Env(config=config, dataset=dataset)
 
         if not verbose:
             os.environ["GLOG_minloglevel"] = "2"
```

### Comparing `allenact_plugins-0.5.2/allenact_plugins/clip_plugin/clip_preprocessors.py` & `allenact_plugins-0.5.3/allenact_plugins/clip_plugin/clip_preprocessors.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         self,
         rgb_input_uuid: str,
         clip_model_type: str,
         pool: bool,
         device: Optional[torch.device] = None,
         device_ids: Optional[List[torch.device]] = None,
         input_img_height_width: Tuple[int, int] = (224, 224),
+        chunk_size: Optional[int] = None,
         **kwargs: Any,
     ):
         assert clip_model_type in clip.available_models()
         assert pool == False or input_img_height_width == (224, 224)
         assert all(iis % 32 == 0 for iis in input_img_height_width)
 
         output_height_width = tuple(iis // 32 for iis in input_img_height_width)
@@ -76,14 +77,16 @@
 
         self.device = torch.device("cpu") if device is None else device
         self.device_ids = device_ids or cast(
             List[torch.device], list(range(torch.cuda.device_count()))
         )
         self._resnet: Optional[ClipResNetEmbedder] = None
 
+        self.chunk_size = chunk_size
+
         low = -np.inf
         high = np.inf
         shape = output_shape
 
         input_uuids = [rgb_input_uuid]
         assert (
             len(input_uuids) == 1
@@ -111,15 +114,27 @@
         return self
 
     def process(self, obs: Dict[str, Any], *args: Any, **kwargs: Any) -> Any:
         x = obs[self.input_uuids[0]].to(self.device).permute(0, 3, 1, 2)  # bhwc -> bchw
         # If the input is depth, repeat it across all 3 channels
         if x.shape[1] == 1:
             x = x.repeat(1, 3, 1, 1)
-        x = self.resnet(x).float()
+
+        n = x.shape[0]
+        if self.chunk_size is not None and x.shape[0] > self.chunk_size:
+            processed_chunks = []
+            for idx in range(0, n, self.chunk_size):
+                processed_chunks.append(
+                    self.resnet(
+                        x[idx : min(idx + self.chunk_size, n)]
+                    ).float()
+                )
+            x = torch.cat(processed_chunks, dim=0)
+        else:
+            x = self.resnet(x).float()
         return x
 
 
 class ClipViTEmbedder(nn.Module):
     def __init__(self, model: CLIP, class_emb_only: bool = False):
         super().__init__()
         self.model = model
```

### Comparing `allenact_plugins-0.5.2/allenact_plugins/babyai_plugin/babyai_tasks.py` & `allenact_plugins-0.5.3/allenact_plugins/babyai_plugin/babyai_tasks.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/babyai_plugin/scripts/get_instr_length_percentiles.py` & `allenact_plugins-0.5.3/allenact_plugins/babyai_plugin/scripts/get_instr_length_percentiles.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/babyai_plugin/scripts/download_babyai_expert_demos.py` & `allenact_plugins-0.5.3/allenact_plugins/babyai_plugin/scripts/download_babyai_expert_demos.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/babyai_plugin/scripts/truncate_expert_demos.py` & `allenact_plugins-0.5.3/allenact_plugins/babyai_plugin/scripts/truncate_expert_demos.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/babyai_plugin/babyai_models.py` & `allenact_plugins-0.5.3/allenact_plugins/babyai_plugin/babyai_models.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/robothor_tasks.py` & `allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/robothor_tasks.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/robothor_environment.py` & `allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/robothor_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,19 +187,19 @@
     def path_from_point_to_point(
         self, position: Dict[str, float], target: Dict[str, float], allowedError: float
     ) -> Optional[List[Dict[str, float]]]:
         try:
             return self.controller.step(
                 action="GetShortestPathToPoint",
                 position=position,
-                x=target["x"],
-                y=target["y"],
-                z=target["z"],
+                target=target,
                 allowedError=allowedError,
             ).metadata["actionReturn"]["corners"]
+        except ValueError:
+            raise
         except Exception:
             get_logger().debug(
                 "Failed to find path for {} in {}. Start point {}, agent state {}.".format(
                     target,
                     self.controller.last_event.metadata["sceneName"],
                     position,
                     self.agent_state(),
```

### Comparing `allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/scripts/make_objectnav_debug_dataset.py` & `allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/scripts/make_objectnav_debug_dataset.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/scripts/make_pointnav_debug_dataset.py` & `allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/scripts/make_pointnav_debug_dataset.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/robothor_models.py` & `allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/robothor_models.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/robothor_sensors.py` & `allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/robothor_sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 
         super().__init__(**prepare_locals_for_super(locals()))
 
     def frame_from_env(
         self, env: THOR_ENV_TYPE, task: Optional[THOR_TASK_TYPE]
     ) -> np.ndarray:
         if not isinstance(env, ai2thor.controller.Controller):
-            env = env.controller.last_event.depth_frame
+            return env.controller.last_event.depth_frame
 
         return env.last_event.depth_frame
 
 
 class DepthSensorRoboThor(DepthSensorThor):
     # For backwards compatibility
     def __init__(self, *args: Any, **kwargs: Any):
```

### Comparing `allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/robothor_distributions.py` & `allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/robothor_distributions.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/robothor_preprocessors.py` & `allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/robothor_preprocessors.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/robothor_task_samplers.py` & `allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/robothor_task_samplers.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/allenact_plugins/robothor_plugin/robothor_viz.py` & `allenact_plugins-0.5.3/allenact_plugins/robothor_plugin/robothor_viz.py`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/README.md` & `allenact_plugins-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `allenact_plugins-0.5.2/PKG-INFO` & `allenact_plugins-0.5.3/allenact_plugins.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: allenact_plugins
-Version: 0.5.2
+Name: allenact-plugins
+Version: 0.5.3
 Summary: Plugins for the AllenAct framework
 Home-page: https://github.com/allenai/allenact
 Author: Allen Institute for Artificial Intelligence
 Author-email: lucaw@allenai.org
 License: MIT
 Description: A collection of plugins/extensions for use within the AllenAct framework.
 Keywords: reinforcement learning,embodied-AI,AI,RL,SLAM
@@ -15,16 +15,16 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Provides-Extra: lighthouse
+Provides-Extra: robothor
+Provides-Extra: babyai
 Provides-Extra: gym
-Provides-Extra: minigrid
-Provides-Extra: ithor
 Provides-Extra: habitat
+Provides-Extra: ithor
 Provides-Extra: clip
-Provides-Extra: babyai
-Provides-Extra: robothor
+Provides-Extra: lighthouse
+Provides-Extra: minigrid
 Provides-Extra: all
```

