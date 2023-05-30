# Comparing `tmp/shepherd_core-2023.5.5.tar.gz` & `tmp/shepherd_core-2023.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shepherd_core-2023.5.5.tar", last modified: Wed May  3 19:29:44 2023, max compression
+gzip compressed data, was "shepherd_core-2023.5.6.tar", last modified: Tue May 30 13:03:18 2023, max compression
```

## Comparing `shepherd_core-2023.5.5.tar` & `shepherd_core-2023.5.6.tar`

### file list

```diff
@@ -1,77 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.457703 shepherd_core-2023.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-03 19:29:44.457703 shepherd_core-2023.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-03 19:29:44.457703 shepherd_core-2023.5.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.445703 shepherd_core-2023.5.5/shepherd_core/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.445703 shepherd_core-2023.5.5/shepherd_core/data_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.445703 shepherd_core-2023.5.5/shepherd_core/data_models/base/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/base/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/base/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/base/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/base/shepherd.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/base/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.449703 shepherd_core-2023.5.5/shepherd_core/data_models/content/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/content/energy_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/content/energy_environment_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/content/firmware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/content/firmware_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/content/virtual_harvester.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/content/virtual_harvester_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/content/virtual_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/content/virtual_source_fixture.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.449703 shepherd_core-2023.5.5/shepherd_core/data_models/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/experiment/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/experiment/observer_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/experiment/target_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/model_virtualSourceDoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.449703 shepherd_core-2023.5.5/shepherd_core/data_models/task/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/task/emulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/task/firmware_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/task/observer_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/task/programmer.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/task/testbed_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.453703 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/cape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/cape_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/gpio_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/mcu.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/mcu_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/observer_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/target_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/testbed.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/testbed_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.457703 shepherd_core-2023.5.5/shepherd_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-03 19:29:44.000000 shepherd_core-2023.5.5/shepherd_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-03 19:29:44.000000 shepherd_core-2023.5.5/shepherd_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:29:44.000000 shepherd_core-2023.5.5/shepherd_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 19:29:44.000000 shepherd_core-2023.5.5/shepherd_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 19:29:44.000000 shepherd_core-2023.5.5/shepherd_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:29:44.000000 shepherd_core-2023.5.5/shepherd_core.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.457703 shepherd_core-2023.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/example_config_experiment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/example_config_experiment_alternative.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/test_content_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/test_content_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/test_experiment_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/test_task_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/test_task_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/test_testbed_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/test_testbed_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.280735 shepherd_core-2023.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-30 13:03:18.280735 shepherd_core-2023.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-30 13:03:18.280735 shepherd_core-2023.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.268735 shepherd_core-2023.5.6/shepherd_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/calibration_hw_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.268735 shepherd_core-2023.5.6/shepherd_core/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.272735 shepherd_core-2023.5.6/shepherd_core/data_models/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/base/cal_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/base/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/base/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/base/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/base/shepherd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/base/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.272735 shepherd_core-2023.5.6/shepherd_core/data_models/content/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/content/energy_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/content/energy_environment_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/content/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/content/firmware_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/content/virtual_harvester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/content/virtual_harvester_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/content/virtual_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/content/virtual_source_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/doc_virtual_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.272735 shepherd_core-2023.5.6/shepherd_core/data_models/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/experiment/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/experiment/observer_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/experiment/target_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.272735 shepherd_core-2023.5.6/shepherd_core/data_models/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/task/emulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/task/firmware_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/task/harvest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/task/observer_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/task/programming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/task/testbed_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.276735 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/cape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/cape_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/gpio_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/mcu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/mcu_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/observer_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/target_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/testbed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/data_models/testbed/testbed_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.276735 shepherd_core-2023.5.6/shepherd_core/vsource/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/vsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/vsource/virtual_converter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/vsource/virtual_harvester_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/vsource/virtual_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/shepherd_core/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.280735 shepherd_core-2023.5.6/shepherd_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-30 13:03:18.000000 shepherd_core-2023.5.6/shepherd_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-30 13:03:18.000000 shepherd_core-2023.5.6/shepherd_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:03:18.000000 shepherd_core-2023.5.6/shepherd_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-30 13:03:18.000000 shepherd_core-2023.5.6/shepherd_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 13:03:18.000000 shepherd_core-2023.5.6/shepherd_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:03:18.000000 shepherd_core-2023.5.6/shepherd_core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.276735 shepherd_core-2023.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.280735 shepherd_core-2023.5.6/tests/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_cal_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_cal_data_faulty.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_cal_meas.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_cal_meas_faulty1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_cal_meas_faulty2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_config_emulator.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_config_experiment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_config_experiment_alternative.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_config_harvester.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_config_testbed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/example_config_virtsource.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/test_base_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/test_content_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/test_content_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/test_experiment_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/test_task_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/test_task_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/test_testbed_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/data_models/test_testbed_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/test_cal_hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:18.280735 shepherd_core-2023.5.6/tests/vsource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/vsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/vsource/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/vsource/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-30 13:03:04.000000 shepherd_core-2023.5.6/tests/vsource/test_harvester.py
```

### Comparing `shepherd_core-2023.5.5/PKG-INFO` & `shepherd_core-2023.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd_core
-Version: 2023.5.5
+Version: 2023.5.6
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-core/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
```

### Comparing `shepherd_core-2023.5.5/README.md` & `shepherd_core-2023.5.6/README.md`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.5/setup.cfg` & `shepherd_core-2023.5.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 python_requires = >= 3.7
 install_requires = 
 	h5py
 	numpy
 	pyYAML
 	chromalog
 	pydantic[email]<2.0.0
+	tqdm
+	scipy
 
 [options.extras_require]
 dev = 
 	black
 	pylint
 	flake8
 	twine
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/__init__.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from .base.calibration import CalibrationCape
+from .base.calibration import CalibrationEmulator
+from .base.calibration import CalibrationHarvester
 from .base.calibration import CalibrationPair
 from .base.calibration import CalibrationSeries
 from .base.content import ContentModel
 from .base.fixture import Fixtures
 from .base.shepherd import ShpModel
 from .base.wrapper import Wrapper
 from .content.energy_environment import EnergyDType
@@ -17,14 +20,17 @@
 from .experiment.observer_features import GpioTracing
 from .experiment.observer_features import PowerTracing
 from .experiment.observer_features import SystemLogging
 from .experiment.target_config import TargetConfig
 
 __all__ = [
     # Core
+    "CalibrationCape",
+    "CalibrationEmulator",
+    "CalibrationHarvester",
     "CalibrationSeries",
     "CalibrationPair",
     "ContentModel",
     "ShpModel",
     "Fixtures",
     "Wrapper",
     # User Content
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/base/content.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/base/content.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,46 +7,49 @@
 from pydantic import constr
 from pydantic import root_validator
 
 from .shepherd import ShpModel
 
 # constr -> to_lower=True, max_length=16, regex=r"^[\w]+$"
 # ⤷ Regex = AlphaNum
-id_int = conint(ge=0, lt=2**128)
-name_str = constr(max_length=32, regex=r'^[^<>:;,?"*|]+$')
-# ⤷ Regex = FS-Compatible ASCII
-safe_str = constr(regex=r"^[ -~]+$")
+IdInt = conint(ge=0, lt=2**128)
+NameStr = constr(max_length=32, regex=r'^[^<>:;,?"*|\/\\]+$')
+# ⤷ Regex = FileSystem-Compatible ASCII
+SafeStr = constr(regex=r"^[ -~]+$")
 # ⤷ Regex = All Printable ASCII-Characters with Space
 
 
 def id_default() -> int:
     time_stamp = str(datetime.now()).encode("utf-8")
     time_hash = hashlib.sha3_224(time_stamp).hexdigest()[-16:]
     return int(time_hash, 16)
 
 
 class ContentModel(ShpModel):
     # General Properties
-    id: id_int = Field(  # noqa: A003
+    id: IdInt = Field(  # noqa: A003
         description="Unique ID",
         default_factory=id_default,
     )
-    name: name_str
-    description: Optional[safe_str] = Field(description="Required when public")
-    comment: Optional[safe_str] = None
+    name: NameStr
+    description: Optional[SafeStr] = Field(description="Required when public")
+    comment: Optional[SafeStr] = None
     created: datetime = Field(default_factory=datetime.now)
 
     # Ownership & Access
-    owner: name_str
-    group: name_str = Field(description="University or Subgroup")
+    owner: NameStr
+    group: NameStr = Field(description="University or Subgroup")
     visible2group: bool = False
     visible2all: bool = False
 
+    def __str__(self):
+        return self.name
+
     @root_validator(pre=False)
-    def content_validation(cls, values: dict):
-        is_visible = values["visible2group"] or values["visible2all"]
-        if is_visible and values["description"] is None:
+    def content_validation(cls, values: dict) -> dict:
+        is_visible = values.get("visible2group") or values.get("visible2all")
+        if is_visible and values.get("description") is None:
             raise ValueError(
                 "Public instances require a description "
                 "(check visible2*- and description-field)"
             )
         return values
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/base/fixture.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/base/fixture.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,16 +44,18 @@
                 self.elements_by_id[_id] = data
         # for iterator
         self._iter_index: int = 0
         self._iter_list: list = list(self.elements_by_name.values())
 
     def __getitem__(self, key) -> dict:
         key = key.lower()
-        if key in self.elements_by_name:
-            return self.elements_by_name[key]
+        if key.lower() in self.elements_by_name:
+            return self.elements_by_name[key.lower()]
+        if key in self.elements_by_id:
+            return self.elements_by_id[key]
         raise ValueError(f"{self.name} '{key}' not found!")
 
     def __iter__(self):
         self._iter_index = 0
         self._iter_list = list(self.elements_by_name.values())
         return self
 
@@ -63,14 +65,17 @@
             self._iter_index += 1
             return member
         raise StopIteration
 
     def keys(self):  # -> _dict_keys[Any, Any]:
         return self.elements_by_name.keys()
 
+    def refs(self) -> dict:
+        return {_i["id"]: _i["name"] for _i in self.elements_by_id.values()}
+
     def inheritance(self, values: dict, chain: Optional[list] = None) -> (dict, list):
         if chain is None:
             chain = []
         values = copy.copy(values)
         post_process: bool = False
         fixture_base: dict = {}
         if "inherit_from" in values:
@@ -98,15 +103,15 @@
             values = base_dict
 
         elif "name" in values and values.get("name").lower() in self.elements_by_name:
             fixture_name = values.get("name").lower()
             fixture_base = copy.copy(self.elements_by_name[fixture_name])
             post_process = True
 
-        elif "id" in values and values["id"] in self.elements_by_id:
+        elif values.get("id") in self.elements_by_id:
             _id = values["id"]
             fixture_base = copy.copy(self.elements_by_id[_id])
             post_process = True
 
         if post_process:
             # last two cases need
             for key, value in values.items():
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/base/shepherd.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/base/shepherd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import hashlib
 import pathlib
+from datetime import datetime
 from pathlib import Path
+from typing import Optional
 from typing import Union
 
 import yaml
 from pydantic import BaseModel
 from pydantic import Extra
 
 from .wrapper import Wrapper
@@ -16,15 +18,24 @@
 
 yaml.add_representer(pathlib.PosixPath, repr_str)
 yaml.add_representer(pathlib.WindowsPath, repr_str)
 yaml.add_representer(pathlib.Path, repr_str)
 
 
 class ShpModel(BaseModel):
-    """Pre-configured Pydantic Base-Model (specifically for shepherd)"""
+    """Pre-configured Pydantic Base-Model (specifically for shepherd)
+
+    Inheritable Features:
+    - constant / frozen, hashable .get_hash()
+    - safe / limited custom types
+    - string-representation str(ShpModel)
+    - accessible as class (model.var) and dict (model[var])
+    - yaml-support with type-safe .from_file() & .to_file()
+    - schema cls.schema() can also be stored to yaml with .dump_schema()
+    """
 
     _min_dict: dict = {}
 
     class Config:
         allow_mutation = False  # const after creation?
         frozen = True  # -> hashable! but currently manually with .get_hash()
         extra = Extra.forbid  # no unnamed attributes allowed
@@ -33,35 +44,48 @@
         min_anystr_length = 4
         max_anystr_length = 512
         # ⤷ local str-length constraints overrule global ones!
         anystr_strip_whitespace = True  # strip leading & trailing whitespaces
         use_enum_values = True  # cleaner export of enum-fields
         allow_inf_nan = False  # float without +-inf or NaN
         underscore_attrs_are_private = True  # allows using them
-
         # Options:
         # - https://docs.pydantic.dev/usage/schema/#field-customization
         # - https://docs.pydantic.dev/usage/model_config/
         # "fields["name"].description = ... should be usable to modify model
 
+    def __repr__(self) -> str:
+        return str(self.dict())
+
+    def __getitem__(self, key):
+        return self.__getattribute__(key)
+
     @classmethod
-    def dump_schema(cls, path: Union[str, Path]):
+    def dump_schema(cls, path: Union[str, Path]) -> None:
+        # TODO: rename to schema_to_file(), if needed at all
         model_dict = cls.schema()
         model_yaml = yaml.dump(model_dict, default_flow_style=False, sort_keys=False)
         with open(Path(path).with_suffix(".yaml"), "w") as f:
             f.write(model_yaml)
 
-    def to_file(self, path: Union[str, Path], minimal: bool = False):
+    def to_file(
+        self,
+        path: Union[str, Path],
+        minimal: bool = False,
+        comment: Optional[str] = None,
+    ) -> Path:
         if minimal:
             model_dict = self._min_dict
         else:
             model_dict = self.dict()
         model_wrap = Wrapper(
             model=type(self).__name__,
             id=model_dict.get("id"),
+            comment=comment,
+            created=datetime.now(),
             fields=model_dict,
         )
         model_yaml = yaml.dump(
             model_wrap.dict(), default_flow_style=False, sort_keys=False
         )
         model_path = Path(path).with_suffix(".yaml")
         with open(model_path, "w") as f:
@@ -74,15 +98,15 @@
 
     @classmethod
     def from_file(cls, path: Union[str, Path]):
         with open(Path(path)) as shp_file:
             shp_dict = yaml.safe_load(shp_file)
         shp_wrap = Wrapper(**shp_dict)
         if shp_wrap.model != cls.__name__:
-            raise ValueError("Model in file does not match the used one")
+            raise ValueError("Model in file does not match the requirement")
         return cls(**shp_wrap.fields)
 
     @classmethod  # @root_validator(pre=True, allow_reuse=True)
     def pre_snitch(cls, values):  # TODO: useless
         values["_min_dict"] = values
         return values
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/content/energy_environment.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/content/firmware.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from enum import Enum
 from pathlib import Path
+from typing import Union
 
-from pydantic import PositiveFloat
+from pydantic import constr
 from pydantic import root_validator
 
 from ..base.content import ContentModel
 from ..base.fixture import Fixtures
+from ..testbed.mcu import MCU
 
-fixture_path = Path(__file__).resolve().with_name("energy_environment_fixture.yaml")
-fixtures = Fixtures(fixture_path, "EnergyEnvironment")
+fixture_path = Path(__file__).resolve().with_name("firmware_fixture.yaml")
+fixtures = Fixtures(fixture_path, "firmware")
 
 
-class EnergyDType(str, Enum):
-    ivsample = "ivsample"
-    ivcurve = "ivcurve"
-    isc_voc = "isc_voc"
+class FirmwareDType(str, Enum):
+    base64_hex = "hex"
+    base64_elf = "elf"
+    path_hex = "path_hex"
+    path_elf = "path_elf"
 
 
-class EnergyEnvironment(ContentModel):
-    """Recording of meta-data representation of a testbed-component"""
+class Firmware(ContentModel, title="Firmware of Target"):
+    """meta-data representation of a data-component"""
 
     # General Metadata & Ownership -> ContentModel
 
-    data_path: Path
-    data_type: EnergyDType
+    mcu: MCU
 
-    duration: PositiveFloat
-    energy_Ws: PositiveFloat
-    valid: bool = False
+    data: Union[constr(min_length=3, max_length=1_000_000), Path]
+    data_type: FirmwareDType
 
     @root_validator(pre=True)
     def from_fixture(cls, values: dict) -> dict:
         values = fixtures.lookup(values)
-        values, chain = fixtures.inheritance(values)
+        values, _ = fixtures.inheritance(values)
         return values
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/content/energy_environment_fixture.yaml` & `shepherd_core-2023.5.6/shepherd_core/data_models/content/energy_environment_fixture.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -27,7 +27,24 @@
     valid: true
 
     owner: Ingmar
     group: NES Lab
     visible2group: true
     visible2all: true
     created: 2022-12-12 12:12:12
+
+- model: EnergyEnvironment
+  id: 666
+  fields:
+    name: nuclear
+    description: Energy harvested
+    data_path: eenv/group/user/thermoelectric_1h_wash.h5
+    data_type: ivcurve
+    duration: 3600
+    energy_Ws: 0.1
+    valid: false
+
+    owner: Ingmar
+    group: NES Lab
+    visible2group: true
+    visible2all: true
+    created: 2022-12-12 12:12:12
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/content/firmware_fixture.yaml` & `shepherd_core-2023.5.6/shepherd_core/data_models/content/firmware_fixture.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,83 @@
 ---
 - model: Firmware
   id: 1001
   fields:
-    id: 1001
     name: nrf52_open4group
     mcu:
       name: nRF52
     owner: Ingmar
     group: NES Lab
     visible2group: true
     visible2all: false
     created: 2022-12-12 12:12:12
 - model: Firmware
   id: 1002
   fields:
-    id: 1002
     name: msp430_open4group
     mcu:
       name: MSP430FR
     owner: Ingmar
     group: NES Lab
     visible2group: true
     visible2all: false
     created: 2022-12-12 12:12:12
 - model: Firmware
   id: 2000
   fields:
-    id: 2000
     name: nrf52_demo_rf
     description: demo implementation for a simple node that sends readings when energy budget allows it
-    data: name.hex
-    data_type: path_hex
+    data: name.elf
+    data_type: path_elf
     visible2all: true
     inherit_from: nrf52_open4group
 - model: Firmware
   id: 2001
   fields:
-    id: 2001
     name: nrf52_spi_radio
     description: default implementation to use nRF as a radio frontend
-    data: name.hex
-    data_type: path_hex
+    data: name.elf
+    data_type: path_elf
     visible2all: true
     inherit_from: nrf52_open4group
 - model: Firmware
   id: 2002
   fields:
-    id: 2002
     name: nrf52_testable
     description: blinks LEDs on boot and listens/answers to UART
-    data: name.hex
-    data_type: path_hex
+    data: name.elf
+    data_type: path_elf
     inherit_from: nrf52_open4group
 - model: firmware
   id: 2003
   fields:
-    id: 2003
     name: nrf52_conn_test_tx
     description: Connection Tester - TX-Unit - sends packet with every possible P_TX, loops 10x
-    data: name.hex
-    data_type: path_hex
+    data: name.elf
+    data_type: path_elf
     inherit_from: nrf52_open4group
 - model: Firmware
   id: 3000
   fields:
-    id: 2000
     name: msp430_deep_sleep
     description: practically turned off msp with lowest possible consumption
-    data: name.hex
-    data_type: path_hex
+    data: name.elf
+    data_type: path_elf
     visible2all: true
     inherit_from: msp430_open4group
 - model: Firmware
-  id: 2001
+  id: 3001
   fields:
-    id: 2001
     name: msp430_spi_fram
     description: default implementation to use MSP as a flash storage
-    data: name.hex
-    data_type: path_hex
+    data: name.elf
+    data_type: path_elf
     visible2all: true
     inherit_from: msp430_open4group
 - model: Firmware
-  id: 2002
+  id: 3002
   fields:
-    id: 2002
     name: msp430_testable
     description: blinks LEDs on boot and listens/answers to UART
-    data: name.hex
-    data_type: path_hex
+    data: name.elf
+    data_type: path_elf
     inherit_from: msp430_open4group
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/content/virtual_harvester_fixture.yaml` & `shepherd_core-2023.5.6/shepherd_core/data_models/content/virtual_harvester_fixture.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -3,43 +3,29 @@
 # - look into the implementation to see which parameters are used
 # - base for neutral fallback values if provided yml is sparse
 # - -> it is encouraged to omit redundant parameters in your own implementation
 - model: VirtualHarvester
   id: 1000
   fields:
     name: neutral
-    description: Can NOT be used as a valid harvester
-    window_size: 8
-    voltage_mV: 2500  # starting-point for some algorithms (mppt_po)
-    voltage_min_mV: 0
-    voltage_max_mV: 5000
-    current_limit_uA: 50000   # allows to keep trajectory in special region (or constant current tracking)
-    voltage_step_mV: 1
-    # TODO: current limit not used atm?!
-    setpoint_n: 0.70
-    interval_ms: 100     # between start of measurements
-    duration_ms: 0.1     # of measurement
-    rising: true
-    # underlying recoder
-    wait_cycles: 1 # first cycle: ADC-Sampling & DAC-Writing, further steps: waiting
     owner: Ingmar
     group: NES Lab
     visible2group: true
     visible2all: true
     created: 2022-12-12 12:12:12
 
 - model: VirtualHarvester
   id: 1010
   fields:
     name: ivcurve
     description: Postpone harvesting by sampling ivcurves (voltage stepped as sawtooth-wave)
     comment: ~200 Hz
     inherit_from: neutral
-    datatype: ivcurve
-    window_size: 250
+    algorithm: ivcurve
+    samples_n: 250
     voltage_min_mV: 0
     voltage_max_mV: 5000
     wait_cycles: 1  # results in 200 Hz (= 100kHz /(2*250))
     rising: false # downward sawtooth seems to have advantages for solar cells
     # todo: also add switch for sawtooth- vs triangle-wave?
     # todo: could also include a version with dynamic upper-boundary, varied if voc is reached very early
 
@@ -51,42 +37,42 @@
 
 - model: VirtualHarvester
   id: 1012
   fields:
     name: iv1000
     comment: Name relates to curves per second
     inherit_from: ivcurve
-    window_size: 100
+    samples_n: 100
     wait_cycles: 0
 
 - model: VirtualHarvester
   id: 1013
   fields:
     name: iv110
     comment: Between 50 & 60 Hz line-frequency to avoid standing waves
     inherit_from: ivcurve
-    window_size: 909
+    samples_n: 909
     wait_cycles: 0
 
 - model: VirtualHarvester
   id: 1020
   fields:
     name: isc_voc
     description: Postpone harvesting by sampling short circuit current & open circuit voltage
     inherit_from: neutral
-    datatype: isc_voc
+    algorithm: isc_voc
     wait_cycles: 1  # results in 25 kHz (isc, wait, voc, wait)
 
 - model: VirtualHarvester
   id: 1030
   fields:
     name: cv20
     description: Harvesting with constant Voltage
     inherit_from: neutral
-    datatype: ivsample
+    algorithm: cv
     voltage_mV: 2000
 
 - model: VirtualHarvester
   id: 1031
   fields:
     name: cv24
     inherit_from: cv20
@@ -96,20 +82,27 @@
   id: 1032
   fields:
     name: cv33
     inherit_from: cv20
     voltage_mV: 3300
 
 - model: VirtualHarvester
+  id: 1032
+  fields:
+    name: cv10
+    inherit_from: cv20
+    voltage_mV: 1000
+
+- model: VirtualHarvester
   id: 1040
   fields:
     name: mppt_voc
     description: MPPT based on open circuit voltage for solar
     inherit_from: neutral
-    datatype: ivsample
+    algorithm: mppt_voc
     setpoint_n: 0.76
     interval_ms: 100     # between measurements
     duration_ms: 1.2     # solar can overshoot when load is removed
     current_limit_uA: 5  # boundary for detecting open circuit in emulated version (working on IV-Curves)
 
 - model: VirtualHarvester
   id: 1041
@@ -145,21 +138,22 @@
 
 - model: VirtualHarvester
   id: 1045
   fields:
     name: mppt_po
     description: MPPT based on perturb & observe algorithm
     inherit_from: neutral
-    datatype: ivsample
+    algorithm: mppt_po
     voltage_min_mV: 0
     voltage_max_mV: 5000
     voltage_step_mV: 10
     interval_ms: 18   # between steps
 
 - model: VirtualHarvester
   id: 1046
   fields:
     name: mppt_opt
-    description: Power-Otimum with very fast PO-Variant (harvesting) or special max-pwr-picker (emulator / ivcurve)
+    description: Power-Optimum with very fast PO-Variant (harvesting) or special max-pwr-picker (emulator / ivcurve)
     inherit_from: mppt_po
+    algorithm: mppt_opt
     voltage_step_mV: 1
     interval_ms: 0.01
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/content/virtual_source_fixture.yaml` & `shepherd_core-2023.5.6/shepherd_core/data_models/content/virtual_source_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/experiment/__init__.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/experiment/experiment.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/experiment/experiment.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,41 +3,41 @@
 from typing import Optional
 
 from pydantic import EmailStr
 from pydantic import Field
 from pydantic import conlist
 from pydantic import root_validator
 
+from ..base.content import IdInt
+from ..base.content import NameStr
+from ..base.content import SafeStr
 from ..base.content import id_default
-from ..base.content import id_int
-from ..base.content import name_str
-from ..base.content import safe_str
 from ..base.shepherd import ShpModel
 from ..testbed.target import Target
 from ..testbed.testbed import Testbed
 from .observer_features import SystemLogging
 from .target_config import TargetConfig
 
 
 class Experiment(ShpModel, title="Config of an Experiment"):
     """Configuration for Experiments on the Shepherd-Testbed
     emulating Energy Environments for Target Nodes"""
 
     # General Properties
-    id: id_int = Field(  # noqa: A003
+    id: IdInt = Field(  # noqa: A003
         description="Unique ID",
         default_factory=id_default,
     )
-    name: name_str
-    description: Optional[safe_str] = Field(description="Required for public instances")
-    comment: Optional[safe_str] = None
+    name: NameStr
+    description: Optional[SafeStr] = Field(description="Required for public instances")
+    comment: Optional[SafeStr] = None
     created: datetime = Field(default_factory=datetime.now)
 
     # Ownership & Access, TODO
-    owner_id: Optional[id_int] = 5472  # UUID?
+    owner_id: Optional[IdInt] = 5472  # UUID?
 
     # feedback
     email_results: Optional[EmailStr]  # TODO: can be bool, as its linked to account
     sys_logging: SystemLogging = SystemLogging(dmesg=True, ptp=False, shepherd=True)
 
     # schedule
     time_start: Optional[datetime] = None  # = ASAP
@@ -50,18 +50,18 @@
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
         cls.validate_targets(values)
         cls.validate_observers(values)
         return values
 
     @staticmethod
-    def validate_targets(values: dict):
+    def validate_targets(values: dict) -> None:
         target_ids = []
         custom_ids = []
-        for _config in values["target_configs"]:
+        for _config in values.get("target_configs"):
             for _id in _config.target_IDs:
                 target_ids.append(_id)
                 Target(id=_id)
                 # ⤷ this can raise exception for non-existing targets
             if _config.custom_IDs is not None:
                 custom_ids = custom_ids + _config.custom_IDs[: len(_config.target_IDs)]
             else:
@@ -70,17 +70,17 @@
             raise ValueError("Target-ID used more than once in Experiment!")
         if len(target_ids) > len(set(custom_ids)):
             raise ValueError(
                 "Custom Target-ID are faulty (some form of id-collisions)!"
             )
 
     @staticmethod
-    def validate_observers(values: dict):
+    def validate_observers(values: dict) -> None:
         target_ids = []
-        for _config in values["target_configs"]:
+        for _config in values.get("target_configs"):
             for _id in _config.target_IDs:
                 target_ids.append(_id)
 
         testbed = Testbed(name="shepherd_tud_nes")
         obs_ids = []
         for _id in target_ids:
             obs_ids.append(testbed.get_observer(_id).id)
@@ -97,10 +97,11 @@
                 target_ids.append(_id)
         return target_ids
 
     def get_target_config(self, target_id: int) -> TargetConfig:
         for _config in self.target_configs:
             if target_id in _config.target_IDs:
                 return _config
+        # .. gets already caught in target_config .. but keep:
         raise ValueError(
             f"Target-ID {target_id} was not found in Experiment '{self.name}'"
         )
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/experiment/observer_features.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/experiment/observer_features.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,39 +13,38 @@
 
 
 class PowerTracing(ShpModel, title="Config for Power-Tracing"):
     """Configuration for recording the Power-Consumption of the Target Nodes
     TODO: postprocessing not implemented ATM
     """
 
-    # initial recording
-    voltage: bool = True
-    current: bool = True
-
     intermediate_voltage: bool = False
-    # ⤷ buffer capacitor instead of output (good for V_out = const)
-    # TODO: also switch current to buffer? seems reasonable
+    # ⤷ record buffer capacitor instead of output (good for V_out = const)
+    # TODO: also switch current to buffer-cap? seems reasonable
 
     # time
     delay: conint(ge=0) = 0
     duration: Optional[conint(ge=0)] = None  # will be max
 
     # post-processing
     calculate_power: bool = False
     samplerate: conint(ge=10, le=100_000) = 100_000  # down-sample
     discard_current: bool = False
     discard_voltage: bool = False
+    # ⤷ reduce file-size by omitting current / voltage
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
-        discard_all = values["discard_current"] and values["discard_voltage"]
-        if not values["calculate_power"] and discard_all:
+        discard_all = values.get("discard_current") and values.get("discard_voltage")
+        if not values.get("calculate_power") and discard_all:
             raise ValueError(
                 "Error in config -> tracing enabled, but output gets discarded"
             )
+        if values.get("calculate_power"):
+            raise ValueError("postprocessing not implemented ATM")
         return values
 
 
 class GpioTracing(ShpModel, title="Config for GPIO-Tracing"):
     """Configuration for recording the GPIO-Output of the Target Nodes
     TODO: postprocessing not implemented ATM
     """
@@ -57,21 +56,22 @@
     # ⤷ TODO: list of GPIO to build mask, one of both should be internal
 
     # time
     delay: conint(ge=0) = 0  # seconds
     duration: Optional[conint(ge=0)] = None  # = max
 
     # post-processing,
-    uart_decode: bool = False
+    uart_decode: bool = False  # todo: is currently done online by system-service
     uart_pin: GPIO = GPIO(name="GPIO8")
     uart_baudrate: conint(ge=2_400, le=921_600) = 115_200
+    # TODO: add a "discard_gpio" (if only uart is wanted)
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
-        if values["mask"] == 0:
+        if values.get("mask") == 0:
             raise ValueError("Error in config -> tracing enabled but mask is 0")
         return values
 
 
 class GpioLevel(str, Enum):
     low = "L"
     high = "H"
@@ -83,40 +83,41 @@
 
     delay: PositiveFloat
     # ⤷ from start_time
     # ⤷ resolution 10 us (guaranteed, but finer steps are possible)
     gpio: GPIO
     level: GpioLevel
     period: confloat(ge=10e-6) = 1
+    # ⤷ time base of periodicity in s
     count: conint(ge=1, le=4096) = 1
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
-        if not values["gpio"].user_controllable():
+        if not values.get("gpio").user_controllable():
             raise ValueError(
-                f"GPIO '{values['gpio'].name}' in actuation-event not controllable by user"
+                f"GPIO '{values.get('gpio').name}' in actuation-event not controllable by user"
             )
         return values
 
-    def get_events(self):
+    def get_events(self) -> np.ndarray:
         stop = self.delay + self.count * self.period
         timings = np.arange(self.delay, stop, self.period)
         return timings
 
 
 class GpioActuation(ShpModel, title="Config for GPIO-Actuation"):
     """Configuration for a GPIO-Actuation-Sequence
     TODO: not implemented ATM:
         - decide if pru control sys-gpio or
         - reverses pru-gpio (preferred if possible)
     """
 
     events: conlist(item_type=GpioEvent, min_items=1, max_items=1024)
 
-    def get_gpios(self):
+    def get_gpios(self) -> set:
         return {_ev.gpio for _ev in self.events}
 
 
 class SystemLogging(ShpModel, title="Config for System-Logging"):
     """Configuration for recording Debug-Output of the Observers System-Services"""
 
     dmesg: bool = True
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/experiment/target_config.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/experiment/target_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from typing import Optional
 
 from pydantic import conint
 from pydantic import conlist
 from pydantic import root_validator
 
+from ..base.content import IdInt
 from ..base.shepherd import ShpModel
 from ..content.energy_environment import EnergyEnvironment
 from ..content.firmware import Firmware
 from ..content.virtual_source import VirtualSource
+from ..testbed.target import IdInt16
 from ..testbed.target import Target
-from ..testbed.target import id_int16
 from .observer_features import GpioActuation
 from .observer_features import GpioTracing
 from .observer_features import PowerTracing
 
 
 class TargetConfig(ShpModel, title="Target Config"):
     """Configuration for Target Nodes (DuT)"""
 
-    target_IDs: conlist(item_type=id_int16, min_items=1, max_items=64)
-    custom_IDs: Optional[conlist(item_type=id_int16, min_items=1, max_items=64)]
+    target_IDs: conlist(item_type=IdInt, min_items=1, max_items=64)
+    custom_IDs: Optional[conlist(item_type=IdInt16, min_items=1, max_items=64)]
     # ⤷ will replace 'const uint16_t SHEPHERD_NODE_ID' in firmware
 
     energy_env: EnergyEnvironment  # alias: input
     virtual_source: VirtualSource = VirtualSource(name="neutral")
     target_delays: Optional[conlist(item_type=conint(ge=0), min_items=1, max_items=64)]
     # ⤷ individual starting times -> allows to use the same environment
 
@@ -32,53 +33,48 @@
 
     power_tracing: Optional[PowerTracing]
     gpio_tracing: Optional[GpioTracing]
     gpio_actuation: Optional[GpioActuation]
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
-        if not values["energy_env"].valid:
+        if not values.get("energy_env").valid:
             raise ValueError(
                 f"EnergyEnv '{values['energy_env'].name}' for target must be valid"
             )
-        for _id in values["target_IDs"]:
+        for _id in values.get("target_IDs"):
             target = Target(id=_id)
-            has_fw1 = values["firmware1"] is not None
-            has_mcu1 = target.mcu1 is not None
-            if has_fw1 and has_mcu1 and values["firmware1"].mcu.id != target.mcu1.id:
-                raise ValueError(
-                    f"Firmware1 for MCU of Target-ID '{target.id}' "
-                    f"(={values['firmware1'].mcu.name}) "
-                    f"is incompatible (={target.mcu1.name})"
-                )
-
-            has_fw2 = values["firmware2"] is not None
-            has_mcu2 = target.mcu2 is not None
-            if not has_fw2 and has_mcu2:
-                fw_def = Firmware(name=target.mcu2.fw_name_default)
-                # ⤷ this will raise if default is faulty
-                if target.mcu2.id != fw_def.mcu.id:
+            for mcu_num in [1, 2]:
+                val_fw = values.get(f"firmware{mcu_num}")
+                has_fw = val_fw is not None
+                tgt_mcu = target[f"mcu{mcu_num}"]
+                has_mcu = tgt_mcu is not None
+                if not has_fw and has_mcu:
+                    fw_def = Firmware(name=tgt_mcu.fw_name_default)
+                    # ⤷ this will raise if default is faulty
+                    if tgt_mcu.id != fw_def.mcu.id:
+                        raise ValueError(
+                            f"Default-Firmware for MCU{mcu_num} of Target-ID '{target.id}' "
+                            f"(={fw_def.mcu.name}) "
+                            f"is incompatible (={tgt_mcu.name})"
+                        )
+                if has_fw and has_mcu and val_fw.mcu.id != tgt_mcu.id:
                     raise ValueError(
-                        f"Default-Firmware for MCU2 of Target-ID '{target.id}' "
-                        f"(={fw_def.mcu.name}) "
-                        f"is incompatible (={target.mcu2.name})"
+                        f"Firmware{mcu_num} for MCU of Target-ID '{target.id}' "
+                        f"(={val_fw.mcu.name}) "
+                        f"is incompatible (={tgt_mcu.name})"
                     )
 
-            if has_fw2 and has_mcu2 and values["firmware2"].mcu.id != target.mcu2.id:
-                raise ValueError(
-                    f"Firmware2 for MCU of Target-ID '{target.id}' "
-                    f"(={values['firmware2'].mcu.name}) "
-                    f"is incompatible (={target.mcu2.name})"
-                )
-        c_ids = values["custom_IDs"]
-        if c_ids is not None and (len(set(c_ids)) < len(set(values["target_IDs"]))):
+        c_ids = values.get("custom_IDs")
+        t_ids = values.get("target_IDs")
+        if c_ids is not None and (len(set(c_ids)) < len(set(t_ids))):
             raise ValueError(
                 f"Provided custom IDs {c_ids} not enough "
-                f"to cover target range {values['target_IDs']}"
+                f"to cover target range {t_ids}"
             )
         # TODO: if custom ids present, firmware must be ELF
         return values
 
-    def get_custom_id(self, target_id: int):
-        if target_id in self.target_IDs:
+    def get_custom_id(self, target_id: int) -> Optional[int]:
+        if self.custom_IDs is not None and target_id in self.target_IDs:
             return self.custom_IDs[self.target_IDs.index(target_id)]
         return None
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/model_virtualSourceDoc.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/doc_virtual_source.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/task/emulation.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/task/emulation.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,99 +1,126 @@
 import copy
 from datetime import datetime
 from datetime import timedelta
 from enum import Enum
 from pathlib import Path
 from typing import Optional
+from typing import Union
 
 from pydantic import confloat
 from pydantic import root_validator
 from pydantic import validate_arguments
 
 from shepherd_core.data_models.testbed import Testbed
 
+from ..base.content import IdInt
 from ..base.shepherd import ShpModel
 from ..content.virtual_source import VirtualSource
 from ..experiment.experiment import Experiment
 from ..experiment.observer_features import GpioActuation
 from ..experiment.observer_features import GpioTracing
 from ..experiment.observer_features import PowerTracing
 from ..experiment.observer_features import SystemLogging
 from ..testbed.cape import TargetPort
 
 
 class Compression(str, Enum):
     lzf = "lzf"  # not native hdf5
     gzip1 = 1  # higher compr & load
+    gzip = 1
+    default = 1
+    null = None
 
 
-compressions_allowed: list = [None, "lzf", 1]  # TODO: is it still needed?
+compressions_allowed: list = [None, "lzf", 1]
+c_translate = {"lzf": "lzf", "1": 1, "None": None, None: None}
 
 
 class EmulationTask(ShpModel):
     """Configuration for the Observer in Emulation-Mode"""
 
     # General config
     input_path: Path
+    # ⤷ hdf5 file containing harvesting data
     output_path: Optional[Path]
-    # ⤷ output_path:
+    # ⤷ dir- or file-path for storing the recorded data:
     #   - providing a directory -> file is named emu_timestamp.h5
     #   - for a complete path the filename is not changed except it exists and
     #     overwrite is disabled -> emu#num.h5
+    # TODO: should the path be mandatory?
     force_overwrite: bool = False
-    output_compression: Optional[Compression] = Compression.lzf
+    # ⤷ Overwrite existing file
+    output_compression: Optional[Compression] = Compression.default
     # ⤷ should be 1 (level 1 gzip), lzf, or None (order of recommendation)
 
-    time_start: Optional[datetime] = None  # = ASAP
-    duration: Optional[timedelta] = None  # = till EOF
+    time_start: Optional[datetime] = None
+    # timestamp or unix epoch time, None = ASAP
+    duration: Optional[timedelta] = None
+    # ⤷ Duration of recording in seconds, None = till EOF
+    abort_on_error: bool = False
 
     # emulation-specific
     use_cal_default: bool = False
-    # ⤷ do not load calibration from EEPROM
+    # ⤷ Use default calibration values, skip loading from EEPROM
 
     enable_io: bool = False  # TODO: direction of pins!
-    # ⤷ pre-req for sampling gpio
+    # ⤷ Switch the GPIO level converter to targets on/off
+    #   pre-req for sampling gpio,
     io_port: TargetPort = TargetPort.A
-    # ⤷ either Port A or B
+    # ⤷ Either Port A or B that gets connected to IO
     pwr_port: TargetPort = TargetPort.A
-    # ⤷ that one will be current monitored (main), the other is aux
-    voltage_aux: confloat(ge=0, le=5) = 0
+    # ⤷ chosen port will be current-monitored (main, connected to virtual Source),
+    #   the other port is aux
+    voltage_aux: Union[confloat(ge=0, le=4.5), str] = 0
     # ⤷ aux_voltage options:
-    #   - None to disable (0 V),
-    #   - 0-4.5 for specific const Voltage,
-    #   - "mid" will output intermediate voltage (vsource storage cap),
-    #   - true or "main" to mirror main target voltage
+    #   - 0-4.5 for specific const Voltage (0 V = disabled),
+    #   - "buffer" will output intermediate voltage (storage cap of vsource),
+    #   - "main" will mirror main target voltage
 
     # sub-elements, could be partly moved to emulation
     virtual_source: VirtualSource = VirtualSource(name="neutral")  # {"name": "neutral"}
+    # ⤷ Use the desired setting for the virtual source,
+    #   provide parameters or name like BQ25570
 
-    power_tracing: Optional[PowerTracing]
-    gpio_tracing: Optional[GpioTracing]
-    gpio_actuation: Optional[GpioActuation]
-    sys_logging: Optional[SystemLogging]
+    power_tracing: Optional[PowerTracing] = PowerTracing()
+    gpio_tracing: Optional[GpioTracing] = GpioTracing()
+    gpio_actuation: Optional[GpioActuation] = None
+    sys_logging: Optional[SystemLogging] = SystemLogging()
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
         # TODO: limit paths
-        has_start = values["time_start"] is not None
-        if has_start and values["time_start"] < datetime.utcnow():
+        has_start = values.get("time_start") is not None
+        if has_start and values.get("time_start") < datetime.utcnow():
             raise ValueError("Start-Time for Emulation can't be in the past.")
+        if isinstance(values.get("voltage_aux"), str) and values.get(
+            "voltage_aux"
+        ) not in [
+            "main",
+            "buffer",
+        ]:
+            raise ValueError(
+                "Voltage Aux must be in float (0 - 4.5) or string 'main' / 'mid'."
+            )
+        if values.get("gpio_actuation") is not None:
+            raise ValueError("GPIO Actuation not yet implemented!")
         return values
 
     @classmethod
     @validate_arguments
-    def from_xp(cls, xp: Experiment, tb: Testbed, tgt_id: int, root_path: Path):
+    def from_xp(cls, xp: Experiment, tb: Testbed, tgt_id: IdInt, root_path: Path):
         obs = tb.get_observer(tgt_id)
         tgt_cfg = xp.get_target_config(tgt_id)
 
         return cls(
             input_path=tb.data_on_observer / tgt_cfg.energy_env.data_path,
             output_path=root_path / f"emu_{obs.name}.h5",
             time_start=copy.copy(xp.time_start),
             duration=xp.duration,
+            abort_on_error=xp.abort_on_error,
             enable_io=(tgt_cfg.gpio_tracing is not None)
             or (tgt_cfg.gpio_actuation is not None),
             io_port=obs.get_target_port(tgt_id),
             pwr_port=obs.get_target_port(tgt_id),
             virtual_source=tgt_cfg.virtual_source,
             power_tracing=tgt_cfg.power_tracing,
             gpio_tracing=tgt_cfg.gpio_tracing,
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/task/firmware_mod.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/task/firmware_mod.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,65 @@
 import copy
 from pathlib import Path
+from typing import Optional
 from typing import Union
 
 from pydantic import constr
 from pydantic import root_validator
 from pydantic import validate_arguments
 
 from ...logger import logger
+from ..base.content import IdInt
 from ..base.shepherd import ShpModel
 from ..content.firmware import FirmwareDType
 from ..experiment.experiment import Experiment
-from ..testbed.target import id_int16
+from ..testbed import Testbed
+from ..testbed.target import IdInt16
+from ..testbed.target import MCUPort
 
 
 class FirmwareModTask(ShpModel):
     """Config for Task that adds the custom ID to the firmware & stores it into a file"""
 
     data: Union[constr(min_length=3, max_length=1_000_000), Path]
     data_type: FirmwareDType
-    custom_id: id_int16
+    custom_id: Optional[IdInt16]
     firmware_file: Path
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
-        if values["data_type"] in [FirmwareDType.base64_hex, FirmwareDType.path_hex]:
+        if values.get("data_type") in [
+            FirmwareDType.base64_hex,
+            FirmwareDType.path_hex,
+        ]:
             logger.warning(
                 "Firmware is scheduled to get custom-ID but is not in elf-format"
             )
         return values
 
     @classmethod
     @validate_arguments
-    def from_xp(cls, xp: Experiment, tgt_id: int, prog_port: int, fw_path: Path):
+    def from_xp(
+        cls,
+        xp: Experiment,
+        tb: Testbed,
+        tgt_id: IdInt,
+        mcu_port: MCUPort,
+        fw_path: Path,
+    ):
         tgt_cfg = xp.get_target_config(tgt_id)
 
-        fw = tgt_cfg.firmware1 if prog_port == 1 else tgt_cfg.firmware2
-        if (fw is None) or (tgt_cfg.get_custom_id(tgt_id) is None):
+        fw = tgt_cfg.firmware1 if mcu_port == 1 else tgt_cfg.firmware2
+        if fw is None:
             return None
 
+        fw_id = tgt_cfg.get_custom_id(tgt_id)
+        if fw_id is None:
+            obs = tb.get_observer(tgt_id)
+            fw_id = obs.get_target(tgt_id).fw_id
+
         return cls(
             data=fw.data,
             data_type=fw.data_type,
-            custom_id=tgt_cfg.get_custom_id(tgt_id),
+            custom_id=fw_id,
             firmware_file=copy.copy(fw_path),
         )
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/task/observer_tasks.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/task/observer_tasks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from datetime import datetime
 from pathlib import Path
 from typing import Optional
 
 from pydantic import EmailStr
 from pydantic import validate_arguments
 
-from ..base.content import id_int
-from ..base.content import name_str
+from ..base.content import IdInt
+from ..base.content import NameStr
 from ..base.shepherd import ShpModel
 from ..experiment.experiment import Experiment
 from ..testbed.testbed import Testbed
 from .emulation import EmulationTask
 from .firmware_mod import FirmwareModTask
-from .programmer import ProgrammerTask
+from .programming import ProgrammingTask
 
 
 class ObserverTasks(ShpModel):
     """Collection of tasks for selected observer included in experiment"""
 
-    observer: name_str
-    owner_id: id_int
+    observer: NameStr
+    owner_id: IdInt
 
     # PRE PROCESS
     time_prep: datetime
     root_path: Path
     abort_on_error: bool
 
     # fw mod, store as hex-file and program
     fw1_mod: Optional[FirmwareModTask]
     fw2_mod: Optional[FirmwareModTask]
-    fw1_prog: Optional[ProgrammerTask]
-    fw2_prog: Optional[ProgrammerTask]
+    fw1_prog: Optional[ProgrammingTask]
+    fw2_prog: Optional[ProgrammingTask]
 
     # MAIN PROCESS
     emulation: Optional[EmulationTask]
 
     # POST PROCESS
     email: Optional[EmailStr]
 
@@ -42,15 +42,15 @@
     #  - delete firmwares
     #  - decode uart
     #  - downsample
     #  - zip it
 
     @classmethod
     @validate_arguments
-    def from_xp(cls, xp: Experiment, tb: Testbed, tgt_id: int):
+    def from_xp(cls, xp: Experiment, tb: Testbed, tgt_id: IdInt):
         if not tb.shared_storage:
             raise ValueError("Implementation currently relies on shared storage!")
 
         obs = tb.get_observer(tgt_id)
         xp_dir = "experiment/" + xp.time_start.strftime("%Y-%m-%d_%H:%M:%S")
         root_path = tb.data_on_observer / xp_dir
 
@@ -58,14 +58,14 @@
 
         return cls(
             observer=obs.name,
             owner_id=xp.owner_id,
             time_prep=xp.time_start - tb.prep_duration,
             root_path=root_path,
             abort_on_error=xp.abort_on_error,
-            fw1_mod=FirmwareModTask.from_xp(xp, tgt_id, 1, fw_paths[0]),
-            fw2_mod=FirmwareModTask.from_xp(xp, tgt_id, 2, fw_paths[1]),
-            fw1_prog=ProgrammerTask.from_xp(xp, tb, tgt_id, 1, fw_paths[0]),
-            fw2_prog=ProgrammerTask.from_xp(xp, tb, tgt_id, 2, fw_paths[1]),
+            fw1_mod=FirmwareModTask.from_xp(xp, tb, tgt_id, 1, fw_paths[0]),
+            fw2_mod=FirmwareModTask.from_xp(xp, tb, tgt_id, 2, fw_paths[1]),
+            fw1_prog=ProgrammingTask.from_xp(xp, tb, tgt_id, 1, fw_paths[0]),
+            fw2_prog=ProgrammingTask.from_xp(xp, tb, tgt_id, 2, fw_paths[1]),
             emulation=EmulationTask.from_xp(xp, tb, tgt_id, root_path),
             email=xp.email_results,
         )
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/task/programmer.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/task/programming.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,51 +2,63 @@
 from pathlib import Path
 
 from pydantic import confloat
 from pydantic import conint
 from pydantic import root_validator
 from pydantic import validate_arguments
 
+from ..base.content import IdInt
+from ..base.content import SafeStr
 from ..base.shepherd import ShpModel
 from ..experiment.experiment import Experiment
 from ..testbed.cape import TargetPort
 from ..testbed.mcu import ProgrammerProtocol
+from ..testbed.target import MCUPort
 from ..testbed.testbed import Testbed
 
 
-class ProgrammerTask(ShpModel):
+class ProgrammingTask(ShpModel):
     """Config for Task programming the target selected"""
 
     firmware_file: Path
-    sel_a: bool = True
+    target_port: TargetPort = TargetPort.A
+    mcu_port: MCUPort = 1
+    mcu_type: SafeStr
+    # ⤷ for later
     voltage: confloat(ge=1, lt=5) = 3
     datarate: conint(gt=0, le=1_000_000) = 500_000
     protocol: ProgrammerProtocol
-    prog1: bool = True
+
     simulate: bool = False
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
-        if values["firmware_file"].suffix.lower() != ".hex":
+        if values.get("firmware_file").suffix.lower() != ".hex":
             ValueError(f"Firmware is not intel-.hex ('{values['firmware_file']}')")
         return values
 
     @classmethod
     @validate_arguments
     def from_xp(
-        cls, xp: Experiment, tb: Testbed, tgt_id: int, prog_port: int, fw_path: Path
+        cls,
+        xp: Experiment,
+        tb: Testbed,
+        tgt_id: IdInt,
+        mcu_port: MCUPort,
+        fw_path: Path,
     ):
         obs = tb.get_observer(tgt_id)
         tgt_cfg = xp.get_target_config(tgt_id)
 
-        fw = tgt_cfg.firmware1 if prog_port == 1 else tgt_cfg.firmware2
+        fw = tgt_cfg.firmware1 if mcu_port == 1 else tgt_cfg.firmware2
         if fw is None:
             return None
 
         return cls(
             firmware_file=copy.copy(fw_path),
-            sel_a=obs.get_target_port(tgt_id) == TargetPort.A,
+            target_port=obs.get_target_port(tgt_id),
+            mcu_port=mcu_port,
+            mcu_type=fw.mcu.name,
             voltage=fw.mcu.prog_voltage,
             datarate=fw.mcu.prog_datarate,
             protocol=fw.mcu.prog_protocol,
-            prog1=prog_port == 1,
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/task/testbed_tasks.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/task/testbed_tasks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+from typing import Optional
+
 from pydantic import conlist
 from pydantic import validate_arguments
 
-from ..base.content import name_str
+from ..base.content import NameStr
 from ..base.shepherd import ShpModel
 from ..experiment.experiment import Experiment
 from ..testbed.testbed import Testbed
 from .observer_tasks import ObserverTasks
 
 
 class TestbedTasks(ShpModel):
     """Collection of tasks for all observers included in experiment"""
 
-    name: name_str
+    name: NameStr
     observer_tasks: conlist(item_type=ObserverTasks, min_items=1, max_items=64)
 
     @classmethod
     @validate_arguments
-    def from_xp(cls, xp: Experiment):
-        tb = Testbed(name="shepherd_tud_nes")  # also as argument?
+    def from_xp(cls, xp: Experiment, tb: Optional[Testbed] = None):
+        if tb is None:
+            # TODO: just for testing OK
+            tb = Testbed(name="shepherd_tud_nes")
         tgt_ids = xp.get_target_ids()
         obs_tasks = [ObserverTasks.from_xp(xp, tb, _id) for _id in tgt_ids]
         return cls(name=xp.name, observer_tasks=obs_tasks)
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/testbed/__init__.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/testbed/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from .cape import Cape
 from .cape import TargetPort
 from .gpio import GPIO
 from .gpio import Direction
 from .mcu import MCU
 from .mcu import ProgrammerProtocol
+from .observer import MACStr
 from .observer import Observer
-from .observer import mac_str
+from .target import IdInt16
 from .target import Target
-from .target import id_int16
 from .testbed import Testbed
 
 # these models import externally from: /base
 
 __all__ = [
     "Testbed",
     "Observer",
@@ -20,10 +20,10 @@
     "MCU",
     "GPIO",
     # enums
     "ProgrammerProtocol",
     "Direction",
     "TargetPort",
     # custom types
-    "id_int16",
-    "mac_str",
+    "IdInt16",
+    "MACStr",
 ]
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/testbed/cape.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/testbed/target.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,62 @@
-from datetime import date
 from datetime import datetime
-from enum import Enum
 from pathlib import Path
 from typing import Optional
 from typing import Union
 
 from pydantic import Field
+from pydantic import conint
 from pydantic import root_validator
 
-from ..base.content import id_int
-from ..base.content import name_str
-from ..base.content import safe_str
+from ..base.content import IdInt
+from ..base.content import NameStr
+from ..base.content import SafeStr
 from ..base.fixture import Fixtures
 from ..base.shepherd import ShpModel
+from .mcu import MCU
 
-fixture_path = Path(__file__).resolve().with_name("cape_fixture.yaml")
-fixtures = Fixtures(fixture_path, "cape")
+fixture_path = Path(__file__).resolve().with_name("target_fixture.yaml")
+fixtures = Fixtures(fixture_path, "target")
 
+IdInt16 = conint(ge=0, lt=2**16)
 
-class TargetPort(str, Enum):
-    A = "A"
-    B = "B"
+MCUPort = conint(ge=1, le=2)
 
 
-class Cape(ShpModel, title="Shepherd-Cape"):
+class Target(ShpModel, title="Target Node (DuT)"):
     """meta-data representation of a testbed-component (physical object)"""
 
-    id: id_int  # noqa: A003
-    name: name_str
-    version: name_str
-    description: safe_str
-    comment: Optional[safe_str] = None
-    # TODO: wake_interval, calibration
+    id: IdInt  # noqa: A003
+    name: NameStr
+    version: NameStr
+    description: SafeStr
 
-    created: Union[date, datetime] = Field(default_factory=datetime.now)
-    calibrated: Union[date, datetime, None] = None
+    comment: Optional[SafeStr] = None
+
+    created: datetime = Field(default_factory=datetime.now)
+
+    fw_id: Optional[IdInt16]
+    mcu1: Union[MCU, NameStr]
+    mcu2: Union[MCU, NameStr, None] = None
+    #
+
+    # TODO programming pins per mcu should be here (or better in Cape)
 
     def __str__(self):
         return self.name
 
     @root_validator(pre=True)
     def from_fixture(cls, values: dict) -> dict:
         values = fixtures.lookup(values)
-        values, chain = fixtures.inheritance(values)
+        values, _ = fixtures.inheritance(values)
+        return values
+
+    @root_validator(pre=False)
+    def post_correction(cls, values: dict) -> dict:
+        if isinstance(values.get("mcu1"), str):
+            values["mcu1"] = MCU(name=values["mcu1"])
+            # ⤷ this will raise if default is faulty
+        if isinstance(values.get("mcu2"), str):
+            values["mcu2"] = MCU(name=values["mcu2"])
+        if values.get("fw_id") is None:
+            values["fw_id"] = values.get("id") % 2**16
         return values
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/testbed/cape_fixture.yaml` & `shepherd_core-2023.5.6/shepherd_core/data_models/testbed/cape_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/testbed/gpio.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/testbed/gpio.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from pathlib import Path
 from typing import Optional
 
 from pydantic import conint
 from pydantic import constr
 from pydantic import root_validator
 
-from ..base.content import id_int
-from ..base.content import name_str
-from ..base.content import safe_str
+from ..base.content import IdInt
+from ..base.content import NameStr
+from ..base.content import SafeStr
 from ..base.fixture import Fixtures
 from ..base.shepherd import ShpModel
 
 fixture_path = Path(__file__).resolve().with_name("gpio_fixture.yaml")
 fixtures = Fixtures(fixture_path, "gpio")
 
 
@@ -24,18 +24,18 @@
     Bidirectional = "IO"
     IO = "IO"
 
 
 class GPIO(ShpModel, title="GPIO of Observer Node"):
     """meta-data representation of a testbed-component"""
 
-    id: id_int  # noqa: A003
-    name: name_str
-    description: Optional[safe_str] = None
-    comment: Optional[safe_str] = None
+    id: IdInt  # noqa: A003
+    name: NameStr
+    description: Optional[SafeStr] = None
+    comment: Optional[SafeStr] = None
 
     direction: Direction = Direction.Input
     dir_switch: Optional[constr(max_length=32)]
 
     reg_pru: Optional[constr(max_length=10)] = None
     pin_pru: Optional[constr(max_length=10)] = None
     reg_sys: Optional[conint(ge=0)] = None
@@ -43,22 +43,22 @@
 
     def __str__(self):
         return self.name
 
     @root_validator(pre=True)
     def from_fixture(cls, values: dict) -> dict:
         values = fixtures.lookup(values)
-        values, chain = fixtures.inheritance(values)
+        values, _ = fixtures.inheritance(values)
         return values
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
         # ensure that either pru or sys is used, otherwise instance is considered faulty
-        no_pru = (values["reg_pru"] is None) or (values["pin_pru"] is None)
-        no_sys = (values["reg_sys"] is None) or (values["pin_sys"] is None)
+        no_pru = (values.get("reg_pru") is None) or (values.get("pin_pru") is None)
+        no_sys = (values.get("reg_sys") is None) or (values.get("pin_sys") is None)
         if no_pru and no_sys:
             raise ValueError(
                 f"GPIO-Instance is faulty -> it needs to use pru or sys, content: {values}"
             )
         return values
 
     def user_controllable(self) -> bool:
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/testbed/gpio_fixture.yaml` & `shepherd_core-2023.5.6/shepherd_core/data_models/testbed/gpio_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/testbed/mcu.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/testbed/mcu.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from pathlib import Path
 from typing import Optional
 
 from pydantic import confloat
 from pydantic import conint
 from pydantic import root_validator
 
-from ..base.content import id_int
-from ..base.content import name_str
-from ..base.content import safe_str
+from ..base.content import IdInt
+from ..base.content import NameStr
+from ..base.content import SafeStr
 from ..base.fixture import Fixtures
 from ..base.shepherd import ShpModel
 
 fixture_path = Path(__file__).resolve().with_name("mcu_fixture.yaml")
 fixtures = Fixtures(fixture_path, "mcu")
 
 
@@ -23,29 +23,29 @@
     jtag = "JTAG"
     uart = "UART"
 
 
 class MCU(ShpModel, title="Microcontroller of the Target Node"):
     """meta-data representation of a testbed-component (physical object)"""
 
-    id: id_int  # noqa: A003
-    name: name_str
-    description: safe_str
-    comment: Optional[safe_str] = None
+    id: IdInt  # noqa: A003
+    name: NameStr
+    description: SafeStr
+    comment: Optional[SafeStr] = None
 
-    platform: name_str
-    core: name_str
+    platform: NameStr
+    core: NameStr
     prog_protocol: ProgrammerProtocol
     prog_voltage: confloat(ge=1, le=5) = 3
     prog_datarate: conint(gt=0, le=1_000_000) = 500_000
 
     fw_name_default: str
     # ⤷ can't be FW-Object (circular import)
 
     def __str__(self):
         return self.name
 
     @root_validator(pre=True)
     def from_fixture(cls, values: dict) -> dict:
         values = fixtures.lookup(values)
-        values, chain = fixtures.inheritance(values)
+        values, _ = fixtures.inheritance(values)
         return values
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/testbed/observer.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/testbed/observer.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,42 +4,42 @@
 
 from pydantic import Field
 from pydantic import IPvAnyAddress
 from pydantic import confloat
 from pydantic import constr
 from pydantic import root_validator
 
-from ..base.content import id_int
-from ..base.content import name_str
-from ..base.content import safe_str
+from ..base.content import IdInt
+from ..base.content import NameStr
+from ..base.content import SafeStr
 from ..base.fixture import Fixtures
 from ..base.shepherd import ShpModel
 from .cape import Cape
 from .cape import TargetPort
 from .target import Target
 
 fixture_path = Path(__file__).resolve().with_name("observer_fixture.yaml")
 fixtures = Fixtures(fixture_path, "observer")
 
-mac_str = constr(max_length=17, regex=r"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$")
+MACStr = constr(max_length=17, regex=r"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$")
 
 
 class Observer(ShpModel, title="Shepherd-Sheep"):
     """meta-data representation of a testbed-component (physical object)"""
 
-    id: id_int  # noqa: A003
-    name: name_str
-    description: safe_str
-    comment: Optional[safe_str] = None
+    id: IdInt  # noqa: A003
+    name: NameStr
+    description: SafeStr
+    comment: Optional[SafeStr] = None
 
     ip: IPvAnyAddress
-    mac: mac_str
+    mac: MACStr
 
-    room: name_str
-    eth_port: name_str
+    room: NameStr
+    eth_port: NameStr
 
     latitude: confloat(ge=-90, le=90) = 51.026573  # cfaed
     longitude: confloat(ge=-180, le=180) = 13.723291
 
     cape: Optional[Cape]
     target_a: Optional[Target]
     target_b: Optional[Target] = None
@@ -49,30 +49,40 @@
 
     def __str__(self):
         return self.name
 
     @root_validator(pre=True)
     def from_fixture(cls, values: dict) -> dict:
         values = fixtures.lookup(values)
-        values, chain = fixtures.inheritance(values)
+        values, _ = fixtures.inheritance(values)
         return values
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
-        has_cape = values["cape"] is not None
-        has_target = (values["target_a"] is not None) or (
-            values["target_b"] is not None
+        has_cape = values.get("cape") is not None
+        has_target = (values.get("target_a") is not None) or (
+            values.get("target_b") is not None
         )
         if not has_cape and has_target:
             raise ValueError(
-                f"Observer '{values['name']}' is faulty " f"-> has targets but no cape"
+                f"Observer '{values.get('name')}' is faulty "
+                f"-> has targets but no cape"
             )
         return values
 
     def get_target_port(self, target_id: int) -> TargetPort:
         if self.target_a is not None and target_id == self.target_a.id:
             return TargetPort.A
         if self.target_b is not None and target_id == self.target_b.id:
             return TargetPort.B
         raise ValueError(
             f"Target-ID {target_id} was not found in Observer '{self.name}'"
         )
+
+    def get_target(self, target_id: int) -> Target:
+        if self.target_a is not None and target_id == self.target_a.id:
+            return self.target_a
+        if self.target_b is not None and target_id == self.target_b.id:
+            return self.target_b
+        raise ValueError(
+            f"Target-ID {target_id} was not found in Observer '{self.name}'"
+        )
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/testbed/observer_fixture.yaml` & `shepherd_core-2023.5.6/shepherd_core/data_models/testbed/observer_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/testbed/target_fixture.yaml` & `shepherd_core-2023.5.6/shepherd_core/data_models/testbed/target_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.5.5/shepherd_core/data_models/testbed/testbed.py` & `shepherd_core-2023.5.6/shepherd_core/data_models/testbed/testbed.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 from datetime import timedelta
 from pathlib import Path
 from typing import Optional
 
+from pydantic import HttpUrl
 from pydantic import conlist
 from pydantic import root_validator
 
-from ..base.content import id_int
-from ..base.content import name_str
-from ..base.content import safe_str
+from ..base.content import IdInt
+from ..base.content import NameStr
+from ..base.content import SafeStr
 from ..base.fixture import Fixtures
 from ..base.shepherd import ShpModel
 from .observer import Observer
 
 fixture_path = Path(__file__).resolve().with_name("testbed_fixture.yaml")
 fixtures = Fixtures(fixture_path, "testbed")
 
 
 class Testbed(ShpModel):
     """meta-data representation of a testbed-component (physical object)"""
 
-    id: id_int  # noqa: A003
-    name: name_str
-    description: safe_str
-    comment: Optional[safe_str] = None
+    id: IdInt  # noqa: A003
+    name: NameStr
+    description: SafeStr
+    comment: Optional[SafeStr] = None
+
+    url: Optional[HttpUrl]
 
     observers: conlist(item_type=Observer, min_items=1, max_items=64)
 
     shared_storage: bool = True
     data_on_server: Path
     data_on_observer: Path
     # ⤷ storage layout: root_path/content_type/group/owner/[object]
 
     prep_duration: timedelta = timedelta(minutes=5)
     # TODO: one BBone is currently time-keeper
 
     @root_validator(pre=True)
     def from_fixture(cls, values: dict) -> dict:
-        values = fixtures.lookup(values)
-        values, chain = fixtures.inheritance(values)
+        values = fixtures.lookup(values)  # TODO: load from url
+        values, _ = fixtures.inheritance(values)
         return values
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
         observers = []
         ips = []
         macs = []
         capes = []
         targets = []
         eth_ports = []
-        for _obs in values["observers"]:
+        for _obs in values.get("observers"):
             observers.append(_obs.id)
             ips.append(_obs.ip)
             macs.append(_obs.mac)
             if _obs.cape is not None:
                 capes.append(_obs.cape)
             if _obs.target_a is not None:
                 targets.append(_obs.target_a)
@@ -60,24 +63,27 @@
                 targets.append(_obs.target_b)
             eth_ports.append(_obs.eth_port)
         if len(observers) > len(set(observers)):
             raise ValueError("Observers used more than once in Testbed")
         if len(ips) > len(set(ips)):
             raise ValueError("Observer-IP used more than once in Testbed")
         if len(macs) > len(set(macs)):
-            raise ValueError("Observers-MAC-Addresse used more than once in Testbed")
+            raise ValueError("Observers-MAC-Address used more than once in Testbed")
         if len(capes) > len(set(capes)):
             raise ValueError("Cape used more than once in Testbed")
         if len(targets) > len(set(targets)):
             raise ValueError("Target used more than once in Testbed")
         if len(eth_ports) > len(set(eth_ports)):
             raise ValueError("Observers-Ethernet-Port used more than once in Testbed")
+
+        if not values.get("shared_storage"):
+            raise ValueError("Only shared-storage-option is implemented")
         return values
 
-    def get_observer(self, target_id: int):
+    def get_observer(self, target_id: int) -> Observer:
         for _observer in self.observers:
             has_tgt_a = _observer.target_a is not None
             if has_tgt_a and target_id == _observer.target_a.id:
                 return _observer
             has_tgt_b = _observer.target_b is not None
             if has_tgt_b and target_id == _observer.target_b.id:
                 return _observer
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/logger.py` & `shepherd_core-2023.5.6/shepherd_core/logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 import logging
 
 import chromalog
+from pydantic import validate_arguments
 
 chromalog.basicConfig(format="%(message)s")
 logger = logging.getLogger("SHPCore")
 logger.addHandler(logging.NullHandler())
 
 verbose_level: int = 2
 
 
 def get_verbose_level() -> int:
     return verbose_level
 
 
+@validate_arguments
 def set_verbose_level(verbose: int) -> None:
     global verbose_level
-    verbose_level = min(3, verbose)
+    verbose_level = min(max(verbose, 0), 3)
 
-    if verbose == 0:
+    if verbose_level == 0:
         logger.setLevel(logging.ERROR)
         logging.basicConfig(level=logging.ERROR)
-    elif verbose == 1:
+    elif verbose_level == 1:
         logger.setLevel(logging.WARNING)
-    elif verbose == 2:
+    elif verbose_level == 2:
         logger.setLevel(logging.INFO)
-    elif verbose > 2:
+    elif verbose_level > 2:
         logger.setLevel(logging.DEBUG)
 
-    if verbose < 3:
+    if verbose_level < 3:
         # reduce log-overhead when not debugging, also more user-friendly exceptions
         logging._srcfile = None
         logging.logThreads = 0
         logging.logProcesses = 0
 
-    if verbose > 2:
+    if verbose_level > 2:
         chromalog.basicConfig(format="%(name)s %(levelname)s: %(message)s")
     else:
         chromalog.basicConfig(format="%(message)s")  # reduce internals
 
 
+set_verbose_level(2)
+
 # short reminder for format-strings:
 # %s    string
 # %d    decimal
 # %f    float
 # %o    decimal as octal
 # %x    decimal as hex
 #
```

### Comparing `shepherd_core-2023.5.5/shepherd_core/writer.py` & `shepherd_core-2023.5.6/shepherd_core/writer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 """
 Writer that inherits from Reader-Baseclass
 """
 import logging
 import math
 from itertools import product
 from pathlib import Path
+from typing import Any
 from typing import Optional
 from typing import Union
 
 import h5py
 import numpy as np
 import yaml
+from pydantic import validate_arguments
 
-from .calibration import cal_default
-from .calibration import si_to_raw
+from .commons import samplerate_sps_default
+from .data_models.base.calibration import CalibrationEmulator as CalEmu
+from .data_models.base.calibration import CalibrationHarvester as CalHrv
+from .data_models.base.calibration import CalibrationSeries as CalSeries
+from .data_models.content.energy_environment import EnergyDType
+from .data_models.task import Compression
+from .data_models.task.emulation import c_translate
 from .reader import BaseReader
 
 
 def unique_path(base_path: Union[str, Path], suffix: str) -> Path:
     """finds an unused filename in case it already exists
 
     :param base_path: file-path to test
@@ -31,149 +38,143 @@
             return path
         counter += 1
 
 
 class BaseWriter(BaseReader):
     """Stores data for Shepherd in HDF5 format
 
+    Choose lossless compression filter
+     - lzf:  low to moderate compression, VERY fast, no options
+             -> 20 % cpu overhead for half the filesize
+     - gzip: good compression, moderate speed, select level from 1-9, default is 4
+             -> lower levels seem fine
+             -> _algo=number instead of "gzip" is read as compression level for gzip
+     -> comparison / benchmarks https://www.h5py.org/lzf/
+
     Args:
         file_path: (Path) Name of the HDF5 file that data will be written to
         mode: (str) Indicates if this is data from harvester or emulator
         datatype: (str) choose type: ivsample (most common), ivcurve or isc_voc
         window_samples: (int) windows size for the datatype ivcurve
         cal_data: (CalibrationData) Data is written as raw ADC
             values. We need calibration data in order to convert to physical
             units later.
         modify_existing: (bool) explicitly enable modifying existing file
             otherwise a unique name will be found
         compression: (str) use either None, lzf or "1" (gzips compression level)
         verbose: (bool) provides more info instead of just warnings / errors
     """
 
-    # choose lossless compression filter
-    # - lzf:  low to moderate compression, VERY fast, no options
-    #         -> 20 % cpu overhead for half the filesize
-    # - gzip: good compression, moderate speed, select level from 1-9, default is 4
-    #         -> lower levels seem fine
-    #         -> _algo=number instead of "gzip" is read as compression level for gzip
-    # -> comparison / benchmarks https://www.h5py.org/lzf/
     comp_default: int = 1
     mode_default: str = "harvester"
-    datatype_default: str = "ivsample"
+    datatype_default: str = EnergyDType.ivsample.name
 
     _chunk_shape: tuple = (BaseReader.samples_per_buffer,)
 
+    @validate_arguments
     def __init__(
         self,
         file_path: Path,
         mode: Optional[str] = None,
         datatype: Optional[str] = None,
         window_samples: Optional[int] = None,
-        cal_data: Optional[dict] = None,
+        cal_data: Union[CalSeries, CalEmu, CalHrv, None] = None,
+        compression: Compression = Compression.default,
         modify_existing: bool = False,
-        compression: Union[None, str, int] = "default",
+        force_overwrite: bool = False,
         verbose: Optional[bool] = True,
     ):
-        file_path = Path(file_path)
         self._modify = modify_existing
+        self._compression = c_translate[compression.value]
 
         if not hasattr(self, "_logger"):
             self._logger: logging.Logger = logging.getLogger("SHPCore.Writer")
         # -> logger gets configured in reader()
 
-        if self._modify or not file_path.exists():
-            self._file_path: Path = file_path
-            self._logger.info("Storing data to   '%s'", self._file_path)
+        if self._modify or force_overwrite or not file_path.exists():
+            self.file_path: Path = file_path
+            self._logger.info("Storing data to   '%s'", self.file_path)
+        elif file_path.exists() and not file_path.is_file():
+            raise TypeError(f"Path is not a file ({file_path})")
         else:
             base_dir = file_path.resolve().parents[0]
-            self._file_path = unique_path(base_dir / file_path.stem, file_path.suffix)
+            self.file_path = unique_path(base_dir / file_path.stem, file_path.suffix)
             self._logger.warning(
-                "File %s already exists -> " "storing under %s instead",
+                "File '%s' already exists -> " "storing under '%s' instead",
                 file_path,
-                self._file_path.name,
+                self.file_path.name,
             )
 
-        if not isinstance(mode, (str, type(None))):
-            raise TypeError(f"Can't handle type '{type(mode)}' for mode [str, None]")
         if isinstance(mode, str) and mode not in self.mode_dtype_dict:
             raise ValueError(
                 f"Can't handle mode '{mode}' " f"(choose one of {self.mode_dtype_dict})"
             )
-        if not isinstance(window_samples, (int, type(None))):
-            raise TypeError(
-                f"Can't handle type '{type(window_samples)}' for window_samples [int, None]"
-            )
-        if not isinstance(cal_data, (dict, type(None))):
-            raise TypeError(
-                f"Can't handle type '{type(cal_data)}' for cal_data [dict, None]"
-            )
 
-        if not isinstance(datatype, (str, type(None))):
-            raise TypeError(
-                f"Can't handle type '{type(datatype)}' for datatype [str, None]"
-            )
-
-        _dtypes = self.mode_dtype_dict[self.mode_default if (mode is None) else mode]
+        _dtypes = self.mode_dtype_dict[mode if mode else self.mode_default]
         if isinstance(datatype, str) and datatype not in _dtypes:
             raise ValueError(
                 f"Can't handle value '{datatype}' of datatype "
                 f"(choose one of {_dtypes})"
             )
 
         if self._modify:
             self._mode = mode
-            self._cal = (
-                cal_data if isinstance(cal_data, dict) else cal_default
-            )  # TODO: switch to pydantic
             self._datatype = datatype
             self._window_samples = window_samples
         else:
             self._mode = mode if isinstance(mode, str) else self.mode_default
-            self._cal = cal_data if isinstance(cal_data, dict) else cal_default
             self._datatype = (
                 datatype if isinstance(datatype, str) else self.datatype_default
             )
             self._window_samples = (
                 window_samples if isinstance(window_samples, int) else 0
             )
 
-        if compression in [None, "lzf", 1]:  # order of recommendation
-            self._compression_algo = compression
+        if isinstance(cal_data, (CalEmu, CalHrv)):
+            self._cal = CalSeries.from_cal(cal_data)
+        elif isinstance(cal_data, CalSeries):
+            self._cal = cal_data
         else:
-            self._compression_algo = self.comp_default
+            self._cal = CalSeries()
 
         # open file
         if self._modify:
-            self.h5file = h5py.File(self._file_path, "r+")  # = rw
+            self.h5file = h5py.File(self.file_path, "r+")  # = rw
         else:
-            self.h5file = h5py.File(self._file_path, "w")  # write, truncate if exist
+            self.h5file = h5py.File(self.file_path, "w")
+            # ⤷ write, truncate if exist
             self._create_skeleton()
 
+        # show key parameters for h5-performance
+        settings = list(self.h5file.id.get_access_plist().get_cache())
+        self._logger.debug(
+            "H5Py Cache_setting=%s (_mdc, _nslots, _nbytes, _w0)", settings
+        )
+
         # Store the mode in order to allow user to differentiate harvesting vs emulation data
         if isinstance(self._mode, str) and self._mode in self.mode_dtype_dict:
             self.h5file.attrs["mode"] = self._mode
 
         if (
             isinstance(self._datatype, str)
             and self._datatype in self.mode_dtype_dict[self.get_mode()]
         ):
             self.h5file["data"].attrs["datatype"] = self._datatype
         elif not self._modify:
             self._logger.error("datatype invalid? '%s' not written", self._datatype)
 
         if isinstance(self._window_samples, int):
             self.h5file["data"].attrs["window_samples"] = self._window_samples
+        if datatype == EnergyDType.ivcurve and (self._window_samples in [None, 0]):
+            raise ValueError("Window Size argument needed for ivcurve-Datatype")
+
+        # include cal-data
+        for ds, param in product(["current", "voltage", "time"], ["gain", "offset"]):
+            self.h5file["data"][ds].attrs[param] = self._cal[ds][param]
 
-        if self._cal is not None:
-            for channel, parameter in product(
-                ["current", "voltage"], ["gain", "offset"]
-            ):
-                self.h5file["data"][channel].attrs[parameter] = self._cal[channel][
-                    parameter
-                ]
         super().__init__(file_path=None, verbose=verbose)
 
     def __enter__(self):
         super().__enter__()
         return self
 
     def __exit__(self, *exc):  # type: ignore
@@ -197,87 +198,88 @@
         actual IV samples recorded either from the harvester (during recording)
         or the target (during emulation). Any log messages, that can be used to
         store relevant events or tag some parts of the recorded data.
 
         """
         # Store voltage and current samples in the data group,
         # both are stored as 4 Byte unsigned int
-        gp_data = self.h5file.create_group("data")
+        grp_data = self.h5file.create_group("data")
         # the size of window_samples-attribute in harvest-data indicates ivcurves as input
         # -> emulator uses virtual-harvester, field will be adjusted by .embed_config()
-        gp_data.attrs["window_samples"] = 0
+        grp_data.attrs["window_samples"] = 0
 
-        gp_data.create_dataset(
+        grp_data.create_dataset(
             "time",
             (0,),
             dtype="u8",
             maxshape=(None,),
             chunks=self._chunk_shape,
-            compression=self._compression_algo,
+            compression=self._compression,
         )
-        gp_data["time"].attrs["unit"] = "ns"
-        gp_data["time"].attrs["description"] = "system time [ns]"
+        grp_data["time"].attrs["unit"] = "s"
+        grp_data["time"].attrs[
+            "description"
+        ] = "system time [s] = value * gain + (offset)"
 
-        gp_data.create_dataset(
+        grp_data.create_dataset(
             "current",
             (0,),
             dtype="u4",
             maxshape=(None,),
             chunks=self._chunk_shape,
-            compression=self._compression_algo,
+            compression=self._compression,
         )
-        gp_data["current"].attrs["unit"] = "A"
-        gp_data["current"].attrs["description"] = "current [A] = value * gain + offset"
+        grp_data["current"].attrs["unit"] = "A"
+        grp_data["current"].attrs["description"] = "current [A] = value * gain + offset"
 
-        gp_data.create_dataset(
+        grp_data.create_dataset(
             "voltage",
             (0,),
             dtype="u4",
             maxshape=(None,),
             chunks=self._chunk_shape,
-            compression=self._compression_algo,
+            compression=self._compression,
         )
-        gp_data["voltage"].attrs["unit"] = "V"
-        gp_data["voltage"].attrs["description"] = "voltage [V] = value * gain + offset"
+        grp_data["voltage"].attrs["unit"] = "V"
+        grp_data["voltage"].attrs["description"] = "voltage [V] = value * gain + offset"
 
     def append_iv_data_raw(
         self,
-        timestamp_ns: Union[np.ndarray, float, int],
+        timestamp: Union[np.ndarray, float, int],
         voltage: np.ndarray,
         current: np.ndarray,
     ) -> None:
         """Writes raw data to database
 
         Args:
-            timestamp_ns: just start of buffer or whole ndarray
+            timestamp: just start of buffer or whole ndarray
             voltage: ndarray as raw unsigned integers
             current: ndarray as raw unsigned integers
         """
         len_new = min(voltage.size, current.size)
 
-        if isinstance(timestamp_ns, float):
-            timestamp_ns = int(timestamp_ns)
-        if isinstance(timestamp_ns, int):
+        if isinstance(timestamp, float):
+            timestamp = int(timestamp)
+        if isinstance(timestamp, int):
             time_series_ns = self.sample_interval_ns * np.arange(len_new).astype("u8")
-            timestamp_ns = timestamp_ns + time_series_ns
-        if isinstance(timestamp_ns, np.ndarray):
-            len_new = min(len_new, timestamp_ns.size)
+            timestamp = timestamp + time_series_ns
+        if isinstance(timestamp, np.ndarray):
+            len_new = min(len_new, timestamp.size)
         else:
-            self._logger.error("timestamp-data was not usable")
-            return
+            raise ValueError("timestamp-data was not usable")
 
         len_old = self.ds_time.shape[0]
 
         # resize dataset
         self.ds_time.resize((len_old + len_new,))
         self.ds_voltage.resize((len_old + len_new,))
         self.ds_current.resize((len_old + len_new,))
 
         # append new data
-        self.ds_time[len_old : len_old + len_new] = timestamp_ns[:len_new]
+        self.ds_time[len_old : len_old + len_new] = timestamp[:len_new]
         self.ds_voltage[len_old : len_old + len_new] = voltage[:len_new]
         self.ds_current[len_old : len_old + len_new] = current[:len_new]
 
     def append_iv_data_si(
         self,
         timestamp: Union[np.ndarray, float],
         voltage: np.ndarray,
@@ -289,58 +291,49 @@
 
         Args:
             timestamp: python timestamp (time.time()) in seconds (si-unit)
                        -> provide start of buffer or whole ndarray
             voltage: ndarray in physical-unit V
             current: ndarray in physical-unit A
         """
-        timestamp = timestamp * 10**9
-        voltage = si_to_raw(voltage, self._cal["voltage"])
-        current = si_to_raw(current, self._cal["current"])
+        timestamp = self._cal.time.si_to_raw(timestamp)
+        voltage = self._cal.voltage.si_to_raw(voltage)
+        current = self._cal.current.si_to_raw(current)
         self.append_iv_data_raw(timestamp, voltage, current)
 
     def _align(self) -> None:
         """Align datasets with buffer-size of shepherd"""
         self._refresh_file_stats()
         n_buff = self.ds_time.size / self.samples_per_buffer
         size_new = int(math.floor(n_buff) * self.samples_per_buffer)
         if size_new < self.ds_time.size:
-            if self.samplerate_sps < 95_000:
+            if self.samplerate_sps != samplerate_sps_default:
                 self._logger.debug("skipped alignment due to altered samplerate")
                 return
             self._logger.info(
                 "aligning with buffer-size, discarding last %s entries",
                 self.ds_time.size - size_new,
             )
             self.ds_time.resize((size_new,))
             self.ds_voltage.resize((size_new,))
             self.ds_current.resize((size_new,))
 
-    def __setitem__(self, key: str, item):  # type: ignore
+    def __setitem__(self, key: str, item: Any):
         """A convenient interface to store relevant key-value data (attribute) if H5-structure"""
         return self.h5file.attrs.__setitem__(key, item)
 
-    def set_config(self, data: dict) -> None:
+    def store_config(self, data: dict) -> None:
         """Important Step to get a self-describing Output-File
-
+        TODO: use data-model?
         :param data: from virtual harvester or converter / source
         """
         self.h5file["data"].attrs["config"] = yaml.safe_dump(
             data, default_flow_style=False, sort_keys=False
         )
-        if "window_samples" in data:
-            self.set_window_samples(data["window_samples"])
-
-    def set_window_samples(self, samples: int = 0) -> None:
-        """parameter essential for ivcurves
-
-        :param samples: length of window / voltage sweep
-        """
-        self.h5file["data"].attrs["window_samples"] = samples
 
-    def set_hostname(self, name: str) -> None:
+    def store_hostname(self, name: str) -> None:
         """option to distinguish the host, target or data-source in the testbed
             -> perfect for plotting later
 
         :param name: something unique, or "artificial" in case of generated content
         """
         self.h5file.attrs["hostname"] = name
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `shepherd_core-2023.5.5/shepherd_core.egg-info/PKG-INFO` & `shepherd_core-2023.5.6/shepherd_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd-core
-Version: 2023.5.5
+Version: 2023.5.6
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-core/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
```

### Comparing `shepherd_core-2023.5.5/shepherd_core.egg-info/SOURCES.txt` & `shepherd_core-2023.5.6/shepherd_core.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 README.md
 pyproject.toml
 setup.cfg
 ./shepherd_core/__init__.py
-./shepherd_core/calibration.py
+./shepherd_core/calibration_hw_def.py
+./shepherd_core/commons.py
 ./shepherd_core/logger.py
 ./shepherd_core/reader.py
 ./shepherd_core/writer.py
 ./shepherd_core/data_models/__init__.py
-./shepherd_core/data_models/model_virtualSourceDoc.py
+./shepherd_core/data_models/doc_virtual_source.py
 ./shepherd_core/data_models/base/__init__.py
+./shepherd_core/data_models/base/cal_measurement.py
 ./shepherd_core/data_models/base/calibration.py
 ./shepherd_core/data_models/base/content.py
 ./shepherd_core/data_models/base/fixture.py
 ./shepherd_core/data_models/base/shepherd.py
 ./shepherd_core/data_models/base/wrapper.py
 ./shepherd_core/data_models/content/__init__.py
 ./shepherd_core/data_models/content/energy_environment.py
@@ -26,49 +28,72 @@
 ./shepherd_core/data_models/experiment/__init__.py
 ./shepherd_core/data_models/experiment/experiment.py
 ./shepherd_core/data_models/experiment/observer_features.py
 ./shepherd_core/data_models/experiment/target_config.py
 ./shepherd_core/data_models/task/__init__.py
 ./shepherd_core/data_models/task/emulation.py
 ./shepherd_core/data_models/task/firmware_mod.py
+./shepherd_core/data_models/task/harvest.py
 ./shepherd_core/data_models/task/observer_tasks.py
-./shepherd_core/data_models/task/programmer.py
+./shepherd_core/data_models/task/programming.py
 ./shepherd_core/data_models/task/testbed_tasks.py
 ./shepherd_core/data_models/testbed/__init__.py
 ./shepherd_core/data_models/testbed/cape.py
 ./shepherd_core/data_models/testbed/cape_fixture.yaml
 ./shepherd_core/data_models/testbed/gpio.py
 ./shepherd_core/data_models/testbed/gpio_fixture.yaml
 ./shepherd_core/data_models/testbed/mcu.py
 ./shepherd_core/data_models/testbed/mcu_fixture.yaml
 ./shepherd_core/data_models/testbed/observer.py
 ./shepherd_core/data_models/testbed/observer_fixture.yaml
 ./shepherd_core/data_models/testbed/target.py
 ./shepherd_core/data_models/testbed/target_fixture.yaml
 ./shepherd_core/data_models/testbed/testbed.py
 ./shepherd_core/data_models/testbed/testbed_fixture.yaml
+./shepherd_core/vsource/__init__.py
+./shepherd_core/vsource/virtual_converter_model.py
+./shepherd_core/vsource/virtual_harvester_model.py
+./shepherd_core/vsource/virtual_source_model.py
 ./tests/__init__.py
 ./tests/conftest.py
-./tests/example_config_experiment.yaml
-./tests/example_config_experiment_alternative.yaml
-./tests/test_content_fixtures.py
-./tests/test_content_models.py
+./tests/test_cal_hw.py
 ./tests/test_examples.py
-./tests/test_experiment_models.py
-./tests/test_task_generation.py
-./tests/test_task_models.py
-./tests/test_testbed_fixtures.py
-./tests/test_testbed_models.py
+./tests/test_logger.py
+./tests/test_reader.py
+./tests/test_writer.py
+./tests/data_models/__init__.py
+./tests/data_models/conftest.py
+./tests/data_models/example_cal_data.yaml
+./tests/data_models/example_cal_data_faulty.yaml
+./tests/data_models/example_cal_meas.yaml
+./tests/data_models/example_cal_meas_faulty1.yaml
+./tests/data_models/example_cal_meas_faulty2.yaml
+./tests/data_models/example_config_emulator.yaml
+./tests/data_models/example_config_experiment.yaml
+./tests/data_models/example_config_experiment_alternative.yaml
+./tests/data_models/example_config_harvester.yaml
+./tests/data_models/example_config_testbed.yaml
+./tests/data_models/example_config_virtsource.yaml
+./tests/data_models/test_base_models.py
+./tests/data_models/test_content_fixtures.py
+./tests/data_models/test_content_models.py
+./tests/data_models/test_examples.py
+./tests/data_models/test_experiment_models.py
+./tests/data_models/test_task_generation.py
+./tests/data_models/test_task_models.py
+./tests/data_models/test_testbed_fixtures.py
+./tests/data_models/test_testbed_models.py
+./tests/vsource/__init__.py
+./tests/vsource/conftest.py
+./tests/vsource/test_converter.py
+./tests/vsource/test_harvester.py
 shepherd_core.egg-info/PKG-INFO
 shepherd_core.egg-info/SOURCES.txt
 shepherd_core.egg-info/dependency_links.txt
 shepherd_core.egg-info/requires.txt
 shepherd_core.egg-info/top_level.txt
 shepherd_core.egg-info/zip-safe
-tests/test_content_fixtures.py
-tests/test_content_models.py
+tests/test_cal_hw.py
 tests/test_examples.py
-tests/test_experiment_models.py
-tests/test_task_generation.py
-tests/test_task_models.py
-tests/test_testbed_fixtures.py
-tests/test_testbed_models.py
+tests/test_logger.py
+tests/test_reader.py
+tests/test_writer.py
```

### Comparing `shepherd_core-2023.5.5/tests/test_content_fixtures.py` & `shepherd_core-2023.5.6/tests/data_models/test_testbed_fixtures.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,52 @@
-from shepherd_core.data_models.content.energy_environment import EnergyEnvironment
-from shepherd_core.data_models.content.energy_environment import fixtures as fix_ee
 from shepherd_core.data_models.content.firmware import Firmware
-from shepherd_core.data_models.content.firmware import fixtures as fix_firmware
-from shepherd_core.data_models.content.virtual_harvester import VirtualHarvester
-from shepherd_core.data_models.content.virtual_harvester import fixtures as fix_hrv
-from shepherd_core.data_models.content.virtual_source import VirtualSource
-from shepherd_core.data_models.content.virtual_source import fixtures as fix_src
-
-
-def test_testbed_fixture_energy_environment():
-    for fix in fix_ee:
-        EnergyEnvironment(name=fix["name"])
-        EnergyEnvironment(id=fix["id"])
-
-
-def test_testbed_fixture_firmware():
-    for fix in fix_firmware:
-        _id = fix["id"]
-        if _id in [1001, 1002]:
-            continue
-        Firmware(name=fix["name"])
-        Firmware(id=fix["id"])
-
-
-def test_experiment_fixture_vsrc():
-    for fix in fix_src:
-        VirtualSource(name=fix["name"])
-        VirtualSource(id=fix["id"])
-
-
-def test_experiment_fixture_vhrv():
-    for fix in fix_hrv:
-        if fix["name"] == "neutral":
-            continue
-        VirtualHarvester(name=fix["name"])
-        VirtualHarvester(id=fix["id"])
+from shepherd_core.data_models.testbed.cape import Cape
+from shepherd_core.data_models.testbed.cape import fixtures as fix_cape
+from shepherd_core.data_models.testbed.gpio import GPIO
+from shepherd_core.data_models.testbed.gpio import fixtures as fix_gpio
+from shepherd_core.data_models.testbed.mcu import MCU
+from shepherd_core.data_models.testbed.mcu import fixtures as fix_mcu
+from shepherd_core.data_models.testbed.observer import Observer
+from shepherd_core.data_models.testbed.observer import fixtures as fix_observer
+from shepherd_core.data_models.testbed.target import Target
+from shepherd_core.data_models.testbed.target import fixtures as fix_target
+from shepherd_core.data_models.testbed.testbed import Testbed as TasteBad
+from shepherd_core.data_models.testbed.testbed import fixtures as fix_testbed
+
+# ⤷ TasteBad avoids pytest-warning
+
+
+def test_testbed_fixture_cape() -> None:
+    for fix in fix_cape:
+        Cape(name=fix["name"])
+        Cape(id=fix["id"])
+
+
+def test_testbed_fixture_gpio() -> None:
+    for fix in fix_gpio:
+        GPIO(name=fix["name"])
+        GPIO(id=fix["id"])
+
+
+def test_testbed_fixture_mcu() -> None:
+    for fix in fix_mcu:
+        MCU(name=fix["name"])
+        mcu = MCU(id=fix["id"])
+        Firmware(name=mcu.fw_name_default)
+
+
+def test_testbed_fixture_observer() -> None:
+    for fix in fix_observer:
+        Observer(name=fix["name"])
+        Observer(id=fix["id"])
+
+
+def test_testbed_fixture_target() -> None:
+    for fix in fix_target:
+        Target(name=fix["name"])
+        Target(id=fix["id"])
+
+
+def test_testbed_fixture_tb() -> None:
+    for fix in fix_testbed:
+        TasteBad(name=fix["name"])
+        TasteBad(id=fix["id"])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `shepherd_core-2023.5.5/tests/test_examples.py` & `shepherd_core-2023.5.6/tests/data_models/test_examples.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 from pathlib import Path
 
 from shepherd_core.data_models.content import VirtualSource
 from shepherd_core.data_models.experiment import Experiment
 from shepherd_core.data_models.task import EmulationTask
+from shepherd_core.data_models.task import HarvestTask
 from shepherd_core.data_models.testbed.testbed import Testbed as TasteBad
 
 from .conftest import load_yaml
 
 # ⤷ TasteBad avoids pytest-warning
 
 
-def test_example_emu():
-    data_dict = load_yaml("example_config_emulator.yml")
-    EmulationTask(**data_dict["parameters"])
+def test_example_emu() -> None:
+    data_dict = load_yaml("example_config_emulator.yaml")
+    assert data_dict["mode"] == "emulator"
+    emu = EmulationTask(**data_dict["parameters"])
+    print(emu)
 
 
-def test_example_exp_recommended():
+def test_example_hrv() -> None:
+    data_dict = load_yaml("example_config_harvester.yaml")
+    assert data_dict["mode"] == "harvester"
+    emu = HarvestTask(**data_dict["parameters"])
+    print(emu)
+
+
+def test_example_exp_recommended() -> None:
     # new way
     path = Path(__file__).with_name("example_config_experiment.yaml")
     Experiment.from_file(path)
 
 
-def test_example_exp():
+def test_example_exp() -> None:
     # non-optimal / old way
     data_dict = load_yaml("example_config_experiment_alternative.yaml")
     Experiment(**data_dict)
 
 
-def test_example_tb():
-    data_dict = load_yaml("example_config_testbed.yml")
+def test_example_tb() -> None:
+    data_dict = load_yaml("example_config_testbed.yaml")
     print(data_dict)
     TasteBad(**data_dict)
 
 
-def test_example_vsrc():
-    data_dict = load_yaml("example_config_virtsource.yml")
+def test_example_vsrc() -> None:
+    data_dict = load_yaml("example_config_virtsource.yaml")
     VirtualSource(**data_dict["VirtualSource"])
```

### Comparing `shepherd_core-2023.5.5/tests/test_experiment_models.py` & `shepherd_core-2023.5.6/tests/data_models/test_task_generation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,101 +1,52 @@
-import hashlib
+from datetime import datetime
+from datetime import timedelta
+from pathlib import Path
+
+from shepherd_core.data_models import EnergyEnvironment
+from shepherd_core.data_models import Experiment
+from shepherd_core.data_models import Firmware
+from shepherd_core.data_models import TargetConfig
+from shepherd_core.data_models import VirtualHarvester
+from shepherd_core.data_models import VirtualSource
+from shepherd_core.data_models.task import TestbedTasks as TasteBadTasks
+
+
+def test_task_generation_file(tmp_path: Path) -> None:
+    path = Path(__file__).with_name("example_config_experiment.yaml")
+    xp1 = Experiment.from_file(path)
+    tb_tasks = TasteBadTasks.from_xp(xp1)
+    tb_tasks.to_file(tmp_path / "tbt1.yaml")
+
+
+def test_task_generation_script(tmp_path: Path) -> None:
+    hrv = VirtualHarvester(name="mppt_bq_thermoelectric")
+
+    target_cfgs = [
+        # first init similar to yaml
+        TargetConfig(
+            target_IDs=list(range(3001, 3004)),
+            custom_IDs=list(range(0, 3)),
+            energy_env={"name": "SolarSunny"},
+            virtual_source={"name": "diode+capacitor"},
+            firmware1={"name": "nrf52_demo_rf"},
+        ),
+        # second Instance fully object-oriented
+        TargetConfig(
+            target_IDs=list(range(2001, 2005)),
+            custom_IDs=list(range(7, 18)),
+            energy_env=EnergyEnvironment(name="ThermoelectricWashingMachine"),
+            virtual_source=VirtualSource(name="BQ25570-Schmitt", harvester=hrv),
+            firmware1=Firmware(name="nrf52_demo_rf"),
+            firmware2=Firmware(name="msp430_deep_sleep"),
+        ),
+    ]
 
-from shepherd_core.data_models.content import EnergyEnvironment
-from shepherd_core.data_models.content import Firmware
-from shepherd_core.data_models.experiment import Experiment
-from shepherd_core.data_models.experiment import GpioActuation
-from shepherd_core.data_models.experiment import GpioEvent
-from shepherd_core.data_models.experiment import GpioLevel
-from shepherd_core.data_models.experiment import GpioTracing
-from shepherd_core.data_models.experiment import PowerTracing
-from shepherd_core.data_models.experiment import SystemLogging
-from shepherd_core.data_models.experiment import TargetConfig
-from shepherd_core.data_models.testbed import GPIO
-from shepherd_core.data_models.testbed import Target
-
-from .conftest import load_yaml
-
-
-def test_experiment_model_min_tgt_cfg():
-    cfg = TargetConfig(
-        target_IDs=[3001],
-        energy_env=EnergyEnvironment(name="SolarSunny"),
-        firmware1=Firmware(name="nrf52_demo_rf"),
-    )
-    for _id in cfg.target_IDs:
-        Target(id=_id)
-
-
-def test_experiment_model_min_exp():
-    Experiment(
-        name="mex per",
-        target_configs=[
-            TargetConfig(
-                target_IDs=[3001],
-                energy_env=EnergyEnvironment(name="SolarSunny"),
-                firmware1=Firmware(name="nrf52_demo_rf"),
-            )
-        ],
-    )
-
-
-def test_experiment_model_yaml_load():
-    exp1_data = load_yaml("example_config_experiment_alternative.yaml")
-    Experiment(**exp1_data)
-
-
-def test_experiment_model_yaml_comparison():
-    exp1_data = load_yaml("example_config_experiment_alternative.yaml")
-    exp1 = Experiment(**exp1_data)
-    exp1_hash = hashlib.sha3_224(str(exp1.dict()).encode("utf-8")).hexdigest()
-    print(f"YamlExp Hash {exp1_hash}")
-
-    target_cfgs = TargetConfig(
-        target_IDs=list(range(2001, 2005)),
-        custom_IDs=list(range(0, 4)),
-        energy_env={"name": "SolarSunny"},
-        virtual_source={"name": "diode+capacitor"},
-        firmware1={"name": "nrf52_demo_rf"},
-    )
-    exp2 = Experiment(
-        id=4567,
+    xperi = Experiment(
+        id="4567",
         name="meaningful Test-Name",
-        created="2023-11-11 11:11:11",
-        time_start="2023-12-12 12:12:12",
-        target_configs=[target_cfgs],
-    )
-    exp2_hash = hashlib.sha3_224(str(exp2.dict()).encode("utf-8")).hexdigest()
-    print(f"  PyExp Hash {exp2_hash}")
-    assert exp1_hash == exp2_hash
-
-
-def test_experiment_model_min_pwrtracing():
-    PowerTracing()
-
-
-def test_experiment_model_min_gpiotracing():
-    GpioTracing()
-
-
-def test_experiment_model_min_gpioevent():
-    GpioEvent(
-        delay=300,
-        gpio=GPIO(name="GPIO3"),
-        level=GpioLevel.high,
+        time_start=datetime.utcnow() + timedelta(minutes=30),
+        target_configs=target_cfgs,
     )
 
-
-def test_experiment_model_min_gpioactuation():
-    GpioActuation(
-        events=[
-            GpioEvent(
-                delay=300,
-                gpio=GPIO(name="GPIO2"),
-                level=GpioLevel.high,
-            )
-        ]
-    )
-
-
-def test_experiment_model_min_syslogging():
-    SystemLogging()
+    tb_tasks = TasteBadTasks.from_xp(xperi)
+    tb_tasks.to_file(tmp_path / "tbt2.yaml")
```

