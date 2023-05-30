# Comparing `tmp/wiliot-testers-4.0.11.tar.gz` & `tmp/wiliot-testers-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-testers-4.0.11.tar", last modified: Tue May 30 19:37:13 2023, max compression
+gzip compressed data, was "wiliot-testers-4.0.6.tar", last modified: Tue Apr 25 08:52:33 2023, max compression
```

## Comparing `wiliot-testers-4.0.11.tar` & `wiliot-testers-4.0.6.tar`

### file list

```diff
@@ -1,111 +1,108 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 19:37:13.486423 wiliot-testers-4.0.11/
--rw-rw-rw-   0 root         (0) root         (0)      830 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     6193 2023-05-30 19:37:13.486423 wiliot-testers-4.0.11/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5688 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/README.md
--rw-rw-rw-   0 root         (0) root         (0)     7247 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-30 19:37:13.486423 wiliot-testers-4.0.11/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2086 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 19:37:13.474423 wiliot-testers-4.0.11/wiliot_testers/
--rw-rw-rw-   0 root         (0) root         (0)    10654 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/API_README.md
--rw-rw-rw-   0 root         (0) root         (0)     4005 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 19:37:13.474423 wiliot-testers-4.0.11/wiliot_testers/calibration_test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/calibration_test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20959 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/calibration_test/calibration_test.py
--rw-rw-rw-   0 root         (0) root         (0)    25345 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/calibration_test/calibration_test_by_tbp.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 19:37:13.478422 wiliot-testers-4.0.11/wiliot_testers/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/config/equipment_config.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 19:37:13.478422 wiliot-testers-4.0.11/wiliot_testers/docs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/docs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    72970 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/docs/tester_api_flow.pdf
--rw-rw-rw-   0 root         (0) root         (0)     4818 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/docs/wiliot_logo.png
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 19:37:13.478422 wiliot-testers-4.0.11/wiliot_testers/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7410 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/examples/wiliot_tester_example.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 19:37:13.478422 wiliot-testers-4.0.11/wiliot_testers/offline/
--rw-rw-rw-   0 root         (0) root         (0)     7114 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/README.md
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/barcode_test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 19:37:13.478422 wiliot-testers-4.0.11/wiliot_testers/offline/configs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/configs/test_configs.json
--rw-rw-rw-   0 root         (0) root         (0)     2082 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/configs/tests_suites.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 19:37:13.482423 wiliot-testers-4.0.11/wiliot_testers/offline/docs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/docs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    37001 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/docs/example_of_timing_diagram.jpg
--rw-rw-rw-   0 root         (0) root         (0)     9764 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/docs/offline_tester_print_sgtin_gui.png
--rw-rw-rw-   0 root         (0) root         (0)    44358 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/docs/offline_tester_run_gui.png
--rw-rw-rw-   0 root         (0) root         (0)    20401 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/docs/offline_tester_start_gui.png
--rw-rw-rw-   0 root         (0) root         (0)    81030 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/docs/r2r_communication_diagram.jpg
--rw-rw-rw-   0 root         (0) root         (0)     4386 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/docs/upload_to_cloud_gui.PNG
--rw-rw-rw-   0 root         (0) root         (0)     4818 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/docs/wiliot_logo.png
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/env_install.bat
--rw-rw-rw-   0 root         (0) root         (0)     9005 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/env_install.py
--rw-rw-rw-   0 root         (0) root         (0)   158407 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/offline_tester.py
--rw-rw-rw-   0 root         (0) root         (0)    64093 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/offline_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/run_barcode_testing.bat
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/run_offline_tester.bat
--rw-rw-rw-   0 root         (0) root         (0)     7447 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/offline/tadbik_r2r_controller.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 19:37:13.482423 wiliot-testers-4.0.11/wiliot_testers/sample/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42248 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/com_connect.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 19:37:13.482423 wiliot-testers-4.0.11/wiliot_testers/sample/configs/
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/configs/.default_surfaces.json
--rw-rw-rw-   0 root         (0) root         (0)     1418 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/configs/.default_test_configs.json
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12210 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/configs_gui.py
--rw-rw-rw-   0 root         (0) root         (0)     4426 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/get_temperature_sensor_name.py
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/sample_test.bat
--rw-rw-rw-   0 root         (0) root         (0)    76637 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/sample_test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 19:37:13.482423 wiliot-testers-4.0.11/wiliot_testers/sample/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22413 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/utils/com_connect.ui
--rw-rw-rw-   0 root         (0) root         (0)     1153 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/utils/comm.gif
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/utils/configs.gif
--rw-rw-rw-   0 root         (0) root         (0)    24482 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/utils/configs.ui
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/utils/edit.gif
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/utils/refresh.gif
--rw-rw-rw-   0 root         (0) root         (0)     3213 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/utils/reset.png
--rw-rw-rw-   0 root         (0) root         (0)    26613 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/utils/sample_test.ui
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/utils/save.png
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/sample/utils/wiliot3.gif
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 19:37:13.482423 wiliot-testers-4.0.11/wiliot_testers/system_test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/system_test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42625 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/system_test/harvester_test.py
--rw-rw-rw-   0 root         (0) root         (0)    73298 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/system_test/system_test_example.py
--rw-rw-rw-   0 root         (0) root         (0)    37198 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/test_equipment.py
--rw-rw-rw-   0 root         (0) root         (0)    66680 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/tester_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      274 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/upload_testers_data.bat
--rw-rw-rw-   0 root         (0) root         (0)    14205 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/upload_testers_data_to_cloud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 19:37:13.482423 wiliot-testers-4.0.11/wiliot_testers/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6048 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)    10904 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/utils/upload_to_cloud_api.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-30 19:37:13.000000 wiliot-testers-4.0.11/wiliot_testers/version.py
--rw-rw-rw-   0 root         (0) root         (0)     8865 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/wiliot_tester_log.py
--rw-rw-rw-   0 root         (0) root         (0)    16956 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/wiliot_tester_tag_result.py
--rw-rw-rw-   0 root         (0) root         (0)    62247 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/wiliot_tester_tag_test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 19:37:13.486423 wiliot-testers-4.0.11/wiliot_testers/yield/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/yield/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 19:37:13.486423 wiliot-testers-4.0.11/wiliot_testers/yield/arduino_counter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/yield/arduino_counter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      809 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/yield/arduino_counter/arduino_counter.ino
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 19:37:13.486423 wiliot-testers-4.0.11/wiliot_testers/yield/configs/
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/yield/configs/.default_configs.json
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/yield/configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1394 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/yield/configs/inlay_data.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/yield/run_yield_tester.bat
--rw-rw-rw-   0 root         (0) root         (0)    27017 2023-05-30 19:37:02.000000 wiliot-testers-4.0.11/wiliot_testers/yield/yield_tester.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 19:37:13.474423 wiliot-testers-4.0.11/wiliot_testers.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6193 2023-05-30 19:37:13.000000 wiliot-testers-4.0.11/wiliot_testers.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3581 2023-05-30 19:37:13.000000 wiliot-testers-4.0.11/wiliot_testers.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-30 19:37:13.000000 wiliot-testers-4.0.11/wiliot_testers.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-30 19:37:13.000000 wiliot-testers-4.0.11/wiliot_testers.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-05-30 19:37:13.000000 wiliot-testers-4.0.11/wiliot_testers.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-05-30 19:37:13.000000 wiliot-testers-4.0.11/wiliot_testers.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.112857 wiliot-testers-4.0.6/
+-rw-rw-rw-   0 root         (0) root         (0)      830 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     5765 2023-04-25 08:52:33.112857 wiliot-testers-4.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5261 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     7247 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-25 08:52:33.112857 wiliot-testers-4.0.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2086 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.100857 wiliot-testers-4.0.6/wiliot_testers/
+-rw-rw-rw-   0 root         (0) root         (0)    10654 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/API_README.md
+-rw-rw-rw-   0 root         (0) root         (0)     4005 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers/calibration_test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/calibration_test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20959 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/calibration_test/calibration_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    25345 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/calibration_test/calibration_test_by_tbp.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/config/equipment_config.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers/docs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/docs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    72970 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/docs/tester_api_flow.pdf
+-rw-rw-rw-   0 root         (0) root         (0)     4818 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/docs/wiliot_logo.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7410 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/examples/wiliot_tester_example.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers/offline/
+-rw-rw-rw-   0 root         (0) root         (0)     7114 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers/offline/configs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/configs/test_configs.json
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/configs/tests_suites.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.108857 wiliot-testers-4.0.6/wiliot_testers/offline/docs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    37001 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/example_of_timing_diagram.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     9764 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/offline_tester_print_sgtin_gui.png
+-rw-rw-rw-   0 root         (0) root         (0)    44358 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/offline_tester_run_gui.png
+-rw-rw-rw-   0 root         (0) root         (0)    20401 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/offline_tester_start_gui.png
+-rw-rw-rw-   0 root         (0) root         (0)    81030 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/r2r_communication_diagram.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     4386 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/upload_to_cloud_gui.PNG
+-rw-rw-rw-   0 root         (0) root         (0)     4818 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/wiliot_logo.png
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/env_install.bat
+-rw-rw-rw-   0 root         (0) root         (0)     9005 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/env_install.py
+-rw-rw-rw-   0 root         (0) root         (0)   155011 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/offline_tester.py
+-rw-rw-rw-   0 root         (0) root         (0)    63768 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/offline_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/run_offline_tester.bat
+-rw-rw-rw-   0 root         (0) root         (0)     7447 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/tadbik_r2r_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.108857 wiliot-testers-4.0.6/wiliot_testers/sample/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    41938 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/com_connect.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.108857 wiliot-testers-4.0.6/wiliot_testers/sample/configs/
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/configs/.default_surfaces.json
+-rw-rw-rw-   0 root         (0) root         (0)     1418 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/configs/.default_test_configs.json
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12551 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/configs_gui.py
+-rw-rw-rw-   0 root         (0) root         (0)     4426 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/get_temperature_sensor_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/sample_test.bat
+-rw-rw-rw-   0 root         (0) root         (0)    74858 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/sample_test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.108857 wiliot-testers-4.0.6/wiliot_testers/sample/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22413 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/com_connect.ui
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/comm.gif
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/configs.gif
+-rw-rw-rw-   0 root         (0) root         (0)    24482 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/configs.ui
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/edit.gif
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/refresh.gif
+-rw-rw-rw-   0 root         (0) root         (0)     3213 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/reset.png
+-rw-rw-rw-   0 root         (0) root         (0)    26613 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/sample_test.ui
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/save.png
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/wiliot3.gif
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.108857 wiliot-testers-4.0.6/wiliot_testers/system_test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/system_test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    42625 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/system_test/harvester_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    73298 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/system_test/system_test_example.py
+-rw-rw-rw-   0 root         (0) root         (0)    31248 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/test_equipment.py
+-rw-rw-rw-   0 root         (0) root         (0)    75770 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/tester_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/upload_testers_data.bat
+-rw-rw-rw-   0 root         (0) root         (0)    14651 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/upload_testers_data_to_cloud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.108857 wiliot-testers-4.0.6/wiliot_testers/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6048 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     8865 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/wiliot_tester_log.py
+-rw-rw-rw-   0 root         (0) root         (0)    16346 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/wiliot_tester_tag_result.py
+-rw-rw-rw-   0 root         (0) root         (0)    61986 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/wiliot_tester_tag_test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.112857 wiliot-testers-4.0.6/wiliot_testers/yield/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.112857 wiliot-testers-4.0.6/wiliot_testers/yield/arduino_counter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/arduino_counter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/arduino_counter/arduino_counter.ino
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.112857 wiliot-testers-4.0.6/wiliot_testers/yield/configs/
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/configs/.default_configs.json
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1394 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/configs/inlay_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/run_yield_tester.bat
+-rw-rw-rw-   0 root         (0) root         (0)    22306 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/yield_tester.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     5765 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3451 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers.egg-info/top_level.txt
```

### Comparing `wiliot-testers-4.0.11/.gitignore` & `wiliot-testers-4.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/LICENSE` & `wiliot-testers-4.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/PKG-INFO` & `wiliot-testers-4.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-testers
-Version: 4.0.11
+Version: 4.0.6
 Summary: A library for interacting with Wiliot's Testers app
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -56,29 +56,15 @@
 * [Sample Test](wiliot_testers/sample/sample_test.py)
 * [Yield Tester](wiliot_testers/yield/yield_tester.py)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
-Version 4.0.11:
------------------
-* offline tester:
-    * fix bug when several tags under test and test status is still pass
-    * support 8 characters barcode label
-    * Support label scanner for both barcode and QR
-    * check printer communication during the run
-    
-* upload data:
-    * fix .bat file for upload data to the cloud
-    
-* sample test:
-    * fix script error when installing on a clean environment
-    
-    
+
 Version 4.0.6:
 -----------------
 * offline tester:
     *  update test suite.
     *  enable line selection using text communication with the printing (currently available only if printing offset > 0 and no QR check.
     *  add tag reel location to packet data csv (i.e. the location on the reel even if multiple runs were done on the same reel)
     *  check gw trigger (optic sensor signal) and apply printing validation, right after a trigger was received (or missing label was decided)
```

### Comparing `wiliot-testers-4.0.11/README.md` & `wiliot-testers-4.0.6/wiliot_testers.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: wiliot-testers
+Version: 4.0.6
+Summary: A library for interacting with Wiliot's Testers app
+Home-page: UNKNOWN
+Author: Wiliot
+Author-email: support@wiliot.com
+License: MIT
+Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyWiliot: wiliot-testers #
 
 wiliot-testers is a python library for accessing Wiliot's Testers scripts
 
 ## Public Library
 
 ### MAC Installation
@@ -39,29 +56,15 @@
 * [Sample Test](wiliot_testers/sample/sample_test.py)
 * [Yield Tester](wiliot_testers/yield/yield_tester.py)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
-Version 4.0.11:
------------------
-* offline tester:
-    * fix bug when several tags under test and test status is still pass
-    * support 8 characters barcode label
-    * Support label scanner for both barcode and QR
-    * check printer communication during the run
-    
-* upload data:
-    * fix .bat file for upload data to the cloud
-    
-* sample test:
-    * fix script error when installing on a clean environment
-    
-    
+
 Version 4.0.6:
 -----------------
 * offline tester:
     *  update test suite.
     *  enable line selection using text communication with the printing (currently available only if printing offset > 0 and no QR check.
     *  add tag reel location to packet data csv (i.e. the location on the reel even if multiple runs were done on the same reel)
     *  check gw trigger (optic sensor signal) and apply printing validation, right after a trigger was received (or missing label was decided)
@@ -100,7 +103,9 @@
 Version 4.0.0:
 -----------------
 * First version
 
 
 The package previous content was published under the name 'wiliot' package.
 for more information please read 'wiliot' package's release notes
+
+
```

### Comparing `wiliot-testers-4.0.11/bitbucket-pipelines.yml` & `wiliot-testers-4.0.6/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/setup.py` & `wiliot-testers-4.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/API_README.md` & `wiliot-testers-4.0.6/wiliot_testers/API_README.md`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/__init__.py` & `wiliot-testers-4.0.6/wiliot_testers/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/calibration_test/calibration_test.py` & `wiliot-testers-4.0.6/wiliot_testers/calibration_test/calibration_test.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/calibration_test/calibration_test_by_tbp.py` & `wiliot-testers-4.0.6/wiliot_testers/calibration_test/calibration_test_by_tbp.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/docs/tester_api_flow.pdf` & `wiliot-testers-4.0.6/wiliot_testers/docs/tester_api_flow.pdf`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/docs/wiliot_logo.png` & `wiliot-testers-4.0.6/wiliot_testers/docs/wiliot_logo.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/examples/wiliot_tester_example.py` & `wiliot-testers-4.0.6/wiliot_testers/examples/wiliot_tester_example.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/offline/README.md` & `wiliot-testers-4.0.6/wiliot_testers/offline/README.md`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/offline/configs/tests_suites.json` & `wiliot-testers-4.0.6/wiliot_testers/offline/configs/tests_suites.json`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/offline/docs/example_of_timing_diagram.jpg` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/example_of_timing_diagram.jpg`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/offline/docs/offline_tester_print_sgtin_gui.png` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/offline_tester_print_sgtin_gui.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/offline/docs/offline_tester_run_gui.png` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/offline_tester_run_gui.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/offline/docs/offline_tester_start_gui.png` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/offline_tester_start_gui.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/offline/docs/r2r_communication_diagram.jpg` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/r2r_communication_diagram.jpg`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/offline/docs/upload_to_cloud_gui.PNG` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/upload_to_cloud_gui.PNG`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/offline/docs/wiliot_logo.png` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/wiliot_logo.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/offline/env_install.py` & `wiliot-testers-4.0.6/wiliot_testers/offline/env_install.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/offline/offline_tester.py` & `wiliot-testers-4.0.6/wiliot_testers/offline/offline_tester.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,16 @@
 from PyQt5.QtGui import *
 import pyqtgraph as pg
 from wiliot_testers.test_equipment import BarcodeScanner
 from numpy import mean
 from wiliot_testers.wiliot_tester_tag_test import *
 from wiliot_testers.wiliot_tester_log import *
 from wiliot_testers.tester_utils import *
-from wiliot_testers.utils.upload_to_cloud_api import *
 from wiliot_testers.offline.offline_utils import *
-from wiliot_core import WiliotDir, check_user_config_is_ok, csv_to_dict, InlayTypes, DualGWMode, WiliotGateway
+from wiliot_core import WiliotDir, check_user_config_is_ok, csv_to_dict, InlayTypes, DualGWMode
 from wiliot_testers.utils.get_version import get_version
 from wiliot_core import WiliotGateway, DualGWMode
 from appdirs import user_data_dir
 from queue import Queue
 import socket
 
 # a global variable which will be in the log_file name that says the R2R code version
@@ -101,54 +100,37 @@
 run_start_time_ = datetime.datetime.now()
 qr_que_list = []
 external_id_for_printer = 999999999
 yield_over_time = 0
 calculate_interval = 10
 calculate_on = 50
 
-MIN_TEST_TIME = 1.5  # seconds
-TIME_BTWN_PRINTER_REQUESTS = 0.25  # seconds
-PRINTER_SOCKET_TIMEOUT = 1  # seconds
+MIN_TEST_TIME = 0.3  # seconds
 
 lock_print = threading.Lock()
 
 
 class QRThread(threading.Thread):
-    def __init__(self, events, ports_and_guis, print=False):
+    def __init__(self, events, ports_and_guis):
         threading.Thread.__init__(self)
         self.events = events
-        self.is_print = print
         self.ports_and_guis = ports_and_guis
         self.qr_comport = self.ports_and_guis.Tag_Value['QRcomport']
         self.max_wrong_readouts_in_row = int(self.ports_and_guis.Tag_Value['maxQRWrongTags'])
-        self.QRtimeout = str(self.ports_and_guis.Tag_Value['QRtimeout'])
-
-        try:
-            if self.is_print:
-                self.scanner = BarcodeScanner(com='COM{}'.format(self.qr_comport), log_type='LOG', write_to_log=False, timeout=self.QRtimeout)
-            else:
-                self.scanner = BarcodeScanner(com='COM{}'.format(self.qr_comport), log_type='LOG', write_to_log=True, timeout=self.QRtimeout)
-
-            self.ports_and_guis.my_logger.logger.info('Connected to scanner at port COM{}'.format(self.qr_comport))
-
-        except Exception as e:
-            self.ports_and_guis.my_logger.logger.info('No barcode scanner found')
-            raise Exception(f'could not connect to bracode scanner {e}')
-
+        self.scanner = BarcodeScanner(com='COM{}'.format(self.qr_comport), log_type='LOG')
         self.read_out_attempts = 5
         self.failed_qr_list = []
         self.qr_max_bad_tags = 10
         self.wrong_readout = 0
         self.wrong_readout_in_row = 0
 
     def run(self):
 
         def success_read():
             self.ports_and_guis.my_logger.logger.info("QR code validated successfully")
-            self.events.qr_val.set()
             self.events.qr_read_success.set()
             self.success = True
             self.wrong_readout_in_row = 0
 
         die = False
 
         while not die:
@@ -156,80 +138,63 @@
             self.events.start_compare.wait(timeout=10)
             if not self.events.start_compare.is_set():
                 if self.events.done_to_tag_thread.is_set() or self.events.done_to_r2r_thread.is_set():
                     die = True
                     break
                 continue
 
-            if not self.is_print:
+            if not self.events.qr_queue.empty():
                 self.events.start_compare.clear()
-                self.events.qr_val.clear()
+                try:
+                    self.tag_comparted = self.events.qr_queue.get(block=False, timeout=0.1)
+                except Exception:
+                    die = True
+                    break
                 self.success = False
+                self.ports_and_guis.my_logger.logger.info('Comparing {}'.format(self.tag_comparted))
                 for i in range(self.read_out_attempts):
                     self.qr_tag = self.scanner.scan_ext_id()
-                    self.ports_and_guis.my_logger.logger.info('Scanned {}'.format(self.qr_tag))
-                self.events.qr_val.set()
-                self.events.qr_read_success.set()
-
-
-            else:
-                if not self.events.qr_queue.empty():
-                    self.events.start_compare.clear()
-                    self.events.qr_val.clear()
-                    try:
-                        self.tag_comparted = self.events.qr_queue.get(block=False, timeout=0.1)
-                    except Exception:
-                        die = True
-                        break
-                    self.success = False
-                    self.ports_and_guis.my_logger.logger.info('Comparing {}'.format(self.tag_comparted))
-                    for i in range(self.read_out_attempts):
-                        self.qr_tag = self.scanner.scan_ext_id()
-                        self.ports_and_guis.my_logger.logger.info(
-                            f'--- SCANNING: expected ex id: {self.tag_comparted["externalID"]}, '
-                            f'read ex id: {self.qr_tag[0]} ---')
-                        if self.qr_tag[1] is not None:
-                            if self.tag_comparted['status'] == 'Pass':
-                                if self.tag_comparted['externalID'][-4:] == self.qr_tag[1]:
-                                    success_read()
-                                    break
-
-                        else:
-                            if self.tag_comparted['status'] == 'Fail':
+                    time.sleep(0.05)
+                    if self.qr_tag[1] is not None:
+                        if self.tag_comparted['status'] == 'Pass':
+                            if self.tag_comparted['externalID'][-4:] == self.qr_tag[1]:
                                 success_read()
                                 break
 
-                        self.ports_and_guis.my_logger.logger.info(
-                            "Scanning failed, trying again attempt {}/{}".format(i, self.read_out_attempts))
-
-                    if not self.success:
-                        self.ports_and_guis.my_logger.logger.warning('Scan failed for tag {}'.format(self.tag_comparted))
-                        self.wrong_readout += 1
-                        self.wrong_readout_in_row += 1
-                        if self.wrong_readout < self.qr_max_bad_tags and \
-                                self.wrong_readout_in_row < self.max_wrong_readouts_in_row:
-                            self.events.qr_val.clear()
-                            self.events.qr_read_success.set()
-
-                if self.wrong_readout >= self.qr_max_bad_tags:
-                    die = True
-                    self.ports_and_guis.my_logger.logger.warning('Maximum bad tags comparing reached')
-                    break
+                    else:
+                        if self.tag_comparted['status'] == 'Fail':
+                            success_read()
+                            break
 
-                if self.wrong_readout_in_row >= self.max_wrong_readouts_in_row:
-                    self.ports_and_guis.my_logger.logger.warning('Maximum bad tags comparing in row reached')
-                    die = True
-                    break
+                    self.ports_and_guis.my_logger.logger.info(
+                        "Scanning failed, trying again attempt {}/{}".format(i, self.read_out_attempts))
 
-                if self.events.done_to_tag_thread.is_set() or self.events.done_to_r2r_thread.is_set():
-                    die = True
-                    break
+                if not self.success:
+                    self.ports_and_guis.my_logger.logger.warning('Scan failed for tag {}'.format(self.tag_comparted))
+                    self.wrong_readout += 1
+                    self.wrong_readout_in_row += 1
+                    if self.wrong_readout < self.qr_max_bad_tags and \
+                            self.wrong_readout_in_row < self.max_wrong_readouts_in_row:
+                        self.events.qr_read_success.set()
+
+            if self.wrong_readout >= self.qr_max_bad_tags:
+                die = True
+                self.ports_and_guis.my_logger.logger.warning('Maximum bad tags comparing reached')
+                break
+
+            if self.wrong_readout_in_row >= self.max_wrong_readouts_in_row:
+                self.ports_and_guis.my_logger.logger.warning('Maximum bad tags comparing in row reached')
+                die = True
+                break
+
+            if self.events.done_to_tag_thread.is_set() or self.events.done_to_r2r_thread.is_set():
+                die = True
+                break
 
         if die:
-            self.scanner.close_port()
             msg = 'Pausing run because QR comparing went wrong or run end'
             printing_func(msg, 'QRThread', lock_print, logger_type='warning',
                           logger_name=self.ports_and_guis.my_logger.logger.name)
             self.events.done_to_tag_thread.set()
             self.events.stop_to_r2r_thread.set()
 
 
@@ -306,15 +271,14 @@
             self.start_value = start_value
             self.cur_value = 0
             self.pass_job_name = pass_job_name
             self.fail_job_name = self.ports_and_guis.Tag_Printing_Value['failJobName']
             self.pass_job_num = self.ports_and_guis.Tag_Printing_Value['passJobNum']
             self.fail_job_num = 1
 
-
             # open the socket & config the printer
             self.initialization()
 
         except Exception:
             exception_details = sys.exc_info()
             self.exception_queue.put(exception_details)
 
@@ -469,15 +433,15 @@
                                 try:
                                     self.printer_status()
                                     break
                                 except Exception as e:
                                     self.ports_and_guis.my_logger.logger.info(f'got exception from printer, '
                                                                               f'try again ({e})')
                                     dt = (datetime.datetime.now() - t_i).total_seconds()
-                                    time.sleep(TIME_BTWN_PRINTER_REQUESTS)
+                                    time.sleep(0.010)
                             if self.enable_line_selection:
                                 self.set_printing_type()  # set the printing type for the next tag #TODO need to enable it for QR as well
 
                 except Exception:
                     do_the_thread_again = False
                     exception_details = sys.exc_info()
                     self.exception_queue.put(exception_details)
@@ -658,16 +622,14 @@
         """
         if print_and_log:
             msg = "Sent command to printer: " + cmd.strip('\r\n')
             printing_func(msg, 'PrinterThread', lock_print, logger_type='debug',
                           logger_name=self.ports_and_guis.my_logger.logger.name)
         self.ports_and_guis.Printer_socket.send(cmd.encode())
         data = self.ports_and_guis.Printer_socket.recv(int(self.TCP_BUFFER))
-        if len(data) == 0:
-            raise PrinterNeedsResetException(f'The printer did not ack to the following cmd :{cmd}')
         value = data.decode("utf-8")
         # Cut the last character as the device returns a null terminated string
         value = value[:-1]
         if print_and_log:
             msg = "Received answer from printer: " + str(value.strip('\r\n'))
             printing_func(msg, 'PrinterThread', lock_print, logger_type='debug',
                           logger_name=self.ports_and_guis.my_logger.logger.name)
@@ -698,15 +660,14 @@
             time.sleep(1)  # to make sure the socket is closed when we start the reopen
             self.initialization()
         except Exception:
             printing_func('reopen_sock() failed, please end this run', 'PrinterThread',
                           lock_print, logger_type='warning', logger_name=self.ports_and_guis.my_logger.logger.name)
             raise (PrinterNeedsResetException('reopen_sock() failed'))
 
-    # UNUSED FUNCTION
     def line_assigment(self, job_name, line_number, field_name, field_value):
         """
         builds the command to send to printer for configuration of the printing format
         @param job_name: (string) what is the job name (should be the same as in the printer)
         @param line_number: what is the line to assign to (2 = pass, 1 = fail)
         @param field_name: field name in the printer
         @param field_value: what to put in this field
@@ -714,15 +675,14 @@
         """
         # Send Line Assignment Command: job name + line number+starting value
         cmd = 'LAS|' + str(job_name) + '|' + str(line_number) + '|' + str(field_name) + '=' + str(
             field_value) + '|\r\n'
         # changing to bytes
         return cmd
 
-    # UNUSED FUNCTION
     def clear_line(self, line_number):
         """
         builds the command to send to printer for clearing a line
         @param line_number: the line to clear
         @return: the cmd to send to printer
         """
         # On success, returns the default success response (ACK). On failure, returns the default failure response (ERR)
@@ -739,15 +699,14 @@
         3 Running
         4 Offline
         @return: the cmd to send to printer
         """
         cmd = 'SST|' + str(desired_state) + '|\r\n'
         return cmd
 
-    # UNUSED FUNCTION
     def get_job_name(self):
         """
         gets the last job that were used by the printer
         @return: the name of the current job in the printer in the following format:
             JOB|<job name>|<line number>|<CR>
         """
         cmd = 'GJN\r\n'
@@ -875,15 +834,15 @@
              'packet_status', 'adv_address', 'selected_tag', 'is_test_pass', 'status_offline', 'fail_bin',
              'fail_bin_str',
              'test_status', 'num_packets', 'num_cycles', 'sprinkler_counter_mean', 'sprinkler_counter_std',
              'sprinkler_counter_min', 'sprinkler_counter_max', 'tbp_mean', 'tbp_std', 'tbp_min', 'tbp_max',
              'tbp_num_vals',
              'per_mean', 'per_std', 'rssi_mean', 'rssi_std', 'rssi_min', 'rssi_max', 'ttfp', 'rx_rate_normalized',
              'rx_rate', 'total_test_duration', 'total_location_duration', 'test_start_time', 'trigger_time',
-             'test_end_time', 'label_validated_at_loc', 'rx_channel', 'energizing_pattern', 'time_profile',
+             'test_end_time', 'qr_validated', 'rx_channel', 'energizing_pattern', 'time_profile',
              'decrypted_packet_type',
              'group_id', 'flow_ver', 'test_mode', 'en', 'type', 'data_uid', 'nonce', 'enc_uid', 'mic', 'enc_payload',
              'gw_packet', 'stat_param', 'temperature_sensor']
 
         try:
             self.GwObj, self.t = self.config()
 
@@ -935,40 +894,25 @@
                     self.ports_and_guis.my_logger.logger.info('Sent start to test QR')
                 else:
                     self.events.qr_read_success.set()
                     self.ports_and_guis.my_logger.logger.info('Queue not full yet')
 
             else:
                 self.events.start_compare.set()
-        elif self.qr_enable == 'Yes' and not self.ports_and_guis.print_test:
-            self.events.printer_validation_success.clear()
-            self.events.qr_read_success.clear()
-            self.events.start_compare.set()
 
     def check_printer_validation(self):
         if self.to_print and not self.ports_and_guis.print_test:
             self.events.validation_success.wait(timeout=5)
             if not self.events.validation_success.isSet():
                 self.ports_and_guis.my_logger.logger.warning(
                     "QR Validation didn't succeed or Printer counter is not right")
                 self.events.stop_to_r2r_thread.set()
                 self.events.done_to_tag_thread.set()
             else:
-                self.ports_and_guis.my_logger.logger.info('Validation criteria is ok')
-            self.events.printer_validation_success.clear()
-            self.events.qr_read_success.clear()
-
-    def check_qr_validation(self):
-        if self.qr_enable == 'Yes' and not self.to_print:
-            self.events.validation_success.wait(timeout=5)
-            if not self.events.validation_success.isSet():
-                self.ports_and_guis.my_logger.logger.warning(
-                    "QR Validation didn't succeed or Printer counter is not right")
-            else:
-                self.ports_and_guis.my_logger.logger.info('Validation criteria is ok')
+                self.ports_and_guis.my_logger.logger.info('Validation is ok')
             self.events.printer_validation_success.clear()
             self.events.qr_read_success.clear()
 
     @pyqtSlot()
     def run(self):
         """
         runs the thread
@@ -1096,17 +1040,14 @@
                         except Exception:
                             self.ports_and_guis.my_logger.logger.warning('Problem with temperature sensor detection')
                             pass
                         self.ports_and_guis.my_logger.logger.debug('Temperature is: {}'.format(str(temperature_sensor)))
                     else:
                         temperature_sensor = float(-1)
 
-                    if self.qr_enable == 'Yes' and not self.to_print:
-                        self.check_qr_validation()
-
                     self.test_data['tag_run_location'] = self.tag_location
                     self.test_data['tag_reel_location'] = int(self.tag_reel_location) + int(self.tag_location)
                     self.test_data['temperature_sensor'] = temperature_sensor
                     if self.events.done_to_tag_thread.is_set():
                         break
                     # printing processes:
                     if self.to_print and not self.ports_and_guis.print_test:
@@ -1129,15 +1070,15 @@
                             self.test_data['is_test_pass'] = False
                             self.ports_and_guis.my_logger.logger.warning(
                                 'Tag location: {} failed - Missing Label'.format(str(self.tag_location)))
                             self.events.start_to_r2r_thread.set()
 
                             total_loc_time = datetime.datetime.now() - self.start_time
                             self.test_data['total_location_duration'] = total_loc_time.total_seconds()
-                            self.test_data['label_validated_at_loc'] = self.events.qr_val.is_set()
+
                             # add packets to packet_data.csv:
                             self.update_packet_data(packets_data_path=self.ports_and_guis.my_logger.packets_data_path,
                                                     test_data=self.test_data)
                             # update run_data:
                             self.update_run_data(run_data_path=self.ports_and_guis.my_logger.run_data_path,
                                                  run_data=self.run_data)
                             if self.to_print and not self.ports_and_guis.print_test:
@@ -1192,16 +1133,15 @@
                                 if selected_tag in self.all_selected_tags:
                                     # Duplication
                                     self.tester_res.set_total_fail_bin(FailureCodes.DUPLICATION_OFFLINE)
                                     self.tester_res.set_total_test_status(status=False)
                                     black_list_size += 1
                                     self.black_list.append(selected_tag)
                                     self.ports_and_guis.my_logger.logger.warning(
-                                        'Tag location: {} has been already seen in the run before'.format(
-                                            str(self.tag_location)))
+                                        'Tag location: {} has been already seen in the run before'.format(str(self.tag_location)))
                                     self.tester_res.set_packet_status(adv_address=selected_tag,
                                                                       status='duplication')
                                     if self.to_print and not self.ports_and_guis.print_test:
                                         self.events.qr_queue.put({'externalID': selected_tag, 'status': 'Fail'})
                                         if self.enable_line_selection:
                                             self.events.tag_status_queue.put('fail')
 
@@ -1260,27 +1200,26 @@
                                                 'Tag added as fail, failed during test')
                                         self.events.fail_to_r2r_thread.set()
                             self.all_tags += self.tester_res.get_test_unique_adva()
                             self.all_tags = list(set(self.all_tags))
                             self.run_data['total_run_responding_tags'] = len(self.all_tags)
                             total_loc_time = datetime.datetime.now() - self.start_time
                             self.test_data['total_location_duration'] = total_loc_time.total_seconds()
-                            self.test_data['label_validated_at_loc'] = self.events.qr_val.is_set()
                             # add packets to packet_data.csv:
                             self.update_packet_data(res=self.tester_res,
                                                     packets_data_path=self.ports_and_guis.my_logger.packets_data_path,
                                                     test_data=self.test_data)
                             # update run_data:
                             self.update_run_data(run_data_path=self.ports_and_guis.my_logger.run_data_path,
                                                  run_data=self.run_data, res=self.tester_res)
                         self.tag_location += 1
-                        # Check the diff criteria
+                        # Check the diff critiria
                         if self.pass_response_diff is not None:
                             if len(self.all_tags) > self.pass_response_diff_offset:
-                                if (passed * 100) / len(self.all_tags) < 100 - int(self.pass_response_diff):
+                                if (passed*100)/len(self.all_tags) < 100-int(self.pass_response_diff):
                                     self.ports_and_guis.my_logger.logger.warning(
                                         'Problem with setup, stop criteria for responsive tags and pass tags diff is '
                                         'lower then threshold please check setup or change the value')
                                     self.events.done_to_r2r_thread.set()
                                     self.events.done_to_tag_thread.set()
                                     if self.to_print:
                                         self.events.done_to_printer_thread.set()
@@ -1458,34 +1397,32 @@
 
         if self.ports_and_guis.auto_attenuator_enable:
             attn_pwr = int(self.ports_and_guis.Tag_Value['attnval']) - 5
             self.ports_and_guis.my_logger.results_logger.info('Setting ATTN to {}'.format(attn_pwr))
             set_attn_status = self.ports_and_guis.attenuator.Setattn(attn_pwr)
             time.sleep(2)
             if set_attn_status:
-                self.ports_and_guis.my_logger.results_logger.info(
-                    'Attenuation in dB set to {}'.format(self.ports_and_guis.attenuator.Getattn()))
+                self.ports_and_guis.my_logger.results_logger.info('Attenuation in dB set to {}'.format(self.ports_and_guis.attenuator.Getattn()))
 
         self.ttfp_num = 0
         self.ttfp_sum = 0
         return self.GwObj, t
 
     def start_energizer(self):
         if self.ports_and_guis.energizerGW:
-            self.ports_and_guis.energizerGW.write('!gateway_app')
+            self.ports_and_guis.energizerGW.write('!gateway_app', with_ack=True)
 
     def stop_energizer(self):
         if self.ports_and_guis.energizerGW:
             self.ports_and_guis.energizerGW.write('!cancel')
             self.ports_and_guis.energizerGW.reset_buffer()
 
     def get_curr_timestamp_in_sec(self):
         return (datetime.datetime.now() - self.start_time).total_seconds()
 
-    # UNUSED FUNCTION
     def is_gw_respond_with_stat_param_zero(self, chosen_tag_packets):
         chosen_tag_packets_df = chosen_tag_packets.get_df()
         return len(chosen_tag_packets_df[chosen_tag_packets_df['stat_param'] == 0]) > 1
 
     def closure_fn(self):
         """
            turn off the GW (reset) and closes the GW Comport
@@ -1493,32 +1430,44 @@
                'User pressed Stop!'
            """
         if self.black_list.__len__() > 0:
             self.ports_and_guis.my_logger.logger.warning('Black list tags: {}'.format(list(set(self.black_list))))
         if not self.did_closure_fn_run:
             self.run_data['reel_run_end_time'] = datetime.datetime.now()
             self.run_data['upload_date'] = datetime.datetime.now()
-            dict_to_csv(self.run_data, path=self.ports_and_guis.my_logger.run_data_path)
+            self.dict_to_csv(self.run_data, path=self.ports_and_guis.my_logger.run_data_path)
             self.WiliotTester.exit_tag_test()
             printing_func("TagThread is done", 'TagThread',
                           lock_print, logger_type='warning', logger_name=self.ports_and_guis.my_logger.logger.name)
             self.did_closure_fn_run = True
 
-    # TODO, MAYBE ONE FUNCTION OR OFFLINE AND YIELD?
+    def dict_to_csv(self, dict_in, path, append=False, only_titles=False):
+        if append:
+            method = 'a'
+        else:
+            method = 'w'
+        with open(path, method, newline='') as f:
+            dict_writer = DictWriter(f, fieldnames=dict_in.keys())
+            if not append:
+                dict_writer.writeheader()
+            if not only_titles:
+                dict_writer.writerow(dict_in)
+            f.close()
+
     def update_run_data(self, run_data_path, run_data, res=None, save_to_csv=True):
         if res is not None:
             run_data['total_run_tested'] += 1
             run_data['total_run_passed_offline'] += res.get_total_test_status()
             run_data['run_responsive_tags_yield'] = \
                 (run_data['total_run_responding_tags'] / run_data['total_run_tested']) * 100
             run_data['run_offline_yield'] = \
                 (run_data['total_run_passed_offline'] / run_data['total_run_tested']) * 100
 
         if save_to_csv:
-            dict_to_csv(dict_in=run_data, path=run_data_path)
+            self.dict_to_csv(dict_in=run_data, path=run_data_path)
 
     def update_packet_data(self, packets_data_path, res=None, test_data=None, only_titles=False):
 
         def save_default_packet_data(summary=None):
             default_data = {'raw_packet': None, 'adv_address': None, 'decrypted_packet_type': None,
                             'group_id': None, 'flow_ver': None,
                             'test_mode': None, 'en': None, 'type': None, 'data_uid': None, 'nonce': None,
@@ -1528,15 +1477,15 @@
                             'tag_run_location': test_data['tag_run_location'],
                             'tag_reel_location': test_data['tag_reel_location'],
                             'total_test_duration': test_data['total_test_duration'],
                             'total_location_duration': test_data['total_location_duration'],
                             'status_offline': test_data['status_offline'],
                             'fail_bin': test_data['fail_bin'], 'fail_bin_str': test_data['fail_bin_str'],
                             'external_id': None,
-                            'label_validated_at_loc': test_data['label_validated_at_loc'], 'test_num': test_data['test_num'],
+                            'qr_validated': test_data['qr_validated'], 'test_num': test_data['test_num'],
                             'trigger_time': test_data['trigger_time'], 'packet_status': None,
                             'temperature_sensor': float(-1)}
             if summary is None:
                 default_sum = {'is_test_pass': None, 'selected_tag': None, 'test_start_time': None,
                                'test_end_time': None, 'test_status': None, 'rx_channel': None,
                                'energizing_pattern': None, 'time_profile': None, 'num_packets': 0,
                                'num_cycles': 0, 'sprinkler_counter_mean': None, 'sprinkler_counter_std': None,
@@ -1547,16 +1496,16 @@
                                'rx_rate': None}
             else:
                 default_sum = summary
 
             default_packet_att = {'is_valid_packet': None, 'inlay_type': None}
             default_dict = {**default_data, **default_sum, **default_packet_att}
             default_ordered_dict = {k: default_dict[k] for k in self.packet_headers_default}
-            dict_to_csv(dict_in=default_ordered_dict, path=packets_data_path, append=(not only_titles),
-                        only_titles=only_titles)
+            self.dict_to_csv(dict_in=default_ordered_dict, path=packets_data_path, append=(not only_titles),
+                             only_titles=only_titles)
 
         if res is not None:
             test_data['status_offline'] = int(res.get_total_test_status())
             if test_data['status_offline'] == 0:
                 test_data['external_id'] = None
             test_data['total_test_duration'] = res.get_total_test_duration()
             test_data['fail_bin'] = res.get_total_fail_bin()
@@ -1618,29 +1567,28 @@
                          'conversion_type': ConversionTypes(self.ports_and_guis.Tag_Value['conversion']).name,
                          'inlay': InlayTypes(self.ports_and_guis.Tag_Value['inlay']).name,
                          'test_suite': self.ports_and_guis.Tag_Value['inlayType'],
                          'test_suite_dict': self.ports_and_guis.tests_suite,
                          'surface': SurfaceTypes(self.ports_and_guis.Tag_Value['surface']).name,
                          'to_print': self.ports_and_guis.Tag_Value['toPrint'],
                          'qr_validation': self.ports_and_guis.Tag_Value['QRRead'],
-                         'qr_offset': self.ports_and_guis.Tag_Value['QRoffset'],
                          'print_pass_job_name': print_pass_job_name, 'printing_format': printing_format,
                          'external_id_prefix': self.string_before_counter,
                          'external_id_suffix_init_value': self.init_external_id,
                          'coupler_partnumber': '',
                          'gw_version': self.ports_and_guis.ver, 'py_wiliot_version': get_version(), 'upload_date': None,
                          'owner_id': 'wiliot-ops', 'temperature_sensor_enable': self.ports_and_guis.temperature_enabled,
                          'ttfp_avg': float('nan')}
 
         self.test_data = {'common_run_name': common_run_name, 'tag_run_location': tested,
                           'total_location_duration': None, 'total_test_duration': None,
                           'status_offline': False, 'fail_bin': FailureCodes.NONE.value,
                           'fail_bin_str': FailureCodes.NONE.name,
                           'external_id': self.printed_external_id,
-                          'label_validated_at_loc': self.events.qr_val.is_set(), 'trigger_time': None,
+                          'qr_validated': self.qr_enable, 'trigger_time': None,
                           'test_num': 0, 'temperature_sensor': float(-1), 'tag_reel_location': self.tag_reel_location}
 
 
 class R2RThread(threading.Thread):
     """
     Thread that controls R2R machine
 
@@ -1834,15 +1782,14 @@
         # both printer and tag thread will wait on it. only printer will .clear() it (in printing mode)
         self.r2r_ready = threading.Event()
         # start qr read_out
         self.qr_queue = Queue()
         self.tag_status_queue = Queue()
         self.start_compare = threading.Event()
         self.qr_read_success = threading.Event()
-        self.qr_val = threading.Event()
         # printer events
         self.was_pass_to_printer = threading.Event()
         self.was_fail_to_printer = threading.Event()
         self.printer_success = threading.Event()
         self.printer_error = threading.Event()
         self.printer_event = or_event_set(self.printer_success, self.printer_error)
         self.printer_validation_success = threading.Event()
@@ -1961,16 +1908,15 @@
 
         self.auto_attenuator_enable = self.Tag_Value['externalAttenuator']
         if self.auto_attenuator_enable:
             try:
                 if self.Tag_Value['attnComport'].upper() == 'AUTO':
                     self.attenuator = Attenuator('API').GetActiveTE()
                 else:
-                    self.attenuator = Attenuator('API',
-                                                 comport='COM' + str(self.Tag_Value['attnComport'])).GetActiveTE()
+                    self.attenuator = Attenuator('API',comport = 'COM'+str(self.Tag_Value['attnComport'])).GetActiveTE()
                 current_attn = self.attenuator.Getattn()
             except Exception as e:
                 raise EquipmentError('Attenuator Error - Verify Attenuator connection')
 
         self.config_equipment(temperature_sensor=True)
 
         # check if the system variable exist
@@ -1981,45 +1927,43 @@
         # serial for GW
         self.GwObj = WiliotGateway(auto_connect=True, logger_name=self.my_logger.gw_logger.name,
                                    is_multi_processes=True, log_dir_for_multi_processes=os.path.join(self.new_path,
                                                                                                      common_run_name))
         self.ver, _ = self.GwObj.get_gw_version()
 
         if 'additionalGW' in self.tests_suite:
-            self.energizerGW = WiliotGateway(logger_name=self.my_logger.gw_logger.name,
-                                             port=self.tests_suite['additionalGW']['port'])
+            self.energizerGW = WiliotGateway(logger_name=self.my_logger.gw_logger.name, port=self.tests_suite['additionalGW']['port'])
             if self.energizerGW.connected:
                 self.energizerGW.reset_gw()
                 sleep(1)
-                self.energizerGW.write('!listen_to_tag_only 1')
-                self.energizerGW.write('!set_tester_mode 1')
-                self.energizerGW.write('!pl_gw_config 0')
-                self.energizerGW.write('!sub1g_sync 1')
+                self.energizerGW.write('!listen_to_tag_only 1', with_ack=True)
+                self.energizerGW.write('!set_tester_mode 1', with_ack=True)
+                self.energizerGW.write('!pl_gw_config 0', with_ack=True)
+                self.energizerGW.write('!sub1g_sync 1', with_ack=True)
 
                 try:
                     self.additional_gw_mode = DualGWMode(self.tests_suite['additionalGW']['mode'])
                 except Exception as e:
                     raise Exception('no mode in additionalGW dict in test suite or invalid mode: {}'.format(e))
 
-                self.energizerGW.config_gw(received_channel=self.tests_suite['additionalGW']['rxChannel'],
-                                           energy_pattern_val=self.tests_suite['additionalGW']['energizingPattern'],
-                                           time_profile_val=self.tests_suite['additionalGW']['timeProfile'],
-                                           output_power_val=self.tests_suite['additionalGW']['gw_output_power'],
-                                           bypass_pa_val=self.tests_suite['additionalGW']['bypass_pa'], with_ack=False,
+                self.energizerGW.config_gw(energy_pattern_val=self.tests_suite['additionalGW']['energizingPattern'],
+                                         time_profile_val=self.tests_suite['additionalGW']['timeProfile'],
+                                         output_power_val=self.tests_suite['additionalGW']['gw_output_power'],
+                                         bypass_pa_val=self.tests_suite['additionalGW']['bypass_pa'],with_ack=True,
                                            start_gw_app=False)
                 if 'sub1g_power' in self.tests_suite['additionalGW']:
                     self.energizerGW.config_gw(sub1g_output_power_val=self.tests_suite['additionalGW']['sub1g_power'],
-                                               start_gw_app=False)
+                                               with_ack=True, start_gw_app=False)
 
                 if 'gw_commands' in self.tests_suite['additionalGW']:
                     if len(self.tests_suite['additionalGW']['gw_commands']) > 0:
                         for command in self.tests_suite['additionalGW']['gw_commands']:
-                            self.energizerGW.write(command)
+                            self.energizerGW.write(command, with_ack=True)
                 if self.additional_gw_mode == DualGWMode.STATIC:
-                    self.energizerGW.write('!gateway_app')
+                    self.energizerGW.write('!gateway_app', with_ack=True)
 
         else:
             self.energizerGW = False
 
 
 
         # for Printer thread ###########
@@ -2043,15 +1987,14 @@
         self.R2R_myGPIO = R2rGpio()
 
     def open_printer_socket(self):
         """
         opens the printer socket
         """
         self.Printer_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self.Printer_socket.settimeout(PRINTER_SOCKET_TIMEOUT)
         self.Printer_socket.connect((self.configs_for_printer_values['TCP_IP'],
                                      int(self.configs_for_printer_values['TCP_PORT'])))
 
     def update_printer_gui_inputs(self):
         """
         save the last pass value for crash support.
         passed global variable will be updated at tag Thread and should be correct here
@@ -2352,30 +2295,29 @@
 
             if (self.printer is not None and not self.printer.exception_queue.empty()) or \
                     not self.tag_checker_thread.exception_queue.empty() or not self.r2r_thread.exception_queue.empty():
                 self.events.stop_to_r2r_thread.set()
                 self.handle_r2r_exception()
                 self.init_ok = False
 
+            if self.to_scan == 'Yes':
+                self.tag_comparing_qr = QRThread(self.events, self.ports_and_guis)
+
             self.events.tag_thread_is_ready_to_main.wait()
             self.events.tag_thread_is_ready_to_main.clear()
 
             self.pass_job_name = self.tag_checker_thread.printing_value['passJobName']  # will be set inside config
             self.to_print = self.tag_checker_thread.to_print
             self.start_value = int(self.tag_checker_thread.printing_value['firstPrintingValue'])
 
             # printer set-up ####################################################################
             # happens here so we will wait less until the printer will start up (will happen in the background)
             if self.to_print:
                 self.printer = Printer(self.start_value, self.pass_job_name, self.events, self.ports_and_guis)
                 self.look_for_exceptions()
-
-            if self.to_scan == 'Yes':
-                self.tag_comparing_qr = QRThread(self.events, self.ports_and_guis, print=self.to_print)
-
             self.gw_version = self.ports_and_guis.ver
             self.wiliot_ver = get_version()
             self.open_ui()  # starts recurring_timer() that starts look_for_exceptions()
             if self.init_ok:
                 self.r2r_thread.start()
                 self.tag_checker_thread.start()
                 self.events.tag_thread_is_ready_to_main.wait()
@@ -2389,17 +2331,14 @@
                         self.printer.start()
                     self.events.printer_event.wait()
                     if self.events.printer_success.isSet():
                         self.events.printer_success.clear()
                         msg = 'Printer is ready to start'
                         printing_func(msg, 'MainWindow', lock_print, logger_type='debug',
                                       logger_name=self.ports_and_guis.my_logger.logger.name)
-                else:
-                    if self.to_scan == 'Yes':
-                        self.tag_comparing_qr.start()
 
                 self.events.start_to_r2r_thread.set()
         except Exception:
             exception_details = sys.exc_info()
             msg = 'Exception detected during initialization:'
             try:
                 printing_func(msg, 'MainWindow', lock_print, logger_type='warning',
@@ -2624,19 +2563,18 @@
 
         res = None
         if values['upload'] == 'Yes':
             if tested > 0:
                 try:
                     res = upload_to_cloud_api(batch_name=reel_name, tester_type='offline-test',
                                               run_data_csv_name=self.ports_and_guis.my_logger.run_data_path,
-                                              packets_data_csv_name=self.ports_and_guis.my_logger.packets_data_path,
-                                              env=self.ports_and_guis.env,
-                                              owner_id=self.ports_and_guis.Tag_Value['OwnerId'],
+                                              tags_data_csv_name=self.ports_and_guis.my_logger.packets_data_path,
+                                              to_logging=True, env=self.ports_and_guis.env,
                                               logger_=self.ports_and_guis.my_logger.gw_logger.name, is_path=True,
-                                              client=self.client)
+                                              client=self.client, packets_instead_tags=True)
                     sleep(2)
                 except Exception:
                     exception_details = sys.exc_info()
                     print_exception(exception_details=exception_details, printing_lock=lock_print)
                     res = False
             else:
                 self.ports_and_guis.my_logger.results_logger.warning(
@@ -2908,14 +2846,17 @@
                     run_dict_list = [{k: v[0] for k, v in run_dict.items()}]
                     with open(self.ports_and_guis.my_logger.run_data_path, 'w', newline='') as f:
                         csv_writer = csv.DictWriter(f, run_dict.keys())
                         csv_writer.writeheader()
                         csv_writer.writerows(run_dict_list)
                         f.close()
 
+
+
+
 def set_attn_power_offline(attn_obj, attn_power, simulation=False):
     """
     configure Attenuator to a specific value
     gets:
         attn_obj:       Attenuator obj
         attn_power:     value to set attn
```

### Comparing `wiliot-testers-4.0.11/wiliot_testers/offline/offline_utils.py` & `wiliot-testers-4.0.6/wiliot_testers/offline/offline_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,16 +105,15 @@
                                        'batchName': 'test_reel',
                                        'tagGen': 'N/A',
                                        'inlayType': 'Ble_Test_Only', 'inlay': InlayTypes.TEO_086.value,
                                        'desiredTags': '9999999', 'desiredPass': '9999999',
                                        'surface': SurfaceTypes.AIR.value,
                                        'conversion': ConversionTypes.STANDARD.value, 'blackListAfter': '2',
                                        'Environment': 'production', 'OwnerId': 'wiliot-ops', 'operator': '',
-                                       'QRRead': 'No', 'QRcomport': 'COM3', 'QRoffset': '2', 'maxQRWrongTags': '1',
-                                       'QRtimeout': '200',
+                                       'QRRead': 'No', 'QRcomport': 'COM3', 'QRoffset': '2', 'maxQRWrongTags': '2',
                                        'comments': '', 'maxFailStop': '50', 'maxYieldStop': '40'}
         elif gui_type == 'Test':
             self.default_gui_values = {'passJobName': 'SGTIN_QR', 'passJobNum': 2, 'sgtin': 'test_test_test_test_X_',
                                        'stringBeforeCounter': 'test',
                                        'reelNumManually': 'test', 'firstPrintingValue': '0', 'tagLocation': '0',
                                        'tag_reel_location': '0',
                                        'enableLineSelection': 'No'}
@@ -331,17 +330,14 @@
                   SimGUI.Spin(values=[i for i in range(1, 15)], initial_value=(
                       int(gui_inputs_values['QRcomport'][-1]) if len(str(gui_inputs_values['QRcomport'])) > 1 else int(
                           gui_inputs_values['QRcomport'])),
                               size=(6, 1), key='QRcomport')],
                  [SimGUI.Text('QR offset (tags between GW and QR scanner):', size=(40, 1), visible=True),
                   SimGUI.Spin(values=[i for i in range(1, 10)], initial_value=int(gui_inputs_values['QRoffset']),
                               size=(6, 1), key='QRoffset')],
-                 [SimGUI.Text('QR Timeout:', size=(40, 1), visible=True),
-                  SimGUI.Spin(values=[i for i in range(100, 1000, 100)], initial_value=int(gui_inputs_values['QRtimeout']),
-                              size=(6, 1), key='QRtimeout')],
                  [SimGUI.Text('Max appears before entering black list (min=2)',
                               size=(40, 1)),
                   SimGUI.Spin(values=[i for i in range(1, 100)],
                               initial_value=int(
                                   gui_inputs_values['blackListAfter']),
                               size=(6, 1), key='blackListAfter')]]
 
@@ -439,16 +435,15 @@
                     reel_name_ver = check_structure(values['batchName'])
                 else:
                     reel_name_ver = True
 
                 if reel_name_ver:
                     break
                 else:
-                    SimGUI.popup('Reel name error \n Reel name should be: <6 uppercase alphanumeric chars>.'
-                                 '<2 integers minimum 01 maximum 25>_<upper case char minimum A maximum F>',
+                    SimGUI.popup('Reel name error \n Reel name should be: <6 uppercase alphanumeric chars>.<2 integers minimum 01 maximum 25>_<upper case char minimum A maximum F>'.format(values['printOffset']),
                                  button_type='ok', font=14)
 
         elif event == 'Advanced Calibration':
             # calib_val = True
             # break
             window.hide()
             calib_values = open_calibration_config()
```

### Comparing `wiliot-testers-4.0.11/wiliot_testers/offline/tadbik_r2r_controller.py` & `wiliot-testers-4.0.6/wiliot_testers/offline/tadbik_r2r_controller.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/sample/com_connect.py` & `wiliot-testers-4.0.6/wiliot_testers/sample/com_connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 from os.path import abspath
 from json import dump
 from os.path import join, dirname
 from wiliot_testers.test_equipment import *
 from wiliot_core import WiliotGateway, ActionType, DataType
 from configs_gui import CONFIGS_DIR
 
+logger = logging.getLogger('sample')
+
 barcodeMutex = threading.Lock()
 
 CONNECT_HW = 'Connect HW'
 GO = 'Go'
 CONTINUE = 'Continue'
 READ = 'Read'
 FINISH = 'Finish'
@@ -128,159 +130,154 @@
     barcode_error = []
     chambers_to_close = []
     gw_latest_version = ['']
     gw_update_status = 'disabled'
     start_time = 0
     temperature_sensor_readings = []
     all_sensors = []
-    ttk = None
-
-    def __init__(self, top_builder=None, new_tag_func=None, update_go=None, default_dict=None, logger=None):
+    
+    def __init__(self, top_builder=None, new_tag_func=None, update_go=None, default_dict=None):
         '''
         Constructor
         '''
         self.gateway = WiliotGateway(logger_name='sample')
         self.top_builder = top_builder
         self.add_tag_to_test = new_tag_func
         self.update_go_state = update_go
         self.default_dict = default_dict
-        if logger is None:
-            self.logger = logging.getLogger('sample')
-        else:
-            self.logger = logger
-
+    
     def __del__(self):
         if self.gateway is not None and self.is_gw_serial_open():
             self.gateway.close_port()
-
+        
         for com_port, barcode in self.barcodes_serials.items():
             if barcode is not None and barcode.is_open():
                 barcode.close_port()
-
+        
         for com_port, chamber in self.chambers_serials.items():
             if chamber is not None and chamber.is_connected():
                 chamber.open_chamber()
                 chamber.close_port()
-
+        
         # for com_port, atten in self.atten_serials.items():
         #     if atten!=None and 'serial' in atten.keys() and atten['serial']!=None and atten:
         #         atten.disconnect()
-
+    
     def gui(self, ttk_frame=None):
         self.builder = builder = pygubu.Builder()
         ui_file = join(abspath(dirname(__file__)), 'utils', 'com_connect.ui')
         self.builder.add_from_file(ui_file)
-
+        
         img_path = join(abspath(dirname(__file__)), '')
         builder.add_resource_path(img_path)
         img_path = join(abspath(dirname(__file__)), 'utils')
         builder.add_resource_path(img_path)
-
+        
         self.ttk = ttk_frame
-
+        
         self.ttk.title("ComConnect")
-
+        
         self.mainwindow = self.builder.get_object('mainwindow', self.ttk)
-
+        
         self.builder.connect_callbacks(self)
         self.isGui = True
         self.find_com_ports()
         self.set_gui_defaults()
-
+        
         self.ttk.protocol("WM_DELETE_WINDOW", self.close)
         self.ttk.lift()
         self.ttk.attributes("-topmost", True)
         self.ttk.attributes("-topmost", False)
-
+        
         # self.set_gui_defaults()
-
+        
         self.ttk.mainloop()
-
+    
     def find_com_ports(self, *args):
         com_ports = serial_ports()
         available_ports = [com_port for com_port in com_ports if com_port not in self.used_ports]
-
+        
         self.update_com_gui(available_ports, com_ports)
-
+    
     def set_gui_defaults(self):
-
+        
         if self.serials_connected(CHAMBERS):
             self.builder.get_object('connect_chambers').configure(text='Disconnect')
             self.builder.get_object('chosenChambers')['state'] = 'disabled'
             self.builder.get_object('availableChambers')['state'] = 'disabled'
             self.builder.get_object('chambers_up')['state'] = 'disabled'
             self.builder.get_object('chambers_down')['state'] = 'disabled'
             self.builder.get_object('addChambers')['state'] = 'disabled'
         else:
             self.builder.get_object('connect_chambers').configure(text='Connect')
-
+        
         ble_atten = ''
         lora_atten = ''
         for com_port, atten in self.atten_serials.items():
             ble_atten = com_port if atten['type'] == BLE else ble_atten
             lora_atten = com_port if atten['type'] == LORA else lora_atten
-
+        
         self.builder.get_object('attenComBle').set(ble_atten)
         self.builder.get_object('attenComLoRa').set(lora_atten)
         if self.serials_connected(ATTENUATORS):
             self.builder.get_object('connect_atten').configure(text='Disconnect')
             self.builder.get_object('attenComBle')['state'] = 'disabled'
             self.builder.get_object('attenComLoRa')['state'] = 'disabled'
         else:
             self.builder.get_object('connect_atten').configure(text='Connect')
         pass
-
+    
     def update_com_gui(self, available_ports, com_ports):
         self.builder.get_object('gwCom')['values'] = available_ports + ['']
         self.builder.get_object('attenComBle')['values'] = available_ports + ['']
         self.builder.get_object('attenComLoRa')['values'] = available_ports + ['']
         self.update_multi_serials(available_ports, BARCODES)
         self.update_multi_serials(available_ports, CHAMBERS)
-
+        
         self.missing_com_port = False
-
+        
         self.check_chosen_ports(com_ports)
         self.check_opened_ports()
-
+    
     def check_chosen_ports(self, com_ports):
         if len(self.gw_com_port) == 0 or self.gw_com_port[0] not in com_ports:
             self.gw_com_port = ['']
             self.builder.get_object('gwCom').set('')
             self.missing_com_port = True
-
+        
         i = 0
         while i < len(self.atten_serials.keys()):
             port = list(self.atten_serials.keys())[i]
             atten = list(self.atten_serials.values())[i]
             if port != '' and port not in com_ports:
                 self.atten_serials.pop(port)
                 self.builder.get_object(f"attenCom{atten['type']}").set('')
                 self.missing_com_port = True
                 continue
             i += 1
-
+        
         self.check_multi_coms(BARCODES, com_ports)
         self.check_multi_coms(CHAMBERS, com_ports)
-
+    
     def check_multi_coms(self, obj, com_ports):
         self.builder.get_object(f'chosen{obj}').delete(0, END)
         ports = getattr(self, f'{obj.lower()}_serials')
         for port in ports.keys():
             if port in com_ports:
                 self.builder.get_object(f'chosen{obj}').insert(END, port)
             else:
                 self.missing_com_port = True
-
+    
     def check_opened_ports(self):
         if self.is_gui_opened():
             self.check_gw_open()
             self.check_multi_open(BARCODES)
             self.check_multi_open(CHAMBERS)
             self.check_atten_open()
-
+    
     def check_multi_open(self, obj):
         if self.serials_connected(obj):
             self.builder.get_object(f'connect_{obj.lower()}').configure(text='Disconnect')
             self.builder.get_object(f'chosen{obj}')['state'] = 'disabled'
             self.builder.get_object(f'available{obj}')['state'] = 'disabled'
             self.builder.get_object(f'{obj.lower()}_up')['state'] = 'disabled'
             self.builder.get_object(f'{obj.lower()}_down')['state'] = 'disabled'
@@ -288,15 +285,15 @@
         else:
             self.builder.get_object(f'connect_{obj.lower()}').configure(text='Connect')
             self.builder.get_object(f'chosen{obj}')['state'] = 'normal'
             self.builder.get_object(f'available{obj}')['state'] = 'normal'
             self.builder.get_object(f'{obj.lower()}_up')['state'] = 'normal'
             self.builder.get_object(f'{obj.lower()}_down')['state'] = 'normal'
             self.builder.get_object(f'add{obj}')['state'] = 'normal'
-
+    
     def check_gw_open(self):
         if len(self.gw_com_port) > 0 and self.gw_com_port[0] != '':
             self.builder.get_object('gwCom').set(self.gw_com_port[0])
         if self.is_gw_serial_open():
             self.builder.get_object('connect_gw').configure(text='Disconnect')
             self.builder.get_object('gwCom')['state'] = 'disabled'
             self.builder.get_object('version').configure(text=GW_VERSION + self.gwVersion[0])
@@ -304,35 +301,34 @@
             self.builder.get_object('update_gw')['state'] = self.gw_update_status
         else:
             self.builder.get_object('connect_gw').configure(text='Connect')
             self.builder.get_object('gwCom')['state'] = 'normal'
             self.builder.get_object('version').configure(text=GW_VERSION)
             self.builder.get_object('latestVersion').configure(text=GW_AVAILABLE_VERSION)
             self.builder.get_object('update_gw')['state'] = 'disabled'
-
+    
     def check_atten_open(self):
         connected = False
         for com, atten in self.atten_serials.items():
             if atten['serial'] is not None and atten['serial'].GetActiveTE().is_open():
                 connected = True
         if connected:
             self.builder.get_object(f'connect_atten').configure(text='Disconnect')
             self.builder.get_object(f'attenComLoRa')['state'] = 'disabled'
             self.builder.get_object(f'attenComBle')['state'] = 'disabled'
         else:
             self.builder.get_object(f'connect_atten').configure(text='Connect')
             self.builder.get_object(f'attenComLoRa')['state'] = 'normal'
             self.builder.get_object(f'attenComBle')['state'] = 'normal'
 
-    def choose_com_ports(self):
-        default_dict = self.default_dict
+    def choose_com_ports(self, default_dict):
         com_ports = [s.device for s in tools.list_ports.comports()]
         if len(com_ports) == 0:
             com_ports = [s.name for s in tools.list_ports.comports()]
-
+        
         if 'gw' in default_dict.keys() and default_dict['gw'] in com_ports:
             self.gw_com_port = [default_dict['gw']]
             self.used_ports.append(default_dict['gw'])
         else:
             self.gw_com_port = ['']
             self.missing_com_port = True
         if 'atten' in default_dict.keys() and BLE in default_dict['atten'].keys() and default_dict['atten'][BLE] \
@@ -349,123 +345,123 @@
             self.atten_serials[default_dict['atten'][LORA]] = {}
             self.atten_serials[default_dict['atten'][LORA]]['type'] = LORA
             self.atten_serials[default_dict['atten'][LORA]]['serial'] = None
             self.used_ports.append(default_dict['atten'][LORA])
         elif 'atten' in default_dict.keys() and LORA in default_dict['atten'].keys() \
                 and default_dict['atten'][LORA].strip() != '':
             self.missing_com_port = True
-
+        
         if 'barcodes' in default_dict.keys():
             self.barcodes_serials = dict.fromkeys([barcode for barcode in default_dict['barcodes'] if barcode
                                                    in com_ports], None)
             self.used_ports += list(self.barcodes_serials.keys())
-
+        
         if 'chambers' in default_dict.keys():
             self.chambers_serials = dict.fromkeys([chamber for chamber in default_dict['chambers'] if chamber
                                                    in com_ports], None)
             self.used_ports += list(self.chambers_serials.keys())
 
         if 'temperature_sensors' in default_dict.keys():
             self.sensors_serials = dict.fromkeys([sensor for sensor in default_dict['temperature_sensors']], None)
-
+        
         missing_barcodes = []
         missing_chambers = []
         if 'barcodes' in default_dict.keys():
             missing_barcodes = [barcode for barcode in default_dict['barcodes'] if barcode not in com_ports]
         if 'chambers' in default_dict.keys():
             missing_chambers = [chamber for chamber in default_dict['chambers'] if chamber not in com_ports]
         if any(missing_barcodes + missing_chambers):
             self.missing_com_port = True
-
+        
         return self.missing_com_port
-
+    
     def choose_gw(self, *args):
         if len(self.gw_com_port) > 0 and self.gw_com_port[0] != '':
             self.used_ports.pop(self.used_ports.index(self.gw_com_port[0]))
         self.gw_com_port = [self.builder.get_object('gwCom').get()]
         self.used_ports.append(self.gw_com_port[0])
-
+    
     def choose_ble_atten(self, *args):
         ble_com = self.builder.get_object('attenComBle').get()
         ble_last_com = [com for com, item in self.atten_serials.items() if item['type'] == BLE]
         if len(ble_last_com) > 0:
             self.atten_serials.pop(ble_last_com[0])
             self.used_ports.pop(self.used_ports.index(ble_last_com[0]))
         if ble_com.strip() != '':
             self.atten_serials[ble_com] = {}
             self.atten_serials[ble_com]['type'] = BLE
             self.atten_serials[ble_com]['serial'] = None
             self.used_ports.append(ble_com)
-
+    
     def choose_lora_atten(self, *args):
         lora_com = self.builder.get_object('attenComLoRa').get()
         lora_last_com = [com for com, item in self.atten_serials.items() if item['type'] == LORA]
         if len(lora_last_com) > 0:
             self.atten_serials.pop(lora_last_com[0])
             self.used_ports.pop(self.used_ports.index(lora_last_com[0]))
         if lora_com.strip() != '':
             self.atten_serials[lora_com] = {}
             self.atten_serials[lora_com]['type'] = LORA
             self.atten_serials[lora_com]['serial'] = None
             self.used_ports.append(lora_com)
-
+    
     def connect_all(self, gui=True):
         if not self.is_gw_serial_open():
             success = self.connect_gw(gui)
             if not success:
                 return
         if not self.serials_connected(ATTENUATORS):
             self.connect_atten(gui)
         if not self.serials_connected(BARCODES):
             self.connect_barcodes(gui)
         if not self.serials_connected(CHAMBERS):
             self.connect_chambers(gui)
         self.connect_temperature_sensor()
         self.hwConnected = True
-
+    
     def connect_gw(self, gui=True, disconnect=False):
         if not self.is_gw_serial_open() and not disconnect:
             if len(self.gw_com_port) == 0 or self.gw_com_port[0].strip() == '':
-                self.popup_message('No default com port for GW, please choose GW com port.', title='Error', log='error')
+                popup_message('No default com port for GW, please choose GW com port.', title='Error', log='error')
                 return False
             com_port = self.gw_com_port[0]
             self.gateway.open_port(port=com_port, baud=921600)
             if self.is_gw_serial_open():
                 self.start_listener(not_print_str=True)
-                self.logger.info(f'GW is connected on port: {com_port}.')
+                logger.info(f'GW is connected on port: {com_port}.')
                 self.gateway.reset_gw()
                 sleep(1)
                 version = self.gateway.get_gw_version()
                 self.gwVersion = version
                 self.gw_latest_version = latest_version = self.gateway.get_latest_version_number()
                 cur_version = int(version[0].replace('.', ''))
                 self.gw_update_status = 'normal' if cur_version < int(latest_version[0].replace('.', '')) \
                     else 'disabled'
                 if cur_version >= int(GW_TBP_VERSION.replace('.', '')):
                     self.cur_gw_tbp_version = True
             else:
-                self.logger.error(f'Error connecting to GW on port: {com_port}.')
+                logger.error(f'Error connecting to GW on port: {com_port}.')
                 return False
         else:
             self.gateway.close_port()
             self.builder.get_object('connect_gw').configure(text='Connect')
             self.builder.get_object('version').configure(text=GW_VERSION)
             self.builder.get_object('latestVersion').configure(text=GW_AVAILABLE_VERSION)
             self.builder.get_object('gwCom')['state'] = 'normal'
         if gui:
             self.check_gw_open()
-
+        
         return True
-
+    
     def connect_barcodes(self, gui=True):
         self.connect_multi_serials(BARCODES, gui=gui)
-
+    
     def connect_chambers(self, gui=True):
         self.connect_multi_serials(CHAMBERS, gui=gui)
-
+    
     def connect_atten(self, gui=True):
         is_connected = self.connect_multi_serials(ATTENUATORS, gui=gui)
         if gui:
             atten_state = 'disabled' if is_connected else 'normal'
             self.builder.get_object('attenComLoRa')['state'] = atten_state
             self.builder.get_object('attenComBle')['state'] = atten_state
 
@@ -474,22 +470,22 @@
         self.temperature_sensor_readings = []
         for sensor_name in self.sensors_serials.keys():
             self.temperature_sensor_readings.append([])
             try:
                 sensor_temp = YoctoTemperatureSensor()
                 is_connected = sensor_temp.connect(target=sensor_name)
                 if is_connected:
-                    self.logger.info('Temperature Sensor {} is connected'.format(sensor_temp.get_sensor_name()))
+                    logger.info('Temperature Sensor {} is connected'.format(sensor_temp.get_sensor_name()))
                     self.all_sensors.append(sensor_temp)
                 else:
-                    self.logger.info('Could not connect to Temperature Sensor according to '
-                                     'the following name: {}'.format(sensor_name))
+                    logger.info('Could not connect to Temperature Sensor according to '
+                                'the following name: {}'.format(sensor_name))
                     self.all_sensors.append(None)
             except Exception as e:
-                self.logger.info('while connecting to the Temperature Sensor the following error occurs : {}'.format(e))
+                logger.info('while connecting to the Temperature Sensor the following error occurs : {}'.format(e))
                 self.all_sensors.append(None)
 
     def read_temperature_sensor(self):
         for i, sensor in enumerate(self.all_sensors):
             if sensor is not None:
                 self.temperature_sensor_readings[i].append(sensor.get_temperature())
 
@@ -517,15 +513,15 @@
                     self.builder.get_object(f'add{obj}')['state'] = 'disabled'
                 except:
                     pass
         if gui:
             self.find_com_ports()
         # self.update_go_state()
         return is_connected
-
+    
     def open_serials(self, obj, serials):
         threads = []
         for com_port, com_serial in serials.items():
             if 'barcode' in obj.lower():
                 if com_serial is not None and com_serial.is_open():
                     continue
                 com_serial = BarcodeScanner(com=com_port, log_type='LOG_NL')
@@ -543,166 +539,163 @@
                     # 8 if serial['serial']!=None and
                     # serial['serial'].GetActiveTE().s.is_open():
                     continue
                 com_serial = Attenuator('API', comport=com_port)
                 if com_serial.GetActiveTE().is_open():
                     # self.used_ports.append(com_port)
                     serials[com_port]['serial'] = com_serial
-
+        
         for thread in threads:
             thread.join()
-
+    
     def close(self):
         if self.is_gw_serial_open() and self.serials_connected(ATTENUATORS) and self.serials_connected(BARCODES):
             self.hwConnected = True
             self.enable_hw_connected()
         if self.isGui:
             self.isGui = False
             self.ttk.destroy()
         return self.hwConnected
-
+    
     def save(self):
         # default_dict = {}
         # if isfile(join(CONFIGS_DIR, '.defaults.json')):
         #     with open(join(CONFIGS_DIR, '.defaults.json'), 'r') as defaultComs:
         #         default_dict = load(defaultComs)
         self.default_dict['gw'] = self.gw_com_port[0]
         self.default_dict['atten'] = {}
         for com_port, atten in self.atten_serials.items():
             self.default_dict['atten'][atten['type']] = com_port
         self.default_dict['barcodes'] = list(self.barcodes_serials.keys())
         self.default_dict['chambers'] = list(self.chambers_serials.keys())
         with open(join(CONFIGS_DIR, '.defaults.json'), 'w+') as defaultComs:
             dump(dict(self.default_dict), defaultComs, indent=4)
-
-        self.logger.info(f'Com ports saved successfully.')
-
+        
+        logger.info(f'Com ports saved successfully.')
+    
     def focus_barcode_available(self, *args):
         self.focus_available(BARCODES)
-
+    
     def focus_barcode_chosen(self, *args):
         self.focus_chosen(BARCODES)
-
+    
     def focus_chamber_available(self, *args):
         self.focus_available(CHAMBERS)
-
+    
     def focus_chamber_chosen(self, *args):
         self.focus_chosen(CHAMBERS)
-
+    
     def focus_available(self, obj):
         self.builder.get_object(f'add{obj}').configure(text='>')
         setattr(self, f'{obj.lower()}_state', ADD)
-
+    
     def focus_chosen(self, obj):
         self.builder.get_object(f'add{obj}').configure(text='<')
         setattr(self, f'{obj.lower()}_state', REMOVE)
         setattr(self, f'{obj.lower()}_move_com', '')
-
+    
     def add_barcode(self):
         if getattr(self, f'{BARCODES.lower()}_state') == ADD:
             com_chosen = self.builder.get_object(f'available{BARCODES}').get(ACTIVE)
-            try:
-                temp_barcode = BarcodeScanner(com=com_chosen)
-            except Exception as e:
-                self.popup_message(f'Could NOT connect. {e}', title='Error', log='error')
+            temp_barcode = BarcodeScanner()
+            if not temp_barcode.check_com_port(com_chosen):
+                popup_message(f'{com_chosen} is not barcode scanner', title='Error', log='error')
         self.add(BARCODES)
         self.find_com_ports()
-
+    
     def add_chamber(self):
         self.add(CHAMBERS)
         self.find_com_ports()
-
+    
     def add(self, obj):
         if getattr(self, f'{obj.lower()}_state') == ADD:
             sending = self.builder.get_object(f'available{obj}')
             receiving = self.builder.get_object(f'chosen{obj}')
         else:
             sending = self.builder.get_object(f'chosen{obj}')
             receiving = self.builder.get_object(f'available{obj}')
-
+        
         com_list = list(sending.get(0, END))
         com_chosen = sending.get(ACTIVE)
         receiving.insert(END, com_chosen)
         com_index = com_list.index(com_chosen)
         sending.delete(com_index, com_index)
-
+        
         serials = getattr(self, f'{obj.lower()}_serials')
         com_ports = self.builder.get_object(f'chosen{obj}').get(0, END)
         old_ports = [port for port in serials.keys() if port not in com_ports]
         new_serials = dict(zip(com_ports, [None] * len(com_ports)))
         self.used_ports = [port for port in self.used_ports if port not in old_ports] + list(com_ports)
         setattr(self, f'{obj.lower()}_serials', new_serials)
-
+    
     def chamber_up(self):
         self.up(CHAMBERS)
-
+    
     def chamber_down(self):
         self.down(CHAMBERS)
-
+    
     def barcode_up(self):
         self.up(BARCODES)
-
+    
     def barcode_down(self):
         self.down(BARCODES)
-
+    
     def up(self, obj):
         com_list = list(self.builder.get_object(f'chosen{obj}').get(0, END))
         if getattr(self, f'{obj.lower()}_move_com') == '':
             chosen_com = self.builder.get_object(f'chosen{obj}').get(ACTIVE)
             setattr(self, f'{obj.lower()}_move_com', chosen_com)
         else:
             chosen_com = getattr(self, f'{obj.lower()}_move_com')
-        if chosen_com != '':
-            com_index = com_list.index(chosen_com)
-            if com_index > 0:
-                com_list.pop(com_list.index(chosen_com))
-                com_list.insert(com_index - 1, chosen_com)
-                self.builder.get_object(f'chosen{obj}').delete(0, END)
-                for com in com_list:
-                    self.builder.get_object(f'chosen{obj}').insert(END, com)
-                self.builder.get_object(f'chosen{obj}').select_set(com_index - 1)
-
+        com_index = com_list.index(chosen_com)
+        if com_index > 0:
+            com_list.pop(com_list.index(chosen_com))
+            com_list.insert(com_index - 1, chosen_com)
+            self.builder.get_object(f'chosen{obj}').delete(0, END)
+            for com in com_list:
+                self.builder.get_object(f'chosen{obj}').insert(END, com)
+            self.builder.get_object(f'chosen{obj}').select_set(com_index - 1)
+    
     def down(self, obj):
         com_list = list(self.builder.get_object(f'chosen{obj}').get(0, END))
         if getattr(self, f'{obj.lower()}_move_com') == '':
             chosen_com = self.builder.get_object(f'chosen{obj}').get(ACTIVE)
             setattr(self, f'{obj.lower()}_move_com', chosen_com)
         else:
             chosen_com = getattr(self, f'{obj.lower()}_move_com')
-        if chosen_com != '':
-            com_index = com_list.index(chosen_com)
-            if com_index < (len(com_list) - 1):
-                com_list.pop(com_list.index(chosen_com))
-                com_list.insert(com_index + 1, chosen_com)
-                self.builder.get_object(f'chosen{obj}').delete(0, END)
-                for com in com_list:
-                    self.builder.get_object(f'chosen{obj}').insert(END, com)
-                self.builder.get_object(f'chosen{obj}').select_set(com_index + 1)
-
+        com_index = com_list.index(chosen_com)
+        if com_index < (len(com_list) - 1):
+            com_list.pop(com_list.index(chosen_com))
+            com_list.insert(com_index + 1, chosen_com)
+            self.builder.get_object(f'chosen{obj}').delete(0, END)
+            for com in com_list:
+                self.builder.get_object(f'chosen{obj}').insert(END, com)
+            self.builder.get_object(f'chosen{obj}').select_set(com_index + 1)
+    
     def update_multi_serials(self, available_ports, obj):
         self.builder.get_object(f'available{obj}').delete(0, END)
         for port in available_ports:
             if port not in self.used_ports:
                 self.builder.get_object(f'available{obj}').insert(END, port)
-
+    
     def update_atten_serials(self, available_ports):
         for com, item in self.atten_serials.items():
             if item['serial'] is None or not item['serial'].is_open():
                 self.builder.get_object(f'attenCom{item["type"]}')['values'] = available_ports
             else:
                 self.builder.get_object(f'attenCom{item["type"]}').set(com)
-
+    
     def connect_chamber(self, com_port, serials):
         com_serial = Tescom(com_port)
         if com_serial.is_connected():
             # self.used_ports.append(com_port)
             serials[com_port] = com_serial
             if not com_serial.is_door_open():
                 com_serial.open_chamber()
-
+    
     def close_serials(self, obj, serials):
         if 'atten' in obj.lower():
             for serial in serials.values():
                 # serial['serial'].GetActiveTE.s.close_port()
                 if serial['serial'] is not None and serial['serial'].GetActiveTE().is_open():
                     serial['serial'].GetActiveTE().close_port()
                 serial['serial'] = None
@@ -710,15 +703,15 @@
         else:
             for com_serial in serials.values():
                 if 'chamber' in obj.lower():
                     com_serial.open_chamber()
                 com_serial.close_port()
                 # self.used_ports.remove(com_port)
                 # serials.pop(com_port)
-
+    
     def serials_connected(self, obj):
         serials = getattr(self, f'{obj.lower()}_serials')
         if 'atten' in obj.lower():
             serials = dict(zip(serials.keys(), [atten['serial'] for atten in serials.values()]))
         connected_serials = 0
         for com_port, com_serial in serials.items():
             if com_serial is not None:
@@ -730,246 +723,236 @@
                     connected_serials += 1
             # if com_port.strip()=='':
             #     connected_serials += 1
         if connected_serials > 0 and connected_serials == len(serials.keys()):
             return True
         else:
             return False
-
+    
     def get_data(self, actionType=ActionType.ALL_SAMPLE, dataType=DataType.PACKET_LIST):
         return self.gateway.get_packets(action_type=actionType, data_type=dataType)
-
-    def read_barcode(self, scanner_index=0, close_chamber=False, add_to_test=False, n_try=5):
-        if len(list(self.barcodes_serials.values())) == 0:
-            self.logger.error('Trying to read barcode but no scanner were connected')
-            return None, None
+    
+    def read_barcode(self, scanner_index=0, close_chamber=False, add_to_test=False):
         scanner = list(self.barcodes_serials.values())[scanner_index]
-        for i in range(n_try):
-            full_data, cur_id, reel_id, gtin = scanner.scan_ext_id()
-            if full_data is None and cur_id is None and reel_id is None and full_data is None:
-                continue
-            break
-
+        full_data, cur_id, reel_id, gtin = scanner.scan_ext_id(scanDur=5)
+        
         cur_id = cur_id if cur_id is not None else full_data
         reel_id = reel_id if reel_id is not None else full_data
         gtin = gtin if gtin is not None else ''
         if reel_id is not None:
             self.reel_id = reel_id
             self.gtin = gtin
         if cur_id is None:
             barcodeMutex.acquire()
             if close_chamber:
                 self.barcode_error.append(scanner_index)
             barcodeMutex.release()
             return None, None
-
+        
         if not close_chamber:
             reel_id_obj = self.top_builder.tkvariables.get('reelId')
             reel_id_obj.set(self.reel_id)
-
+        
         else:
             success = self.add_tag_to_test(cur_id, reel_id, scanner_index=scanner_index, add_to_test=add_to_test)
             if success:
                 self.chambers_to_close.append(scanner_index)
-
+        
         return cur_id, reel_id
-
+    
     def read_scanners_barcodes(self, indexes=()):
         if len(indexes) == 0:
             indexes = list(range(len(self.barcodes_serials.values())))
         scanner_threads = []
         self.barcode_error = []
         self.chambers_to_close = []
-
+        
         for i in indexes:
             t = threading.Thread(target=self.read_barcode, args=(i, True, True))
             scanner_threads.append(t)
             t.start()
         for i in range(len(scanner_threads)):
             t = scanner_threads[i]
             t.join()
-
+        
         read_message = ''
         title = 'Warning'
         font = 18
         if len(self.barcode_error) > 0:
             read_message += f'Error reading external ID from chambers {self.barcode_error}, try repositioning the tags.\n'
             title = 'Error'
             font = 16
-
+        
         if len(self.chambers_to_close) > 0:
             read_message += f'Chambers are closing!!\nWatch your hands!!!'
-
-        popupThread = threading.Thread(target=self.popup_message,
+        
+        popupThread = threading.Thread(target=popup_message,
                                        args=(read_message, title, ("Helvetica", font), title.lower()))
         popupThread.start()
         popupThread.join()
-
+        
         if len(self.chambers_to_close) > 0:
             self.close_chambers(self.chambers_to_close)
-
+        
         self.update_go_state()
-
+    
     def enable_hw_connected(self):
         self.top_builder.get_object('read_qr')['state'] = 'normal'
         self.top_builder.get_object('reelId')['state'] = 'normal'
         if self.top_builder.tkvariables.get('go').get() == CONNECT_HW:
             self.top_builder.tkvariables.get('go').set(READ)
             self.top_builder.get_object('go')['state'] = 'disabled'
-
+    
     def send_gw_app(self, params):
         str_rsp = []
         self.gateway.reset_buffer()
         self.gateway.clear_rsp_str_input_q()
-
+        
         self.gateway.reset_start_time()
-
+        
         for param, value in params.items():
             if param.startswith(ATTENUATION):
                 for com_port, atten in self.atten_serials.items():
                     if param.lower().endswith(atten['type'].lower()):
                         try:
                             attenuation = atten['serial'].GetActiveTE().Setattn(float(value))
-                            self.logger.info(f"{atten['type']} Attenuation set to: {str(attenuation).strip()}")
-                        except Exception as e:
-                            self.logger.error(f"{atten['type']} Attenuator error: try reconnect the attenuator [{e}].")
+                            logger.info(f"{atten['type']} Attenuation set to: {str(attenuation).strip()}")
+                        except:
+                            logger.error(f"{atten['type']} Attenuator error: try reconnect the attenuator.")
                             return False
-
+        
         self.start_time = time()
         try:
-            str_rsp.append(self.gateway.write('!sub1g_sync 1', with_ack=True))
             str_rsp.append(self.gateway.write('!listen_to_tag_only 1', with_ack=True))
             str_rsp.append(self.gateway.write('!set_tester_mode 1', with_ack=True))
             if 'EmulateSurfaceValue' in params.keys():
                 str_rsp.append(self.gateway.write('!set_sub_1_ghz_energizing_frequency {}'.format(
                     params['EmulateSurfaceValue']), with_ack=True))
             _, gw_ans = self.gateway.config_gw(effective_output_power_val=22, sub1g_output_power_val=29,
                                                energy_pattern_val=params['pattern'], received_channel=params['channel'],
                                                time_profile_val=[params['tOn'], params['tTotal']], start_gw_app=True,
                                                filter_val=False, pacer_val=0,
                                                with_ack=True)
             for rsp in gw_ans:
                 str_rsp.append(rsp)
-
-        except Exception as e:
-            self.logger.error(f'Gateway error: try reconnect the gateway [{e}].')
+        
+        except:
+            logger.error(f'Gateway error: try reconnect the gateway.')
             self.cancel_gw_commands()
             return False
-
+        
         for command in str_rsp:
             if "Command Complete Event" not in command['raw'] and "Energizing" not in command['raw']:
-                self.logger.error(f'Gateway response: {command["raw"]}')
+                logger.error(f'Gateway response: {command["raw"]}')
                 self.cancel_gw_commands()
                 return False
-
+        
         return True
-
+    
     def connect_and_close(self):
         self.connect_all()
         self.close()
-
+    
     def get_reel_id(self):
         return self.reel_id
-
+    
     def get_gtin(self):
         return self.gtin
-
+    
     def get_reel_external(self):
         return self.gtin + self.reel_id
-
+    
     def is_gw_serial_open(self):
         serial_open, _, _ = self.gateway.get_connection_status()
         return serial_open
-
+    
     def is_gw_data_available(self):
         return self.gateway.is_data_available()
-
+    
     def is_gui_opened(self):
         return self.isGui
-
+    
     def get_gw_version(self):
         return self.gwVersion[0]
-
+    
     def update_gw(self):
         self.gateway.update_version()
-
+    
     def get_gw_time(self):
         return self.start_time
-
+    
     def cancel_gw_commands(self):
         # self.gateway.write(GW_CANCEL)
         self.gateway.reset_gw()
         # self.gateway.stop_continuous_listener()
         # self.gateway.reset_buffer()
         sleep(0.1)
-
+    
     def start_listener(self, not_print_str=True):
         # self.gateway.start_continuous_listener(not_print_str)
         self.gateway.start_continuous_listener()
-
+    
     def is_hw_connected(self):
         return self.hwConnected
-
+    
     def get_chambers(self):
         return list(self.chambers_serials.values())
-
+    
     def open_chambers(self, indexes=()):
         chambers_threads = []
         chambers = list(self.chambers_serials.values())
         if len(indexes) == 0:
             indexes = list(range(len(chambers)))
         for index in indexes:
             if len(chambers) > index and chambers[index] is not None:
                 temp_thread = Thread(target=chambers[index].open_chamber, args=())
                 temp_thread.start()
                 chambers_threads.append(temp_thread)
-
+        
         for thread in chambers_threads:
             thread.join()
-
+    
     def close_chambers(self, indexes=()):
         chambers = list(self.chambers_serials.values())
         chambers_threads = []
         if len(indexes) == 0:
             indexes = list(range(len(chambers)))
         for index in indexes:
             if len(chambers) > index and chambers[index] is not None:
                 t = threading.Thread(target=chambers[index].close_chamber, args=())
                 chambers_threads.append(t)
                 t.start()
         for thread in chambers_threads:
             thread.join()
-
+    
     def get_num_of_barcode_scanners(self):
         return len(self.barcodes_serials.keys())
-
+    
     def get_error_barcode(self):
         return self.barcode_error
-
+    
     def gw_tbp_version(self):
         return self.cur_gw_tbp_version
-
+    
     def gw_get_packets(self):
         self.gateway.get_packets(action_type=ActionType.ALL_SAMPLE, data_type=DataType.PROCESSED)
-
+    
     def get_default_dict(self):
         return self.default_dict
 
-    def popup_message(self, msg, title='Error', font=("Helvetica", 10), log='info', bg=None, tk_frame=None):
-        if tk_frame:
-            popup = Toplevel(tk_frame)
-        else:
-            popup = Tk()
-        popup.eval('tk::PlaceWindow . center')
-        popup.wm_title(title)
-        if bg is not None:
-            popup.configure(bg=bg)
-        getattr(self.logger, log)(f'{title} - {msg}')
-
-        def popup_exit():
-            popup.destroy()
-
-        label = Label(popup, text=msg, font=font)
-        label.pack(side="top", fill="x", padx=10, pady=10)
-        b1 = Button(popup, text="Okay", command=popup_exit)
-        b1.pack(padx=10, pady=10)
-        popup.mainloop()
+
+def popup_message(msg, title='Error', font=("Helvetica", 10), log='info', bg=None):
+    popup = Tk()
+    popup.eval('tk::PlaceWindow . center')
+    popup.wm_title(title)
+    if bg is not None:
+        popup.configure(bg=bg)
+    getattr(logger, log)(f'{title} - {msg}')
+    
+    def popup_exit():
+        popup.destroy()
+    
+    label = Label(popup, text=msg, font=font)
+    label.pack(side="top", fill="x", padx=10, pady=10)
+    b1 = Button(popup, text="Okay", command=popup_exit)
+    b1.pack(padx=10, pady=10)
+    popup.mainloop()
```

### Comparing `wiliot-testers-4.0.11/wiliot_testers/sample/configs/.default_test_configs.json` & `wiliot-testers-4.0.6/wiliot_testers/sample/configs/.default_test_configs.json`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/sample/configs_gui.py` & `wiliot-testers-4.0.6/wiliot_testers/sample/configs_gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,23 +67,24 @@
 from wiliot_core import WiliotDir
 from wiliot_testers.utils.get_version import get_version
 
 VER = get_version()
 MEASURED = {'button': 'Measured', 'label': '[meter]'}
 MANUAL = {'button': 'Manual', 'label': '[db]'}
 DEFAULT_EMULATED_SURFACE = 'no simulation'
+logger = logging.getLogger('sample')
 
 wiliot_env = WiliotDir()
-sample_test_dir = abspath(join(wiliot_env.get_common_dir(), 'sample_test'))
-OUTPUT_DIR = abspath(join(sample_test_dir, 'logs'))
-CONFIGS_DIR = abspath(join(sample_test_dir, 'configs'))
-if not isdir(abspath(join(OUTPUT_DIR))):
-    makedirs(abspath(join(OUTPUT_DIR)))
-if not isdir(abspath(join(CONFIGS_DIR))):
-    makedirs(abspath(join(CONFIGS_DIR)))
+sample_test_dir = join(wiliot_env.get_common_dir(), 'sample_test')
+OUTPUT_DIR = join(sample_test_dir, 'logs')
+CONFIGS_DIR = join(sample_test_dir, 'configs')
+if not isdir(join(OUTPUT_DIR)):
+    makedirs(join(OUTPUT_DIR))
+if not isdir(join(CONFIGS_DIR)):
+    makedirs(join(CONFIGS_DIR))
 
 
 class ConfigsGui(object):
     '''
     classdocs
     '''
     isGui = False
@@ -97,38 +98,38 @@
     all_configs_fields = []
     
     def __init__(self, top_builder=None):
         '''
         Constructor
         '''
         self.top_builder = top_builder
-        self.config_path = abspath(join(dirname(__file__), 'configs', '.default_test_configs.json'))
+        self.config_path = join(dirname(__file__), 'configs', '.default_test_configs.json')
         if isfile(self.config_path):
             with open(self.config_path, 'r') as jsonFile:
                 self.configsDict = load(jsonFile)
                 if len(self.configsDict):
                     self.all_configs_fields = list(self.configsDict[next(iter(self.configsDict))].keys())
             self.fix_antenna_type()
 
-        with open(abspath(join(dirname(__file__), 'configs', '.default_surfaces.json')), 'r') as jsonFile:
+        with open(join(dirname(__file__), 'configs', '.default_surfaces.json'), 'r') as jsonFile:
             self.defaultSurfacesDict = load(jsonFile)
 
         self.copy_config_file()
 
     def copy_config_file(self):
-        copyfile(self.config_path, abspath(join(CONFIGS_DIR, f'.default_test_configs(ViewOnly)_{VER}.json')))
+        copyfile(self.config_path, join(CONFIGS_DIR, f'.default_test_configs(ViewOnly)_{VER}.json'))
 
     def gui(self, ttk_frame=None):
         self.builder = builder = pygubu.Builder()
-        ui_file = abspath(join(abspath(dirname(__file__)), 'utils', 'configs.ui'))
+        ui_file = join(abspath(dirname(__file__)), 'utils', 'configs.ui')
         self.builder.add_from_file(ui_file)
         
-        img_path = abspath(join(abspath(dirname(__file__)), ''))
+        img_path = join(abspath(dirname(__file__)), '')
         builder.add_resource_path(img_path)
-        img_path = abspath(join(abspath(dirname(__file__)), 'utils'))
+        img_path = join(abspath(dirname(__file__)), 'utils')
         builder.add_resource_path(img_path)
         
         self.ttk = ttk_frame
         
         self.ttk.title("Sample Test Configs")
         
         self.mainwindow = self.builder.get_object('mainwindow', self.ttk)
@@ -176,14 +177,21 @@
         ble_label = self.builder.tkvariables.get('attenBleLabel')
         ble_label.set(ble_label.get().split()[0] + ' ' + self.atten_cur_mode['label'])
         lora_label = self.builder.tkvariables.get('attenLoRaLabel')
         lora_label.set(lora_label.get().split()[0] + ' ' + self.atten_cur_mode['label'])
     
     def close(self):
         self.isGui = False
+        for param in self.all_configs_fields:
+            if self.builder.tkvariables.get(param) is not None:
+                value = self.builder.tkvariables.get(param).get()
+                self.paramDict[param] = value
+                self.configsDict[self.config][param] = value
+                if param == 'EmulateSurface':
+                    self.paramDict['EmulateSurfaceValue'] = self.defaultSurfacesDict['EmulateSurface'][value]
         self.ttk.destroy()
     
     def is_gui_opened(self):
         return self.isGui
     
     def get_params(self):
         return self.paramDict
@@ -238,17 +246,16 @@
         self.top_builder.get_object('test_config')['values'] = [key for key, item in self.configsDict.items()
                                                                 if isinstance(item, dict)]
         self.top_builder.get_object('test_config').set(config)
         
         with open(self.config_path, 'w+') as jsonFile:
             dump(self.configsDict, jsonFile, indent=4)
         self.copy_config_file()
-
-        self.set_params(config)
-        print(f'{config} configuration saved successfully.')
+        
+        logger.info(f'{config} configuration saved successfully.')
     
     def reset(self):
         def_dict = deepcopy(self.defaultConfigsDict)
         self.configsDict.update(def_dict)
         self.set_gui_defaults()
     
     def test_time_update(self, *args):
```

### Comparing `wiliot-testers-4.0.11/wiliot_testers/sample/get_temperature_sensor_name.py` & `wiliot-testers-4.0.6/wiliot_testers/sample/get_temperature_sensor_name.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/sample/sample_test.py` & `wiliot-testers-4.0.6/wiliot_testers/sample/sample_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,28 +67,37 @@
 import pygubu
 from threading import Thread, Lock
 from time import sleep
 import time
 import csv
 import datetime
 from wiliot_testers.sample.configs_gui import ConfigsGui, OUTPUT_DIR, CONFIGS_DIR
-from wiliot_testers.sample.com_connect import ComConnect, GO, CONTINUE, CONNECT_HW, READ, SEND
+from wiliot_testers.sample.com_connect import ComConnect, GO, CONTINUE, CONNECT_HW, READ, SEND, \
+    popup_message
 from traceback import print_exc
 from json import load, dump
 import argparse
 import sys
 from os.path import isfile, abspath, dirname, join, isdir, exists
 from wiliot_testers.utils.get_version import get_version
 # sys.path.append(abspath(dirname(join('..', '..', '..', '..', 'pywiliot_internal'))))
 from wiliot_testers.tester_utils \
     import setLogger, changeFileHandler, removeFileHandler, CsvLog, HeaderType, TesterName, StreamToLogger
 from wiliot_core import TagCollection, PacketList
-from wiliot_core import check_user_config_is_ok, InlayTypes, WiliotDir
+from wiliot_core import check_user_config_is_ok, InlayTypes
 from wiliot_api import ManufacturingClient
-from wiliot_testers.utils.upload_to_cloud_api import *
+from wiliot_testers.tester_utils import upload_to_cloud_api
+
+LOG_LEVEL = 'INFO'
+
+# default_log_file = join(abspath(dirname(__file__)), 'SampleTest.log')
+default_log_file = join(OUTPUT_DIR, 'SampleTest.log')
+logger = setLogger('sample', LOG_LEVEL, outputFile=default_log_file, file_mode='a+')
+sys.stdout = StreamToLogger(logger, logging.INFO)
+sys.stderr = StreamToLogger(logger, logging.ERROR)
 
 addToDictMutex = Lock()
 calibMutex = Lock()
 recvDataMutex = Lock()
 timerMutex = Lock()
 mutex = Lock()
 
@@ -158,108 +167,87 @@
     add_to_dict_threads = []
     unknown_packets = PacketList()
     antenna = ''
     low = 0
     high = 0
     step = 1
     n_repetitions = 1
-    logger = logging.getLogger('sample')
-
+    
     # numOfTags = ''
     multiTag = TagCollection()
     
     def __init__(self, calib=None, environment='', post_data=True, offline=False):
-
-        self.set_logger()
+        
         self.calib = calib
         self.offline = offline
         self.offline_tag_index = 0
         self.environment = environment
         self.post_data = post_data
         if self.offline:
             self.post_data = False
 
         self.pywiliot_version = get_version()
-        self.logger.info(f'PyWiliot version: {self.pywiliot_version}')
+        logger.info(f'PyWiliot version: {self.pywiliot_version}')
         
-        if isfile(abspath(join(CONFIGS_DIR, '.defaults.json'))):
-            with open(abspath(join(CONFIGS_DIR, '.defaults.json')), 'r') as defaultComs:
+        if isfile(join(CONFIGS_DIR, '.defaults.json')):
+            with open(join(CONFIGS_DIR, '.defaults.json'), 'r') as defaultComs:
                 self.defaultDict = load(defaultComs)
 
         self.popup_login()
         
         self.builder = builder = pygubu.Builder()
         
         self.comConnect = ComConnect(top_builder=builder, new_tag_func=self.add_tag_to_test,
-                                     update_go=self.update_go_state, default_dict=self.defaultDict, logger=self.logger)
+                                     update_go=self.update_go_state, default_dict=self.defaultDict)
         self.update_data()
         if not self.offline:
             _, api_key, is_success = check_user_config_is_ok(env='prod', owner_id=self.owner)
             if not is_success:
-                self.logger.warning('invalid User credential')
+                logger.warning('invalid User credential')
                 return
             self.client = ManufacturingClient(api_key=api_key, logger_='root')
         self.configsGui = ConfigsGui(top_builder=builder)
-        self.logger.info(f'Sample test is up and running')
-
-    def set_logger(self):
-        formatter = logging.Formatter('%(asctime)s,%(msecs)d %(name)s %(levelname)s: %(message)s', '%Y-%m-%d %H:%M:%S')
-        stream_handler = logging.StreamHandler()
-        stream_handler.setLevel(logging.DEBUG)
-        stream_handler.setFormatter(formatter)
-        wiliot_dir = WiliotDir()
-        logger_path = abspath(join(wiliot_dir.get_wiliot_root_app_dir(), 'sample_test'))
-        if not isdir(logger_path):
-            os.mkdir(logger_path)
-        logger_path = abspath(join(logger_path, 'logs'))
-        if not isdir(logger_path):
-            os.mkdir(logger_path)
-        logger_name = 'sample_test_{}.log'.format(datetime.datetime.now().strftime('%Y%m%d_%H%M%S'))
-        self.logger_path = abspath(join(logger_path, logger_name))
-        file_handler = logging.FileHandler(self.logger_path, mode='a')
-        file_formatter = logging.Formatter('%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s', '%H:%M:%S')
-        file_handler.setFormatter(file_formatter)
-        self.logger.addHandler(file_handler)
-        self.logger.addHandler(stream_handler)
-        self.logger.setLevel(logging.INFO)
-
+    
     def gui(self):
-        self.logger.info(f'Sample test setting the GUI')
         self.set_gui()
-        self.logger.info(f'Sample test GUI is running')
+        
         self.ttk.mainloop()
     
     def set_gui(self):
-        uifile = abspath(join(abspath(dirname(__file__)), 'utils', 'sample_test.ui'))
+        uifile = join(abspath(dirname(__file__)), 'utils', 'sample_test.ui')
         self.builder.add_from_file(uifile)
-
-        img_path = abspath(join(abspath(dirname(__file__)), ''))
+        
+        img_path = join(abspath(dirname(__file__)), '')
         self.builder.add_resource_path(img_path)
-        img_path = abspath(join(abspath(dirname(__file__)), 'utils'))
+        img_path = join(abspath(dirname(__file__)), 'utils')
         self.builder.add_resource_path(img_path)
-
+        
+        missing_com_port = self.comConnect.choose_com_ports(self.defaultDict)
+        
+        if missing_com_port:
+            popup_message('All or some of the default com ports are not available, '
+                          'please check connections.', title='Warning', log='warning')
+        
         self.ttk = Tk()
 
         self.ttk.title("Wiliot Sample Test")
         self.mainWindow = self.builder.get_object('mainwindow', self.ttk)
         self.ttk.protocol("WM_DELETE_WINDOW", self.close)
         self.builder.connect_callbacks(self)
-
+        
         self.builder.get_object('reelId').bind("<Key>", self.get_reel_id)
         list_box = self.builder.get_object('scanned')
         scrollbar = self.builder.get_object('scrollbar1')
         list_box.configure(yscrollcommand=scrollbar.set)
         scrollbar.configure(command=list_box.yview)
         self.builder.get_object('scrollbar1').set(self.builder.get_object('scanned').index(ACTIVE),
                                                   self.builder.get_object('scanned').index(END))
-        self.logger.info(f'checking available serial connection')
-        self.comConnect.choose_com_ports()
-        self.logger.info(f'setting up gui defaults')
+        
         self.set_gui_defaults()
-
+    
     def choose_param(self, *args):
         var = args[0].widget['style'].split('.')[0]
         if self.builder.tkvariables.get(var) is not None:
             value = self.builder.get_object(var).get()
             if var not in self.defaultDict.keys():
                 self.defaultDict[var] = []
             if value in self.defaultDict[var]:
@@ -299,60 +287,60 @@
             self.advas_dict = {}
             self.builder.tkvariables.get('stop').set(STOP)
             self.stopButtonState = STOP
             # self.numOfTags = int(self.builder.tkvariables.get('numTags').get())
             self.testId = testId = time.time()
             self.testName = testName = self.builder.get_object('testName').get()
             # self.operator = operator = self.builder.get_object('operator').get()
-            if not isdir(abspath(join(OUTPUT_DIR, testName))):
-                makedirs(abspath(join(OUTPUT_DIR, testName)))
+            if not isdir(join(OUTPUT_DIR, testName)):
+                makedirs(join(OUTPUT_DIR, testName))
             self.testDir = testDir = datetime.datetime.fromtimestamp(testId).strftime('%d%m%y_%H%M%S')
-            mkdir(abspath(join(OUTPUT_DIR, testName, testDir)))
+            mkdir(join(OUTPUT_DIR, testName, testDir))
             self.common_run_name = common_run_name = self.reel_id + '_' + testDir
-            self.test_log_file = abspath(join(OUTPUT_DIR, testName, testDir, f'{common_run_name}.log'))
-            changeFileHandler(self.logger, self.test_log_file, append_handler=True)
-            self.logger.info(f'Starts new test: {common_run_name}')
-            removeFileHandler(self.logger, self.logger_path)
+            self.test_log_file = join(OUTPUT_DIR, testName, testDir, f'{common_run_name}.log')
+            changeFileHandler(logger, self.test_log_file, append_handler=True)
+            logger.info(f'Starts new test: {common_run_name}')
+            removeFileHandler(logger, default_log_file)
             self.update_params()
             self.testStartTime = time.time()
             self.comConnect.read_temperature_sensor()  # read temperature
             if self.calib:
                 self.calibModeThread = Thread(target=self.calib_thread, args=())
                 self.calibModeThread.start()
                 self.calibModeThread.join()
                 self.calibModeThread = Thread(target=self.calib_mode, args=())
                 self.calibModeThread.start()
             else:
                 self.sendCommandThread = Thread(target=self.send_gw_commands, args=())
                 self.sendCommandThread.start()
-
+        
         elif goButtonState == CONTINUE:
             self.builder.tkvariables.get('stop').set(STOP)
             self.stopButtonState = STOP
             self.total_bad_advas.extend(x for x in self.bad_advas if x not in self.total_bad_advas)
             self.bad_advas = []
             self.advas_dict = {}
             self.sendCommandThread = Thread(target=self.send_gw_commands, args=())
             self.sendCommandThread.start()
-
+    
     def calib_thread(self):
         self.popup_calib()
-
+    
     def read_scanners_barcodes(self, indexes):
         self.comConnect.read_scanners_barcodes(indexes)
         # self.update_params_state(state='normal', group=CONTINUE)
-
+    
     def connect_all(self, gui=True):
         self.comConnect.connect_all(gui=gui)
         self.builder.tkvariables.get('go').set(READ)
         # self.update_params_state(state='normal', group=READ)
         self.builder.get_object('read_qr')['state'] = 'normal'
         self.builder.get_object('reelId')['state'] = 'normal'
         self.builder.get_object('connect')['state'] = 'normal'
-
+    
     def add_tag_to_test(self, cur_id, reel_id, scanner_index=0, add_to_test=False):
         mutex.acquire()
         if cur_id not in self.test_barcodes.keys() and cur_id not in self.barcodes_read.keys() and add_to_test:
             self.barcodes_read[cur_id] = {'chamber': scanner_index,
                                           'packets': [],
                                           'reel': self.reel_id,
                                           'ext ID': cur_id,
@@ -362,42 +350,42 @@
                                           'adv_address': [],
                                           'packetList': PacketList()}
             # self.test_barcodes[cur_id] = scanner_index
             self.builder.get_object('scanned').insert(END, f'{cur_id}, {scanner_index}')
             mutex.release()
         else:
             mutex.release()
-            self.comConnect.popup_message(f'Tag {cur_id} in chamber {scanner_index} already read.', title='Warning', log='warning')
+            popup_message(f'Tag {cur_id} in chamber {scanner_index} already read.', title='Warning', log='warning')
             return False
 
         if self.reel_id != '' and self.reel_id != reel_id and self.wiliotTags:
-            self.comConnect.popup_message('Tag reel different from test reel.', title='Warning', log='error')
-
+            popup_message('Tag reel different from test reel.', title='Warning', log='error')
+        
         return True
-
+    
     def update_go_state(self, force_go=False):
         if (self.comConnect.get_num_of_barcode_scanners() == len(self.barcodes_read.keys()) or force_go) and \
                 len(self.test_barcodes.keys()) > 0:
             self.builder.tkvariables.get('go').set(CONTINUE)
             self.update_params_state(state='normal', group=CONTINUE)
         elif self.comConnect.get_num_of_barcode_scanners() == len(self.barcodes_read.keys()) or force_go:
             self.builder.tkvariables.get('go').set(GO)
             self.update_params_state(state='normal', group=GO)
         else:
             self.builder.tkvariables.get('go').set(READ)
             self.update_params_state(state='normal', group=READ)
         # self.top_builder.get_object('go')['state'] = 'normal'
-
+    
     def get_missing_ids_chambers(self):
         indexes = list(range(self.comConnect.get_num_of_barcode_scanners()))
         if len(self.barcodes_read.keys()) > 0:
             used_indexes = [barcode['chamber'] for barcode in self.barcodes_read.values()]
             indexes = [index for index in indexes if index not in used_indexes]
         return indexes
-
+    
     def force_go(self):
         """
         enable go in the GUI even if some of the chambers are empty
         """
         if self.builder.get_variable('forceGo').get() == '1':
             self.builder.get_object('forceGo')['state'] = 'disabled'
             self.builder.get_object('stop')['state'] = 'disabled'
@@ -406,23 +394,23 @@
             self.builder.get_object('remove')['state'] = 'disabled'
             if self.closeChambersThread is not None and self.closeChambersThread.is_alive():
                 self.closeChambersThread.join()
             self.closeChambersThread = Thread(target=self.force_go_close_chambers, args=())
             self.closeChambersThread.start()
         else:
             self.update_go_state()
-
+    
     def force_go_close_chambers(self):
         indexes = self.get_missing_ids_chambers()
         self.comConnect.close_chambers(indexes)
         self.update_go_state(force_go=True)
         self.builder.get_object('forceGo')['state'] = 'normal'
         self.builder.get_object('stop')['state'] = 'normal'
         self.builder.get_object('go')['state'] = 'normal'
-
+    
     def calib_mode(self):
         self.testFinished = False
         attenuations = numpy.arange(float(self.low), float(self.high) + float(self.step), float(self.step))
         n_rep = int(self.n_repetitions)
         for i in attenuations:
             for j in range(n_rep):
                 calibMutex.acquire()
@@ -445,44 +433,43 @@
 
                 self.sendCommandThread = Thread(target=self.send_gw_commands, args=())
                 self.sendCommandThread.start()
                 self.sendCommandThread.join()
                 sleep(5)
                 if self.forceCloseRequested:
                     break
-
+        
         calibMutex.acquire()
         self.calib_mode_post_process()
         self.comConnect.open_chambers()
         # self.builder.tkvariables.get('numTags').set(0)
         # self.builder.tkvariables.get('go').set(READ)
         # self.test_barcodes = {}
         # self.builder.get_object('connect')['state'] = 'normal'
         # self.builder.get_object('read_qr')['state'] = 'normal'
         calibMutex.release()
         self.finish_test(post_data=False, reset_tester=True, post_process=False)
-        self.comConnect.popup_message('Sample Test - Calib Mode Finished running.', title='Info', log='info')
-
+        popup_message('Sample Test - Calib Mode Finished running.', title='Info', log='info')
+    
     def calib_mode_post_process(self):
         common_run_name = self.reel_id + '_' + self.testDir
         unique_valid = []
-        full_test_dir = abspath(join(OUTPUT_DIR, self.testName, self.testDir))
+        full_test_dir = join(OUTPUT_DIR, self.testName, self.testDir)
         is_first = True
         for atten, runData in self.packets_dict.items():
             for extId, data in runData.items():
                 if data['packetList'].size() > 0:
                     packet_df = data['packetList'].get_df(add_sprinkler_info=True)
                     packet_df.insert(loc=len(packet_df.columns), column='status', value='PASSED')
                     packet_df.insert(loc=len(packet_df.columns), column='attenuation', value=float(atten.split('_')[0]))
                     packet_df.insert(loc=len(packet_df.columns), column='test_num', value=int(atten.split('_')[1]))
                     packet_df.insert(loc=len(packet_df.columns), column='external_id', value=extId)
                     packet_df.insert(loc=len(packet_df.columns), column='chamber', value=data['chamber'])
                     data['packetList'].export_packet_df(
-                        packet_df=packet_df,
-                        path=abspath(join(full_test_dir, f'{common_run_name}@packets_data_calib_mode.csv')),
+                        packet_df=packet_df, path=join(full_test_dir, f'{common_run_name}@packets_data_calib_mode.csv'),
                         append=not is_first)
                     is_first = False
                 
                 unique_valid.append({
                     'adv_address': data['adv_address'],
                     'tbp': data['tbp'],
                     'ttfp': data['ttfp'],
@@ -490,16 +477,15 @@
                     'reel': data['reel'],
                     'attenuation': float(atten.split('_')[0]),
                     'test_num': int(atten.split('_')[1]),
                     'chamber': data['chamber']
                 })
         
         if len(unique_valid):
-            with open(abspath(join(full_test_dir, f'{common_run_name}@unique_data.csv')), 'w+',
-                      newline='') as new_tagsCsv:
+            with open(join(full_test_dir, f'{common_run_name}@unique_data.csv'), 'w+', newline='') as new_tagsCsv:
                 writer = csv.DictWriter(new_tagsCsv, fieldnames=list(unique_valid[0].keys()))
                 writer.writeheader()
                 writer.writerows(unique_valid)
         
         self.barcodes_read = {}
         self.test_barcodes = {}
         self.builder.get_object('scanned').delete(0, END)
@@ -550,32 +536,31 @@
             if self.builder.tkvariables.get('stop').get() == SEND:
                 self.builder.get_object('scanned').delete(0, END)
                 self.remove_barcodes()
                 self.stopButtonState = FINISH
                 self.builder.tkvariables.get('stop').set(FINISH)
             
             if len(new_tag.split(',')) < 2:
-                self.comConnect.popup_message(f'Missing chamber index, add chamber index after a comma.', title='Error', log='error')
+                popup_message(f'Missing chamber index, add chamber index after a comma.', title='Error', log='error')
                 return
             cur_id = new_tag.split(',')[0].strip()
             scan_index = int(new_tag.split(',')[1].strip())
             if 0 < self.comConnect.get_num_of_barcode_scanners() < (scan_index + 1):
-                self.comConnect.popup_message(f'Chamber number {scan_index} not exists.', title='Error', log='error')
+                popup_message(f'Chamber number {scan_index} not exists.', title='Error', log='error')
                 return
             
             barcodes = self.builder.get_object('scanned').get(0, END)
             if any([barcode for barcode in barcodes if int(barcode.split()[1].strip()) == scan_index]):
-                self.comConnect.popup_message(f'Chamber {scan_index} tag already scanned.', title='Error', log='error')
+                popup_message(f'Chamber {scan_index} tag already scanned.', title='Error', log='error')
                 return
             # logger.info(scan_index)
             
             self.builder.tkvariables.get('addTag').set('')
-            popup_thread = Thread(target=self.comConnect.popup_message,
-                                  args=('Chambers are closing!!\nWatch your hands!!!',
-                                        'Warning', ("Helvetica", 18), 'warning'))
+            popup_thread = Thread(target=popup_message, args=('Chambers are closing!!\nWatch your hands!!!',
+                                                              'Warning', ("Helvetica", 18), 'warning'))
             popup_thread.start()
             popup_thread.join()
             self.add_tag_to_test(cur_id, self.reel_id, scan_index, add_to_test=True)
             chambers = self.comConnect.get_chambers()
             if len(chambers) > scan_index and chambers[scan_index] is not None:
                 chambers[scan_index].close_chamber()
             self.update_go_state()
@@ -678,15 +663,15 @@
         self.builder.get_variable('isCalib').set(str(int(self.calib)))
         self.builder.get_variable('isOffline').set(str(int(self.offline)))
         self.builder.get_variable('isTestEnv').set(str(int(self.environment == 'test')))
         
         if 'config' in self.defaultDict.keys():
             self.testConfig = self.defaultDict['config']
         else:
-            self.testConfig = ''
+            self.testConfig = []
         self.builder.get_object('test_config').set(self.testConfig)
         self.configsGui.set_default_config(self.testConfig)
         self.configsGui.set_params(self.testConfig)
     
     def open_configs(self):
         """
         open Configs GUI
@@ -710,15 +695,15 @@
             self.comTtk = Toplevel(self.ttk)
             self.ttk.eval(f'tk::PlaceWindow {str(self.comTtk)} center')
             self.comConnect.gui(self.comTtk)
     
     def read_qr(self):
         barcode, reel = self.comConnect.read_barcode()
         if barcode is None:
-            read_qr_thread = Thread(target=self.comConnect.popup_message, args=(
+            read_qr_thread = Thread(target=popup_message, args=(
                 [f'Error reading external ID, try repositioning the tag.', 'Error', ("Helvetica", 10), 'error']))
             read_qr_thread.start()
             read_qr_thread.join()
             if not self.calib:
                 return
         
         if reel is not None:
@@ -805,18 +790,18 @@
     def stop_state(self):
         self.builder.get_object('stop')['state'] = 'normal'
     
     def recv_data_from_gw(self):
         self.tagsFinished = {}
         self.testGo = True
         self.startTime = self.comConnect.get_gw_time()
-        self.logger.info(f'Tags in the test: {",".join(list(self.barcodes_read.keys()))}')
+        logger.info(f'Tags in the test: {",".join(list(self.barcodes_read.keys()))}')
         gw_passed = self.comConnect.send_gw_app(self.params)
         if not gw_passed:
-            self.comConnect.popup_message(f'Error sending GW commands.', 'Error', ("Helvetica", 10), 'error')
+            popup_message(f'Error sending GW commands.', 'Error', ("Helvetica", 10), 'error')
             self.update_params_state(state='normal', group=CONTINUE)
             return
         self.gatewayDataThread = Thread(target=self.stop_state(), args=())
         self.gatewayDataThread.start()
         last_time = time.time()
         self.targetTime = last_time + self.testTime
         if self.timerThread is not None:
@@ -827,15 +812,15 @@
         self.sync_thread.start()
         packets_list = PacketList()
         recvDataMutex.acquire()
         while True:
             sleep(0.001)
             try:
                 if self.closeListener:
-                    self.logger.info("DataHandlerProcess Stop")
+                    logger.info("DataHandlerProcess Stop")
                     break
                 
                 if self.comConnect.is_gw_data_available():
                     
                     gw_data = self.comConnect.get_data()
                     
                     packets_list.__add__(gw_data)
@@ -933,37 +918,37 @@
                 print(packet.get_packet_string())
                 full_data, success = self.get_packet_ext_id(packet)
 
                 if not success:
                     if not post_run:
                         self.unknown_packets.append(packet)
                         if adv_address not in self.advas_dict.keys():
-                            self.logger.error(
+                            logger.error(
                                 f'Could not get external ID for adv_address {adv_address} '
                                 f'from the cloud - saving data for post process')
                         self.advas_dict[adv_address] = None
                     else:
-                        self.logger.error(
+                        logger.error(
                             f'Could not get external ID for adv_address {adv_address} '
                             f'from the cloud - dumping packet')
                     continue
 
                 ext_id = full_data['barcode'] if full_data['barcode'] in self.barcodes_read.keys() else full_data[
                     'cur_id']
                 if ext_id is not None and ext_id not in self.barcodes_read.keys():
-                    self.logger.info(
+                    logger.info(
                         f'Tag with adv_address {adv_address} and external ID {full_data["cur_id"]} '
                         f'detected but not belong to the test.')
                     self.bad_advas.append(adv_address)
                     continue
 
                 self.advas_dict[adv_address] = ext_id
 
                 if adv_address not in self.barcodes_read[ext_id]['adv_address']:
-                    self.logger.info(
+                    logger.info(
                         f'New Tag detected with adv_address {adv_address} and external ID {full_data["cur_id"]}.')
                     self.barcodes_read[ext_id]['adv_address'].append(adv_address)
             
             self.barcodes_read[ext_id]['packets'].append(packet.get_packet_string())
             self.barcodes_read[ext_id]['packetList'].append(packet.copy())
             
             if self.barcodes_read[ext_id]['packetList'].get_statistics()['sprinkler_counter_max'] > 3 and not post_run:
@@ -995,21 +980,21 @@
         
         self.finish_test()
         
         # read_tags = ''
         # if self.tagsCount < self.numOfTags and not force_finish:
         read_tags = '\nReplace tags and click on "Read"'
         
-        finishThread = Thread(target=self.comConnect.popup_message, args=(f'{serial_warning}'
-                                                                          f'{stat}'
-                                                                          f'{read_tags}',
-                                                                          'info',
-                                                                          ("Helvetica", 10),
-                                                                          'info',
-                                                                          bg_color))
+        finishThread = Thread(target=popup_message, args=(f'{serial_warning}'
+                                                          f'{stat}'
+                                                          f'{read_tags}',
+                                                          'info',
+                                                          ("Helvetica", 10),
+                                                          'info',
+                                                          bg_color))
         finishThread.start()
         finishThread.join()
         
         self.update_params_state(state='normal', group=READ)
         
         self.builder.tkvariables.get('numTags').set(len(self.test_barcodes.keys()))
         self.builder.tkvariables.get('addTag').set('')
@@ -1034,15 +1019,15 @@
         self.remove_barcodes()
         self.finish_test(True, True)
         # self.finishTestThread = Thread(target=self.finish_test, args=([True, True]))
         # self.finishTestThread.start()
     
     def handle_unknown_packets(self):
         if self.unknown_packets.size() > 0:
-            self.logger.info(f'Start handling unknown packets.')
+            logger.info(f'Start handling unknown packets.')
             self.process_packets(self.unknown_packets, post_run=True)
     
     def post_process_iteration(self):
         tbp_count = 0
         ttfp_count = 0
         ttfp_avg = 0
         tbp_avg = 0
@@ -1102,40 +1087,39 @@
             bg_color = 'green' if not (serial_warning or adva_warning) else 'yellow'
             bg_color = bg_color if pass_fail else 'red'
             pass_fail = 'Passed' if pass_fail else 'Failed'
             
             self.files_and_cloud(post_data)
         
         if reset_tester and post_process:
-            self.comConnect.popup_message(f'Test {self.common_run_name} has {pass_fail}\n' +
-                                          f'{fail_str}\n' +
-                                          f'{serial_warning}' +
-                                          f'Average TTFP: {self.dataBaseDict["ttfpAvg"]} [sec]\n' +
-                                          f'Average TBP: {self.dataBaseDict["tbpAvg"]} [msec]\n' +
-                                          f'STD TBP: {self.dataBaseDict["tbpStd"]} [msec]\n' +
-                                          f'Yield: {self.dataBaseDict["responding[%]"]}', title='Finished test',
-                                          bg=bg_color,
-                                          log='info')
+            popup_message(f'Test {self.common_run_name} has {pass_fail}\n' +
+                          f'{fail_str}\n' +
+                          f'{serial_warning}' +
+                          f'Average TTFP: {self.dataBaseDict["ttfpAvg"]} [sec]\n' +
+                          f'Average TBP: {self.dataBaseDict["tbpAvg"]} [msec]\n' +
+                          f'STD TBP: {self.dataBaseDict["tbpStd"]} [msec]\n' +
+                          f'Yield: {self.dataBaseDict["responding[%]"]}', title='Finished test', bg=bg_color,
+                          log='info')
         
         if reset_tester:
             # self.tagsCount = 0
             self.builder.get_object('reelId').bind("<Key>", self.get_reel_id)
             self.builder.tkvariables.get('numTags').set(0)
             self.builder.tkvariables.get('go').set(READ)
             self.testFinished = True
             self.packets_dict = {}
             self.test_barcodes = {}
             self.barcodes_read = {}
             self.reel_id = ''
             self.gtin = ''
             self.builder.tkvariables.get('reelId').set('')
             
-            changeFileHandler(self.logger, self.logger_path, file_mode='a+', append_handler=True)
-            self.logger.info(f'Test {self.common_run_name} ended.')
-            removeFileHandler(self.logger, self.test_log_file)
+            changeFileHandler(logger, default_log_file, file_mode='a+', append_handler=True)
+            logger.info(f'Test {self.common_run_name} ended.')
+            removeFileHandler(logger, self.test_log_file)
             self.update_params_state(state='normal', group=READ)
             self.builder.tkvariables.get('stop').set(STOP)
             self.builder.get_object('stop')['state'] = 'disabled'
 
         if self.offline:
             self.offline_tag_index = 0
 
@@ -1179,22 +1163,22 @@
                                    'adv_address': data['adv_address'],
                                    'state(tbp_exists:0,no_tbp:-1,no_ttfp:-2,dup_adv_address:-3)': tag_state,
                                    'status': data['status'], 'chamber': data['chamber'],
                                    'temperature_from_sensor': temperature_from_sensor
                                    }
                         
                         packets_csv.append_dict_as_row([tag_row])
-
-        with open(abspath(join(OUTPUT_DIR, self.testName, self.testDir, f'{self.common_run_name}@configs_data.csv')),
+        
+        with open(join(OUTPUT_DIR, self.testName, self.testDir, f'{self.common_run_name}@configs_data.csv'),
                   'w+', newline='') as newCsv:
             writer = csv.DictWriter(newCsv, fieldnames=self.dataBaseDict.keys())
             writer.writeheader()
             writer.writerows([self.dataBaseDict])
-
-        with open(abspath(join(OUTPUT_DIR, self.testName, self.testDir, f'{self.common_run_name}@tags_data.csv')),
+        
+        with open(join(OUTPUT_DIR, self.testName, self.testDir, f'{self.common_run_name}@tags_data.csv'),
                   'w+', newline='') as newCsv:
             ids_dict = self.test_barcodes
             tags = []
             for extId, tag in ids_dict.items():
                 if tag['chamber'] < len(self.comConnect.temperature_sensor_readings):
                     all_reading_temp = self.comConnect.temperature_sensor_readings[tag['chamber']]
                 else:
@@ -1221,18 +1205,18 @@
             writer = csv.DictWriter(newCsv, fieldnames=tags[0].keys())
             writer.writeheader()
             writer.writerows(tags)
         
         if post_data and self.post_data:
             post_success = self.post_to_cloud(run_data_path, tags_data_path, environment=self.environment)
             if not post_success:
-                self.comConnect.popup_message(f'Failed uploading run and/or tags data, Upload manually:\n' +
-                                              f'{self.common_run_name}@run_data.csv\n' +
-                                              f'{self.common_run_name}@packets_data.csv', log='warning')
-    
+                popup_message(f'Failed uploading run and/or tags data, Upload manually:\n' +
+                              f'{self.common_run_name}@run_data.csv\n' +
+                              f'{self.common_run_name}@packets_data.csv', log='warning')
+
     def get_packet_ext_id(self, packet):
         """
         get external ID of a tag by sending an example packet to the cloud.
         :type packet: Packet
         :param packet: contains the raw and time of the packet.
         :return: external ID of the tag, and the external ID parsed when it's wiliot tag.
         """
@@ -1295,19 +1279,16 @@
             if not first_iter:
                 try_again = popup_yes_no(f'Could not post data to cloud, try again?')
                 if not try_again:
                     return False
             
             success = upload_to_cloud_api(batch_name=self.reel_id, tester_type='sample-test',
                                           run_data_csv_name=run_data_file_path,
-                                          packets_data_csv_name=packets_data_file_path,
-                                          is_path=True,
-                                          env=environment,
-                                          owner_id=self.owner,
-                                          logger_='sample')
+                                          tags_data_csv_name=packets_data_file_path, env=environment, is_path=True,
+                                          client=self.client, packets_instead_tags=True)
             first_iter = False
         
         return success
 
     def post_process(self):
         tbp_arr = []
         ttfp_arr = []
@@ -1411,16 +1392,16 @@
         temp_coms = self.comConnect.get_default_dict()
         if self.station_name.strip() != '':
             temp_coms['stationName'] = self.station_name
         if self.testConfig != '':
             temp_coms['config'] = self.testConfig
         if self.calib:
             temp_coms[f'{self.antenna}_calib'] = {'low': self.low, 'high': self.high, 'step': self.step}
-
-        with open(abspath(join(CONFIGS_DIR, '.defaults.json')), 'w+') as defaultComs:
+        
+        with open(join(CONFIGS_DIR, '.defaults.json'), 'w+') as defaultComs:
             dump(temp_coms, defaultComs, indent=4)
     
     def popup_login(self):
         """
         popup to insert fusion auth credentials, and choosing owner.
         """
         default_font = ("Helvetica", 10)
@@ -1467,24 +1448,24 @@
 
         popup.mainloop()
 
         if self.owner not in owner_id_list:
             owner_id_list.append(self.owner)
             owner_id_list = [o for o in owner_id_list if o != '']
             self.defaultDict['owner'] = owner_id_list
-            with open(abspath(join(CONFIGS_DIR, '.defaults.json')), 'w+') as defaultComs:
+            with open(join(CONFIGS_DIR, '.defaults.json'), 'w+') as defaultComs:
                 dump(self.defaultDict, defaultComs, indent=4)
     
     def popup_calib(self):
         """
         popup to choose calib mode parameters
         """
         default_font = ("Helvetica", 10)
         popup = Tk()
-        # popup.eval('tk::PlaceWindow . center')
+        popup.eval('tk::PlaceWindow . center')
         popup.wm_title('Login')
         
         # defaultDict = {}
         # if isfile(join(CONFIGS_DIR, '.defaults.json')):
         #     with open(join(CONFIGS_DIR, '.defaults.json'), 'r') as defaultComs:
         #         defaultDict = load(defaultComs)
         
@@ -1509,15 +1490,15 @@
                 e3.delete(0, END)
                 e4.delete(0, END)
                 e5.delete(0, END)
                 e2.insert(0, antennaDict['low'])
                 e3.insert(0, antennaDict['high'])
                 e4.insert(0, antennaDict['step'])
                 e5.insert(0, 1)
-
+        
         l1 = Label(popup, text='Enter calibration parameters:', font=default_font)
         l1.grid(row=1, column=0, padx=10, pady=10, columnspan=3)
         l2 = Label(popup, text='Antenna Type:', font=default_font)
         l2.grid(row=2, column=0, padx=10, pady=10)
         c2 = ttk.Combobox(popup, values=['BLE', 'LoRa'])
         c2.grid(row=2, column=1, padx=10, pady=10)
         c2.bind("<FocusOut>", update_antenna_params)
@@ -1545,36 +1526,32 @@
         
         popup.mainloop()
         
         # return antenna, low, high, step
 
     def on_send_to_cloud(self):
         self.post_data = bool(int(self.builder.get_variable('sendToCloud').get()))
-        self.logger.info(f'send to cloud was changed to {self.post_data}')
+        logger.info(f'send to cloud was changed to {self.post_data}')
 
     def on_power_calib(self):
         self.calib = bool(int(self.builder.get_variable('isCalib').get()))
-        self.logger.info(f'calibration mode was changed to {self.calib}')
+        logger.info(f'calibration mode was changed to {self.calib}')
 
     def on_offline(self):
         self.offline = bool(int(self.builder.get_variable('isOffline').get()))
-        self.logger.info(f'offline mode was changed to {self.offline}')
+        logger.info(f'offline mode was changed to {self.offline}')
 
     def on_test_env(self):
         self.environment = 'test' if bool(int(self.builder.get_variable('isTestEnv').get())) else ''
         env_for_printing = self.environment if self.environment != '' else 'production'
-        self.logger.info(f'sending data to {env_for_printing} environment')
+        logger.info(f'sending data to {env_for_printing} environment')
 
 
-def popup_yes_no(question, tk_frame=None):
-    if tk_frame is None:
-        root = Tk()
-        root.eval(f'tk::PlaceWindow {str(root)} center')
-    else:
-        root = tk_frame
+def popup_yes_no(question):
+    root = Tk()
     root.wm_withdraw()
     result = messagebox.askquestion("Sample Test", question, icon='warning')
     root.destroy()
     if result == 'yes':
         return True
     else:
         return False
@@ -1604,17 +1581,17 @@
     post_data = args.post_data
     offline = args.offline
     
     # Run the UI
     # calib = True
     # offline = True
     if calib:
-        print(f'Sample Test - calibration mode active.')
+        logger.warning(f'Sample Test - calibration mode active.')
     if offline:
-        print(f'Sample Test - offline mode active.')
+        logger.warning(f'Sample Test - offline mode active.')
     app_folder = abspath(join(dirname(__file__), '../wiliot_testers'))
     try:
         sampleTest = SampleTest(calib=calib, environment=args.environment, post_data=post_data,
                                 offline=offline)
         sampleTest.gui()
     except BaseException:
         print_exc()
```

### Comparing `wiliot-testers-4.0.11/wiliot_testers/sample/utils/com_connect.ui` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/com_connect.ui`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/sample/utils/comm.gif` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/comm.gif`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/sample/utils/configs.gif` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/configs.gif`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/sample/utils/configs.ui` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/configs.ui`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/sample/utils/reset.png` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/reset.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/sample/utils/sample_test.ui` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/sample_test.ui`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/sample/utils/wiliot3.gif` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/wiliot3.gif`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/system_test/harvester_test.py` & `wiliot-testers-4.0.6/wiliot_testers/system_test/harvester_test.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/system_test/system_test_example.py` & `wiliot-testers-4.0.6/wiliot_testers/system_test/system_test_example.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/test_equipment.py` & `wiliot-testers-4.0.6/wiliot_testers/test_equipment.py`

 * *Files 12% similar despite different names*

```diff
@@ -236,2090 +236,1718 @@
 00000eb0: 4d41 4745 532c 204c 4f53 5345 532c 204f  MAGES, LOSSES, O
 00000ec0: 5220 434f 5354 533b 2041 4e44 0a20 2020  R COSTS; AND.   
 00000ed0: 2843 2920 4556 454e 2049 4620 414e 5920  (C) EVEN IF ANY 
 00000ee0: 5245 4d45 4459 2046 4149 4c53 204f 4620  REMEDY FAILS OF 
 00000ef0: 4954 5320 4553 5345 4e54 4941 4c20 5055  ITS ESSENTIAL PU
 00000f00: 5250 4f53 452e 0a22 2222 0a66 726f 6d20  RPOSE..""".from 
 00000f10: 7469 6d65 2069 6d70 6f72 7420 7469 6d65  time import time
-00000f20: 2c20 736c 6565 702c 2070 6572 665f 636f  , sleep, perf_co
-00000f30: 756e 7465 725f 6e73 0a66 726f 6d20 7374  unter_ns.from st
-00000f40: 6174 6973 7469 6373 2069 6d70 6f72 7420  atistics import 
-00000f50: 6d6f 6465 0a69 6d70 6f72 7420 7379 730a  mode.import sys.
-00000f60: 696d 706f 7274 2073 6572 6961 6c0a 696d  import serial.im
-00000f70: 706f 7274 2073 6572 6961 6c2e 746f 6f6c  port serial.tool
-00000f80: 732e 6c69 7374 5f70 6f72 7473 0a66 726f  s.list_ports.fro
-00000f90: 6d20 796f 6374 6f70 7563 652e 796f 6374  m yoctopuce.yoct
-00000fa0: 6f5f 7465 6d70 6572 6174 7572 6520 696d  o_temperature im
-00000fb0: 706f 7274 2059 4150 492c 2059 5265 6650  port YAPI, YRefP
-00000fc0: 6172 616d 2c20 5954 656d 7065 7261 7475  aram, YTemperatu
-00000fd0: 7265 0a69 6d70 6f72 7420 6f73 0a66 726f  re.import os.fro
-00000fe0: 6d20 6461 7465 7469 6d65 2069 6d70 6f72  m datetime impor
-00000ff0: 7420 6461 7465 7469 6d65 0a66 726f 6d20  t datetime.from 
-00001000: 7769 6c69 6f74 5f63 6f72 6520 696d 706f  wiliot_core impo
-00001010: 7274 2057 696c 696f 7444 6972 0a0a 636c  rt WiliotDir..cl
-00001020: 6173 7320 4571 7569 706d 656e 7445 7272  ass EquipmentErr
-00001030: 6f72 2845 7863 6570 7469 6f6e 293a 0a0a  or(Exception):..
-00001040: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00001050: 2873 656c 662c 202a 6172 6773 293a 0a20  (self, *args):. 
-00001060: 2020 2020 2020 2069 6620 6172 6773 3a0a         if args:.
-00001070: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001080: 2e6d 6573 7361 6765 203d 2061 7267 735b  .message = args[
-00001090: 305d 0a20 2020 2020 2020 2065 6c73 653a  0].        else:
-000010a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000010b0: 662e 6d65 7373 6167 6520 3d20 4e6f 6e65  f.message = None
-000010c0: 0a0a 2020 2020 6465 6620 5f5f 7374 725f  ..    def __str_
-000010d0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-000010e0: 2023 2070 7269 6e74 2827 6361 6c6c 696e   # print('callin
-000010f0: 6720 7374 7227 290a 2020 2020 2020 2020  g str').        
-00001100: 6966 2073 656c 662e 6d65 7373 6167 653a  if self.message:
-00001110: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00001120: 7572 6e20 2745 7175 6970 6d65 6e74 4572  urn 'EquipmentEr
-00001130: 726f 723a 207b 6d73 677d 272e 666f 726d  ror: {msg}'.form
-00001140: 6174 286d 7367 3d73 656c 662e 6d65 7373  at(msg=self.mess
-00001150: 6167 6529 0a20 2020 2020 2020 2065 6c73  age).        els
-00001160: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00001170: 6574 7572 6e20 2745 7175 6970 6d65 6e74  eturn 'Equipment
-00001180: 4572 726f 7220 6861 7320 6265 656e 2072  Error has been r
-00001190: 6169 7365 6427 0a0a 0a64 6566 2073 6572  aised'...def ser
-000011a0: 6961 6c5f 706f 7274 7328 293a 0a20 2020  ial_ports():.   
-000011b0: 2022 2222 204c 6973 7473 2073 6572 6961   """ Lists seria
-000011c0: 6c20 706f 7274 206e 616d 6573 0a0a 2020  l port names..  
-000011d0: 2020 2020 2020 3a72 6169 7365 7320 456e        :raises En
-000011e0: 7669 726f 6e6d 656e 7445 7272 6f72 3a0a  vironmentError:.
-000011f0: 2020 2020 2020 2020 2020 2020 4f6e 2075              On u
-00001200: 6e73 7570 706f 7274 6564 206f 7220 756e  nsupported or un
-00001210: 6b6e 6f77 6e20 706c 6174 666f 726d 730a  known platforms.
-00001220: 2020 2020 2020 2020 3a72 6574 7572 6e73          :returns
-00001230: 3a0a 2020 2020 2020 2020 2020 2020 4120  :.            A 
-00001240: 6c69 7374 206f 6620 7468 6520 7365 7269  list of the seri
-00001250: 616c 2070 6f72 7473 2061 7661 696c 6162  al ports availab
-00001260: 6c65 206f 6e20 7468 6520 7379 7374 656d  le on the system
-00001270: 0a20 2020 2022 2222 0a20 2020 2061 7661  .    """.    ava
-00001280: 696c 6162 6c65 5f70 6f72 7473 203d 205b  ilable_ports = [
-00001290: 732e 6465 7669 6365 2066 6f72 2073 2069  s.device for s i
-000012a0: 6e20 7365 7269 616c 2e74 6f6f 6c73 2e6c  n serial.tools.l
-000012b0: 6973 745f 706f 7274 732e 636f 6d70 6f72  ist_ports.compor
-000012c0: 7473 2829 5d0a 2020 2020 6966 206c 656e  ts()].    if len
-000012d0: 2861 7661 696c 6162 6c65 5f70 6f72 7473  (available_ports
-000012e0: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
-000012f0: 6176 6169 6c61 626c 655f 706f 7274 7320  available_ports 
-00001300: 3d20 5b73 2e6e 616d 6520 666f 7220 7320  = [s.name for s 
-00001310: 696e 2073 6572 6961 6c2e 746f 6f6c 732e  in serial.tools.
-00001320: 6c69 7374 5f70 6f72 7473 2e63 6f6d 706f  list_ports.compo
-00001330: 7274 7328 295d 0a20 2020 2020 2020 2069  rts()].        i
-00001340: 6620 6c65 6e28 6176 6169 6c61 626c 655f  f len(available_
-00001350: 706f 7274 7329 203d 3d20 303a 0a20 2020  ports) == 0:.   
-00001360: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-00001370: 6e6f 2073 6572 6961 6c20 706f 7274 7320  no serial ports 
-00001380: 7765 7265 2066 6f75 6e64 2e20 706c 6561  were found. plea
-00001390: 7365 2063 6865 636b 2079 6f75 7220 636f  se check your co
-000013a0: 6e6e 6563 7469 6f6e 7322 290a 2020 2020  nnections").    
-000013b0: 7265 7475 726e 2061 7661 696c 6162 6c65  return available
-000013c0: 5f70 6f72 7473 0a0a 0a63 6c61 7373 2041  _ports...class A
-000013d0: 7474 656e 7561 746f 7228 6f62 6a65 6374  ttenuator(object
-000013e0: 293a 0a20 2020 2027 2727 0a20 2020 2053  ):.    '''.    S
-000013f0: 7570 706f 7274 2061 6c6c 2061 7474 6e20  upport all attn 
-00001400: 636c 6173 7365 7320 666f 723a 0a20 2020  classes for:.   
-00001410: 2027 2727 0a0a 2020 2020 6465 6620 5f5f   '''..    def __
-00001420: 696e 6974 5f5f 2873 656c 662c 2041 5454  init__(self, ATT
-00001430: 4e5f 7479 7065 2c20 636f 6d70 6f72 743d  N_type, comport=
-00001440: 2741 5554 4f27 293a 0a20 2020 2020 2020  'AUTO'):.       
-00001450: 2069 6620 274d 4344 492d 5553 4227 2069   if 'MCDI-USB' i
-00001460: 6e20 4154 544e 5f74 7970 653a 0a20 2020  n ATTN_type:.   
-00001470: 2020 2020 2020 2020 2073 656c 662e 5f61           self._a
-00001480: 6374 6976 655f 5445 203d 2041 7474 656e  ctive_TE = Atten
-00001490: 7561 746f 722e 4d43 4449 5f55 5342 2829  uator.MCDI_USB()
-000014a0: 0a20 2020 2020 2020 2065 6c69 6620 274d  .        elif 'M
-000014b0: 4344 4927 2069 6e20 4154 544e 5f74 7970  CDI' in ATTN_typ
-000014c0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000014d0: 656c 662e 5f61 6374 6976 655f 5445 203d  elf._active_TE =
-000014e0: 2041 7474 656e 7561 746f 722e 4d43 4449   Attenuator.MCDI
-000014f0: 2829 0a20 2020 2020 2020 2065 6c69 6620  ().        elif 
-00001500: 2741 5049 2720 696e 2041 5454 4e5f 7479  'API' in ATTN_ty
-00001510: 7065 206f 7220 2757 6569 6e73 6368 656c  pe or 'Weinschel
-00001520: 2720 696e 2041 5454 4e5f 7479 7065 3a0a  ' in ATTN_type:.
-00001530: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001540: 2e5f 6163 7469 7665 5f54 4520 3d20 4174  ._active_TE = At
-00001550: 7465 6e75 6174 6f72 2e41 5049 2863 6f6d  tenuator.API(com
-00001560: 706f 7274 290a 0a20 2020 2020 2020 2065  port)..        e
-00001570: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00001580: 2070 6173 730a 0a20 2020 2064 6566 2047   pass..    def G
-00001590: 6574 4163 7469 7665 5445 2873 656c 6629  etActiveTE(self)
-000015a0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000015b0: 2073 656c 662e 5f61 6374 6976 655f 5445   self._active_TE
-000015c0: 0a0a 2020 2020 636c 6173 7320 4d43 4449  ..    class MCDI
-000015d0: 286f 626a 6563 7429 3a0a 0a20 2020 2020  (object):..     
-000015e0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-000015f0: 7365 6c66 293a 0a20 2020 2020 2020 2020  self):.         
-00001600: 2020 2064 6f74 6e65 7420 3d20 4661 6c73     dotnet = Fals
-00001610: 650a 2020 2020 2020 2020 2020 2020 7574  e.            ut
-00001620: 696c 735f 6469 7220 3d20 6f73 2e70 6174  ils_dir = os.pat
-00001630: 682e 6a6f 696e 286f 732e 7061 7468 2e64  h.join(os.path.d
-00001640: 6972 6e61 6d65 285f 5f66 696c 655f 5f29  irname(__file__)
-00001650: 2c20 2775 7469 6c73 2729 0a20 2020 2020  , 'utils').     
-00001660: 2020 2020 2020 2073 7973 2e70 6174 682e         sys.path.
-00001670: 6170 7065 6e64 2875 7469 6c73 5f64 6972  append(utils_dir
-00001680: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00001690: 2064 6f74 6e65 7420 3d3d 2054 7275 653a   dotnet == True:
-000016a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000016b0: 2069 6d70 6f72 7420 636c 7220 2023 2070   import clr  # p
-000016c0: 7974 686f 6e6e 6574 2c20 6d61 6e75 616c  ythonnet, manual
-000016d0: 6c79 2069 6e73 7461 6c6c 6564 2077 6974  ly installed wit
-000016e0: 6820 6120 646f 776e 6c6f 6164 6564 2077  h a downloaded w
-000016f0: 6865 656c 2061 6e64 2070 6970 0a20 2020  heel and pip.   
-00001700: 2020 2020 2020 2020 2020 2020 2069 6d70               imp
-00001710: 6f72 7420 6374 7970 6573 2020 2320 6d6f  ort ctypes  # mo
-00001720: 6475 6c65 2074 6f20 6f70 656e 2075 7469  dule to open uti
-00001730: 6c73 2066 696c 6573 0a20 2020 2020 2020  ls files.       
-00001740: 2020 2020 2020 2020 2063 6c72 2e41 6464           clr.Add
-00001750: 5265 6665 7265 6e63 6528 2253 7973 7465  Reference("Syste
-00001760: 6d2e 494f 2229 0a20 2020 2020 2020 2020  m.IO").         
-00001770: 2020 2020 2020 2069 6d70 6f72 7420 5379         import Sy
-00001780: 7374 656d 2e49 4f0a 2020 2020 2020 2020  stem.IO.        
-00001790: 2020 2020 2020 2020 5379 7374 656d 2e49          System.I
-000017a0: 4f2e 4469 7265 6374 6f72 792e 5365 7443  O.Directory.SetC
-000017b0: 7572 7265 6e74 4469 7265 6374 6f72 7928  urrentDirectory(
-000017c0: 7574 696c 735f 6469 7229 0a20 2020 2020  utils_dir).     
-000017d0: 2020 2020 2020 2020 2020 2063 6c72 2e41             clr.A
-000017e0: 6464 5265 6665 7265 6e63 6528 276d 636c  ddReference('mcl
-000017f0: 5f52 5544 4154 5f4e 4554 3435 2729 0a20  _RUDAT_NET45'). 
-00001800: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00001810: 726f 6d20 6d63 6c5f 5255 4441 545f 4e45  rom mcl_RUDAT_NE
-00001820: 5434 3520 696d 706f 7274 2055 5342 5f52  T45 import USB_R
-00001830: 5544 4154 0a20 2020 2020 2020 2020 2020  UDAT.           
-00001840: 2020 2020 2073 656c 662e 4465 7669 6365       self.Device
-00001850: 203d 2055 5342 5f52 5544 4154 2829 0a20   = USB_RUDAT(). 
-00001860: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001870: 656c 662e 4465 7669 6365 2e43 6f6e 6e65  elf.Device.Conne
-00001880: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
-00001890: 2020 2020 2069 6e66 6f20 3d20 7365 6c66       info = self
-000018a0: 2e44 6576 6963 6549 6e66 6f28 290a 2020  .DeviceInfo().  
-000018b0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000018c0: 696e 7428 2746 6f75 6e64 2041 7474 656e  int('Found Atten
-000018d0: 7561 746f 723a 204d 6f64 656c 207b 7d2c  uator: Model {},
-000018e0: 207b 7d20 2c7b 7d20 272e 666f 726d 6174   {} ,{} '.format
-000018f0: 2869 6e66 6f5b 305d 2c20 696e 666f 5b31  (info[0], info[1
-00001900: 5d2c 2069 6e66 6f5b 325d 2929 0a20 2020  ], info[2])).   
-00001910: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00001920: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00001930: 726f 6d20 5553 425f 5255 4441 5420 696d  rom USB_RUDAT im
-00001940: 706f 7274 2055 5342 4441 540a 2020 2020  port USBDAT.    
-00001950: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001960: 2e44 6576 6963 6520 3d20 5553 4244 4154  .Device = USBDAT
-00001970: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00001980: 2020 2069 6e66 6f20 3d20 7365 6c66 2e44     info = self.D
-00001990: 6576 6963 6549 6e66 6f28 290a 2020 2020  eviceInfo().    
-000019a0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000019b0: 7428 2746 6f75 6e64 2041 7474 656e 7561  t('Found Attenua
-000019c0: 746f 723a 204d 6f64 656c 207b 7d2c 207b  tor: Model {}, {
-000019d0: 7d20 2c7b 7d20 272e 666f 726d 6174 2869  } ,{} '.format(i
-000019e0: 6e66 6f5b 305d 2c20 696e 666f 5b31 5d2c  nfo[0], info[1],
-000019f0: 2069 6e66 6f5b 325d 2929 0a0a 2020 2020   info[2]))..    
-00001a00: 2020 2020 6465 6620 4465 7669 6365 496e      def DeviceIn
-00001a10: 666f 2873 656c 6629 3a0a 2020 2020 2020  fo(self):.      
-00001a20: 2020 2020 2020 636d 6420 3d20 223a 4d4e        cmd = ":MN
-00001a30: 3f22 0a20 2020 2020 2020 2020 2020 206d  ?".            m
-00001a40: 6f64 656c 5f6e 616d 6520 3d20 7365 6c66  odel_name = self
-00001a50: 2e44 6576 6963 652e 5365 6e64 5f53 4350  .Device.Send_SCP
-00001a60: 4928 636d 642c 2022 2229 0a20 2020 2020  I(cmd, "").     
-00001a70: 2020 2020 2020 2063 6d64 203d 2022 3a53         cmd = ":S
-00001a80: 4e3f 220a 2020 2020 2020 2020 2020 2020  N?".            
-00001a90: 7365 7269 616c 203d 2073 656c 662e 4465  serial = self.De
-00001aa0: 7669 6365 2e53 656e 645f 5343 5049 2863  vice.Send_SCPI(c
-00001ab0: 6d64 2c20 2222 290a 2020 2020 2020 2020  md, "").        
-00001ac0: 2020 2020 636d 6420 3d20 223a 4649 524d      cmd = ":FIRM
-00001ad0: 5741 5245 3f22 0a20 2020 2020 2020 2020  WARE?".         
-00001ae0: 2020 2066 7720 3d20 7365 6c66 2e44 6576     fw = self.Dev
-00001af0: 6963 652e 5365 6e64 5f53 4350 4928 636d  ice.Send_SCPI(cm
-00001b00: 642c 2022 2229 0a20 2020 2020 2020 2020  d, "").         
-00001b10: 2020 2023 2072 6574 7572 6e20 5b6d 6f64     # return [mod
-00001b20: 656c 5f6e 616d 655b 315d 2c20 7365 7269  el_name[1], seri
-00001b30: 616c 5b31 5d2c 2066 775b 315d 5d20 2023  al[1], fw[1]]  #
-00001b40: 646f 746e 6574 0a20 2020 2020 2020 2020  dotnet.         
-00001b50: 2020 2072 6574 7572 6e20 5b6d 6f64 656c     return [model
-00001b60: 5f6e 616d 652c 2073 6572 6961 6c2c 2066  _name, serial, f
-00001b70: 775d 0a0a 2020 2020 2020 2020 6465 6620  w]..        def 
-00001b80: 5365 7461 7474 6e28 7365 6c66 2c20 6174  Setattn(self, at
-00001b90: 746e 293a 0a20 2020 2020 2020 2020 2020  tn):.           
-00001ba0: 2063 6d64 203d 2022 3a53 4554 4154 543a   cmd = ":SETATT:
-00001bb0: 2220 2b20 7374 7228 6174 746e 290a 2020  " + str(attn).  
-00001bc0: 2020 2020 2020 2020 2020 7374 6174 7573            status
-00001bd0: 203d 2069 6e74 2873 656c 662e 4465 7669   = int(self.Devi
-00001be0: 6365 2e53 656e 645f 5343 5049 2863 6d64  ce.Send_SCPI(cmd
-00001bf0: 2c20 2222 2929 0a20 2020 2020 2020 2020  , "")).         
-00001c00: 2020 2069 6620 7374 6174 7573 203d 3d20     if status == 
-00001c10: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-00001c20: 2020 2070 7269 6e74 2827 436f 6d6d 616e     print('Comman
-00001c30: 6420 6661 696c 6564 206f 7220 696e 7661  d failed or inva
-00001c40: 6c69 6420 6174 7465 6e75 6174 696f 6e20  lid attenuation 
-00001c50: 7365 7427 290a 2020 2020 2020 2020 2020  set').          
-00001c60: 2020 656c 6966 2073 7461 7475 7320 3d3d    elif status ==
-00001c70: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-00001c80: 2020 2020 2320 7072 696e 7428 2743 6f6d      # print('Com
-00001c90: 6d61 6e64 2063 6f6d 706c 6574 6564 2073  mand completed s
-00001ca0: 7563 6365 7373 6675 6c6c 7927 290a 2020  uccessfully').  
-00001cb0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00001cc0: 696e 7428 2741 7474 656e 7561 7469 6f6e  int('Attenuation
-00001cd0: 2073 6574 2074 6f20 207b 7d5b 6442 5d27   set to  {}[dB]'
-00001ce0: 2e66 6f72 6d61 7428 666c 6f61 7428 7365  .format(float(se
-00001cf0: 6c66 2e47 6574 6174 746e 2829 2929 290a  lf.Getattn()))).
-00001d00: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00001d10: 2073 7461 7475 7320 3d3d 2032 3a0a 2020   status == 2:.  
-00001d20: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00001d30: 696e 7428 0a20 2020 2020 2020 2020 2020  int(.           
-00001d40: 2020 2020 2020 2020 2027 5265 7175 6573           'Reques
-00001d50: 7465 6420 6174 7465 6e75 6174 696f 6e20  ted attenuation 
-00001d60: 7761 7320 6869 6768 6572 2074 6861 6e20  was higher than 
-00001d70: 7468 6520 616c 6c6f 7765 6420 7261 6e67  the allowed rang
-00001d80: 652c 2074 6865 2061 7474 656e 7561 7469  e, the attenuati
-00001d90: 6f6e 2077 6173 2073 6574 2074 6f20 7468  on was set to th
-00001da0: 6520 6465 7669 6365 efbf bd73 206d 6178  e device...s max
-00001db0: 696d 756d 2061 6c6c 6f77 6564 2076 616c  imum allowed val
-00001dc0: 7565 2729 0a20 2020 2020 2020 2020 2020  ue').           
-00001dd0: 2023 2070 7269 6e74 2873 7461 7475 7329   # print(status)
-00001de0: 0a0a 2020 2020 2020 2020 6465 6620 4765  ..        def Ge
-00001df0: 7461 7474 6e28 7365 6c66 293a 0a20 2020  tattn(self):.   
-00001e00: 2020 2020 2020 2020 2063 6d64 203d 2022           cmd = "
-00001e10: 3a41 5454 3f22 0a20 2020 2020 2020 2020  :ATT?".         
-00001e20: 2020 2052 6573 7020 3d20 666c 6f61 7428     Resp = float(
-00001e30: 7365 6c66 2e44 6576 6963 652e 5365 6e64  self.Device.Send
-00001e40: 5f53 4350 4928 636d 642c 2022 2229 290a  _SCPI(cmd, "")).
-00001e50: 2020 2020 2020 2020 2020 2020 2320 7072              # pr
-00001e60: 696e 7428 5265 7370 290a 2020 2020 2020  int(Resp).      
-00001e70: 2020 2020 2020 2320 6966 2073 7461 7475        # if statu
-00001e80: 7320 3d3d 2030 3a0a 2020 2020 2020 2020  s == 0:.        
-00001e90: 2020 2020 2320 2020 2020 7072 696e 7428      #     print(
-00001ea0: 2743 6f6d 6d61 6e64 2066 6169 6c65 6420  'Command failed 
-00001eb0: 6f72 2069 6e76 616c 6964 2061 7474 656e  or invalid atten
-00001ec0: 7561 7469 6f6e 2073 6574 2729 0a20 2020  uation set').   
-00001ed0: 2020 2020 2020 2020 2023 2065 6c69 6620           # elif 
-00001ee0: 7374 6174 7573 203d 3d20 313a 0a20 2020  status == 1:.   
-00001ef0: 2020 2020 2020 2020 2023 2020 2020 2070           #     p
-00001f00: 7269 6e74 2827 436f 6d6d 616e 6420 636f  rint('Command co
-00001f10: 6d70 6c65 7465 6420 7375 6363 6573 7366  mpleted successf
-00001f20: 756c 6c79 2729 0a20 2020 2020 2020 2020  ully').         
-00001f30: 2020 2072 6574 7572 6e20 5265 7370 0a0a     return Resp..
-00001f40: 2020 2020 636c 6173 7320 4d43 4449 5f55      class MCDI_U
-00001f50: 5342 286f 626a 6563 7429 3a0a 2020 2020  SB(object):.    
-00001f60: 2020 2020 2320 3634 2062 6974 2061 7272      # 64 bit arr
-00001f70: 6179 2074 6f20 7365 6e64 2074 6f20 5553  ay to send to US
-00001f80: 420a 2020 2020 2020 2020 636d 6431 203d  B.        cmd1 =
-00001f90: 205b 302c 2030 2c20 302c 2030 2c20 302c   [0, 0, 0, 0, 0,
-00001fa0: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
-00001fb0: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
-00001fc0: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
-00001fd0: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
-00001fe0: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
-00001ff0: 2c20 302c 2030 2c20 302c 0a20 2020 2020  , 0, 0, 0,.     
-00002000: 2020 2020 2020 2020 2020 2030 2c20 302c             0, 0,
-00002010: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
-00002020: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
-00002030: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
-00002040: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
-00002050: 302c 2030 2c20 302c 2030 2c20 302c 0a20  0, 0, 0, 0, 0,. 
-00002060: 2020 2020 2020 2020 2020 2020 2020 2030                 0
-00002070: 5d20 2023 2036 3420 6269 7420 6172 7261  ]  # 64 bit arra
-00002080: 7920 746f 2073 656e 6420 746f 2055 5342  y to send to USB
-00002090: 0a0a 2020 2020 2020 2020 6465 6620 5f5f  ..        def __
-000020a0: 696e 6974 5f5f 2873 656c 6629 3a0a 2020  init__(self):.  
-000020b0: 2020 2020 2020 2020 2020 2320 6669 6e64            # find
-000020c0: 2074 6865 2064 6576 6963 650a 2020 2020   the device.    
-000020d0: 2020 2020 2020 2020 7365 6c66 2e64 6576          self.dev
-000020e0: 203d 2075 7362 2e63 6f72 652e 6669 6e64   = usb.core.find
-000020f0: 2869 6456 656e 646f 723d 3078 3230 6365  (idVendor=0x20ce
-00002100: 2c20 6964 5072 6f64 7563 743d 3078 3030  , idProduct=0x00
-00002110: 3233 290a 2020 2020 2020 2020 2020 2020  23).            
-00002120: 2320 7761 7320 6974 2066 6f75 6e64 3f0a  # was it found?.
-00002130: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00002140: 656c 662e 6465 7620 6973 204e 6f6e 653a  elf.dev is None:
-00002150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002160: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00002170: 7228 2744 6576 6963 6520 6e6f 7420 666f  r('Device not fo
-00002180: 756e 6427 290a 2020 2020 2020 2020 2020  und').          
-00002190: 2020 2320 7365 7420 7468 6520 6163 7469    # set the acti
-000021a0: 7665 2063 6f6e 6669 6775 7261 7469 6f6e  ve configuration
-000021b0: 2e20 7769 7468 206e 6f20 6172 6773 2077  . with no args w
-000021c0: 6520 7573 6520 6669 7273 7420 636f 6e66  e use first conf
-000021d0: 6967 2e0a 2020 2020 2020 2020 2020 2020  ig..            
-000021e0: 2320 2066 6f72 204c 696e 7578 206f 6e6c  #  for Linux onl
-000021f0: 790a 2020 2020 2020 2020 2020 2020 6966  y.            if
-00002200: 2073 7973 2e70 6c61 7466 6f72 6d20 3d3d   sys.platform ==
-00002210: 2027 6c69 6e75 7827 3a0a 0a20 2020 2020   'linux':..     
-00002220: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
-00002230: 6f6e 6669 6775 7261 7469 6f6e 2069 6e20  onfiguration in 
-00002240: 7365 6c66 2e64 6576 3a0a 2020 2020 2020  self.dev:.      
-00002250: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00002260: 7220 696e 7465 7266 6163 6520 696e 2063  r interface in c
-00002270: 6f6e 6669 6775 7261 7469 6f6e 3a0a 2020  onfiguration:.  
-00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002290: 2020 2020 2020 6966 6e75 6d20 3d20 696e        ifnum = in
-000022a0: 7465 7266 6163 652e 6249 6e74 6572 6661  terface.bInterfa
-000022b0: 6365 4e75 6d62 6572 0a20 2020 2020 2020  ceNumber.       
-000022c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000022d0: 6e6f 7420 7365 6c66 2e64 6576 2e69 735f  not self.dev.is_
-000022e0: 6b65 726e 656c 5f64 7269 7665 725f 6163  kernel_driver_ac
-000022f0: 7469 7665 2869 666e 756d 293a 0a20 2020  tive(ifnum):.   
-00002300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002310: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
-00002320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002330: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00002340: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00002350: 2070 7269 6e74 2022 6465 7461 6368 206b   print "detach k
-00002360: 6572 6e65 6c20 6472 6976 6572 2066 726f  ernel driver fro
-00002370: 6d20 6465 7669 6365 2025 733a 2069 6e74  m device %s: int
-00002380: 6572 6661 6365 2025 7322 2025 2028 6465  erface %s" % (de
-00002390: 762c 2069 666e 756d 290a 2020 2020 2020  v, ifnum).      
-000023a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023b0: 2020 7365 6c66 2e64 6576 2e64 6574 6163    self.dev.detac
-000023c0: 685f 6b65 726e 656c 5f64 7269 7665 7228  h_kernel_driver(
-000023d0: 6966 6e75 6d29 0a20 2020 2020 2020 2020  ifnum).         
-000023e0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-000023f0: 7420 7573 622e 636f 7265 2e55 5342 4572  t usb.core.USBEr
-00002400: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
-00002410: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-00002420: 730a 0a20 2020 2020 2020 2020 2020 2073  s..            s
-00002430: 656c 662e 6465 762e 7365 745f 636f 6e66  elf.dev.set_conf
-00002440: 6967 7572 6174 696f 6e28 290a 2020 2020  iguration().    
-00002450: 2020 2020 2020 2020 7365 6c66 2e63 6d64          self.cmd
-00002460: 315b 305d 203d 2034 310a 2020 2020 2020  1[0] = 41.      
-00002470: 2020 2020 2020 7365 6c66 2e64 6576 2e77        self.dev.w
-00002480: 7269 7465 2830 7830 312c 2073 656c 662e  rite(0x01, self.
-00002490: 636d 6431 2920 2023 2053 4e0a 2020 2020  cmd1)  # SN.    
-000024a0: 2020 2020 2020 2020 7320 3d20 7365 6c66          s = self
-000024b0: 2e64 6576 2e72 6561 6428 3078 3831 2c20  .dev.read(0x81, 
-000024c0: 3634 290a 2020 2020 2020 2020 2020 2020  64).            
-000024d0: 7365 6c66 2e53 6572 6961 6c4e 756d 6265  self.SerialNumbe
-000024e0: 7220 3d20 2222 0a20 2020 2020 2020 2020  r = "".         
-000024f0: 2020 2069 203d 2031 0a20 2020 2020 2020     i = 1.       
-00002500: 2020 2020 2077 6869 6c65 2028 735b 695d       while (s[i]
-00002510: 203e 2030 293a 0a20 2020 2020 2020 2020   > 0):.         
-00002520: 2020 2020 2020 2073 656c 662e 5365 7269         self.Seri
-00002530: 616c 4e75 6d62 6572 203d 2073 656c 662e  alNumber = self.
-00002540: 5365 7269 616c 4e75 6d62 6572 202b 2063  SerialNumber + c
-00002550: 6872 2873 5b69 5d29 0a20 2020 2020 2020  hr(s[i]).       
-00002560: 2020 2020 2020 2020 2069 203d 2069 202b           i = i +
-00002570: 2031 0a20 2020 2020 2020 2020 2020 2073   1.            s
-00002580: 656c 662e 636d 6431 5b30 5d20 3d20 3430  elf.cmd1[0] = 40
-00002590: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000025a0: 662e 6465 762e 7772 6974 6528 3078 3031  f.dev.write(0x01
-000025b0: 2c20 7365 6c66 2e63 6d64 3129 2020 2320  , self.cmd1)  # 
-000025c0: 4d6f 6465 6c0a 2020 2020 2020 2020 2020  Model.          
-000025d0: 2020 7320 3d20 7365 6c66 2e64 6576 2e72    s = self.dev.r
-000025e0: 6561 6428 3078 3831 2c20 3634 290a 2020  ead(0x81, 64).  
-000025f0: 2020 2020 2020 2020 2020 7365 6c66 2e4d            self.M
-00002600: 6f64 656c 4e61 6d65 203d 2022 220a 2020  odelName = "".  
-00002610: 2020 2020 2020 2020 2020 6920 3d20 310a            i = 1.
-00002620: 2020 2020 2020 2020 2020 2020 7768 696c              whil
-00002630: 6520 2873 5b69 5d20 3e20 3029 3a0a 2020  e (s[i] > 0):.  
-00002640: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00002650: 6c66 2e4d 6f64 656c 4e61 6d65 203d 2073  lf.ModelName = s
-00002660: 656c 662e 4d6f 6465 6c4e 616d 6520 2b20  elf.ModelName + 
-00002670: 6368 7228 735b 695d 290a 2020 2020 2020  chr(s[i]).      
-00002680: 2020 2020 2020 2020 2020 6920 3d20 6920            i = i 
-00002690: 2b20 310a 0a20 2020 2020 2020 2020 2020  + 1..           
-000026a0: 2073 656c 662e 4d61 7869 6d75 6d5f 4174   self.Maximum_At
-000026b0: 746e 203d 2066 6c6f 6174 2873 656c 662e  tn = float(self.
-000026c0: 4d6f 6465 6c4e 616d 655b 3131 3a5d 290a  ModelName[11:]).
-000026d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000026e0: 2e63 6d64 315b 305d 203d 2039 390a 2020  .cmd1[0] = 99.  
-000026f0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00002700: 6576 2e77 7269 7465 2830 7830 312c 2073  ev.write(0x01, s
-00002710: 656c 662e 636d 6431 2920 2023 2046 570a  elf.cmd1)  # FW.
-00002720: 2020 2020 2020 2020 2020 2020 7320 3d20              s = 
-00002730: 7365 6c66 2e64 6576 2e72 6561 6428 3078  self.dev.read(0x
-00002740: 3831 2c20 3634 290a 2020 2020 2020 2020  81, 64).        
-00002750: 2020 2020 7365 6c66 2e46 5720 3d20 2222      self.FW = ""
-00002760: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00002770: 662e 4657 203d 2063 6872 2873 5b35 5d29  f.FW = chr(s[5])
-00002780: 202b 2063 6872 2873 5b36 5d29 0a20 2020   + chr(s[6]).   
-00002790: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-000027a0: 6174 7573 5f6d 6573 7361 6765 203d 2027  atus_message = '
-000027b0: 466f 756e 6420 4174 7465 6e75 6174 6f72  Found Attenuator
-000027c0: 3a20 4d6f 6465 6c20 7b7d 2c20 534e 3a20  : Model {}, SN: 
-000027d0: 7b7d 202c 2046 573a 207b 7d2c 204d 6178  {} , FW: {}, Max
-000027e0: 696d 756d 2061 7474 656e 7561 7469 6f6e  imum attenuation
-000027f0: 3a20 7b7d 6442 2027 2e66 6f72 6d61 7428  : {}dB '.format(
-00002800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002810: 2073 7472 2873 656c 662e 4d6f 6465 6c4e   str(self.ModelN
-00002820: 616d 6529 2c20 7374 7228 7365 6c66 2e53  ame), str(self.S
-00002830: 6572 6961 6c4e 756d 6265 7229 2c20 7374  erialNumber), st
-00002840: 7228 7365 6c66 2e46 5729 2c20 7374 7228  r(self.FW), str(
-00002850: 7365 6c66 2e4d 6178 696d 756d 5f41 7474  self.Maximum_Att
-00002860: 6e29 290a 2020 2020 2020 2020 2020 2020  n)).            
-00002870: 7072 696e 7428 7365 6c66 2e73 7461 7475  print(self.statu
-00002880: 735f 6d65 7373 6167 6529 0a0a 2020 2020  s_message)..    
-00002890: 2020 2020 6465 6620 5265 6164 534e 2873      def ReadSN(s
-000028a0: 656c 6629 3a0a 2020 2020 2020 2020 2020  elf):.          
-000028b0: 2020 7265 7475 726e 2073 7472 2873 656c    return str(sel
-000028c0: 662e 5365 7269 616c 4e75 6d62 6572 290a  f.SerialNumber).
-000028d0: 0a20 2020 2020 2020 2064 6566 2052 6561  .        def Rea
-000028e0: 644d 4e28 7365 6c66 293a 0a20 2020 2020  dMN(self):.     
-000028f0: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
-00002900: 7228 7365 6c66 2e4d 6f64 656c 4e61 6d65  r(self.ModelName
-00002910: 290a 0a20 2020 2020 2020 2064 6566 2052  )..        def R
-00002920: 6561 6446 5728 7365 6c66 293a 0a20 2020  eadFW(self):.   
-00002930: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00002940: 7374 7228 7365 6c66 2e46 5729 0a0a 2020  str(self.FW)..  
-00002950: 2020 2020 2020 6465 6620 5265 6164 4d61        def ReadMa
-00002960: 7852 616e 6765 2873 656c 6629 3a0a 2020  xRange(self):.  
-00002970: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00002980: 2073 656c 662e 4d61 7869 6d75 6d5f 4174   self.Maximum_At
-00002990: 746e 0a0a 2020 2020 2020 2020 6465 6620  tn..        def 
-000029a0: 5365 7461 7474 6e28 7365 6c66 2c20 4174  Setattn(self, At
-000029b0: 746e 293a 0a20 2020 2020 2020 2020 2020  tn):.           
-000029c0: 2073 656c 662e 636d 6431 5b30 5d20 3d20   self.cmd1[0] = 
-000029d0: 3139 0a20 2020 2020 2020 2020 2020 2073  19.            s
-000029e0: 656c 662e 636d 6431 5b31 5d20 3d20 696e  elf.cmd1[1] = in
-000029f0: 7428 4174 746e 290a 2020 2020 2020 2020  t(Attn).        
-00002a00: 2020 2020 7365 6c66 2e63 6d64 315b 325d      self.cmd1[2]
-00002a10: 203d 2069 6e74 2828 4174 746e 202d 2069   = int((Attn - i
-00002a20: 6e74 2841 7474 6e29 2920 2a20 3429 0a20  nt(Attn)) * 4). 
-00002a30: 2020 2020 2020 2020 2020 2069 6620 4174             if At
-00002a40: 746e 203e 2073 656c 662e 4d61 7869 6d75  tn > self.Maximu
-00002a50: 6d5f 4174 746e 3a0a 2020 2020 2020 2020  m_Attn:.        
-00002a60: 2020 2020 2020 2020 7072 696e 7428 2741          print('A
-00002a70: 7474 656e 7561 7469 6f6e 206e 6f74 2069  ttenuation not i
-00002a80: 6e20 5261 6e67 652c 7365 7474 696e 6720  n Range,setting 
-00002a90: 6d61 7869 6d75 6d20 3d20 7b7d 2027 2e66  maximum = {} '.f
-00002aa0: 6f72 6d61 7428 7374 7228 7365 6c66 2e4d  ormat(str(self.M
-00002ab0: 6178 696d 756d 5f41 7474 6e29 2929 0a20  aximum_Attn))). 
-00002ac0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00002ad0: 656c 662e 636d 6431 5b31 5d20 3d20 696e  elf.cmd1[1] = in
-00002ae0: 7428 7365 6c66 2e4d 6178 696d 756d 5f41  t(self.Maximum_A
-00002af0: 7474 6e29 0a20 2020 2020 2020 2020 2020  ttn).           
-00002b00: 2020 2020 2073 656c 662e 636d 6431 5b32       self.cmd1[2
-00002b10: 5d20 3d20 696e 7428 2873 656c 662e 4d61  ] = int((self.Ma
-00002b20: 7869 6d75 6d5f 4174 746e 202d 2069 6e74  ximum_Attn - int
-00002b30: 2873 656c 662e 4d61 7869 6d75 6d5f 4174  (self.Maximum_At
-00002b40: 746e 2929 202a 2034 290a 2020 2020 2020  tn)) * 4).      
-00002b50: 2020 2020 2020 2320 7365 6c66 2e64 6576        # self.dev
-00002b60: 2e73 6574 5f63 6f6e 6669 6775 7261 7469  .set_configurati
-00002b70: 6f6e 2829 0a0a 2020 2020 2020 2020 2020  on()..          
-00002b80: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00002b90: 2020 2020 2020 2073 656c 662e 6465 762e         self.dev.
-00002ba0: 7772 6974 6528 3078 3031 2c20 7365 6c66  write(0x01, self
-00002bb0: 2e63 6d64 3129 2020 2320 5365 7420 6174  .cmd1)  # Set at
-00002bc0: 7465 6e75 6174 696f 6e0a 2020 2020 2020  tenuation.      
-00002bd0: 2020 2020 2020 2020 2020 7320 3d20 7365            s = se
-00002be0: 6c66 2e64 6576 2e72 6561 6428 3078 3831  lf.dev.read(0x81
-00002bf0: 2c20 3634 290a 2020 2020 2020 2020 2020  , 64).          
-00002c00: 2020 2020 2020 7365 6c66 2e6e 6577 5f61        self.new_a
-00002c10: 7474 203d 2027 5365 7474 696e 6720 4174  tt = 'Setting At
-00002c20: 7465 6e75 6174 696f 6e20 3d20 7b7d 6442  tenuation = {}dB
-00002c30: 2027 2e66 6f72 6d61 7428 7374 7228 735b   '.format(str(s[
-00002c40: 315d 202b 2073 5b32 5d20 2f20 3429 290a  1] + s[2] / 4)).
-00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c60: 7072 696e 7428 7365 6c66 2e6e 6577 5f61  print(self.new_a
-00002c70: 7474 290a 2020 2020 2020 2020 2020 2020  tt).            
-00002c80: 2020 2020 7265 7475 726e 2073 5b31 5d20      return s[1] 
-00002c90: 2b20 735b 325d 202f 2034 0a20 2020 2020  + s[2] / 4.     
-00002ca0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-00002cb0: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
-00002cc0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00002cd0: 696e 7428 6529 0a20 2020 2020 2020 2020  int(e).         
-00002ce0: 2020 2020 2020 2073 656c 662e 6e65 775f         self.new_
-00002cf0: 6174 7420 3d20 650a 2020 2020 2020 2020  att = e.        
-00002d00: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00002d10: 0a0a 2020 2020 2020 2020 6465 6620 4765  ..        def Ge
-00002d20: 7461 7474 6e28 7365 6c66 293a 0a20 2020  tattn(self):.   
-00002d30: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
-00002d40: 6465 762e 7365 745f 636f 6e66 6967 7572  dev.set_configur
-00002d50: 6174 696f 6e28 290a 2020 2020 2020 2020  ation().        
-00002d60: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00002d70: 2020 2020 2020 2020 2073 656c 662e 636d           self.cm
-00002d80: 6431 5b30 5d20 3d20 3138 0a20 2020 2020  d1[0] = 18.     
-00002d90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002da0: 6465 762e 7772 6974 6528 3078 3031 2c20  dev.write(0x01, 
-00002db0: 7365 6c66 2e63 6d64 3129 2020 2320 4765  self.cmd1)  # Ge
-00002dc0: 7420 6174 7465 6e75 6174 7469 6f6e 0a20  t attenuattion. 
-00002dd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00002de0: 203d 2073 656c 662e 6465 762e 7265 6164   = self.dev.read
-00002df0: 2830 7838 312c 2036 3429 0a20 2020 2020  (0x81, 64).     
-00002e00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002e10: 6e65 775f 6174 7420 3d20 2743 7572 7265  new_att = 'Curre
-00002e20: 6e74 2041 7474 656e 7561 7469 6f6e 203d  nt Attenuation =
-00002e30: 207b 7d64 4220 272e 666f 726d 6174 2873   {}dB '.format(s
-00002e40: 7472 2873 5b31 5d20 2b20 735b 325d 202f  tr(s[1] + s[2] /
-00002e50: 2034 2929 0a20 2020 2020 2020 2020 2020   4)).           
-00002e60: 2020 2020 2070 7269 6e74 2873 656c 662e       print(self.
-00002e70: 6e65 775f 6174 7429 0a20 2020 2020 2020  new_att).       
-00002e80: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00002e90: 735b 315d 202b 2073 5b32 5d20 2f20 340a  s[1] + s[2] / 4.
-00002ea0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00002eb0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00002ec0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00002ed0: 2020 2070 7269 6e74 2865 290a 2020 2020     print(e).    
-00002ee0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002ef0: 2e6e 6577 5f61 7474 203d 2065 0a20 2020  .new_att = e.   
-00002f00: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00002f10: 7572 6e20 730a 0a20 2020 2020 2020 2064  urn s..        d
-00002f20: 6566 2053 656e 645f 5343 5049 2873 656c  ef Send_SCPI(sel
-00002f30: 662c 2053 4350 4963 6d64 2c20 746d 7029  f, SCPIcmd, tmp)
-00002f40: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00002f50: 7365 6e64 2053 4350 4920 636f 6d6d 616e  send SCPI comman
-00002f60: 6473 2028 746f 2073 7570 706f 7274 6564  ds (to supported
-00002f70: 2066 6972 6d77 6172 6520 6f6e 6c79 2129   firmware only!)
-00002f80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00002f90: 662e 636d 6431 5b30 5d20 3d20 3432 0a20  f.cmd1[0] = 42. 
-00002fa0: 2020 2020 2020 2020 2020 206c 3120 3d20             l1 = 
-00002fb0: 300a 2020 2020 2020 2020 2020 2020 6c31  0.            l1
-00002fc0: 203d 206c 656e 2853 4350 4963 6d64 290a   = len(SCPIcmd).
-00002fd0: 2020 2020 2020 2020 2020 2020 696e 6478              indx
-00002fe0: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
-00002ff0: 2077 6869 6c65 2028 696e 6478 203c 3d20   while (indx <= 
-00003000: 6c31 293a 0a20 2020 2020 2020 2020 2020  l1):.           
-00003010: 2020 2020 2073 656c 662e 636d 6431 5b69       self.cmd1[i
-00003020: 6e64 785d 203d 206f 7264 2853 4350 4963  ndx] = ord(SCPIc
-00003030: 6d64 5b69 6e64 7820 2d20 315d 290a 2020  md[indx - 1]).  
-00003040: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00003050: 6478 203d 2069 6e64 7820 2b20 310a 2020  dx = indx + 1.  
-00003060: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00003070: 6d64 315b 696e 6478 5d20 3d20 300a 2020  md1[indx] = 0.  
-00003080: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00003090: 6576 2e77 7269 7465 2830 7830 312c 2073  ev.write(0x01, s
-000030a0: 656c 662e 636d 6431 2920 2023 2053 4350  elf.cmd1)  # SCP
-000030b0: 2043 6f6d 6d61 6e64 2075 7020 746f 2036   Command up to 6
-000030c0: 3020 6368 6172 733b 0a20 2020 2020 2020  0 chars;.       
-000030d0: 2020 2020 2073 203d 2073 656c 662e 6465       s = self.de
-000030e0: 762e 7265 6164 2830 7838 312c 2036 3429  v.read(0x81, 64)
-000030f0: 0a20 2020 2020 2020 2020 2020 2069 203d  .            i =
-00003100: 2031 0a20 2020 2020 2020 2020 2020 2052   1.            R
-00003110: 6574 5374 7220 3d20 2222 0a20 2020 2020  etStr = "".     
-00003120: 2020 2020 2020 2077 6869 6c65 2028 735b         while (s[
-00003130: 695d 203e 2030 293a 0a20 2020 2020 2020  i] > 0):.       
-00003140: 2020 2020 2020 2020 2052 6574 5374 7220           RetStr 
-00003150: 3d20 5265 7453 7472 202b 2063 6872 2873  = RetStr + chr(s
-00003160: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
-00003170: 2020 2020 2069 203d 2069 202b 2031 0a20       i = i + 1. 
-00003180: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00003190: 6e20 7374 7228 5265 7453 7472 290a 0a20  n str(RetStr).. 
-000031a0: 2020 2063 6c61 7373 2041 5049 286f 626a     class API(obj
-000031b0: 6563 7429 3a0a 0a20 2020 2020 2020 2064  ect):..        d
-000031c0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-000031d0: 2c20 636f 6d70 6f72 743d 2241 5554 4f22  , comport="AUTO"
-000031e0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-000031f0: 656c 662e 6261 7564 7261 7465 203d 2039  elf.baudrate = 9
-00003200: 3630 300a 2020 2020 2020 2020 2020 2020  600.            
-00003210: 6966 2063 6f6d 706f 7274 203d 3d20 2241  if comport == "A
-00003220: 5554 4f22 3a0a 2020 2020 2020 2020 2020  UTO":.          
-00003230: 2020 2020 2020 706f 7274 735f 6c69 7374        ports_list
-00003240: 203d 2073 6572 6961 6c5f 706f 7274 7328   = serial_ports(
-00003250: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00003260: 2020 666f 7220 706f 7274 2069 6e20 706f    for port in po
-00003270: 7274 735f 6c69 7374 3a0a 2020 2020 2020  rts_list:.      
-00003280: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00003290: 6c66 2e63 6f6d 706f 7274 203d 2070 6f72  lf.comport = por
-000032a0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-000032b0: 2020 2020 2020 7365 6c66 2e73 203d 2073        self.s = s
-000032c0: 6572 6961 6c2e 5365 7269 616c 2873 656c  erial.Serial(sel
-000032d0: 662e 636f 6d70 6f72 742c 2073 656c 662e  f.comport, self.
-000032e0: 6261 7564 7261 7465 2c20 7469 6d65 6f75  baudrate, timeou
-000032f0: 743d 302e 3529 0a20 2020 2020 2020 2020  t=0.5).         
-00003300: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
-00003310: 2831 290a 2020 2020 2020 2020 2020 2020  (1).            
-00003320: 2020 2020 2020 2020 7365 6c66 2e73 2e66          self.s.f
-00003330: 6c75 7368 496e 7075 7428 290a 2020 2020  lushInput().    
-00003340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003350: 7365 6c66 2e73 2e66 6c75 7368 4f75 7470  self.s.flushOutp
-00003360: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
-00003370: 2020 2020 2020 2020 2073 6c65 6570 2830           sleep(0
-00003380: 2e31 290a 2020 2020 2020 2020 2020 2020  .1).            
-00003390: 2020 2020 2020 2020 2320 5475 726e 2074          # Turn t
-000033a0: 6865 2063 6f6e 736f 6c65 206f 6666 0a20  he console off. 
-000033b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033c0: 2020 2073 656c 662e 732e 7772 6974 6528     self.s.write(
-000033d0: 2243 4f4e 534f 4c45 2044 4953 4142 4c45  "CONSOLE DISABLE
-000033e0: 5c72 5c6e 222e 656e 636f 6465 2829 290a  \r\n".encode()).
-000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003400: 2020 2020 2320 466c 7573 6820 7468 6520      # Flush the 
-00003410: 6275 6666 6572 730a 2020 2020 2020 2020  buffers.        
-00003420: 2020 2020 2020 2020 2020 2020 736c 6565              slee
-00003430: 7028 302e 3129 0a20 2020 2020 2020 2020  p(0.1).         
-00003440: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003450: 732e 666c 7573 6828 290a 2020 2020 2020  s.flush().      
-00003460: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00003470: 6c66 2e73 2e66 6c75 7368 496e 7075 7428  lf.s.flushInput(
-00003480: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00003490: 2020 2020 2020 7365 6c66 2e73 2e66 6c75        self.s.flu
-000034a0: 7368 4f75 7470 7574 2829 0a20 2020 2020  shOutput().     
-000034b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000034c0: 656c 662e 732e 7772 6974 6528 222a 4944  elf.s.write("*ID
-000034d0: 4e3f 5c72 5c6e 222e 656e 636f 6465 2829  N?\r\n".encode()
-000034e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000034f0: 2020 2020 2020 736c 6565 7028 302e 3129        sleep(0.1)
-00003500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003510: 2020 2020 2069 6620 7365 6c66 2e73 2e69       if self.s.i
-00003520: 6e5f 7761 6974 696e 6720 3e20 313a 0a20  n_waiting > 1:. 
-00003530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003540: 2020 2020 2020 2072 6573 7020 3d20 7365         resp = se
-00003550: 6c66 2e73 2e72 6561 646c 696e 6528 292e  lf.s.readline().
-00003560: 6465 636f 6465 2822 7574 662d 3822 290a  decode("utf-8").
-00003570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003580: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00003590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035a0: 2020 7265 7370 203d 2027 270a 2020 2020    resp = ''.    
+00000f20: 2c20 736c 6565 700a 6672 6f6d 2073 7461  , sleep.from sta
+00000f30: 7469 7374 6963 7320 696d 706f 7274 206d  tistics import m
+00000f40: 6f64 650a 696d 706f 7274 2073 7973 0a69  ode.import sys.i
+00000f50: 6d70 6f72 7420 7365 7269 616c 0a69 6d70  mport serial.imp
+00000f60: 6f72 7420 7365 7269 616c 2e74 6f6f 6c73  ort serial.tools
+00000f70: 2e6c 6973 745f 706f 7274 730a 6672 6f6d  .list_ports.from
+00000f80: 2079 6f63 746f 7075 6365 2e79 6f63 746f   yoctopuce.yocto
+00000f90: 5f74 656d 7065 7261 7475 7265 2069 6d70  _temperature imp
+00000fa0: 6f72 7420 5941 5049 2c20 5952 6566 5061  ort YAPI, YRefPa
+00000fb0: 7261 6d2c 2059 5465 6d70 6572 6174 7572  ram, YTemperatur
+00000fc0: 650a 696d 706f 7274 206f 730a 0a0a 636c  e.import os...cl
+00000fd0: 6173 7320 4571 7569 706d 656e 7445 7272  ass EquipmentErr
+00000fe0: 6f72 2845 7863 6570 7469 6f6e 293a 0a0a  or(Exception):..
+00000ff0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00001000: 2873 656c 662c 202a 6172 6773 293a 0a20  (self, *args):. 
+00001010: 2020 2020 2020 2069 6620 6172 6773 3a0a         if args:.
+00001020: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001030: 2e6d 6573 7361 6765 203d 2061 7267 735b  .message = args[
+00001040: 305d 0a20 2020 2020 2020 2065 6c73 653a  0].        else:
+00001050: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00001060: 662e 6d65 7373 6167 6520 3d20 4e6f 6e65  f.message = None
+00001070: 0a0a 2020 2020 6465 6620 5f5f 7374 725f  ..    def __str_
+00001080: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+00001090: 2023 2070 7269 6e74 2827 6361 6c6c 696e   # print('callin
+000010a0: 6720 7374 7227 290a 2020 2020 2020 2020  g str').        
+000010b0: 6966 2073 656c 662e 6d65 7373 6167 653a  if self.message:
+000010c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000010d0: 7572 6e20 2745 7175 6970 6d65 6e74 4572  urn 'EquipmentEr
+000010e0: 726f 723a 207b 6d73 677d 272e 666f 726d  ror: {msg}'.form
+000010f0: 6174 286d 7367 3d73 656c 662e 6d65 7373  at(msg=self.mess
+00001100: 6167 6529 0a20 2020 2020 2020 2065 6c73  age).        els
+00001110: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00001120: 6574 7572 6e20 2745 7175 6970 6d65 6e74  eturn 'Equipment
+00001130: 4572 726f 7220 6861 7320 6265 656e 2072  Error has been r
+00001140: 6169 7365 6427 0a0a 0a64 6566 2073 6572  aised'...def ser
+00001150: 6961 6c5f 706f 7274 7328 293a 0a20 2020  ial_ports():.   
+00001160: 2022 2222 204c 6973 7473 2073 6572 6961   """ Lists seria
+00001170: 6c20 706f 7274 206e 616d 6573 0a0a 2020  l port names..  
+00001180: 2020 2020 2020 3a72 6169 7365 7320 456e        :raises En
+00001190: 7669 726f 6e6d 656e 7445 7272 6f72 3a0a  vironmentError:.
+000011a0: 2020 2020 2020 2020 2020 2020 4f6e 2075              On u
+000011b0: 6e73 7570 706f 7274 6564 206f 7220 756e  nsupported or un
+000011c0: 6b6e 6f77 6e20 706c 6174 666f 726d 730a  known platforms.
+000011d0: 2020 2020 2020 2020 3a72 6574 7572 6e73          :returns
+000011e0: 3a0a 2020 2020 2020 2020 2020 2020 4120  :.            A 
+000011f0: 6c69 7374 206f 6620 7468 6520 7365 7269  list of the seri
+00001200: 616c 2070 6f72 7473 2061 7661 696c 6162  al ports availab
+00001210: 6c65 206f 6e20 7468 6520 7379 7374 656d  le on the system
+00001220: 0a20 2020 2022 2222 0a20 2020 2061 7661  .    """.    ava
+00001230: 696c 6162 6c65 5f70 6f72 7473 203d 205b  ilable_ports = [
+00001240: 732e 6465 7669 6365 2066 6f72 2073 2069  s.device for s i
+00001250: 6e20 7365 7269 616c 2e74 6f6f 6c73 2e6c  n serial.tools.l
+00001260: 6973 745f 706f 7274 732e 636f 6d70 6f72  ist_ports.compor
+00001270: 7473 2829 5d0a 2020 2020 6966 206c 656e  ts()].    if len
+00001280: 2861 7661 696c 6162 6c65 5f70 6f72 7473  (available_ports
+00001290: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
+000012a0: 6176 6169 6c61 626c 655f 706f 7274 7320  available_ports 
+000012b0: 3d20 5b73 2e6e 616d 6520 666f 7220 7320  = [s.name for s 
+000012c0: 696e 2073 6572 6961 6c2e 746f 6f6c 732e  in serial.tools.
+000012d0: 6c69 7374 5f70 6f72 7473 2e63 6f6d 706f  list_ports.compo
+000012e0: 7274 7328 295d 0a20 2020 2020 2020 2069  rts()].        i
+000012f0: 6620 6c65 6e28 6176 6169 6c61 626c 655f  f len(available_
+00001300: 706f 7274 7329 203d 3d20 303a 0a20 2020  ports) == 0:.   
+00001310: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+00001320: 6e6f 2073 6572 6961 6c20 706f 7274 7320  no serial ports 
+00001330: 7765 7265 2066 6f75 6e64 2e20 706c 6561  were found. plea
+00001340: 7365 2063 6865 636b 2079 6f75 7220 636f  se check your co
+00001350: 6e6e 6563 7469 6f6e 7322 290a 2020 2020  nnections").    
+00001360: 7265 7475 726e 2061 7661 696c 6162 6c65  return available
+00001370: 5f70 6f72 7473 0a0a 0a63 6c61 7373 2041  _ports...class A
+00001380: 7474 656e 7561 746f 7228 6f62 6a65 6374  ttenuator(object
+00001390: 293a 0a20 2020 2027 2727 0a20 2020 2053  ):.    '''.    S
+000013a0: 7570 706f 7274 2061 6c6c 2061 7474 6e20  upport all attn 
+000013b0: 636c 6173 7365 7320 666f 723a 0a20 2020  classes for:.   
+000013c0: 2027 2727 0a0a 2020 2020 6465 6620 5f5f   '''..    def __
+000013d0: 696e 6974 5f5f 2873 656c 662c 2041 5454  init__(self, ATT
+000013e0: 4e5f 7479 7065 2c20 636f 6d70 6f72 743d  N_type, comport=
+000013f0: 2741 5554 4f27 293a 0a20 2020 2020 2020  'AUTO'):.       
+00001400: 2069 6620 274d 4344 492d 5553 4227 2069   if 'MCDI-USB' i
+00001410: 6e20 4154 544e 5f74 7970 653a 0a20 2020  n ATTN_type:.   
+00001420: 2020 2020 2020 2020 2073 656c 662e 5f61           self._a
+00001430: 6374 6976 655f 5445 203d 2041 7474 656e  ctive_TE = Atten
+00001440: 7561 746f 722e 4d43 4449 5f55 5342 2829  uator.MCDI_USB()
+00001450: 0a20 2020 2020 2020 2065 6c69 6620 274d  .        elif 'M
+00001460: 4344 4927 2069 6e20 4154 544e 5f74 7970  CDI' in ATTN_typ
+00001470: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00001480: 656c 662e 5f61 6374 6976 655f 5445 203d  elf._active_TE =
+00001490: 2041 7474 656e 7561 746f 722e 4d43 4449   Attenuator.MCDI
+000014a0: 2829 0a20 2020 2020 2020 2065 6c69 6620  ().        elif 
+000014b0: 2741 5049 2720 696e 2041 5454 4e5f 7479  'API' in ATTN_ty
+000014c0: 7065 206f 7220 2757 6569 6e73 6368 656c  pe or 'Weinschel
+000014d0: 2720 696e 2041 5454 4e5f 7479 7065 3a0a  ' in ATTN_type:.
+000014e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000014f0: 2e5f 6163 7469 7665 5f54 4520 3d20 4174  ._active_TE = At
+00001500: 7465 6e75 6174 6f72 2e41 5049 2863 6f6d  tenuator.API(com
+00001510: 706f 7274 290a 0a20 2020 2020 2020 2065  port)..        e
+00001520: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00001530: 2070 6173 730a 0a20 2020 2064 6566 2047   pass..    def G
+00001540: 6574 4163 7469 7665 5445 2873 656c 6629  etActiveTE(self)
+00001550: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00001560: 2073 656c 662e 5f61 6374 6976 655f 5445   self._active_TE
+00001570: 0a0a 2020 2020 636c 6173 7320 4d43 4449  ..    class MCDI
+00001580: 286f 626a 6563 7429 3a0a 0a20 2020 2020  (object):..     
+00001590: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000015a0: 7365 6c66 293a 0a20 2020 2020 2020 2020  self):.         
+000015b0: 2020 2064 6f74 6e65 7420 3d20 4661 6c73     dotnet = Fals
+000015c0: 650a 2020 2020 2020 2020 2020 2020 7574  e.            ut
+000015d0: 696c 735f 6469 7220 3d20 6f73 2e70 6174  ils_dir = os.pat
+000015e0: 682e 6a6f 696e 286f 732e 7061 7468 2e64  h.join(os.path.d
+000015f0: 6972 6e61 6d65 285f 5f66 696c 655f 5f29  irname(__file__)
+00001600: 2c20 2775 7469 6c73 2729 0a20 2020 2020  , 'utils').     
+00001610: 2020 2020 2020 2073 7973 2e70 6174 682e         sys.path.
+00001620: 6170 7065 6e64 2875 7469 6c73 5f64 6972  append(utils_dir
+00001630: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00001640: 2064 6f74 6e65 7420 3d3d 2054 7275 653a   dotnet == True:
+00001650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001660: 2069 6d70 6f72 7420 636c 7220 2023 2070   import clr  # p
+00001670: 7974 686f 6e6e 6574 2c20 6d61 6e75 616c  ythonnet, manual
+00001680: 6c79 2069 6e73 7461 6c6c 6564 2077 6974  ly installed wit
+00001690: 6820 6120 646f 776e 6c6f 6164 6564 2077  h a downloaded w
+000016a0: 6865 656c 2061 6e64 2070 6970 0a20 2020  heel and pip.   
+000016b0: 2020 2020 2020 2020 2020 2020 2069 6d70               imp
+000016c0: 6f72 7420 6374 7970 6573 2020 2320 6d6f  ort ctypes  # mo
+000016d0: 6475 6c65 2074 6f20 6f70 656e 2075 7469  dule to open uti
+000016e0: 6c73 2066 696c 6573 0a20 2020 2020 2020  ls files.       
+000016f0: 2020 2020 2020 2020 2063 6c72 2e41 6464           clr.Add
+00001700: 5265 6665 7265 6e63 6528 2253 7973 7465  Reference("Syste
+00001710: 6d2e 494f 2229 0a20 2020 2020 2020 2020  m.IO").         
+00001720: 2020 2020 2020 2069 6d70 6f72 7420 5379         import Sy
+00001730: 7374 656d 2e49 4f0a 2020 2020 2020 2020  stem.IO.        
+00001740: 2020 2020 2020 2020 5379 7374 656d 2e49          System.I
+00001750: 4f2e 4469 7265 6374 6f72 792e 5365 7443  O.Directory.SetC
+00001760: 7572 7265 6e74 4469 7265 6374 6f72 7928  urrentDirectory(
+00001770: 7574 696c 735f 6469 7229 0a20 2020 2020  utils_dir).     
+00001780: 2020 2020 2020 2020 2020 2063 6c72 2e41             clr.A
+00001790: 6464 5265 6665 7265 6e63 6528 276d 636c  ddReference('mcl
+000017a0: 5f52 5544 4154 5f4e 4554 3435 2729 0a20  _RUDAT_NET45'). 
+000017b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000017c0: 726f 6d20 6d63 6c5f 5255 4441 545f 4e45  rom mcl_RUDAT_NE
+000017d0: 5434 3520 696d 706f 7274 2055 5342 5f52  T45 import USB_R
+000017e0: 5544 4154 0a20 2020 2020 2020 2020 2020  UDAT.           
+000017f0: 2020 2020 2073 656c 662e 4465 7669 6365       self.Device
+00001800: 203d 2055 5342 5f52 5544 4154 2829 0a20   = USB_RUDAT(). 
+00001810: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001820: 656c 662e 4465 7669 6365 2e43 6f6e 6e65  elf.Device.Conne
+00001830: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
+00001840: 2020 2020 2069 6e66 6f20 3d20 7365 6c66       info = self
+00001850: 2e44 6576 6963 6549 6e66 6f28 290a 2020  .DeviceInfo().  
+00001860: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00001870: 696e 7428 2746 6f75 6e64 2041 7474 656e  int('Found Atten
+00001880: 7561 746f 723a 204d 6f64 656c 207b 7d2c  uator: Model {},
+00001890: 207b 7d20 2c7b 7d20 272e 666f 726d 6174   {} ,{} '.format
+000018a0: 2869 6e66 6f5b 305d 2c20 696e 666f 5b31  (info[0], info[1
+000018b0: 5d2c 2069 6e66 6f5b 325d 2929 0a20 2020  ], info[2])).   
+000018c0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+000018d0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000018e0: 726f 6d20 5553 425f 5255 4441 5420 696d  rom USB_RUDAT im
+000018f0: 706f 7274 2055 5342 4441 540a 2020 2020  port USBDAT.    
+00001900: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001910: 2e44 6576 6963 6520 3d20 5553 4244 4154  .Device = USBDAT
+00001920: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00001930: 2020 2069 6e66 6f20 3d20 7365 6c66 2e44     info = self.D
+00001940: 6576 6963 6549 6e66 6f28 290a 2020 2020  eviceInfo().    
+00001950: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00001960: 7428 2746 6f75 6e64 2041 7474 656e 7561  t('Found Attenua
+00001970: 746f 723a 204d 6f64 656c 207b 7d2c 207b  tor: Model {}, {
+00001980: 7d20 2c7b 7d20 272e 666f 726d 6174 2869  } ,{} '.format(i
+00001990: 6e66 6f5b 305d 2c20 696e 666f 5b31 5d2c  nfo[0], info[1],
+000019a0: 2069 6e66 6f5b 325d 2929 0a0a 2020 2020   info[2]))..    
+000019b0: 2020 2020 6465 6620 4465 7669 6365 496e      def DeviceIn
+000019c0: 666f 2873 656c 6629 3a0a 2020 2020 2020  fo(self):.      
+000019d0: 2020 2020 2020 636d 6420 3d20 223a 4d4e        cmd = ":MN
+000019e0: 3f22 0a20 2020 2020 2020 2020 2020 206d  ?".            m
+000019f0: 6f64 656c 5f6e 616d 6520 3d20 7365 6c66  odel_name = self
+00001a00: 2e44 6576 6963 652e 5365 6e64 5f53 4350  .Device.Send_SCP
+00001a10: 4928 636d 642c 2022 2229 0a20 2020 2020  I(cmd, "").     
+00001a20: 2020 2020 2020 2063 6d64 203d 2022 3a53         cmd = ":S
+00001a30: 4e3f 220a 2020 2020 2020 2020 2020 2020  N?".            
+00001a40: 7365 7269 616c 203d 2073 656c 662e 4465  serial = self.De
+00001a50: 7669 6365 2e53 656e 645f 5343 5049 2863  vice.Send_SCPI(c
+00001a60: 6d64 2c20 2222 290a 2020 2020 2020 2020  md, "").        
+00001a70: 2020 2020 636d 6420 3d20 223a 4649 524d      cmd = ":FIRM
+00001a80: 5741 5245 3f22 0a20 2020 2020 2020 2020  WARE?".         
+00001a90: 2020 2066 7720 3d20 7365 6c66 2e44 6576     fw = self.Dev
+00001aa0: 6963 652e 5365 6e64 5f53 4350 4928 636d  ice.Send_SCPI(cm
+00001ab0: 642c 2022 2229 0a20 2020 2020 2020 2020  d, "").         
+00001ac0: 2020 2023 2072 6574 7572 6e20 5b6d 6f64     # return [mod
+00001ad0: 656c 5f6e 616d 655b 315d 2c20 7365 7269  el_name[1], seri
+00001ae0: 616c 5b31 5d2c 2066 775b 315d 5d20 2023  al[1], fw[1]]  #
+00001af0: 646f 746e 6574 0a20 2020 2020 2020 2020  dotnet.         
+00001b00: 2020 2072 6574 7572 6e20 5b6d 6f64 656c     return [model
+00001b10: 5f6e 616d 652c 2073 6572 6961 6c2c 2066  _name, serial, f
+00001b20: 775d 0a0a 2020 2020 2020 2020 6465 6620  w]..        def 
+00001b30: 5365 7461 7474 6e28 7365 6c66 2c20 6174  Setattn(self, at
+00001b40: 746e 293a 0a20 2020 2020 2020 2020 2020  tn):.           
+00001b50: 2063 6d64 203d 2022 3a53 4554 4154 543a   cmd = ":SETATT:
+00001b60: 2220 2b20 7374 7228 6174 746e 290a 2020  " + str(attn).  
+00001b70: 2020 2020 2020 2020 2020 7374 6174 7573            status
+00001b80: 203d 2069 6e74 2873 656c 662e 4465 7669   = int(self.Devi
+00001b90: 6365 2e53 656e 645f 5343 5049 2863 6d64  ce.Send_SCPI(cmd
+00001ba0: 2c20 2222 2929 0a20 2020 2020 2020 2020  , "")).         
+00001bb0: 2020 2069 6620 7374 6174 7573 203d 3d20     if status == 
+00001bc0: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+00001bd0: 2020 2070 7269 6e74 2827 436f 6d6d 616e     print('Comman
+00001be0: 6420 6661 696c 6564 206f 7220 696e 7661  d failed or inva
+00001bf0: 6c69 6420 6174 7465 6e75 6174 696f 6e20  lid attenuation 
+00001c00: 7365 7427 290a 2020 2020 2020 2020 2020  set').          
+00001c10: 2020 656c 6966 2073 7461 7475 7320 3d3d    elif status ==
+00001c20: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+00001c30: 2020 2020 2320 7072 696e 7428 2743 6f6d      # print('Com
+00001c40: 6d61 6e64 2063 6f6d 706c 6574 6564 2073  mand completed s
+00001c50: 7563 6365 7373 6675 6c6c 7927 290a 2020  uccessfully').  
+00001c60: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00001c70: 696e 7428 2741 7474 656e 7561 7469 6f6e  int('Attenuation
+00001c80: 2073 6574 2074 6f20 207b 7d5b 6442 5d27   set to  {}[dB]'
+00001c90: 2e66 6f72 6d61 7428 666c 6f61 7428 7365  .format(float(se
+00001ca0: 6c66 2e47 6574 6174 746e 2829 2929 290a  lf.Getattn()))).
+00001cb0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00001cc0: 2073 7461 7475 7320 3d3d 2032 3a0a 2020   status == 2:.  
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00001ce0: 696e 7428 0a20 2020 2020 2020 2020 2020  int(.           
+00001cf0: 2020 2020 2020 2020 2027 5265 7175 6573           'Reques
+00001d00: 7465 6420 6174 7465 6e75 6174 696f 6e20  ted attenuation 
+00001d10: 7761 7320 6869 6768 6572 2074 6861 6e20  was higher than 
+00001d20: 7468 6520 616c 6c6f 7765 6420 7261 6e67  the allowed rang
+00001d30: 652c 2074 6865 2061 7474 656e 7561 7469  e, the attenuati
+00001d40: 6f6e 2077 6173 2073 6574 2074 6f20 7468  on was set to th
+00001d50: 6520 6465 7669 6365 efbf bd73 206d 6178  e device...s max
+00001d60: 696d 756d 2061 6c6c 6f77 6564 2076 616c  imum allowed val
+00001d70: 7565 2729 0a20 2020 2020 2020 2020 2020  ue').           
+00001d80: 2023 2070 7269 6e74 2873 7461 7475 7329   # print(status)
+00001d90: 0a0a 2020 2020 2020 2020 6465 6620 4765  ..        def Ge
+00001da0: 7461 7474 6e28 7365 6c66 293a 0a20 2020  tattn(self):.   
+00001db0: 2020 2020 2020 2020 2063 6d64 203d 2022           cmd = "
+00001dc0: 3a41 5454 3f22 0a20 2020 2020 2020 2020  :ATT?".         
+00001dd0: 2020 2052 6573 7020 3d20 666c 6f61 7428     Resp = float(
+00001de0: 7365 6c66 2e44 6576 6963 652e 5365 6e64  self.Device.Send
+00001df0: 5f53 4350 4928 636d 642c 2022 2229 290a  _SCPI(cmd, "")).
+00001e00: 2020 2020 2020 2020 2020 2020 2320 7072              # pr
+00001e10: 696e 7428 5265 7370 290a 2020 2020 2020  int(Resp).      
+00001e20: 2020 2020 2020 2320 6966 2073 7461 7475        # if statu
+00001e30: 7320 3d3d 2030 3a0a 2020 2020 2020 2020  s == 0:.        
+00001e40: 2020 2020 2320 2020 2020 7072 696e 7428      #     print(
+00001e50: 2743 6f6d 6d61 6e64 2066 6169 6c65 6420  'Command failed 
+00001e60: 6f72 2069 6e76 616c 6964 2061 7474 656e  or invalid atten
+00001e70: 7561 7469 6f6e 2073 6574 2729 0a20 2020  uation set').   
+00001e80: 2020 2020 2020 2020 2023 2065 6c69 6620           # elif 
+00001e90: 7374 6174 7573 203d 3d20 313a 0a20 2020  status == 1:.   
+00001ea0: 2020 2020 2020 2020 2023 2020 2020 2070           #     p
+00001eb0: 7269 6e74 2827 436f 6d6d 616e 6420 636f  rint('Command co
+00001ec0: 6d70 6c65 7465 6420 7375 6363 6573 7366  mpleted successf
+00001ed0: 756c 6c79 2729 0a20 2020 2020 2020 2020  ully').         
+00001ee0: 2020 2072 6574 7572 6e20 5265 7370 0a0a     return Resp..
+00001ef0: 2020 2020 636c 6173 7320 4d43 4449 5f55      class MCDI_U
+00001f00: 5342 286f 626a 6563 7429 3a0a 2020 2020  SB(object):.    
+00001f10: 2020 2020 2320 3634 2062 6974 2061 7272      # 64 bit arr
+00001f20: 6179 2074 6f20 7365 6e64 2074 6f20 5553  ay to send to US
+00001f30: 420a 2020 2020 2020 2020 636d 6431 203d  B.        cmd1 =
+00001f40: 205b 302c 2030 2c20 302c 2030 2c20 302c   [0, 0, 0, 0, 0,
+00001f50: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+00001f60: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
+00001f70: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
+00001f80: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+00001f90: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
+00001fa0: 2c20 302c 2030 2c20 302c 0a20 2020 2020  , 0, 0, 0,.     
+00001fb0: 2020 2020 2020 2020 2020 2030 2c20 302c             0, 0,
+00001fc0: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+00001fd0: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
+00001fe0: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
+00001ff0: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+00002000: 302c 2030 2c20 302c 2030 2c20 302c 0a20  0, 0, 0, 0, 0,. 
+00002010: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+00002020: 5d20 2023 2036 3420 6269 7420 6172 7261  ]  # 64 bit arra
+00002030: 7920 746f 2073 656e 6420 746f 2055 5342  y to send to USB
+00002040: 0a0a 2020 2020 2020 2020 6465 6620 5f5f  ..        def __
+00002050: 696e 6974 5f5f 2873 656c 6629 3a0a 2020  init__(self):.  
+00002060: 2020 2020 2020 2020 2020 2320 6669 6e64            # find
+00002070: 2074 6865 2064 6576 6963 650a 2020 2020   the device.    
+00002080: 2020 2020 2020 2020 7365 6c66 2e64 6576          self.dev
+00002090: 203d 2075 7362 2e63 6f72 652e 6669 6e64   = usb.core.find
+000020a0: 2869 6456 656e 646f 723d 3078 3230 6365  (idVendor=0x20ce
+000020b0: 2c20 6964 5072 6f64 7563 743d 3078 3030  , idProduct=0x00
+000020c0: 3233 290a 2020 2020 2020 2020 2020 2020  23).            
+000020d0: 2320 7761 7320 6974 2066 6f75 6e64 3f0a  # was it found?.
+000020e0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000020f0: 656c 662e 6465 7620 6973 204e 6f6e 653a  elf.dev is None:
+00002100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002110: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00002120: 7228 2744 6576 6963 6520 6e6f 7420 666f  r('Device not fo
+00002130: 756e 6427 290a 2020 2020 2020 2020 2020  und').          
+00002140: 2020 2320 7365 7420 7468 6520 6163 7469    # set the acti
+00002150: 7665 2063 6f6e 6669 6775 7261 7469 6f6e  ve configuration
+00002160: 2e20 7769 7468 206e 6f20 6172 6773 2077  . with no args w
+00002170: 6520 7573 6520 6669 7273 7420 636f 6e66  e use first conf
+00002180: 6967 2e0a 2020 2020 2020 2020 2020 2020  ig..            
+00002190: 2320 2066 6f72 204c 696e 7578 206f 6e6c  #  for Linux onl
+000021a0: 790a 2020 2020 2020 2020 2020 2020 6966  y.            if
+000021b0: 2073 7973 2e70 6c61 7466 6f72 6d20 3d3d   sys.platform ==
+000021c0: 2027 6c69 6e75 7827 3a0a 0a20 2020 2020   'linux':..     
+000021d0: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
+000021e0: 6f6e 6669 6775 7261 7469 6f6e 2069 6e20  onfiguration in 
+000021f0: 7365 6c66 2e64 6576 3a0a 2020 2020 2020  self.dev:.      
+00002200: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00002210: 7220 696e 7465 7266 6163 6520 696e 2063  r interface in c
+00002220: 6f6e 6669 6775 7261 7469 6f6e 3a0a 2020  onfiguration:.  
+00002230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002240: 2020 2020 2020 6966 6e75 6d20 3d20 696e        ifnum = in
+00002250: 7465 7266 6163 652e 6249 6e74 6572 6661  terface.bInterfa
+00002260: 6365 4e75 6d62 6572 0a20 2020 2020 2020  ceNumber.       
+00002270: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00002280: 6e6f 7420 7365 6c66 2e64 6576 2e69 735f  not self.dev.is_
+00002290: 6b65 726e 656c 5f64 7269 7665 725f 6163  kernel_driver_ac
+000022a0: 7469 7665 2869 666e 756d 293a 0a20 2020  tive(ifnum):.   
+000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022c0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+000022d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022e0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+000022f0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00002300: 2070 7269 6e74 2022 6465 7461 6368 206b   print "detach k
+00002310: 6572 6e65 6c20 6472 6976 6572 2066 726f  ernel driver fro
+00002320: 6d20 6465 7669 6365 2025 733a 2069 6e74  m device %s: int
+00002330: 6572 6661 6365 2025 7322 2025 2028 6465  erface %s" % (de
+00002340: 762c 2069 666e 756d 290a 2020 2020 2020  v, ifnum).      
+00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002360: 2020 7365 6c66 2e64 6576 2e64 6574 6163    self.dev.detac
+00002370: 685f 6b65 726e 656c 5f64 7269 7665 7228  h_kernel_driver(
+00002380: 6966 6e75 6d29 0a20 2020 2020 2020 2020  ifnum).         
+00002390: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+000023a0: 7420 7573 622e 636f 7265 2e55 5342 4572  t usb.core.USBEr
+000023b0: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
+000023c0: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+000023d0: 730a 0a20 2020 2020 2020 2020 2020 2073  s..            s
+000023e0: 656c 662e 6465 762e 7365 745f 636f 6e66  elf.dev.set_conf
+000023f0: 6967 7572 6174 696f 6e28 290a 2020 2020  iguration().    
+00002400: 2020 2020 2020 2020 7365 6c66 2e63 6d64          self.cmd
+00002410: 315b 305d 203d 2034 310a 2020 2020 2020  1[0] = 41.      
+00002420: 2020 2020 2020 7365 6c66 2e64 6576 2e77        self.dev.w
+00002430: 7269 7465 2830 7830 312c 2073 656c 662e  rite(0x01, self.
+00002440: 636d 6431 2920 2023 2053 4e0a 2020 2020  cmd1)  # SN.    
+00002450: 2020 2020 2020 2020 7320 3d20 7365 6c66          s = self
+00002460: 2e64 6576 2e72 6561 6428 3078 3831 2c20  .dev.read(0x81, 
+00002470: 3634 290a 2020 2020 2020 2020 2020 2020  64).            
+00002480: 7365 6c66 2e53 6572 6961 6c4e 756d 6265  self.SerialNumbe
+00002490: 7220 3d20 2222 0a20 2020 2020 2020 2020  r = "".         
+000024a0: 2020 2069 203d 2031 0a20 2020 2020 2020     i = 1.       
+000024b0: 2020 2020 2077 6869 6c65 2028 735b 695d       while (s[i]
+000024c0: 203e 2030 293a 0a20 2020 2020 2020 2020   > 0):.         
+000024d0: 2020 2020 2020 2073 656c 662e 5365 7269         self.Seri
+000024e0: 616c 4e75 6d62 6572 203d 2073 656c 662e  alNumber = self.
+000024f0: 5365 7269 616c 4e75 6d62 6572 202b 2063  SerialNumber + c
+00002500: 6872 2873 5b69 5d29 0a20 2020 2020 2020  hr(s[i]).       
+00002510: 2020 2020 2020 2020 2069 203d 2069 202b           i = i +
+00002520: 2031 0a20 2020 2020 2020 2020 2020 2073   1.            s
+00002530: 656c 662e 636d 6431 5b30 5d20 3d20 3430  elf.cmd1[0] = 40
+00002540: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00002550: 662e 6465 762e 7772 6974 6528 3078 3031  f.dev.write(0x01
+00002560: 2c20 7365 6c66 2e63 6d64 3129 2020 2320  , self.cmd1)  # 
+00002570: 4d6f 6465 6c0a 2020 2020 2020 2020 2020  Model.          
+00002580: 2020 7320 3d20 7365 6c66 2e64 6576 2e72    s = self.dev.r
+00002590: 6561 6428 3078 3831 2c20 3634 290a 2020  ead(0x81, 64).  
+000025a0: 2020 2020 2020 2020 2020 7365 6c66 2e4d            self.M
+000025b0: 6f64 656c 4e61 6d65 203d 2022 220a 2020  odelName = "".  
+000025c0: 2020 2020 2020 2020 2020 6920 3d20 310a            i = 1.
+000025d0: 2020 2020 2020 2020 2020 2020 7768 696c              whil
+000025e0: 6520 2873 5b69 5d20 3e20 3029 3a0a 2020  e (s[i] > 0):.  
+000025f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00002600: 6c66 2e4d 6f64 656c 4e61 6d65 203d 2073  lf.ModelName = s
+00002610: 656c 662e 4d6f 6465 6c4e 616d 6520 2b20  elf.ModelName + 
+00002620: 6368 7228 735b 695d 290a 2020 2020 2020  chr(s[i]).      
+00002630: 2020 2020 2020 2020 2020 6920 3d20 6920            i = i 
+00002640: 2b20 310a 0a20 2020 2020 2020 2020 2020  + 1..           
+00002650: 2073 656c 662e 4d61 7869 6d75 6d5f 4174   self.Maximum_At
+00002660: 746e 203d 2066 6c6f 6174 2873 656c 662e  tn = float(self.
+00002670: 4d6f 6465 6c4e 616d 655b 3131 3a5d 290a  ModelName[11:]).
+00002680: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002690: 2e63 6d64 315b 305d 203d 2039 390a 2020  .cmd1[0] = 99.  
+000026a0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+000026b0: 6576 2e77 7269 7465 2830 7830 312c 2073  ev.write(0x01, s
+000026c0: 656c 662e 636d 6431 2920 2023 2046 570a  elf.cmd1)  # FW.
+000026d0: 2020 2020 2020 2020 2020 2020 7320 3d20              s = 
+000026e0: 7365 6c66 2e64 6576 2e72 6561 6428 3078  self.dev.read(0x
+000026f0: 3831 2c20 3634 290a 2020 2020 2020 2020  81, 64).        
+00002700: 2020 2020 7365 6c66 2e46 5720 3d20 2222      self.FW = ""
+00002710: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00002720: 662e 4657 203d 2063 6872 2873 5b35 5d29  f.FW = chr(s[5])
+00002730: 202b 2063 6872 2873 5b36 5d29 0a20 2020   + chr(s[6]).   
+00002740: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+00002750: 6174 7573 5f6d 6573 7361 6765 203d 2027  atus_message = '
+00002760: 466f 756e 6420 4174 7465 6e75 6174 6f72  Found Attenuator
+00002770: 3a20 4d6f 6465 6c20 7b7d 2c20 534e 3a20  : Model {}, SN: 
+00002780: 7b7d 202c 2046 573a 207b 7d2c 204d 6178  {} , FW: {}, Max
+00002790: 696d 756d 2061 7474 656e 7561 7469 6f6e  imum attenuation
+000027a0: 3a20 7b7d 6442 2027 2e66 6f72 6d61 7428  : {}dB '.format(
+000027b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000027c0: 2073 7472 2873 656c 662e 4d6f 6465 6c4e   str(self.ModelN
+000027d0: 616d 6529 2c20 7374 7228 7365 6c66 2e53  ame), str(self.S
+000027e0: 6572 6961 6c4e 756d 6265 7229 2c20 7374  erialNumber), st
+000027f0: 7228 7365 6c66 2e46 5729 2c20 7374 7228  r(self.FW), str(
+00002800: 7365 6c66 2e4d 6178 696d 756d 5f41 7474  self.Maximum_Att
+00002810: 6e29 290a 2020 2020 2020 2020 2020 2020  n)).            
+00002820: 7072 696e 7428 7365 6c66 2e73 7461 7475  print(self.statu
+00002830: 735f 6d65 7373 6167 6529 0a0a 2020 2020  s_message)..    
+00002840: 2020 2020 6465 6620 5265 6164 534e 2873      def ReadSN(s
+00002850: 656c 6629 3a0a 2020 2020 2020 2020 2020  elf):.          
+00002860: 2020 7265 7475 726e 2073 7472 2873 656c    return str(sel
+00002870: 662e 5365 7269 616c 4e75 6d62 6572 290a  f.SerialNumber).
+00002880: 0a20 2020 2020 2020 2064 6566 2052 6561  .        def Rea
+00002890: 644d 4e28 7365 6c66 293a 0a20 2020 2020  dMN(self):.     
+000028a0: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
+000028b0: 7228 7365 6c66 2e4d 6f64 656c 4e61 6d65  r(self.ModelName
+000028c0: 290a 0a20 2020 2020 2020 2064 6566 2052  )..        def R
+000028d0: 6561 6446 5728 7365 6c66 293a 0a20 2020  eadFW(self):.   
+000028e0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000028f0: 7374 7228 7365 6c66 2e46 5729 0a0a 2020  str(self.FW)..  
+00002900: 2020 2020 2020 6465 6620 5265 6164 4d61        def ReadMa
+00002910: 7852 616e 6765 2873 656c 6629 3a0a 2020  xRange(self):.  
+00002920: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00002930: 2073 656c 662e 4d61 7869 6d75 6d5f 4174   self.Maximum_At
+00002940: 746e 0a0a 2020 2020 2020 2020 6465 6620  tn..        def 
+00002950: 5365 7461 7474 6e28 7365 6c66 2c20 4174  Setattn(self, At
+00002960: 746e 293a 0a20 2020 2020 2020 2020 2020  tn):.           
+00002970: 2073 656c 662e 636d 6431 5b30 5d20 3d20   self.cmd1[0] = 
+00002980: 3139 0a20 2020 2020 2020 2020 2020 2073  19.            s
+00002990: 656c 662e 636d 6431 5b31 5d20 3d20 696e  elf.cmd1[1] = in
+000029a0: 7428 4174 746e 290a 2020 2020 2020 2020  t(Attn).        
+000029b0: 2020 2020 7365 6c66 2e63 6d64 315b 325d      self.cmd1[2]
+000029c0: 203d 2069 6e74 2828 4174 746e 202d 2069   = int((Attn - i
+000029d0: 6e74 2841 7474 6e29 2920 2a20 3429 0a20  nt(Attn)) * 4). 
+000029e0: 2020 2020 2020 2020 2020 2069 6620 4174             if At
+000029f0: 746e 203e 2073 656c 662e 4d61 7869 6d75  tn > self.Maximu
+00002a00: 6d5f 4174 746e 3a0a 2020 2020 2020 2020  m_Attn:.        
+00002a10: 2020 2020 2020 2020 7072 696e 7428 2741          print('A
+00002a20: 7474 656e 7561 7469 6f6e 206e 6f74 2069  ttenuation not i
+00002a30: 6e20 5261 6e67 652c 7365 7474 696e 6720  n Range,setting 
+00002a40: 6d61 7869 6d75 6d20 3d20 7b7d 2027 2e66  maximum = {} '.f
+00002a50: 6f72 6d61 7428 7374 7228 7365 6c66 2e4d  ormat(str(self.M
+00002a60: 6178 696d 756d 5f41 7474 6e29 2929 0a20  aximum_Attn))). 
+00002a70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002a80: 656c 662e 636d 6431 5b31 5d20 3d20 696e  elf.cmd1[1] = in
+00002a90: 7428 7365 6c66 2e4d 6178 696d 756d 5f41  t(self.Maximum_A
+00002aa0: 7474 6e29 0a20 2020 2020 2020 2020 2020  ttn).           
+00002ab0: 2020 2020 2073 656c 662e 636d 6431 5b32       self.cmd1[2
+00002ac0: 5d20 3d20 696e 7428 2873 656c 662e 4d61  ] = int((self.Ma
+00002ad0: 7869 6d75 6d5f 4174 746e 202d 2069 6e74  ximum_Attn - int
+00002ae0: 2873 656c 662e 4d61 7869 6d75 6d5f 4174  (self.Maximum_At
+00002af0: 746e 2929 202a 2034 290a 2020 2020 2020  tn)) * 4).      
+00002b00: 2020 2020 2020 2320 7365 6c66 2e64 6576        # self.dev
+00002b10: 2e73 6574 5f63 6f6e 6669 6775 7261 7469  .set_configurati
+00002b20: 6f6e 2829 0a0a 2020 2020 2020 2020 2020  on()..          
+00002b30: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00002b40: 2020 2020 2020 2073 656c 662e 6465 762e         self.dev.
+00002b50: 7772 6974 6528 3078 3031 2c20 7365 6c66  write(0x01, self
+00002b60: 2e63 6d64 3129 2020 2320 5365 7420 6174  .cmd1)  # Set at
+00002b70: 7465 6e75 6174 696f 6e0a 2020 2020 2020  tenuation.      
+00002b80: 2020 2020 2020 2020 2020 7320 3d20 7365            s = se
+00002b90: 6c66 2e64 6576 2e72 6561 6428 3078 3831  lf.dev.read(0x81
+00002ba0: 2c20 3634 290a 2020 2020 2020 2020 2020  , 64).          
+00002bb0: 2020 2020 2020 7365 6c66 2e6e 6577 5f61        self.new_a
+00002bc0: 7474 203d 2027 5365 7474 696e 6720 4174  tt = 'Setting At
+00002bd0: 7465 6e75 6174 696f 6e20 3d20 7b7d 6442  tenuation = {}dB
+00002be0: 2027 2e66 6f72 6d61 7428 7374 7228 735b   '.format(str(s[
+00002bf0: 315d 202b 2073 5b32 5d20 2f20 3429 290a  1] + s[2] / 4)).
+00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c10: 7072 696e 7428 7365 6c66 2e6e 6577 5f61  print(self.new_a
+00002c20: 7474 290a 2020 2020 2020 2020 2020 2020  tt).            
+00002c30: 2020 2020 7265 7475 726e 2073 5b31 5d20      return s[1] 
+00002c40: 2b20 735b 325d 202f 2034 0a20 2020 2020  + s[2] / 4.     
+00002c50: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+00002c60: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
+00002c70: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00002c80: 696e 7428 6529 0a20 2020 2020 2020 2020  int(e).         
+00002c90: 2020 2020 2020 2073 656c 662e 6e65 775f         self.new_
+00002ca0: 6174 7420 3d20 650a 2020 2020 2020 2020  att = e.        
+00002cb0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00002cc0: 0a0a 2020 2020 2020 2020 6465 6620 4765  ..        def Ge
+00002cd0: 7461 7474 6e28 7365 6c66 293a 0a20 2020  tattn(self):.   
+00002ce0: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
+00002cf0: 6465 762e 7365 745f 636f 6e66 6967 7572  dev.set_configur
+00002d00: 6174 696f 6e28 290a 2020 2020 2020 2020  ation().        
+00002d10: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00002d20: 2020 2020 2020 2020 2073 656c 662e 636d           self.cm
+00002d30: 6431 5b30 5d20 3d20 3138 0a20 2020 2020  d1[0] = 18.     
+00002d40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002d50: 6465 762e 7772 6974 6528 3078 3031 2c20  dev.write(0x01, 
+00002d60: 7365 6c66 2e63 6d64 3129 2020 2320 4765  self.cmd1)  # Ge
+00002d70: 7420 6174 7465 6e75 6174 7469 6f6e 0a20  t attenuattion. 
+00002d80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002d90: 203d 2073 656c 662e 6465 762e 7265 6164   = self.dev.read
+00002da0: 2830 7838 312c 2036 3429 0a20 2020 2020  (0x81, 64).     
+00002db0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002dc0: 6e65 775f 6174 7420 3d20 2743 7572 7265  new_att = 'Curre
+00002dd0: 6e74 2041 7474 656e 7561 7469 6f6e 203d  nt Attenuation =
+00002de0: 207b 7d64 4220 272e 666f 726d 6174 2873   {}dB '.format(s
+00002df0: 7472 2873 5b31 5d20 2b20 735b 325d 202f  tr(s[1] + s[2] /
+00002e00: 2034 2929 0a20 2020 2020 2020 2020 2020   4)).           
+00002e10: 2020 2020 2070 7269 6e74 2873 656c 662e       print(self.
+00002e20: 6e65 775f 6174 7429 0a20 2020 2020 2020  new_att).       
+00002e30: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00002e40: 735b 315d 202b 2073 5b32 5d20 2f20 340a  s[1] + s[2] / 4.
+00002e50: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00002e60: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00002e70: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00002e80: 2020 2070 7269 6e74 2865 290a 2020 2020     print(e).    
+00002e90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002ea0: 2e6e 6577 5f61 7474 203d 2065 0a20 2020  .new_att = e.   
+00002eb0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00002ec0: 7572 6e20 730a 0a20 2020 2020 2020 2064  urn s..        d
+00002ed0: 6566 2053 656e 645f 5343 5049 2873 656c  ef Send_SCPI(sel
+00002ee0: 662c 2053 4350 4963 6d64 2c20 746d 7029  f, SCPIcmd, tmp)
+00002ef0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00002f00: 7365 6e64 2053 4350 4920 636f 6d6d 616e  send SCPI comman
+00002f10: 6473 2028 746f 2073 7570 706f 7274 6564  ds (to supported
+00002f20: 2066 6972 6d77 6172 6520 6f6e 6c79 2129   firmware only!)
+00002f30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00002f40: 662e 636d 6431 5b30 5d20 3d20 3432 0a20  f.cmd1[0] = 42. 
+00002f50: 2020 2020 2020 2020 2020 206c 3120 3d20             l1 = 
+00002f60: 300a 2020 2020 2020 2020 2020 2020 6c31  0.            l1
+00002f70: 203d 206c 656e 2853 4350 4963 6d64 290a   = len(SCPIcmd).
+00002f80: 2020 2020 2020 2020 2020 2020 696e 6478              indx
+00002f90: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
+00002fa0: 2077 6869 6c65 2028 696e 6478 203c 3d20   while (indx <= 
+00002fb0: 6c31 293a 0a20 2020 2020 2020 2020 2020  l1):.           
+00002fc0: 2020 2020 2073 656c 662e 636d 6431 5b69       self.cmd1[i
+00002fd0: 6e64 785d 203d 206f 7264 2853 4350 4963  ndx] = ord(SCPIc
+00002fe0: 6d64 5b69 6e64 7820 2d20 315d 290a 2020  md[indx - 1]).  
+00002ff0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00003000: 6478 203d 2069 6e64 7820 2b20 310a 2020  dx = indx + 1.  
+00003010: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00003020: 6d64 315b 696e 6478 5d20 3d20 300a 2020  md1[indx] = 0.  
+00003030: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00003040: 6576 2e77 7269 7465 2830 7830 312c 2073  ev.write(0x01, s
+00003050: 656c 662e 636d 6431 2920 2023 2053 4350  elf.cmd1)  # SCP
+00003060: 2043 6f6d 6d61 6e64 2075 7020 746f 2036   Command up to 6
+00003070: 3020 6368 6172 733b 0a20 2020 2020 2020  0 chars;.       
+00003080: 2020 2020 2073 203d 2073 656c 662e 6465       s = self.de
+00003090: 762e 7265 6164 2830 7838 312c 2036 3429  v.read(0x81, 64)
+000030a0: 0a20 2020 2020 2020 2020 2020 2069 203d  .            i =
+000030b0: 2031 0a20 2020 2020 2020 2020 2020 2052   1.            R
+000030c0: 6574 5374 7220 3d20 2222 0a20 2020 2020  etStr = "".     
+000030d0: 2020 2020 2020 2077 6869 6c65 2028 735b         while (s[
+000030e0: 695d 203e 2030 293a 0a20 2020 2020 2020  i] > 0):.       
+000030f0: 2020 2020 2020 2020 2052 6574 5374 7220           RetStr 
+00003100: 3d20 5265 7453 7472 202b 2063 6872 2873  = RetStr + chr(s
+00003110: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
+00003120: 2020 2020 2069 203d 2069 202b 2031 0a20       i = i + 1. 
+00003130: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00003140: 6e20 7374 7228 5265 7453 7472 290a 0a20  n str(RetStr).. 
+00003150: 2020 2063 6c61 7373 2041 5049 286f 626a     class API(obj
+00003160: 6563 7429 3a0a 0a20 2020 2020 2020 2064  ect):..        d
+00003170: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00003180: 2c20 636f 6d70 6f72 743d 2241 5554 4f22  , comport="AUTO"
+00003190: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+000031a0: 656c 662e 6261 7564 7261 7465 203d 2039  elf.baudrate = 9
+000031b0: 3630 300a 2020 2020 2020 2020 2020 2020  600.            
+000031c0: 6966 2063 6f6d 706f 7274 203d 3d20 2241  if comport == "A
+000031d0: 5554 4f22 3a0a 2020 2020 2020 2020 2020  UTO":.          
+000031e0: 2020 2020 2020 706f 7274 735f 6c69 7374        ports_list
+000031f0: 203d 2073 6572 6961 6c5f 706f 7274 7328   = serial_ports(
+00003200: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003210: 2020 666f 7220 706f 7274 2069 6e20 706f    for port in po
+00003220: 7274 735f 6c69 7374 3a0a 2020 2020 2020  rts_list:.      
+00003230: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003240: 6c66 2e63 6f6d 706f 7274 203d 2070 6f72  lf.comport = por
+00003250: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00003260: 2020 2020 2020 7365 6c66 2e73 203d 2073        self.s = s
+00003270: 6572 6961 6c2e 5365 7269 616c 2873 656c  erial.Serial(sel
+00003280: 662e 636f 6d70 6f72 742c 2073 656c 662e  f.comport, self.
+00003290: 6261 7564 7261 7465 2c20 7469 6d65 6f75  baudrate, timeou
+000032a0: 743d 302e 3529 0a20 2020 2020 2020 2020  t=0.5).         
+000032b0: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
+000032c0: 2831 290a 2020 2020 2020 2020 2020 2020  (1).            
+000032d0: 2020 2020 2020 2020 7365 6c66 2e73 2e66          self.s.f
+000032e0: 6c75 7368 496e 7075 7428 290a 2020 2020  lushInput().    
+000032f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003300: 7365 6c66 2e73 2e66 6c75 7368 4f75 7470  self.s.flushOutp
+00003310: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
+00003320: 2020 2020 2020 2020 2073 6c65 6570 2830           sleep(0
+00003330: 2e31 290a 2020 2020 2020 2020 2020 2020  .1).            
+00003340: 2020 2020 2020 2020 2320 5475 726e 2074          # Turn t
+00003350: 6865 2063 6f6e 736f 6c65 206f 6666 0a20  he console off. 
+00003360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003370: 2020 2073 656c 662e 732e 7772 6974 6528     self.s.write(
+00003380: 2243 4f4e 534f 4c45 2044 4953 4142 4c45  "CONSOLE DISABLE
+00003390: 5c72 5c6e 222e 656e 636f 6465 2829 290a  \r\n".encode()).
+000033a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033b0: 2020 2020 2320 466c 7573 6820 7468 6520      # Flush the 
+000033c0: 6275 6666 6572 730a 2020 2020 2020 2020  buffers.        
+000033d0: 2020 2020 2020 2020 2020 2020 736c 6565              slee
+000033e0: 7028 302e 3129 0a20 2020 2020 2020 2020  p(0.1).         
+000033f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003400: 732e 666c 7573 6828 290a 2020 2020 2020  s.flush().      
+00003410: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003420: 6c66 2e73 2e66 6c75 7368 496e 7075 7428  lf.s.flushInput(
+00003430: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003440: 2020 2020 2020 7365 6c66 2e73 2e66 6c75        self.s.flu
+00003450: 7368 4f75 7470 7574 2829 0a20 2020 2020  shOutput().     
+00003460: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00003470: 656c 662e 732e 7772 6974 6528 222a 4944  elf.s.write("*ID
+00003480: 4e3f 5c72 5c6e 222e 656e 636f 6465 2829  N?\r\n".encode()
+00003490: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000034a0: 2020 2020 2020 736c 6565 7028 302e 3129        sleep(0.1)
+000034b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000034c0: 2020 2020 2069 6620 7365 6c66 2e73 2e69       if self.s.i
+000034d0: 6e5f 7761 6974 696e 6720 3e20 313a 0a20  n_waiting > 1:. 
+000034e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034f0: 2020 2020 2020 2072 6573 7020 3d20 7365         resp = se
+00003500: 6c66 2e73 2e72 6561 646c 696e 6528 292e  lf.s.readline().
+00003510: 6465 636f 6465 2822 7574 662d 3822 290a  decode("utf-8").
+00003520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003530: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00003540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003550: 2020 7265 7370 203d 2027 270a 2020 2020    resp = ''.    
+00003560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003570: 7365 6c66 2e6d 6f64 656c 203d 2072 6573  self.model = res
+00003580: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
+00003590: 2020 2020 2020 6966 2028 2241 6572 6f66        if ("Aerof
+000035a0: 6c65 7822 2069 6e20 7265 7370 293a 0a20  lex" in resp):. 
 000035b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035c0: 7365 6c66 2e6d 6f64 656c 203d 2072 6573  self.model = res
-000035d0: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
-000035e0: 2020 2020 2020 6966 2028 2241 6572 6f66        if ("Aerof
-000035f0: 6c65 7822 2069 6e20 7265 7370 293a 0a20  lex" in resp):. 
-00003600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003610: 2020 2020 2020 2070 7269 6e74 2827 466f         print('Fo
-00003620: 756e 6420 2720 2b20 7265 7370 2e73 7472  und ' + resp.str
-00003630: 6970 2827 5c72 5c6e 2729 202b 2027 206f  ip('\r\n') + ' o
-00003640: 6e20 706f 7274 3a20 2720 2b20 706f 7274  n port: ' + port
-00003650: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00003660: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
-00003670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003680: 2020 2020 656c 6966 2027 3833 3131 2720      elif '8311' 
-00003690: 696e 2072 6573 7020 6f72 2027 3833 3331  in resp or '8331
-000036a0: 2720 696e 2072 6573 703a 0a20 2020 2020  ' in resp:.     
+000035c0: 2020 2020 2020 2070 7269 6e74 2827 466f         print('Fo
+000035d0: 756e 6420 2720 2b20 7265 7370 2e73 7472  und ' + resp.str
+000035e0: 6970 2827 5c72 5c6e 2729 202b 2027 206f  ip('\r\n') + ' o
+000035f0: 6e20 706f 7274 3a20 2720 2b20 706f 7274  n port: ' + port
+00003600: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003610: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+00003620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003630: 2020 2020 656c 6966 2027 3833 3131 2720      elif '8311' 
+00003640: 696e 2072 6573 7020 6f72 2027 3833 3331  in resp or '8331
+00003650: 2720 696e 2072 6573 703a 0a20 2020 2020  ' in resp:.     
+00003660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003670: 2020 2070 7269 6e74 2827 466f 756e 6420     print('Found 
+00003680: 2720 2b20 7265 7370 2e73 7472 6970 2827  ' + resp.strip('
+00003690: 5c72 5c6e 2729 202b 2027 206f 6e20 706f  \r\n') + ' on po
+000036a0: 7274 3a20 2720 2b20 706f 7274 290a 2020  rt: ' + port).  
 000036b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036c0: 2020 2070 7269 6e74 2827 466f 756e 6420     print('Found 
-000036d0: 2720 2b20 7265 7370 2e73 7472 6970 2827  ' + resp.strip('
-000036e0: 5c72 5c6e 2729 202b 2027 206f 6e20 706f  \r\n') + ' on po
-000036f0: 7274 3a20 2720 2b20 706f 7274 290a 2020  rt: ' + port).  
-00003700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003710: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00003720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003730: 7061 7373 0a20 2020 2020 2020 2020 2020  pass.           
-00003740: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00003750: 2020 2020 2020 2073 656c 662e 7320 3d20         self.s = 
-00003760: 7365 7269 616c 2e53 6572 6961 6c28 636f  serial.Serial(co
-00003770: 6d70 6f72 742c 2073 656c 662e 6261 7564  mport, self.baud
-00003780: 7261 7465 2c20 7469 6d65 6f75 743d 302e  rate, timeout=0.
-00003790: 3529 0a20 2020 2020 2020 2020 2020 2020  5).             
-000037a0: 2020 2073 6c65 6570 2831 290a 2020 2020     sleep(1).    
-000037b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000037c0: 2e73 2e77 7269 7465 2822 434f 4e53 4f4c  .s.write("CONSOL
-000037d0: 4520 4449 5341 424c 455c 725c 6e22 2e65  E DISABLE\r\n".e
-000037e0: 6e63 6f64 6528 2929 0a20 2020 2020 2020  ncode()).       
-000037f0: 2020 2020 2020 2020 2023 2046 6c75 7368           # Flush
-00003800: 2074 6865 2062 7566 6665 7273 0a20 2020   the buffers.   
-00003810: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00003820: 662e 732e 666c 7573 6828 290a 2020 2020  f.s.flush().    
-00003830: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003840: 2e73 2e66 6c75 7368 496e 7075 7428 290a  .s.flushInput().
-00003850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003860: 7365 6c66 2e73 2e66 6c75 7368 4f75 7470  self.s.flushOutp
-00003870: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
-00003880: 2020 2020 2073 656c 662e 5175 6572 7928       self.Query(
-00003890: 222a 4944 4e3f 5c72 5c6e 2229 0a20 2020  "*IDN?\r\n").   
-000038a0: 2020 2020 2020 2020 2020 2020 2072 6573               res
-000038b0: 7020 3d20 7365 6c66 2e51 7565 7279 2822  p = self.Query("
-000038c0: 2a49 444e 3f5c 725c 6e22 290a 2020 2020  *IDN?\r\n").    
-000038d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000038e0: 2e6d 6f64 656c 203d 2072 6573 700a 2020  .model = resp.  
-000038f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00003900: 2028 2241 6572 6f66 6c65 7822 2069 6e20   ("Aeroflex" in 
-00003910: 7265 7370 2920 6f72 2028 2234 3230 3522  resp) or ("4205"
-00003920: 2069 6e20 7265 7370 293a 0a20 2020 2020   in resp):.     
-00003930: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00003940: 7269 6e74 2827 466f 756e 6420 2720 2b20  rint('Found ' + 
-00003950: 7265 7370 2e73 7472 6970 2827 5c72 5c6e  resp.strip('\r\n
-00003960: 2729 202b 2027 206f 6e20 706f 7274 3a20  ') + ' on port: 
-00003970: 2720 2b20 636f 6d70 6f72 7429 0a20 2020  ' + comport).   
-00003980: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-00003990: 6620 2738 3331 3127 2069 6e20 7265 7370  f '8311' in resp
-000039a0: 206f 7220 2738 3333 3127 2069 6e20 7265   or '8331' in re
-000039b0: 7370 3a0a 2020 2020 2020 2020 2020 2020  sp:.            
-000039c0: 2020 2020 2020 2020 7072 696e 7428 2746          print('F
-000039d0: 6f75 6e64 2027 202b 2072 6573 702e 7374  ound ' + resp.st
-000039e0: 7269 7028 275c 725c 6e27 2920 2b20 2720  rip('\r\n') + ' 
-000039f0: 6f6e 2070 6f72 743a 2027 202b 2063 6f6d  on port: ' + com
-00003a00: 706f 7274 290a 2020 2020 2020 2020 2020  port).          
-00003a10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00003a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a30: 7365 6c66 2e63 6c6f 7365 5f70 6f72 7428  self.close_port(
-00003a40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00003a50: 2020 2020 2020 7072 696e 7428 2741 6572        print('Aer
-00003a60: 6f66 6c65 7820 4174 7465 6e75 6174 6f72  oflex Attenuator
-00003a70: 206e 6f74 2066 6f75 6e64 206f 6e20 7365   not found on se
-00003a80: 6c65 6374 6564 2070 6f72 742c 2063 6865  lected port, che
-00003a90: 636b 2063 6f6e 6e65 6374 696f 6e27 2c20  ck connection', 
-00003aa0: 6669 6c65 3d73 7973 2e73 7464 6572 7229  file=sys.stderr)
-00003ab0: 0a0a 2020 2020 2020 2020 6465 6620 5772  ..        def Wr
-00003ac0: 6974 6528 7365 6c66 2c20 636d 642c 2077  ite(self, cmd, w
-00003ad0: 6169 743d 4661 6c73 6529 3a0a 2020 2020  ait=False):.    
-00003ae0: 2020 2020 2020 2020 2222 2253 656e 6420          """Send 
-00003af0: 7468 6520 696e 7075 7420 636d 6420 7374  the input cmd st
-00003b00: 7269 6e67 2076 6961 2043 4f4d 2053 6f63  ring via COM Soc
-00003b10: 6b65 7422 2222 0a20 2020 2020 2020 2020  ket""".         
-00003b20: 2020 2069 6620 7365 6c66 2e73 2e69 734f     if self.s.isO
-00003b30: 7065 6e28 293a 0a20 2020 2020 2020 2020  pen():.         
-00003b40: 2020 2020 2020 2070 6173 730a 2020 2020         pass.    
-00003b50: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00003b60: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00003b70: 6c66 2e73 2e6f 7065 6e28 290a 2020 2020  lf.s.open().    
-00003b80: 2020 2020 2020 2020 7365 6c66 2e73 2e66          self.s.f
-00003b90: 6c75 7368 496e 7075 7428 290a 2020 2020  lushInput().    
-00003ba0: 2020 2020 2020 2020 736c 6565 7028 3129          sleep(1)
-00003bb0: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
-00003bc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003bd0: 2020 7365 6c66 2e73 2e77 7269 7465 2873    self.s.write(s
-00003be0: 7472 2e65 6e63 6f64 6528 636d 6429 290a  tr.encode(cmd)).
-00003bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c00: 736c 6565 7028 302e 3129 2020 2320 436f  sleep(0.1)  # Co
-00003c10: 6d6d 616e 6473 206d 6179 2062 6520 6c6f  mmands may be lo
-00003c20: 7374 2077 6865 6e20 7772 6974 696e 6720  st when writing 
-00003c30: 746f 6f20 6661 7374 0a0a 2020 2020 2020  too fast..      
-00003c40: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
-00003c50: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00003c60: 7373 0a20 2020 2020 2020 2020 2020 2023  ss.            #
-00003c70: 2073 656c 662e 732e 636c 6f73 6528 290a   self.s.close().
-00003c80: 0a20 2020 2020 2020 2064 6566 2051 7565  .        def Que
-00003c90: 7279 2873 656c 662c 2063 6d64 293a 0a20  ry(self, cmd):. 
-00003ca0: 2020 2020 2020 2020 2020 2022 2222 5365             """Se
-00003cb0: 6e64 2074 6865 2069 6e70 7574 2063 6d64  nd the input cmd
-00003cc0: 2073 7472 696e 6720 7669 6120 434f 4d20   string via COM 
-00003cd0: 536f 636b 6574 2061 6e64 2072 6574 7572  Socket and retur
-00003ce0: 6e20 7468 6520 7265 706c 7920 7374 7269  n the reply stri
-00003cf0: 6e67 2222 220a 2020 2020 2020 2020 2020  ng""".          
-00003d00: 2020 6966 2073 656c 662e 732e 6973 4f70    if self.s.isOp
-00003d10: 656e 2829 3a0a 2020 2020 2020 2020 2020  en():.          
-00003d20: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
-00003d30: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00003d40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00003d50: 662e 732e 6f70 656e 2829 0a20 2020 2020  f.s.open().     
-00003d60: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
-00003d70: 2830 2e31 290a 2020 2020 2020 2020 2020  (0.1).          
-00003d80: 2020 2320 7365 6c66 2e73 2e66 6c75 7368    # self.s.flush
-00003d90: 496e 7075 7428 290a 2020 2020 2020 2020  Input().        
-00003da0: 2020 2020 736c 6565 7028 3129 0a20 2020      sleep(1).   
-00003db0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-00003dc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00003dd0: 6c66 2e73 2e77 7269 7465 2863 6d64 2e65  lf.s.write(cmd.e
-00003de0: 6e63 6f64 6528 2929 0a20 2020 2020 2020  ncode()).       
-00003df0: 2020 2020 2020 2020 2073 6c65 6570 2830           sleep(0
-00003e00: 2e31 290a 2020 2020 2020 2020 2020 2020  .1).            
-00003e10: 2020 2020 6966 2073 656c 662e 732e 696e      if self.s.in
-00003e20: 5f77 6169 7469 6e67 203e 2030 3a0a 2020  _waiting > 0:.  
-00003e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e40: 2020 6461 7461 203d 2073 656c 662e 732e    data = self.s.
-00003e50: 7265 6164 6c69 6e65 2829 2e64 6563 6f64  readline().decod
-00003e60: 6528 2275 7466 2d38 2229 0a20 2020 2020  e("utf-8").     
-00003e70: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00003e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003e90: 2020 2020 2064 6174 6120 3d20 2727 0a20       data = ''. 
-00003ea0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00003eb0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-00003ec0: 2020 2064 6174 6120 3d20 2727 0a20 2020     data = ''.   
-00003ed0: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
-00003ee0: 732e 636c 6f73 6528 290a 2020 2020 2020  s.close().      
-00003ef0: 2020 2020 2020 7265 7475 726e 2064 6174        return dat
-00003f00: 610a 0a20 2020 2020 2020 2064 6566 2063  a..        def c
-00003f10: 6c6f 7365 5f70 6f72 7428 7365 6c66 293a  lose_port(self):
-00003f20: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00003f30: 7365 6c66 2e73 2069 7320 6e6f 7420 4e6f  self.s is not No
-00003f40: 6e65 2061 6e64 2073 656c 662e 732e 6973  ne and self.s.is
-00003f50: 4f70 656e 2829 3a0a 2020 2020 2020 2020  Open():.        
-00003f60: 2020 2020 2020 2020 7365 6c66 2e73 2e63          self.s.c
-00003f70: 6c6f 7365 2829 0a0a 2020 2020 2020 2020  lose()..        
-00003f80: 6465 6620 6973 5f6f 7065 6e28 7365 6c66  def is_open(self
-00003f90: 2c20 6368 6563 6b5f 706f 7274 3d46 616c  , check_port=Fal
-00003fa0: 7365 293a 0a20 2020 2020 2020 2020 2020  se):.           
-00003fb0: 2069 6620 7365 6c66 2e73 2069 7320 6e6f   if self.s is no
-00003fc0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00003fd0: 2020 2020 2020 2020 6966 2063 6865 636b          if check
-00003fe0: 5f70 6f72 743a 0a20 2020 2020 2020 2020  _port:.         
-00003ff0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-00004000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004010: 2020 2020 2020 2020 7365 6c66 2e51 7565          self.Que
-00004020: 7279 2822 2a49 444e 3f5c 725c 6e22 290a  ry("*IDN?\r\n").
-00004030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004040: 2020 2020 2020 2020 7265 7370 203d 2073          resp = s
-00004050: 656c 662e 5175 6572 7928 222a 4944 4e3f  elf.Query("*IDN?
-00004060: 5c72 5c6e 2229 0a20 2020 2020 2020 2020  \r\n").         
-00004070: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00004080: 656c 662e 6d6f 6465 6c20 3d20 7265 7370  elf.model = resp
-00004090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000040a0: 2020 2020 2020 2020 2069 6620 2822 4165           if ("Ae
-000040b0: 726f 666c 6578 2220 696e 2072 6573 7029  roflex" in resp)
-000040c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000040d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000040e0: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
-000040f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004100: 2020 656c 6966 2027 3833 3131 2720 696e    elif '8311' in
-00004110: 2072 6573 7020 6f72 2027 3833 3331 2720   resp or '8331' 
-00004120: 696e 2072 6573 703a 0a20 2020 2020 2020  in resp:.       
-00004130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004140: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00004150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004160: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
-00004170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004180: 2020 2020 2073 656c 662e 636c 6f73 655f       self.close_
-00004190: 706f 7274 2829 0a20 2020 2020 2020 2020  port().         
-000041a0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000041b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041c0: 2072 6574 7572 6e20 7365 6c66 2e73 2e69   return self.s.i
-000041d0: 734f 7065 6e28 290a 2020 2020 2020 2020  sOpen().        
-000041e0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-000041f0: 0a0a 2020 2020 2020 2020 6465 6620 5365  ..        def Se
-00004200: 7461 7474 6e28 7365 6c66 2c20 6174 746e  tattn(self, attn
-00004210: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
-00004220: 6d64 203d 2022 4154 544e 207b 3a2e 3266  md = "ATTN {:.2f
-00004230: 7d5c 725c 6e22 2e66 6f72 6d61 7428 6174  }\r\n".format(at
-00004240: 746e 290a 2020 2020 2020 2020 2020 2020  tn).            
-00004250: 7365 6c66 2e57 7269 7465 2863 6d64 290a  self.Write(cmd).
-00004260: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-00004270: 6520 3d20 7365 6c66 2e47 6574 6174 746e  e = self.Getattn
-00004280: 2829 0a20 2020 2020 2020 2020 2020 2076  ().            v
-00004290: 616c 7565 203d 2066 6c6f 6174 2876 616c  alue = float(val
-000042a0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
-000042b0: 6966 2076 616c 7565 2021 3d20 6174 746e  if value != attn
-000042c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000042d0: 2020 7072 696e 7428 6627 4572 726f 7220    print(f'Error 
-000042e0: 7365 7474 696e 6720 6174 7465 6e75 6174  setting attenuat
-000042f0: 696f 6e3a 206e 6577 203a 207b 6174 746e  ion: new : {attn
-00004300: 7d20 6375 7272 656e 743a 207b 7661 6c75  } current: {valu
-00004310: 657d 2729 0a20 2020 2020 2020 2020 2020  e}').           
-00004320: 2072 6574 7572 6e20 7661 6c75 650a 0a20   return value.. 
-00004330: 2020 2020 2020 2064 6566 2047 6574 6174         def Getat
-00004340: 746e 2873 656c 6629 3a0a 2020 2020 2020  tn(self):.      
-00004350: 2020 2020 2020 636d 6420 3d20 2241 5454        cmd = "ATT
-00004360: 4e3f 5c72 5c6e 220a 2020 2020 2020 2020  N?\r\n".        
-00004370: 2020 2020 7661 6c75 6520 3d20 7365 6c66      value = self
-00004380: 2e51 7565 7279 2863 6d64 290a 2020 2020  .Query(cmd).    
-00004390: 2020 2020 2020 2020 7265 7475 726e 2076          return v
-000043a0: 616c 7565 0a0a 0a63 6c61 7373 2054 6573  alue...class Tes
-000043b0: 636f 6d3a 0a20 2020 2022 2222 0a20 2020  com:.    """.   
-000043c0: 2043 6f6e 7472 6f6c 2054 4553 434f 4d20   Control TESCOM 
-000043d0: 7465 7374 696e 6720 6368 616d 6265 7273  testing chambers
-000043e0: 0a20 2020 2022 2222 0a20 2020 206f 7065  .    """.    ope
-000043f0: 6e5f 636d 6420 3d20 6227 4f50 454e 5c72  n_cmd = b'OPEN\r
-00004400: 270a 2020 2020 636c 6f73 655f 636d 6420  '.    close_cmd 
-00004410: 3d20 6227 434c 4f53 455c 7227 0a20 2020  = b'CLOSE\r'.   
-00004420: 2063 6f6d 5f70 6f72 745f 6f62 6a20 3d20   com_port_obj = 
-00004430: 4e6f 6e65 0a20 2020 206d 6f64 656c 735f  None.    models_
-00004440: 6c69 7374 203d 205b 2754 432d 3530 3634  list = ['TC-5064
-00004450: 4327 2c20 2754 412d 3730 3131 4150 272c  C', 'TA-7011AP',
-00004460: 2027 5443 2d35 3036 3341 272c 2027 5443   'TC-5063A', 'TC
-00004470: 2d35 3937 3043 5027 5d0a 0a20 2020 2064  -5970CP']..    d
-00004480: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00004490: 2c20 706f 7274 3d4e 6f6e 6529 3a0a 2020  , port=None):.  
-000044a0: 2020 2020 2020 7365 6c66 2e70 6f72 7420        self.port 
-000044b0: 3d20 706f 7274 0a20 2020 2020 2020 2074  = port.        t
-000044c0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-000044d0: 6966 2070 6f72 7420 6973 206e 6f74 204e  if port is not N
-000044e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000044f0: 2020 2020 2073 656c 662e 636f 6e6e 6563       self.connec
-00004500: 7428 706f 7274 290a 0a20 2020 2020 2020  t(port)..       
-00004510: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-00004520: 6e20 6173 2065 3a0a 2020 2020 2020 2020  n as e:.        
-00004530: 2020 2020 7072 696e 7428 6529 0a20 2020      print(e).   
-00004540: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-00004550: 5465 7363 6f6d 202d 2043 6f6e 6e65 6374  Tescom - Connect
-00004560: 696f 6e20 6661 696c 6564 2229 0a0a 2020  ion failed")..  
-00004570: 2020 6465 6620 636f 6e6e 6563 7428 7365    def connect(se
-00004580: 6c66 2c20 706f 7274 293a 0a20 2020 2020  lf, port):.     
-00004590: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-000045a0: 7061 7261 6d20 706f 7274 3a20 636f 6d20  param port: com 
-000045b0: 706f 7274 2074 6f20 636f 6e6e 6563 740a  port to connect.
-000045c0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-000045d0: 2063 6f6d 2070 6f72 7420 6f62 6a0a 2020   com port obj.  
-000045e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000045f0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00004600: 2020 2063 6f6d 5f70 6f72 745f 6f62 6a20     com_port_obj 
-00004610: 3d20 7365 6c66 2e63 6f6d 5f70 6f72 745f  = self.com_port_
-00004620: 6f62 6a20 3d20 7365 7269 616c 2e53 6572  obj = serial.Ser
-00004630: 6961 6c28 706f 7274 3d70 6f72 742c 2062  ial(port=port, b
-00004640: 6175 6472 6174 653d 3936 3030 2c20 7469  audrate=9600, ti
-00004650: 6d65 6f75 743d 3129 0a20 2020 2020 2020  meout=1).       
-00004660: 2020 2020 2069 6620 636f 6d5f 706f 7274       if com_port
-00004670: 5f6f 626a 2069 7320 6e6f 7420 4e6f 6e65  _obj is not None
-00004680: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004690: 2020 7365 6c66 2e64 6f6f 725f 636d 6420    self.door_cmd 
-000046a0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-000046b0: 2020 2020 2020 2073 656c 662e 636f 6d5f         self.com_
-000046c0: 706f 7274 5f6f 626a 2e77 7269 7465 2862  port_obj.write(b
-000046d0: 274d 4f44 454c 3f5c 7227 290a 2020 2020  'MODEL?\r').    
-000046e0: 2020 2020 2020 2020 2020 2020 736c 6565              slee
-000046f0: 7028 302e 3129 0a20 2020 2020 2020 2020  p(0.1).         
-00004700: 2020 2020 2020 206d 6f64 656c 203d 2073         model = s
-00004710: 7472 2873 656c 662e 636f 6d5f 706f 7274  tr(self.com_port
-00004720: 5f6f 626a 2e72 6561 6428 3134 2929 0a20  _obj.read(14)). 
-00004730: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00004740: 6172 7473 203d 205b 7020 666f 7220 7020  arts = [p for p 
-00004750: 696e 206d 6f64 656c 2e73 706c 6974 2822  in model.split("
-00004760: 2722 295d 0a20 2020 2020 2020 2020 2020  '")].           
-00004770: 2020 2020 2070 6172 7473 203d 205b 7020       parts = [p 
-00004780: 666f 7220 7020 696e 2070 6172 7473 5b31  for p in parts[1
-00004790: 5d2e 7370 6c69 7428 2220 2229 5d0a 2020  ].split(" ")].  
-000047a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000047b0: 6c66 2e6d 6f64 656c 203d 2070 6172 7473  lf.model = parts
-000047c0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-000047d0: 2020 2020 6966 206c 656e 2873 656c 662e      if len(self.
-000047e0: 6d6f 6465 6c29 203e 2030 3a0a 2020 2020  model) > 0:.    
-000047f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004800: 7072 696e 7428 2252 4620 6368 616d 6265  print("RF chambe
-00004810: 7220 636f 6e6e 6563 7465 6420 746f 2070  r connected to p
-00004820: 6f72 7420 2220 2b20 7374 7228 706f 7274  ort " + str(port
-00004830: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00004840: 2020 2020 2020 2070 7269 6e74 2822 5465         print("Te
-00004850: 7363 6f6d 202d 2043 6861 6d62 6572 206d  scom - Chamber m
-00004860: 6f64 656c 3a22 2c20 7365 6c66 2e6d 6f64  odel:", self.mod
-00004870: 656c 290a 2020 2020 2020 2020 2020 2020  el).            
-00004880: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00004890: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000048a0: 696e 7428 2254 6573 636f 6d20 2d20 4572  int("Tescom - Er
-000048b0: 726f 7221 204e 6f20 6368 616d 6265 7220  ror! No chamber 
-000048c0: 666f 756e 6422 290a 2020 2020 2020 2020  found").        
-000048d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000048e0: 726e 0a20 2020 2020 2020 2020 2020 2020  rn.             
-000048f0: 2020 2069 6620 7365 6c66 2e6d 6f64 656c     if self.model
-00004900: 2069 6e20 7365 6c66 2e6d 6f64 656c 735f   in self.models_
-00004910: 6c69 7374 3a0a 2020 2020 2020 2020 2020  list:.          
-00004920: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00004930: 6f6f 725f 636d 6420 3d20 6227 444f 4f52  oor_cmd = b'DOOR
-00004940: 3f5c 7227 0a20 2020 2020 2020 2020 2020  ?\r'.           
-00004950: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00004960: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00004970: 656c 662e 646f 6f72 5f63 6d64 203d 2062  elf.door_cmd = b
-00004980: 274c 4944 3f5c 7227 0a20 2020 2020 2020  'LID?\r'.       
-00004990: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000049a0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000049b0: 2045 7863 6570 7469 6f6e 0a20 2020 2020   Exception.     
-000049c0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-000049d0: 696f 6e20 6173 2065 3a0a 2020 2020 2020  ion as e:.      
-000049e0: 2020 2020 2020 2320 7072 696e 7428 6529        # print(e)
-000049f0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00004a00: 6e74 2828 2254 6573 636f 6d20 2d20 436f  nt(("Tescom - Co
-00004a10: 756c 6420 6e6f 7420 636f 6e6e 6563 7420  uld not connect 
-00004a20: 746f 2070 6f72 7420 2220 2b20 706f 7274  to port " + port
-00004a30: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
-00004a40: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
-00004a50: 6465 6620 636c 6f73 655f 706f 7274 2873  def close_port(s
-00004a60: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00004a70: 220a 2020 2020 2020 2020 636c 6f73 6573  ".        closes
-00004a80: 2063 6f6d 2070 6f72 740a 2020 2020 2020   com port.      
-00004a90: 2020 2222 220a 2020 2020 2020 2020 7472    """.        tr
-00004aa0: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-00004ab0: 656c 662e 636f 6d5f 706f 7274 5f6f 626a  elf.com_port_obj
-00004ac0: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
-00004ad0: 2020 2020 2070 7269 6e74 2822 5246 2063       print("RF c
-00004ae0: 6861 6d62 6572 2064 6973 636f 6e6e 6563  hamber disconnec
-00004af0: 7465 6420 6672 6f6d 2070 6f72 743a 2022  ted from port: "
-00004b00: 202b 2073 7472 2873 656c 662e 706f 7274   + str(self.port
-00004b10: 2929 0a20 2020 2020 2020 2065 7863 6570  )).        excep
-00004b20: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00004b30: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00004b40: 696e 7428 2243 6f75 6c64 206e 6f74 2064  int("Could not d
-00004b50: 6973 636f 6e6e 6563 7422 290a 0a20 2020  isconnect")..   
-00004b60: 2064 6566 206f 7065 6e5f 6368 616d 6265   def open_chambe
-00004b70: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
-00004b80: 2022 2222 0a20 2020 2020 2020 206f 7065   """.        ope
-00004b90: 6e73 2063 6861 6d62 6572 0a20 2020 2020  ns chamber.     
-00004ba0: 2020 203a 7265 7475 726e 3a20 224f 4b22     :return: "OK"
-00004bb0: 2069 6620 636f 6d6d 616e 6420 7761 7320   if command was 
-00004bc0: 7375 6363 6573 7366 756c 0a20 2020 2020  successful.     
-00004bd0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00004be0: 6620 7365 6c66 2e69 735f 646f 6f72 5f6f  f self.is_door_o
-00004bf0: 7065 6e28 293a 0a20 2020 2020 2020 2020  pen():.         
-00004c00: 2020 2070 7269 6e74 2822 4368 616d 6265     print("Chambe
-00004c10: 7220 6973 206f 7065 6e22 290a 2020 2020  r is open").    
-00004c20: 2020 2020 2020 2020 7265 7475 726e 2027          return '
-00004c30: 4f4b 270a 2020 2020 2020 2020 7472 793a  OK'.        try:
-00004c40: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00004c50: 6e74 2866 2243 6861 6d62 6572 207b 7365  nt(f"Chamber {se
-00004c60: 6c66 2e70 6f72 747d 2069 7320 6f70 656e  lf.port} is open
-00004c70: 696e 6722 290a 2020 2020 2020 2020 2020  ing").          
-00004c80: 2020 7365 6c66 2e63 6f6d 5f70 6f72 745f    self.com_port_
-00004c90: 6f62 6a2e 7265 7365 745f 696e 7075 745f  obj.reset_input_
-00004ca0: 6275 6666 6572 2829 0a20 2020 2020 2020  buffer().       
-00004cb0: 2020 2020 2073 656c 662e 636f 6d5f 706f       self.com_po
-00004cc0: 7274 5f6f 626a 2e72 6573 6574 5f6f 7574  rt_obj.reset_out
-00004cd0: 7075 745f 6275 6666 6572 2829 0a20 2020  put_buffer().   
-00004ce0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00004cf0: 6d5f 706f 7274 5f6f 626a 2e77 7269 7465  m_port_obj.write
-00004d00: 2873 656c 662e 6f70 656e 5f63 6d64 290a  (self.open_cmd).
-00004d10: 2020 2020 2020 2020 2020 2020 7265 7320              res 
-00004d20: 3d20 2727 0a20 2020 2020 2020 2020 2020  = ''.           
-00004d30: 2077 6169 745f 636f 756e 7465 7220 3d20   wait_counter = 
-00004d40: 300a 2020 2020 2020 2020 2020 2020 7768  0.            wh
-00004d50: 696c 6520 274f 4b27 206e 6f74 2069 6e20  ile 'OK' not in 
-00004d60: 7265 733a 0a20 2020 2020 2020 2020 2020  res:.           
-00004d70: 2020 2020 2069 6620 7761 6974 5f63 6f75       if wait_cou
-00004d80: 6e74 6572 203e 3d20 3135 3a0a 2020 2020  nter >= 15:.    
-00004d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004da0: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
-00004db0: 6622 4572 726f 7220 696e 206f 7065 6e69  f"Error in openi
-00004dc0: 6e67 2063 6861 6d62 6572 207b 7365 6c66  ng chamber {self
-00004dd0: 2e70 6f72 747d 2229 0a20 2020 2020 2020  .port}").       
-00004de0: 2020 2020 2020 2020 2072 6573 203d 2073           res = s
-00004df0: 656c 662e 636f 6d5f 706f 7274 5f6f 626a  elf.com_port_obj
-00004e00: 2e72 6561 6428 3134 292e 6465 636f 6465  .read(14).decode
-00004e10: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00004e20: 2020 2020 2020 2775 7466 2d38 2729 2e75        'utf-8').u
-00004e30: 7070 6572 2829 2e72 7374 7269 7028 275c  pper().rstrip('\
-00004e40: 7227 290a 2020 2020 2020 2020 2020 2020  r').            
-00004e50: 2020 2020 6966 206c 656e 2873 7472 2872      if len(str(r
-00004e60: 6573 2929 203e 2030 3a0a 2020 2020 2020  es)) > 0:.      
-00004e70: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00004e80: 696e 7428 6627 4368 616d 6265 7220 7b73  int(f'Chamber {s
-00004e90: 656c 662e 706f 7274 7d20 7374 6174 7573  elf.port} status
-00004ea0: 3a20 2720 2b20 7374 7228 7265 7329 290a  : ' + str(res)).
-00004eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ec0: 7761 6974 5f63 6f75 6e74 6572 202b 3d20  wait_counter += 
-00004ed0: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
-00004ee0: 2020 736c 6565 7028 302e 3129 0a20 2020    sleep(0.1).   
-00004ef0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00004f00: 7365 6c66 2e69 735f 646f 6f72 5f6f 7065  self.is_door_ope
-00004f10: 6e28 293a 0a20 2020 2020 2020 2020 2020  n():.           
-00004f20: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
-00004f30: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
-00004f40: 2020 2020 2020 2020 2020 6622 7b73 656c            f"{sel
-00004f50: 662e 706f 7274 7d20 446f 6f72 2073 7461  f.port} Door sta
-00004f60: 7475 7320 646f 6573 6e27 7420 6d61 7463  tus doesn't matc
-00004f70: 6820 636f 6d6d 616e 6420 7365 6e74 2122  h command sent!"
-00004f80: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-00004f90: 696e 7428 6622 4368 616d 6265 7220 7b73  int(f"Chamber {s
-00004fa0: 656c 662e 706f 7274 7d20 6973 206f 7065  elf.port} is ope
-00004fb0: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
-00004fc0: 7265 7475 726e 2027 4f4b 270a 2020 2020  return 'OK'.    
-00004fd0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-00004fe0: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
-00004ff0: 2020 2020 2020 2070 7269 6e74 2865 290a         print(e).
-00005000: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00005010: 726e 2022 4641 494c 220a 0a20 2020 2064  rn "FAIL"..    d
-00005020: 6566 2063 6c6f 7365 5f63 6861 6d62 6572  ef close_chamber
-00005030: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00005040: 2222 220a 2020 2020 2020 2020 636c 6f73  """.        clos
-00005050: 6573 2063 6861 6d62 6572 0a20 2020 2020  es chamber.     
-00005060: 2020 203a 7265 7475 726e 3a20 224f 4b22     :return: "OK"
-00005070: 2069 6620 636f 6d6d 616e 6420 7761 7320   if command was 
-00005080: 7375 6363 6573 7366 756c 0a20 2020 2020  successful.     
-00005090: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-000050a0: 6620 7365 6c66 2e69 735f 646f 6f72 5f63  f self.is_door_c
-000050b0: 6c6f 7365 6428 293a 0a20 2020 2020 2020  losed():.       
-000050c0: 2020 2020 2070 7269 6e74 2822 4368 616d       print("Cham
-000050d0: 6265 7220 636c 6f73 6564 2229 0a20 2020  ber closed").   
-000050e0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000050f0: 274f 4b27 0a20 2020 2020 2020 2074 7279  'OK'.        try
-00005100: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00005110: 696e 7428 6622 4348 414d 4245 5220 7b73  int(f"CHAMBER {s
-00005120: 656c 662e 706f 7274 7d20 4953 2043 4c4f  elf.port} IS CLO
-00005130: 5349 4e47 2c20 434c 4541 5220 4841 4e44  SING, CLEAR HAND
-00005140: 5321 2121 2229 0a20 2020 2020 2020 2020  S!!!").         
-00005150: 2020 2073 6c65 6570 2832 290a 2020 2020     sleep(2).    
-00005160: 2020 2020 2020 2020 7365 6c66 2e63 6f6d          self.com
-00005170: 5f70 6f72 745f 6f62 6a2e 7772 6974 6528  _port_obj.write(
-00005180: 7365 6c66 2e63 6c6f 7365 5f63 6d64 290a  self.close_cmd).
-00005190: 2020 2020 2020 2020 2020 2020 7265 7320              res 
-000051a0: 3d20 2727 0a20 2020 2020 2020 2020 2020  = ''.           
-000051b0: 2077 6169 745f 636f 756e 7465 7220 3d20   wait_counter = 
-000051c0: 300a 2020 2020 2020 2020 2020 2020 7768  0.            wh
-000051d0: 696c 6520 2752 4541 4459 2720 6e6f 7420  ile 'READY' not 
-000051e0: 696e 2072 6573 3a0a 2020 2020 2020 2020  in res:.        
-000051f0: 2020 2020 2020 2020 6966 2077 6169 745f          if wait_
-00005200: 636f 756e 7465 7220 3e3d 2032 303a 0a20  counter >= 20:. 
-00005210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005220: 2020 2072 6169 7365 2045 7863 6570 7469     raise Excepti
-00005230: 6f6e 2866 2245 7272 6f72 2069 6e20 636c  on(f"Error in cl
-00005240: 6f73 696e 6720 6368 616d 6265 7220 7b73  osing chamber {s
-00005250: 656c 662e 706f 7274 7d22 290a 2020 2020  elf.port}").    
-00005260: 2020 2020 2020 2020 2020 2020 7265 7320              res 
-00005270: 3d20 7365 6c66 2e63 6f6d 5f70 6f72 745f  = self.com_port_
-00005280: 6f62 6a2e 7265 6164 2831 3429 2e64 6563  obj.read(14).dec
-00005290: 6f64 6528 0a20 2020 2020 2020 2020 2020  ode(.           
-000052a0: 2020 2020 2020 2020 2027 7574 662d 3827           'utf-8'
-000052b0: 292e 7570 7065 7228 292e 7273 7472 6970  ).upper().rstrip
-000052c0: 2827 5c72 2729 0a20 2020 2020 2020 2020  ('\r').         
-000052d0: 2020 2020 2020 2069 6620 2745 5252 2720         if 'ERR' 
-000052e0: 696e 2072 6573 206f 7220 2752 4541 4459  in res or 'READY
-000052f0: 2720 696e 2072 6573 206f 7220 274f 4b27  ' in res or 'OK'
-00005300: 2069 6e20 7265 733a 0a20 2020 2020 2020   in res:.       
-00005310: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00005320: 6e74 2866 2743 6861 6d62 6572 207b 7365  nt(f'Chamber {se
-00005330: 6c66 2e70 6f72 747d 2073 7461 7475 733a  lf.port} status:
-00005340: 2027 202b 2073 7472 2872 6573 2929 0a20   ' + str(res)). 
-00005350: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00005360: 6620 2745 5252 2720 696e 2072 6573 3a0a  f 'ERR' in res:.
-00005370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005380: 2020 2020 7265 7475 726e 2022 4641 494c      return "FAIL
-00005390: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000053a0: 2020 7761 6974 5f63 6f75 6e74 6572 202b    wait_counter +
-000053b0: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-000053c0: 2020 2020 736c 6565 7028 302e 3129 0a20      sleep(0.1). 
-000053d0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-000053e0: 7420 7365 6c66 2e69 735f 646f 6f72 5f63  t self.is_door_c
-000053f0: 6c6f 7365 6428 293a 0a20 2020 2020 2020  losed():.       
-00005400: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
-00005410: 7863 6570 7469 6f6e 280a 2020 2020 2020  xception(.      
-00005420: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-00005430: 7b73 656c 662e 706f 7274 7d20 446f 6f72  {self.port} Door
-00005440: 2073 7461 7475 7320 646f 6573 6e27 7420   status doesn't 
-00005450: 6d61 7463 6820 636f 6d6d 616e 6420 7365  match command se
-00005460: 6e74 2122 290a 2020 2020 2020 2020 2020  nt!").          
-00005470: 2020 7072 696e 7428 6622 4368 616d 6265    print(f"Chambe
-00005480: 7220 7b73 656c 662e 706f 7274 7d20 636c  r {self.port} cl
-00005490: 6f73 6564 2229 0a20 2020 2020 2020 2020  osed").         
-000054a0: 2020 2072 6574 7572 6e20 274f 4b27 0a20     return 'OK'. 
-000054b0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-000054c0: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
-000054d0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-000054e0: 6622 4572 726f 7220 696e 2063 6c6f 7369  f"Error in closi
-000054f0: 6e67 2063 6861 6d62 6572 207b 7365 6c66  ng chamber {self
-00005500: 2e70 6f72 747d 2229 0a20 2020 2020 2020  .port}").       
-00005510: 2020 2020 2070 7269 6e74 2865 290a 2020       print(e).  
-00005520: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00005530: 2022 4641 494c 220a 0a20 2020 2064 6566   "FAIL"..    def
-00005540: 2069 735f 636f 6e6e 6563 7465 6428 7365   is_connected(se
-00005550: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-00005560: 7365 6c66 2e63 6f6d 5f70 6f72 745f 6f62  self.com_port_ob
-00005570: 6a20 6973 204e 6f6e 653a 0a20 2020 2020  j is None:.     
-00005580: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00005590: 6c73 650a 2020 2020 2020 2020 7265 7475  lse.        retu
-000055a0: 726e 2073 656c 662e 636f 6d5f 706f 7274  rn self.com_port
-000055b0: 5f6f 626a 2e69 734f 7065 6e28 290a 0a20  _obj.isOpen().. 
-000055c0: 2020 2064 6566 2067 6574 5f73 7461 7465     def get_state
-000055d0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000055e0: 7365 6c66 2e63 6f6d 5f70 6f72 745f 6f62  self.com_port_ob
-000055f0: 6a2e 7265 7365 745f 696e 7075 745f 6275  j.reset_input_bu
-00005600: 6666 6572 2829 0a20 2020 2020 2020 2073  ffer().        s
-00005610: 6c65 6570 2830 2e31 290a 2020 2020 2020  leep(0.1).      
-00005620: 2020 7365 6c66 2e63 6f6d 5f70 6f72 745f    self.com_port_
-00005630: 6f62 6a2e 7772 6974 6528 7365 6c66 2e64  obj.write(self.d
-00005640: 6f6f 725f 636d 6429 0a20 2020 2020 2020  oor_cmd).       
-00005650: 2073 6c65 6570 2830 2e31 290a 2020 2020   sleep(0.1).    
-00005660: 2020 2020 7374 6174 6520 3d20 7365 6c66      state = self
-00005670: 2e63 6f6d 5f70 6f72 745f 6f62 6a2e 7265  .com_port_obj.re
-00005680: 6164 2831 3429 2e64 6563 6f64 6528 2775  ad(14).decode('u
-00005690: 7466 2d38 2729 2e75 7070 6572 2829 2e72  tf-8').upper().r
-000056a0: 7374 7269 7028 275c 7227 290a 2020 2020  strip('\r').    
-000056b0: 2020 2020 7265 7475 726e 2073 7461 7465      return state
-000056c0: 0a0a 2020 2020 6465 6620 6973 5f64 6f6f  ..    def is_doo
-000056d0: 725f 6f70 656e 2873 656c 6629 3a0a 2020  r_open(self):.  
-000056e0: 2020 2020 2020 7374 6174 6520 3d20 7365        state = se
-000056f0: 6c66 2e67 6574 5f73 7461 7465 2829 0a20  lf.get_state(). 
-00005700: 2020 2020 2020 2069 6620 274f 5045 4e27         if 'OPEN'
-00005710: 2069 6e20 7374 6174 653a 0a20 2020 2020   in state:.     
-00005720: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00005730: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
-00005740: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
-00005750: 2069 735f 646f 6f72 5f63 6c6f 7365 6428   is_door_closed(
-00005760: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-00005770: 7461 7465 203d 2073 656c 662e 6765 745f  tate = self.get_
-00005780: 7374 6174 6528 290a 2020 2020 2020 2020  state().        
-00005790: 6966 2027 434c 4f53 4527 2069 6e20 7374  if 'CLOSE' in st
-000057a0: 6174 653a 0a20 2020 2020 2020 2020 2020  ate:.           
-000057b0: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
-000057c0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-000057d0: 650a 0a0a 636c 6173 7320 4261 7263 6f64  e...class Barcod
-000057e0: 6553 6361 6e6e 6572 286f 626a 6563 7429  eScanner(object)
-000057f0: 3a0a 2020 2020 7072 6566 6978 203d 2027  :.    prefix = '
-00005800: 7e01 3030 3030 4027 0a20 2020 2073 7566  ~.0000@'.    suf
-00005810: 6669 7820 3d20 273b 0327 0a20 2020 2063  fix = ';.'.    c
-00005820: 6f6d 203d 2027 270a 2020 2020 7365 7269  om = ''.    seri
-00005830: 616c 203d 204e 6f6e 650a 2020 2020 6465  al = None.    de
-00005840: 7669 6365 5f73 6967 6e61 7475 7265 203d  vice_signature =
-00005850: 2022 4e4c 532d 4e31 220a 0a0a 2020 2020   "NLS-N1"...    
-00005860: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00005870: 662c 2063 6f6d 3d4e 6f6e 652c 2062 6175  f, com=None, bau
-00005880: 643d 3131 3532 3030 2c20 636f 6e66 6967  d=115200, config
-00005890: 3d54 7275 652c 206c 6f67 5f74 7970 653d  =True, log_type=
-000058a0: 274e 4f5f 4c4f 4727 2c20 7772 6974 655f  'NO_LOG', write_
-000058b0: 746f 5f6c 6f67 203d 2046 616c 7365 2c20  to_log = False, 
-000058c0: 7469 6d65 6f75 743d 2731 3030 3027 293a  timeout='1000'):
-000058d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000058e0: 2020 2020 2044 6174 6173 6865 6574 3a0a       Datasheet:.
-000058f0: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
-00005900: 6364 6e2e 7274 7363 616e 2e6e 6574 2f77  cdn.rtscan.net/w
-00005910: 702d 636f 6e74 656e 742f 7570 6c6f 6164  p-content/upload
-00005920: 732f 3230 3232 2f30 362f 5573 6572 5f4d  s/2022/06/User_M
-00005930: 616e 7561 6c5f 5254 3231 345f 5254 3231  anual_RT214_RT21
-00005940: 375f 5254 3233 355f 5254 3234 305f 3230  7_RT235_RT240_20
-00005950: 3232 2e30 355f 312e 302e 362e 7064 660a  22.05_1.0.6.pdf.
-00005960: 2020 2020 2020 2020 466f 7220 7468 6520          For the 
-00005970: 6669 7273 7420 7573 652c 2079 6f75 2077  first use, you w
-00005980: 696c 6c20 6e65 6564 2074 6f20 7363 616e  ill need to scan
-00005990: 2033 2062 6172 636f 6465 2074 6f20 696e   3 barcode to in
-000059a0: 6974 6961 6c20 636f 6d70 6f72 7420 636f  itial comport co
-000059b0: 6e6e 6563 7469 6f6e 3a0a 2020 2020 2020  nnection:.      
-000059c0: 2020 6874 7470 733a 2f2f 7769 6c69 6f74    https://wiliot
-000059d0: 2e61 746c 6173 7369 616e 2e6e 6574 2f77  .atlassian.net/w
-000059e0: 696b 692f 7370 6163 6573 2f46 572f 7061  iki/spaces/FW/pa
-000059f0: 6765 732f 3235 3636 3032 3934 3037 2f52  ges/2566029407/R
-00005a00: 5473 6361 6e2b 4261 7263 6f64 652b 5363  Tscan+Barcode+Sc
-00005a10: 616e 6e65 720a 2020 2020 2020 2020 4070  anner.        @p
-00005a20: 6172 616d 2063 6f6d 3a0a 2020 2020 2020  aram com:.      
-00005a30: 2020 4074 7970 6520 636f 6d3a 0a20 2020    @type com:.   
-00005a40: 2020 2020 2040 7061 7261 6d20 6261 7564       @param baud
-00005a50: 3a0a 2020 2020 2020 2020 4074 7970 6520  :.        @type 
-00005a60: 6261 7564 3a0a 2020 2020 2020 2020 4070  baud:.        @p
-00005a70: 6172 616d 2063 6f6e 6669 673a 0a20 2020  aram config:.   
-00005a80: 2020 2020 2040 7479 7065 2063 6f6e 6669       @type confi
-00005a90: 673a 0a20 2020 2020 2020 2040 7061 7261  g:.        @para
-00005aa0: 6d20 6c6f 675f 7479 7065 3a0a 2020 2020  m log_type:.    
-00005ab0: 2020 2020 4074 7970 6520 6c6f 675f 7479      @type log_ty
-00005ac0: 7065 3a0a 2020 2020 2020 2020 4070 6172  pe:.        @par
-00005ad0: 616d 2077 7269 7465 5f74 6f5f 6c6f 673a  am write_to_log:
-00005ae0: 0a20 2020 2020 2020 2040 7479 7065 2077  .        @type w
-00005af0: 7269 7465 5f74 6f5f 6c6f 673a 0a20 2020  rite_to_log:.   
-00005b00: 2020 2020 2040 7061 7261 6d20 7469 6d65       @param time
-00005b10: 6f75 743a 0a20 2020 2020 2020 2040 7479  out:.        @ty
-00005b20: 7065 2074 696d 656f 7574 3a0a 2020 2020  pe timeout:.    
-00005b30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00005b40: 7365 6c66 2e6c 6f67 5f74 7970 6520 3d20  self.log_type = 
-00005b50: 6c6f 675f 7479 7065 0a20 2020 2020 2020  log_type.       
-00005b60: 2073 656c 662e 7772 6974 655f 746f 5f6c   self.write_to_l
-00005b70: 6f67 203d 2077 7269 7465 5f74 6f5f 6c6f  og = write_to_lo
-00005b80: 670a 2020 2020 2020 2020 6966 2063 6f6d  g.        if com
-00005b90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00005ba0: 2020 2020 2020 2020 2020 7365 6c66 2e6f            self.o
-00005bb0: 7065 6e5f 706f 7274 2863 6f6d 2c20 6261  pen_port(com, ba
-00005bc0: 7564 3d62 6175 642c 2063 6f6e 6669 673d  ud=baud, config=
-00005bd0: 636f 6e66 6967 2c20 7469 6d65 6f75 743d  config, timeout=
-00005be0: 7469 6d65 6f75 7429 0a20 2020 2020 2020  timeout).       
-00005bf0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00005c00: 2020 2073 656c 662e 6175 746f 5f63 6f6e     self.auto_con
-00005c10: 6e65 6374 2874 696d 656f 7574 3d74 696d  nect(timeout=tim
-00005c20: 656f 7574 290a 2020 2020 2020 2020 6966  eout).        if
-00005c30: 2073 656c 662e 7772 6974 655f 746f 5f6c   self.write_to_l
-00005c40: 6f67 3a0a 2020 2020 2020 2020 2020 2020  og:.            
-00005c50: 7365 6c66 2e63 7265 6174 655f 6c6f 675f  self.create_log_
-00005c60: 6669 6c65 2829 0a20 2020 2020 2020 2073  file().        s
-00005c70: 656c 662e 7367 7469 6e5f 6c65 6e67 7468  elf.sgtin_length
-00005c80: 203d 2033 310a 0a20 2020 2064 6566 2063   = 31..    def c
-00005c90: 7265 6174 655f 6c6f 675f 6669 6c65 2873  reate_log_file(s
-00005ca0: 656c 6629 3a0a 2020 2020 2020 2020 7769  elf):.        wi
-00005cb0: 6c69 6f74 5f64 6972 203d 2057 696c 696f  liot_dir = Wilio
-00005cc0: 7444 6972 2829 0a20 2020 2020 2020 2077  tDir().        w
-00005cd0: 696c 696f 745f 6469 722e 6372 6561 7465  iliot_dir.create
-00005ce0: 5f64 6972 2827 5152 5f73 6361 6e27 290a  _dir('QR_scan').
-00005cf0: 2020 2020 2020 2020 6170 705f 6469 7220          app_dir 
-00005d00: 3d20 7769 6c69 6f74 5f64 6972 2e67 6574  = wiliot_dir.get
-00005d10: 5f77 696c 696f 745f 726f 6f74 5f61 7070  _wiliot_root_app
-00005d20: 5f64 6972 2829 0a20 2020 2020 2020 206c  _dir().        l
-00005d30: 6f67 5f64 6972 203d 206f 732e 7061 7468  og_dir = os.path
-00005d40: 2e6a 6f69 6e28 6170 705f 6469 722c 2027  .join(app_dir, '
-00005d50: 5152 5f73 6361 6e27 290a 2020 2020 2020  QR_scan').      
-00005d60: 2020 6966 206e 6f74 206f 732e 7061 7468    if not os.path
-00005d70: 2e65 7869 7374 7328 6c6f 675f 6469 7229  .exists(log_dir)
-00005d80: 3a0a 2020 2020 2020 2020 2020 2020 6f73  :.            os
-00005d90: 2e6d 616b 6564 6972 7328 6c6f 675f 6469  .makedirs(log_di
-00005da0: 7229 0a0a 2020 2020 2020 2020 6375 7272  r)..        curr
-00005db0: 656e 745f 7469 6d65 203d 2064 6174 6574  ent_time = datet
-00005dc0: 696d 652e 6e6f 7728 292e 7374 7266 7469  ime.now().strfti
-00005dd0: 6d65 2822 2559 2d25 6d2d 2564 5f25 482d  me("%Y-%m-%d_%H-
-00005de0: 254d 2d25 5322 290a 2020 2020 2020 2020  %M-%S").        
-00005df0: 7365 6c66 2e6c 6f67 5f66 696c 656e 616d  self.log_filenam
-00005e00: 6520 3d20 6f73 2e70 6174 682e 6a6f 696e  e = os.path.join
-00005e10: 286c 6f67 5f64 6972 2c20 6622 5152 5f72  (log_dir, f"QR_r
-00005e20: 6561 645f 6c6f 675f 7b63 7572 7265 6e74  ead_log_{current
-00005e30: 5f74 696d 657d 2e6c 6f67 2229 0a20 2020  _time}.log").   
-00005e40: 2020 2020 2077 6974 6820 6f70 656e 2873       with open(s
-00005e50: 656c 662e 6c6f 675f 6669 6c65 6e61 6d65  elf.log_filename
-00005e60: 2c20 2777 2729 2061 7320 663a 0a20 2020  , 'w') as f:.   
-00005e70: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
-00005e80: 2822 4c6f 6720 6669 6c65 2063 7265 6174  ("Log file creat
-00005e90: 6564 2e5c 6e22 290a 0a20 2020 2064 6566  ed.\n")..    def
-00005ea0: 2061 7574 6f5f 636f 6e6e 6563 7428 7365   auto_connect(se
-00005eb0: 6c66 2c20 6261 7564 3d31 3135 3230 302c  lf, baud=115200,
-00005ec0: 2063 6f6e 6669 673d 5472 7565 2c20 7469   config=True, ti
-00005ed0: 6d65 6f75 743d 2731 3030 3027 293a 0a20  meout='1000'):. 
-00005ee0: 2020 2020 2020 2063 6f6d 203d 2073 656c         com = sel
-00005ef0: 662e 6669 6e64 5f63 6f6d 5f70 6f72 7428  f.find_com_port(
-00005f00: 6261 7564 290a 2020 2020 2020 2020 6966  baud).        if
-00005f10: 2063 6f6d 2069 7320 6e6f 7420 4e6f 6e65   com is not None
-00005f20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00005f30: 6c66 2e6f 7065 6e5f 706f 7274 2863 6f6d  lf.open_port(com
-00005f40: 2c20 6261 7564 2c20 636f 6e66 6967 2c20  , baud, config, 
-00005f50: 7469 6d65 6f75 743d 7469 6d65 6f75 7429  timeout=timeout)
-00005f60: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00005f70: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00005f80: 2822 4e6f 2073 7569 7461 626c 6520 434f  ("No suitable CO
-00005f90: 4d20 706f 7274 2066 6f75 6e64 2e22 290a  M port found.").
-00005fa0: 2020 2020 2020 2020 2020 2020 7379 732e              sys.
-00005fb0: 6578 6974 2831 290a 0a20 2020 2064 6566  exit(1)..    def
-00005fc0: 2069 735f 7274 7363 616e 5f72 7432 3335   is_rtscan_rt235
-00005fd0: 2873 656c 662c 2063 6f6d 2c20 6261 7564  (self, com, baud
-00005fe0: 3d31 3135 3230 3029 3a0a 2020 2020 2020  =115200):.      
-00005ff0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00006000: 2020 2077 6974 6820 7365 7269 616c 2e53     with serial.S
-00006010: 6572 6961 6c28 636f 6d2c 2062 6175 642c  erial(com, baud,
-00006020: 2074 696d 656f 7574 3d31 2920 6173 2073   timeout=1) as s
-00006030: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
-00006040: 2020 2020 7365 722e 7772 6974 6528 7374      ser.write(st
-00006050: 722e 656e 636f 6465 2873 656c 662e 7072  r.encode(self.pr
-00006060: 6566 6978 202b 2022 5152 5950 444e 2220  efix + "QRYPDN" 
-00006070: 2b20 7365 6c66 2e73 7566 6669 7829 290a  + self.suffix)).
-00006080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006090: 736c 6565 7028 302e 3129 0a20 2020 2020  sleep(0.1).     
-000060a0: 2020 2020 2020 2020 2020 2072 6573 706f             respo
-000060b0: 6e73 6520 3d20 7365 722e 7265 6164 5f61  nse = ser.read_a
-000060c0: 6c6c 2829 2e64 6563 6f64 6528 290a 2020  ll().decode().  
-000060d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000060e0: 7475 726e 2073 656c 662e 6465 7669 6365  turn self.device
-000060f0: 5f73 6967 6e61 7475 7265 2069 6e20 7265  _signature in re
-00006100: 7370 6f6e 7365 0a20 2020 2020 2020 2065  sponse.        e
-00006110: 7863 6570 7420 4578 6365 7074 696f 6e3a  xcept Exception:
-00006120: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00006130: 7572 6e20 4661 6c73 650a 0a20 2020 2064  urn False..    d
-00006140: 6566 2066 696e 645f 636f 6d5f 706f 7274  ef find_com_port
-00006150: 2873 656c 662c 2062 6175 643d 3131 3532  (self, baud=1152
-00006160: 3030 293a 0a20 2020 2020 2020 2063 6f6d  00):.        com
-00006170: 5f70 6f72 7473 203d 2073 6572 6961 6c5f  _ports = serial_
-00006180: 706f 7274 7328 290a 2020 2020 2020 2020  ports().        
-00006190: 666f 7220 636f 6d20 696e 2063 6f6d 5f70  for com in com_p
-000061a0: 6f72 7473 3a0a 2020 2020 2020 2020 2020  orts:.          
-000061b0: 2020 6966 2073 656c 662e 6973 5f72 7473    if self.is_rts
-000061c0: 6361 6e5f 7274 3233 3528 636f 6d2c 2062  can_rt235(com, b
-000061d0: 6175 6429 3a0a 2020 2020 2020 2020 2020  aud):.          
-000061e0: 2020 2020 2020 7265 7475 726e 2063 6f6d        return com
-000061f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00006200: 4e6f 6e65 0a0a 2020 2020 6465 6620 6f70  None..    def op
-00006210: 656e 5f70 6f72 7428 7365 6c66 2c20 636f  en_port(self, co
-00006220: 6d2c 2062 6175 643d 3131 3532 3030 2c20  m, baud=115200, 
-00006230: 636f 6e66 6967 3d54 7275 652c 2074 696d  config=True, tim
-00006240: 656f 7574 3d27 3130 3030 2729 3a0a 2020  eout='1000'):.  
-00006250: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00006260: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00006270: 6c66 2e69 735f 7274 7363 616e 5f72 7432  lf.is_rtscan_rt2
-00006280: 3335 2863 6f6d 2c20 6261 7564 293a 0a20  35(com, baud):. 
-00006290: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000062a0: 6169 7365 2045 7863 6570 7469 6f6e 2866  aise Exception(f
-000062b0: 277b 636f 6d7d 2069 7320 6e6f 7420 6261  '{com} is not ba
-000062c0: 7263 6f64 6520 7363 616e 6e65 7227 290a  rcode scanner').
-000062d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000062e0: 2e73 6572 6961 6c20 3d20 7365 7269 616c  .serial = serial
-000062f0: 2e53 6572 6961 6c28 636f 6d2c 2062 6175  .Serial(com, bau
-00006300: 642c 2074 696d 656f 7574 3d28 696e 7428  d, timeout=(int(
-00006310: 7469 6d65 6f75 7429 202b 2035 3029 2f31  timeout) + 50)/1
-00006320: 3030 3029 0a20 2020 2020 2020 2065 7863  000).        exc
-00006330: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-00006340: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
-00006350: 7365 6c66 2e63 6c6f 7365 5f70 6f72 7428  self.close_port(
-00006360: 290a 2020 2020 2020 2020 2020 2020 7261  ).            ra
-00006370: 6973 6520 4578 6365 7074 696f 6e28 6627  ise Exception(f'
-00006380: 636f 756c 6420 6e6f 7420 636f 6e6e 6563  could not connec
-00006390: 7420 746f 207b 636f 6d7d 3a20 7b65 7d27  t to {com}: {e}'
-000063a0: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-000063b0: 6c66 2e73 6572 6961 6c20 6973 206e 6f74  lf.serial is not
-000063c0: 204e 6f6e 6520 616e 6420 7365 6c66 2e6c   None and self.l
-000063d0: 6f67 5f74 7970 6520 213d 2027 4e4f 5f4c  og_type != 'NO_L
-000063e0: 4f47 273a 0a20 2020 2020 2020 2020 2020  OG':.           
-000063f0: 2070 7269 6e74 2866 2742 6172 636f 6465   print(f'Barcode
-00006400: 2073 6361 6e6e 6572 2028 7b63 6f6d 7d29   scanner ({com})
-00006410: 2063 6f6e 6e65 6374 6564 2e27 290a 2020   connected.').  
-00006420: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
-00006430: 7365 7269 616c 2069 7320 4e6f 6e65 3a0a  serial is None:.
-00006440: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00006450: 7428 6627 4261 7263 6f64 6520 7363 616e  t(f'Barcode scan
-00006460: 6e65 7220 2d20 5072 6f62 6c65 6d20 636f  ner - Problem co
-00006470: 6e6e 6563 7469 6e67 207b 636f 6d7d 2729  nnecting {com}')
-00006480: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00006490: 7572 6e0a 0a20 2020 2020 2020 2073 656c  urn..        sel
-000064a0: 662e 636f 6d20 3d20 636f 6d0a 2020 2020  f.com = com.    
-000064b0: 2020 2020 2320 7365 6c66 2e73 6572 6961      # self.seria
-000064c0: 6c2e 7469 6d65 6f75 7420 3d20 2869 6e74  l.timeout = (int
-000064d0: 2874 696d 656f 7574 2920 2b20 3530 292f  (timeout) + 50)/
-000064e0: 3130 3030 2020 2320 7265 6164 2074 696d  1000  # read tim
-000064f0: 656f 7574 0a20 2020 2020 2020 2073 656c  eout.        sel
-00006500: 662e 7365 7269 616c 2e77 7269 7465 5469  f.serial.writeTi
-00006510: 6d65 6f75 7420 3d20 302e 3520 2023 2077  meout = 0.5  # w
-00006520: 7269 7465 2074 696d 656f 7574 2e0a 2020  rite timeout..  
-00006530: 2020 2020 2020 6966 2063 6f6e 6669 673a        if config:
-00006540: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00006550: 662e 636f 6e66 6967 7572 6528 7469 6d65  f.configure(time
-00006560: 5f6f 7574 3d74 696d 656f 7574 290a 0a20  _out=timeout).. 
-00006570: 2020 2064 6566 2063 6c6f 7365 5f70 6f72     def close_por
-00006580: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
-00006590: 2069 6620 7365 6c66 2e73 6572 6961 6c2e   if self.serial.
-000065a0: 6973 4f70 656e 2829 3a0a 2020 2020 2020  isOpen():.      
-000065b0: 2020 2020 2020 7365 6c66 2e73 6572 6961        self.seria
-000065c0: 6c2e 636c 6f73 6528 290a 0a20 2020 2064  l.close()..    d
-000065d0: 6566 2069 735f 6f70 656e 2873 656c 6629  ef is_open(self)
-000065e0: 3a0a 2020 2020 2020 2020 7472 793a 0a20  :.        try:. 
-000065f0: 2020 2020 2020 2020 2020 2072 6573 203d             res =
-00006600: 2073 656c 662e 6d61 6e75 616c 5f63 6f6e   self.manual_con
-00006610: 6669 6775 7265 285b 2751 5259 5044 4e27  figure(['QRYPDN'
-00006620: 5d29 0a20 2020 2020 2020 2020 2020 2069  ]).            i
-00006630: 6620 274e 4c53 2d4e 3127 2069 6e20 7374  f 'NLS-N1' in st
-00006640: 7228 7265 7329 3a0a 2020 2020 2020 2020  r(res):.        
-00006650: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00006660: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-00006670: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
-00006680: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
-00006690: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000066a0: 4661 6c73 650a 0a20 2020 2064 6566 2063  False..    def c
-000066b0: 6f6e 6669 6775 7265 2873 656c 662c 2069  onfigure(self, i
-000066c0: 6c6c 5f73 636e 3d27 3127 2c20 616d 6c5f  ll_scn='1', aml_
-000066d0: 656e 613d 2731 272c 2067 7262 5f65 6e61  ena='1', grb_ena
-000066e0: 3d27 3027 2c20 6772 625f 766c 6c3d 2732  ='0', grb_vll='2
-000066f0: 272c 2061 7473 5f65 6e61 3d27 3027 2c20  ', ats_ena='0', 
-00006700: 6174 735f 6475 723d 2733 3630 3030 272c  ats_dur='36000',
-00006710: 2073 636e 5f6d 6f64 3d27 3027 2c0a 2020   scn_mod='0',.  
-00006720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006730: 7077 625f 656e 613d 2730 272c 7272 6472  pwb_ena='0',rrdr
-00006740: 5f65 6e20 3d20 2731 272c 6772 645f 656e  _en = '1',grd_en
-00006750: 6120 3d20 2730 272c 2067 7264 5f64 7572  a = '0', grd_dur
-00006760: 203d 2027 3127 2c20 7469 6d65 5f6f 7574   = '1', time_out
-00006770: 3d27 3130 272c 2062 6164 5f6d 7367 5f65  ='10', bad_msg_e
-00006780: 6e3d 5472 7565 2c20 7379 6d62 6f6c 6f67  n=True, symbolog
-00006790: 6965 733d 4e6f 6e65 293a 0a20 2020 2020  ies=None):.     
-000067a0: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
-000067b0: 6c6c 5f73 636e 202d 2069 6c6c 756d 696e  ll_scn - illumin
-000067c0: 6174 696f 6e3a 2020 2020 2020 2020 2030  ation:         0
-000067d0: 2d6f 6666 2c20 312d 6e6f 726d 616c 2c20  -off, 1-normal, 
-000067e0: 322d 616c 7761 7973 206f 6e0a 2020 2020  2-always on.    
-000067f0: 2020 2020 616d 6c5f 656e 6120 2d20 6169      aml_ena - ai
-00006800: 6d69 6e67 3a20 2020 2020 2020 2020 2020  ming:           
-00006810: 2020 2020 302d 6f66 662c 2031 2d6e 6f72      0-off, 1-nor
-00006820: 6d61 6c2c 2032 2d61 6c77 6179 7320 6f6e  mal, 2-always on
-00006830: 0a20 2020 2020 2020 2070 7762 5f65 6e61  .        pwb_ena
-00006840: 202d 2070 6f77 6572 206f 6e20 6265 6570   - power on beep
-00006850: 2020 2020 2020 2020 2030 2d6f 6666 2c20           0-off, 
-00006860: 312d 6f6e 0a20 2020 2020 2020 2067 7262  1-on.        grb
-00006870: 5f65 6e61 202d 2067 6f6f 6420 7265 6164  _ena - good read
-00006880: 2062 6565 7020 2020 2020 2020 2030 2d6f   beep        0-o
-00006890: 6666 2c20 312d 6f6e 0a20 2020 2020 2020  ff, 1-on.       
-000068a0: 2067 7264 5f65 6e61 202d 2067 6f6f 6420   grd_ena - good 
-000068b0: 7265 6164 2065 6e61 626c 6520 2020 2020  read enable     
-000068c0: 2030 2d6f 6666 2c20 312d 6f6e 0a20 2020   0-off, 1-on.   
-000068d0: 2020 2020 2067 7264 5f64 7572 202d 2067       grd_dur - g
-000068e0: 6f6f 6420 7265 6164 2064 7572 6174 696f  ood read duratio
-000068f0: 6e20 2020 2031 2d33 3630 3030 205b 6d73  n    1-36000 [ms
-00006900: 6563 5d0a 2020 2020 2020 2020 6174 735f  ec].        ats_
-00006910: 656e 6120 2d20 6175 746f 2073 6c65 6570  ena - auto sleep
-00006920: 2020 2020 2020 2020 2020 2020 302d 6469              0-di
-00006930: 7361 626c 652c 2031 2d65 6e61 626c 650a  sable, 1-enable.
-00006940: 2020 2020 2020 2020 6174 735f 6475 7220          ats_dur 
-00006950: 2d20 736c 6565 7020 6475 7261 7469 6f6e  - sleep duration
-00006960: 2020 2020 2020 2020 312d 3336 3030 3020          1-36000 
-00006970: 5b73 6563 5d0a 2020 2020 2020 2020 7272  [sec].        rr
-00006980: 6472 5f65 6e20 2d20 5265 7265 6164 2072  dr_en - Reread r
-00006990: 6573 6574 2020 2020 2020 2020 2020 302d  eset          0-
-000069a0: 6f66 662c 2031 2d6f 6e0a 2020 2020 2020  off, 1-on.      
-000069b0: 2020 7363 6e5f 6d6f 6420 2d20 7363 616e    scn_mod - scan
-000069c0: 206d 6f64 6520 2020 2020 2020 2020 2020   mode           
-000069d0: 2020 302d 6c65 7665 6c20 6d6f 6465 2c20    0-level mode, 
-000069e0: 322d 7365 6e73 6520 6d6f 6465 2c20 332d  2-sense mode, 3-
-000069f0: 636f 6e74 696e 756f 7573 206d 6f64 652c  continuous mode,
-00006a00: 2037 2d62 6174 6368 206d 6f64 650a 2020   7-batch mode.  
-00006a10: 2020 2020 2020 7379 6d62 6f6c 6f67 6965        symbologie
-00006a20: 7320 2d20 6120 6c69 7374 206f 6620 7374  s - a list of st
-00006a30: 7269 6e67 7320 7265 7072 6573 656e 7469  rings representi
-00006a40: 6e67 2074 6865 2073 796d 626f 6c6f 6769  ng the symbologi
-00006a50: 6573 2074 6f20 656e 6162 6c65 2c20 652e  es to enable, e.
-00006a60: 672e 205b 2751 5227 2c20 2750 4446 3431  g. ['QR', 'PDF41
-00006a70: 3727 2c20 2745 414e 3133 275d 0a0a 2020  7', 'EAN13']..  
-00006a80: 2020 2020 2020 4c65 7665 6c20 4d6f 6465        Level Mode
-00006a90: 3a0a 2020 2020 2020 2020 496e 2074 6869  :.        In thi
-00006aa0: 7320 6d6f 6465 2c20 7468 6520 7363 616e  s mode, the scan
-00006ab0: 6e65 7220 7761 6974 7320 666f 7220 6120  ner waits for a 
-00006ac0: 7472 6967 6765 7220 7075 6c6c 2074 6f20  trigger pull to 
-00006ad0: 6163 7469 7661 7465 2061 2064 6563 6f64  activate a decod
-00006ae0: 6520 7365 7373 696f 6e2e 2054 6865 2064  e session. The d
-00006af0: 6563 6f64 6520 7365 7373 696f 6e20 636f  ecode session co
-00006b00: 6e74 696e 7565 7320 756e 7469 6c20 6120  ntinues until a 
-00006b10: 6261 7263 6f64 6520 6973 2064 6563 6f64  barcode is decod
-00006b20: 6564 206f 7220 796f 7520 7265 6c65 6173  ed or you releas
-00006b30: 6520 7468 6520 7472 6967 6765 722e 0a20  e the trigger.. 
-00006b40: 2020 2020 2020 2043 6f6d 6d61 6e64 2074         Command t
-00006b50: 7269 6767 6572 206d 6f64 653a 0a20 2020  rigger mode:.   
-00006b60: 2020 2020 2054 6869 7320 6d6f 6465 2072       This mode r
-00006b70: 6571 7569 7265 7320 796f 7520 746f 2073  equires you to s
-00006b80: 656e 6420 6120 636f 6d6d 616e 6420 2831  end a command (1
-00006b90: 4220 3331 2069 6e20 6865 7829 2074 6f20  B 31 in hex) to 
-00006ba0: 6163 7469 7661 7465 2061 2064 6563 6f64  activate a decod
-00006bb0: 6520 7365 7373 696f 6e2e 0a0a 2020 2020  e session...    
-00006bc0: 2020 2020 5365 6e73 6520 4d6f 6465 3a0a      Sense Mode:.
-00006bd0: 2020 2020 2020 2020 496e 2074 6869 7320          In this 
-00006be0: 6d6f 6465 2c20 7468 6520 7363 616e 6e65  mode, the scanne
-00006bf0: 7220 6163 7469 7661 7465 7320 6120 6465  r activates a de
-00006c00: 636f 6465 2073 6573 7369 6f6e 2065 7665  code session eve
-00006c10: 7279 2074 696d 6520 6974 2064 6574 6563  ry time it detec
-00006c20: 7473 2061 2062 6172 636f 6465 2070 7265  ts a barcode pre
-00006c30: 7365 6e74 6564 2074 6f20 6974 2e20 5468  sented to it. Th
-00006c40: 6520 6465 636f 6465 2073 6573 7369 6f6e  e decode session
-00006c50: 2063 6f6e 7469 6e75 6573 2075 6e74 696c   continues until
-00006c60: 2061 2062 6172 636f 6465 2069 7320 6465   a barcode is de
-00006c70: 636f 6465 6420 6f72 2074 6865 2064 6563  coded or the dec
-00006c80: 6f64 6520 7365 7373 696f 6e20 7469 6d65  ode session time
-00006c90: 6f75 7420 6578 7069 7265 732e 2059 6f75  out expires. You
-00006ca0: 2063 616e 2061 646a 7573 7420 7468 6520   can adjust the 
-00006cb0: 7365 6e73 6974 6976 6974 7920 616e 6420  sensitivity and 
-00006cc0: 7265 7265 6164 2074 696d 656f 7574 2074  reread timeout t
-00006cd0: 6f20 6176 6f69 6420 756e 6465 7369 7265  o avoid undesire
-00006ce0: 6420 7265 7265 6164 696e 6720 6f66 2074  d rereading of t
-00006cf0: 6865 2073 616d 6520 6261 7263 6f64 6520  he same barcode 
-00006d00: 696e 2061 2067 6976 656e 2070 6572 696f  in a given perio
-00006d10: 6420 6f66 2074 696d 652e 2059 6f75 2063  d of time. You c
-00006d20: 616e 2061 6c73 6f20 6164 6a75 7374 2074  an also adjust t
-00006d30: 6865 2069 6d61 6765 2073 7461 6269 6c69  he image stabili
-00006d40: 7a61 7469 6f6e 2074 696d 656f 7574 2074  zation timeout t
-00006d50: 6f20 6769 7665 2074 6865 2073 6361 6e6e  o give the scann
-00006d60: 6572 2074 696d 6520 746f 2061 6461 7074  er time to adapt
-00006d70: 2074 6f20 616d 6269 656e 7420 656e 7669   to ambient envi
-00006d80: 726f 6e6d 656e 7420 6166 7465 7220 6974  ronment after it
-00006d90: 2064 6563 6f64 6573 2061 2062 6172 636f   decodes a barco
-00006da0: 6465 2061 6e64 20e2 809c 6c6f 6f6b 73e2  de and ...looks.
-00006db0: 809d 2066 6f72 2061 6e6f 7468 6572 2e0a  .. for another..
-00006dc0: 0a20 2020 2020 2020 2043 6f6e 7469 6e75  .        Continu
-00006dd0: 6f75 7320 4d6f 6465 3a0a 2020 2020 2020  ous Mode:.      
-00006de0: 2020 496e 2074 6869 7320 6d6f 6465 2c20    In this mode, 
-00006df0: 7468 6520 7363 616e 6e65 7220 6175 746f  the scanner auto
-00006e00: 6d61 7469 6361 6c6c 7920 7374 6172 7473  matically starts
-00006e10: 206f 6e65 2064 6563 6f64 6520 7365 7373   one decode sess
-00006e20: 696f 6e20 6166 7465 7220 616e 6f74 6865  ion after anothe
-00006e30: 722e 2054 6f20 7375 7370 656e 642f 7265  r. To suspend/re
-00006e40: 7375 6d65 2062 6172 636f 6465 2072 6561  sume barcode rea
-00006e50: 6469 6e67 2c20 7369 6d70 6c79 2070 7265  ding, simply pre
-00006e60: 7373 2074 6865 2074 7269 6767 6572 2e20  ss the trigger. 
-00006e70: 596f 7520 6361 6e20 6164 6a75 7374 2074  You can adjust t
-00006e80: 6865 2072 6572 6561 6420 7469 6d65 6f75  he reread timeou
-00006e90: 7420 746f 2061 766f 6964 2075 6e64 6573  t to avoid undes
-00006ea0: 6972 6564 2072 6572 6561 6469 6e67 206f  ired rereading o
-00006eb0: 6620 7468 6520 7361 6d65 2062 6172 636f  f the same barco
-00006ec0: 6465 2069 6e20 6120 6769 7665 6e20 7065  de in a given pe
-00006ed0: 7269 6f64 206f 6620 7469 6d65 2e20 4e6f  riod of time. No
-00006ee0: 7465 2074 6861 7420 7768 656e 2073 7769  te that when swi
-00006ef0: 7463 6869 6e67 2074 6f20 7468 6973 206d  tching to this m
-00006f00: 6f64 6520 6279 2073 6361 6e6e 696e 6720  ode by scanning 
-00006f10: 7468 6520 436f 6e74 696e 756f 7573 204d  the Continuous M
-00006f20: 6f64 6520 6261 7263 6f64 652c 2074 6865  ode barcode, the
-00006f30: 2073 6361 6e6e 6572 2077 696c 6c20 7374   scanner will st
-00006f40: 6f70 2062 6172 636f 6465 2072 6561 6469  op barcode readi
-00006f50: 6e67 2066 6f72 2033 2073 6563 6f6e 6473  ng for 3 seconds
-00006f60: 2062 6566 6f72 6520 7374 6172 7469 6e67   before starting
-00006f70: 2073 6361 6e6e 696e 6720 636f 6e74 696e   scanning contin
-00006f80: 756f 7573 6c79 2e0a 0a20 2020 2020 2020  uously...       
-00006f90: 2042 6174 6368 204d 6f64 653a 0a20 2020   Batch Mode:.   
-00006fa0: 2020 2020 2049 6e20 7468 6973 206d 6f64       In this mod
-00006fb0: 652c 2061 2074 7269 6767 6572 2070 756c  e, a trigger pul
-00006fc0: 6c20 6163 7469 7661 7465 7320 6120 726f  l activates a ro
-00006fd0: 756e 6420 6f66 206d 756c 7469 706c 6520  und of multiple 
-00006fe0: 6465 636f 6465 2073 6573 7369 6f6e 732e  decode sessions.
-00006ff0: 2054 6865 2072 6f75 6e64 206f 6620 6d75   The round of mu
-00007000: 6c74 6970 6c65 2073 6361 6e73 2063 6f6e  ltiple scans con
-00007010: 7469 6e75 6573 2075 6e74 696c 2079 6f75  tinues until you
-00007020: 2072 656c 6561 7365 2074 6865 2074 7269   release the tri
-00007030: 6767 6572 2e20 5265 7265 6164 696e 6720  gger. Rereading 
-00007040: 7468 6520 7361 6d65 2062 6172 636f 6465  the same barcode
-00007050: 2069 7320 6e6f 7420 616c 6c6f 7765 6420   is not allowed 
-00007060: 696e 2074 6865 2073 616d 6520 726f 756e  in the same roun
-00007070: 642e 0a20 2020 2020 2020 2027 2727 0a0a  d..        '''..
-00007080: 2020 2020 2020 2020 736c 6565 7028 302e          sleep(0.
-00007090: 3129 0a20 2020 2020 2020 2070 6172 616d  1).        param
-000070a0: 7320 3d20 7b27 494c 4c53 434e 273a 2069  s = {'ILLSCN': i
-000070b0: 6c6c 5f73 636e 2c20 2741 4d4c 454e 4127  ll_scn, 'AMLENA'
-000070c0: 3a20 616d 6c5f 656e 612c 2027 4752 4245  : aml_ena, 'GRBE
-000070d0: 4e41 273a 2067 7262 5f65 6e61 2c20 2741  NA': grb_ena, 'A
-000070e0: 5453 454e 4127 3a20 6174 735f 656e 612c  TSENA': ats_ena,
-000070f0: 2027 4e47 5245 4e41 273a 2027 3127 2069   'NGRENA': '1' i
-00007100: 6620 6261 645f 6d73 675f 656e 2065 6c73  f bad_msg_en els
-00007110: 6520 2730 272c 0a20 2020 2020 2020 2020  e '0',.         
-00007120: 2020 2020 2020 2020 2027 4752 4256 4c4c           'GRBVLL
-00007130: 273a 2067 7262 5f76 6c6c 2c20 2741 5453  ': grb_vll, 'ATS
-00007140: 4455 5227 3a20 6174 735f 6475 722c 2027  DUR': ats_dur, '
-00007150: 5343 4e4d 4f44 273a 2073 636e 5f6d 6f64  SCNMOD': scn_mod
-00007160: 2c20 2752 5244 5245 4e27 3a20 7272 6472  , 'RRDREN': rrdr
-00007170: 5f65 6e2c 2027 4752 4445 4e41 2720 3a20  _en, 'GRDENA' : 
-00007180: 6772 645f 656e 612c 2027 4752 4444 5552  grd_ena, 'GRDDUR
-00007190: 2720 3a20 6772 645f 6475 722c 0a20 2020  ' : grd_dur,.   
-000071a0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000071b0: 5057 4245 4e41 273a 2070 7762 5f65 6e61  PWBENA': pwb_ena
-000071c0: 2c20 274f 5254 5345 5427 3a20 7469 6d65  , 'ORTSET': time
-000071d0: 5f6f 7574 7d0a 2020 2020 2020 2020 7061  _out}.        pa
-000071e0: 7261 6d73 203d 205b 6b65 7920 2b20 7661  rams = [key + va
-000071f0: 6c75 6520 666f 7220 6b65 792c 2076 616c  lue for key, val
-00007200: 7565 2069 6e20 7061 7261 6d73 2e69 7465  ue in params.ite
-00007210: 6d73 2829 5d0a 0a20 2020 2020 2020 2069  ms()]..        i
-00007220: 6620 7379 6d62 6f6c 6f67 6965 7320 6973  f symbologies is
-00007230: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00007240: 2020 2020 2020 2066 6f72 2073 796d 626f         for symbo
-00007250: 6c6f 6779 2069 6e20 7379 6d62 6f6c 6f67  logy in symbolog
-00007260: 6965 733a 0a20 2020 2020 2020 2020 2020  ies:.           
-00007270: 2020 2020 2070 6172 616d 732e 6170 7065       params.appe
-00007280: 6e64 2827 5359 4d42 5f27 202b 2073 796d  nd('SYMB_' + sym
-00007290: 626f 6c6f 6779 202b 2027 3127 290a 0a20  bology + '1').. 
-000072a0: 2020 2020 2020 2074 2c20 6973 5375 6363         t, isSucc
-000072b0: 6573 7320 3d20 7365 6c66 2e6d 616e 7561  ess = self.manua
-000072c0: 6c5f 636f 6e66 6967 7572 6528 7061 7261  l_configure(para
-000072d0: 6d73 290a 2020 2020 2020 2020 6966 2069  ms).        if i
-000072e0: 7353 7563 6365 7373 2061 6e64 2073 656c  sSuccess and sel
-000072f0: 662e 6c6f 675f 7479 7065 2021 3d20 274e  f.log_type != 'N
-00007300: 4f5f 4c4f 4727 3a0a 2020 2020 2020 2020  O_LOG':.        
-00007310: 2020 2020 7072 696e 7428 6627 4261 7263      print(f'Barc
-00007320: 6f64 6520 7363 616e 6e65 7220 287b 7365  ode scanner ({se
-00007330: 6c66 2e63 6f6d 7d29 2063 6f6e 6669 6775  lf.com}) configu
-00007340: 7265 6420 7375 6363 6573 7366 756c 6c79  red successfully
-00007350: 2e27 290a 2020 2020 2020 2020 656c 6966  .').        elif
-00007360: 206e 6f74 2069 7353 7563 6365 7373 3a0a   not isSuccess:.
-00007370: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00007380: 7428 6627 4261 7263 6f64 6520 7363 616e  t(f'Barcode scan
-00007390: 6e65 7220 287b 7365 6c66 2e63 6f6d 7d29  ner ({self.com})
-000073a0: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
-000073b0: 6169 6c65 642e 2729 0a0a 2020 2020 6465  ailed.')..    de
-000073c0: 6620 7265 7374 6f72 655f 616c 6c5f 6661  f restore_all_fa
-000073d0: 6374 6f72 795f 6465 6661 756c 7473 2873  ctory_defaults(s
-000073e0: 656c 6629 3a0a 2020 2020 2020 2020 736c  elf):.        sl
-000073f0: 6565 7028 302e 3129 0a20 2020 2020 2020  eep(0.1).       
-00007400: 2070 6172 616d 7320 3d20 7b27 4641 4344   params = {'FACD
-00007410: 4546 273a 2027 277d 0a20 2020 2020 2020  EF': ''}.       
-00007420: 2070 6172 616d 7320 3d20 5b6b 6579 202b   params = [key +
-00007430: 2076 616c 7565 2066 6f72 206b 6579 2c20   value for key, 
-00007440: 7661 6c75 6520 696e 2070 6172 616d 732e  value in params.
-00007450: 6974 656d 7328 295d 0a20 2020 2020 2020  items()].       
-00007460: 2074 2c20 6973 5375 6363 6573 7320 3d20   t, isSuccess = 
-00007470: 7365 6c66 2e6d 616e 7561 6c5f 636f 6e66  self.manual_conf
-00007480: 6967 7572 6528 7061 7261 6d73 290a 2020  igure(params).  
-00007490: 2020 2020 2020 6966 2069 7353 7563 6365        if isSucce
-000074a0: 7373 2061 6e64 2073 656c 662e 6c6f 675f  ss and self.log_
-000074b0: 7479 7065 2021 3d20 274e 4f5f 4c4f 4727  type != 'NO_LOG'
-000074c0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-000074d0: 696e 7428 6627 4261 7263 6f64 6520 7363  int(f'Barcode sc
-000074e0: 616e 6e65 7220 287b 7365 6c66 2e63 6f6d  anner ({self.com
-000074f0: 7d29 2072 6573 746f 7265 6420 6661 6374  }) restored fact
-00007500: 6f72 7920 6465 6661 756c 7420 7375 6363  ory default succ
-00007510: 6573 7366 756c 6c79 2e27 290a 2020 2020  essfully.').    
-00007520: 2020 2020 656c 6966 206e 6f74 2069 7353      elif not isS
-00007530: 7563 6365 7373 3a0a 2020 2020 2020 2020  uccess:.        
-00007540: 2020 2020 7072 696e 7428 6627 4261 7263      print(f'Barc
-00007550: 6f64 6520 7363 616e 6e65 7220 287b 7365  ode scanner ({se
-00007560: 6c66 2e63 6f6d 7d29 2072 6573 746f 7265  lf.com}) restore
-00007570: 6420 6661 6374 6f72 7920 6465 6661 756c  d factory defaul
-00007580: 7420 6661 696c 6564 2e27 290a 0a20 2020  t failed.')..   
-00007590: 2064 6566 206d 616e 7561 6c5f 636f 6e66   def manual_conf
-000075a0: 6967 7572 6528 7365 6c66 2c20 7061 7261  igure(self, para
-000075b0: 6d73 293a 0a20 2020 2020 2020 2073 656c  ms):.        sel
-000075c0: 662e 7365 7269 616c 2e66 6c75 7368 496e  f.serial.flushIn
-000075d0: 7075 7428 290a 2020 2020 2020 2020 7365  put().        se
-000075e0: 6c66 2e73 6572 6961 6c2e 666c 7573 684f  lf.serial.flushO
-000075f0: 7574 7075 7428 290a 2020 2020 2020 2020  utput().        
-00007600: 736c 6565 7028 302e 3129 0a20 2020 2020  sleep(0.1).     
-00007610: 2020 2023 2062 6164 5f6d 7367 203d 2027     # bad_msg = '
-00007620: 3436 3431 3439 3443 2720 2372 6570 7265  4641494C' #repre
-00007630: 7365 6e74 2027 4641 494c 2720 696e 2041  sent 'FAIL' in A
-00007640: 5343 4949 2068 6578 610a 2020 2020 2020  SCII hexa.      
-00007650: 2020 6261 645f 6d73 6720 3d20 2734 3627    bad_msg = '46'
-00007660: 0a20 2020 2020 2020 2065 6e74 6572 5f73  .        enter_s
-00007670: 6574 7570 5f6d 6f64 6520 3d20 2753 4554  etup_mode = 'SET
-00007680: 5550 4531 270a 2020 2020 2020 2020 6578  UPE1'.        ex
-00007690: 6974 5f73 6574 7570 5f6d 6f64 6520 3d20  it_setup_mode = 
-000076a0: 2753 4554 5550 4530 270a 2020 2020 2020  'SETUPE0'.      
-000076b0: 2020 2345 6e74 6572 2073 6574 7570 206d    #Enter setup m
-000076c0: 6f64 650a 2020 2020 2020 2020 7365 6c66  ode.        self
-000076d0: 2e73 6572 6961 6c2e 7772 6974 6528 7374  .serial.write(st
-000076e0: 722e 656e 636f 6465 2873 656c 662e 7072  r.encode(self.pr
-000076f0: 6566 6978 202b 2065 6e74 6572 5f73 6574  efix + enter_set
-00007700: 7570 5f6d 6f64 6520 2b20 7365 6c66 2e73  up_mode + self.s
-00007710: 7566 6669 7829 290a 2020 2020 2020 2020  uffix)).        
-00007720: 2320 496e 7365 7274 2063 6f6e 6669 6775  # Insert configu
-00007730: 7261 7469 6f6e 0a20 2020 2020 2020 2063  ration.        c
-00007740: 6f6e 6669 6773 203d 2073 656c 662e 7072  onfigs = self.pr
-00007750: 6566 6978 202b 2027 3b27 2e6a 6f69 6e28  efix + ';'.join(
-00007760: 7061 7261 6d73 2920 2b20 7365 6c66 2e73  params) + self.s
-00007770: 7566 6669 780a 2020 2020 2020 2020 7365  uffix.        se
-00007780: 6c66 2e73 6572 6961 6c2e 7772 6974 6528  lf.serial.write(
-00007790: 7374 722e 656e 636f 6465 2863 6f6e 6669  str.encode(confi
-000077a0: 6773 2929 0a20 2020 2020 2020 2069 6620  gs)).        if 
-000077b0: 274e 4752 454e 4131 2720 696e 2070 6172  'NGRENA1' in par
-000077c0: 616d 733a 0a20 2020 2020 2020 2020 2020  ams:.           
-000077d0: 2073 656c 662e 7365 7269 616c 2e77 7269   self.serial.wri
-000077e0: 7465 2873 7472 2e65 6e63 6f64 6528 7365  te(str.encode(se
-000077f0: 6c66 2e70 7265 6669 7820 2b20 274e 4752  lf.prefix + 'NGR
-00007800: 5345 5427 2b20 6261 645f 6d73 6720 2b20  SET'+ bad_msg + 
-00007810: 7365 6c66 2e73 7566 6669 7829 2920 2023  self.suffix))  #
-00007820: 2053 6574 206d 6573 7361 6765 2074 6f20   Set message to 
-00007830: 656d 7074 790a 2020 2020 2020 2020 6966  empty.        if
-00007840: 2027 5343 4e4d 4f44 3227 2069 6e20 7061   'SCNMOD2' in pa
-00007850: 7261 6d73 3a0a 2020 2020 2020 2020 2020  rams:.          
-00007860: 2020 7365 6c66 2e73 6572 6961 6c2e 7772    self.serial.wr
-00007870: 6974 6528 7374 722e 656e 636f 6465 2873  ite(str.encode(s
-00007880: 656c 662e 7072 6566 6978 202b 2027 5345  elf.prefix + 'SE
-00007890: 4e4c 564c 3527 202b 2062 6164 5f6d 7367  NLVL5' + bad_msg
-000078a0: 202b 2073 656c 662e 7375 6666 6978 2929   + self.suffix))
-000078b0: 2020 2320 5365 7420 7365 6e73 6974 6976    # Set sensitiv
-000078c0: 6974 7920 746f 2068 6967 6820 312d 3230  ity to high 1-20
-000078d0: 0a20 2020 2020 2020 2023 2045 7869 7420  .        # Exit 
-000078e0: 7365 7475 7020 6d6f 6465 0a20 2020 2020  setup mode.     
-000078f0: 2020 2073 656c 662e 7365 7269 616c 2e77     self.serial.w
-00007900: 7269 7465 2873 7472 2e65 6e63 6f64 6528  rite(str.encode(
-00007910: 7365 6c66 2e70 7265 6669 7820 2b20 6578  self.prefix + ex
-00007920: 6974 5f73 6574 7570 5f6d 6f64 6520 2b20  it_setup_mode + 
-00007930: 7365 6c66 2e73 7566 6669 7829 290a 2020  self.suffix)).  
-00007940: 2020 2020 2020 736c 6565 7028 302e 3129        sleep(0.1)
-00007950: 0a20 2020 2020 2020 2074 2c20 6973 5375  .        t, isSu
-00007960: 6363 6573 7320 3d20 7365 6c66 2e74 7269  ccess = self.tri
-00007970: 6767 6572 5f73 746f 705f 7365 7474 696e  gger_stop_settin
-00007980: 6773 2829 0a20 2020 2020 2020 2072 6574  gs().        ret
-00007990: 7572 6e20 742c 2069 7353 7563 6365 7373  urn t, isSuccess
-000079a0: 0a0a 2020 2020 6465 6620 7363 616e 2873  ..    def scan(s
-000079b0: 656c 6629 3a0a 2020 2020 2020 2020 7420  elf):.        t 
-000079c0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
-000079d0: 656c 662e 7365 7269 616c 2e77 7269 7465  elf.serial.write
-000079e0: 2862 225c 7831 625c 7833 3122 290a 2020  (b"\x1b\x31").  
-000079f0: 2020 2020 2020 7374 6172 745f 7469 6d65        start_time
-00007a00: 203d 2064 6174 6574 696d 652e 6e6f 7728   = datetime.now(
-00007a10: 290a 2020 2020 2020 2020 7420 3d20 7365  ).        t = se
-00007a20: 6c66 2e73 6572 6961 6c2e 7265 6164 6c69  lf.serial.readli
-00007a30: 6e65 2829 0a20 2020 2020 2020 2023 2070  ne().        # p
-00007a40: 7269 6e74 2866 2767 6f74 206d 7367 207b  rint(f'got msg {
-00007a50: 747d 2729 0a20 2020 2020 2020 2065 6e64  t}').        end
-00007a60: 5f74 696d 6520 3d20 6461 7465 7469 6d65  _time = datetime
-00007a70: 2e6e 6f77 2829 0a20 2020 2020 2020 2065  .now().        e
-00007a80: 6c61 7073 6564 5f74 696d 655f 6d73 203d  lapsed_time_ms =
-00007a90: 2028 656e 645f 7469 6d65 202d 2073 7461   (end_time - sta
-00007aa0: 7274 5f74 696d 6529 2e74 6f74 616c 5f73  rt_time).total_s
-00007ab0: 6563 6f6e 6473 2829 202a 2031 3030 300a  econds() * 1000.
-00007ac0: 2020 2020 2020 2020 7265 7475 726e 2074          return t
-00007ad0: 2c20 656c 6170 7365 645f 7469 6d65 5f6d  , elapsed_time_m
-00007ae0: 730a 0a20 2020 2064 6566 2073 6361 6e5f  s..    def scan_
-00007af0: 616e 645f 666c 7573 6828 7365 6c66 293a  and_flush(self):
-00007b00: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00007b10: 2e73 6572 6961 6c20 6973 204e 6f6e 653a  .serial is None:
-00007b20: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00007b30: 6e74 2822 4572 726f 723a 2053 6572 6961  nt("Error: Seria
-00007b40: 6c20 6f62 6a65 6374 206e 6f74 2069 6e69  l object not ini
-00007b50: 7469 616c 697a 6564 2229 0a20 2020 2020  tialized").     
-00007b60: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-00007b70: 6e65 0a20 2020 2020 2020 2074 2c20 656c  ne.        t, el
-00007b80: 6170 7365 645f 7469 6d65 5f6d 7320 3d20  apsed_time_ms = 
-00007b90: 7365 6c66 2e73 6361 6e28 290a 2020 2020  self.scan().    
-00007ba0: 2020 2020 2320 5072 6f63 6573 7320 7265      # Process re
-00007bb0: 6365 6976 6564 2064 6174 6120 6d6f 7265  ceived data more
-00007bc0: 2065 6666 6963 6965 6e74 6c79 0a20 2020   efficiently.   
-00007bd0: 2020 2020 2069 6620 7420 3d3d 2062 2727       if t == b''
-00007be0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00007bf0: 6973 6520 4578 6365 7074 696f 6e28 2745  ise Exception('E
-00007c00: 7272 6f72 2069 6e20 5363 616e 6e65 7220  rror in Scanner 
-00007c10: 5365 7269 616c 2063 6f6e 6e65 6374 696f  Serial connectio
-00007c20: 6e27 290a 2020 2020 2020 2020 656c 6966  n').        elif
-00007c30: 2074 2e73 7461 7274 7377 6974 6828 6227   t.startswith(b'
-00007c40: 5c78 3036 2729 3a0a 2020 2020 2020 2020  \x06'):.        
-00007c50: 2020 2020 6966 2074 203d 3d20 6227 5c78      if t == b'\x
-00007c60: 3036 273a 0a20 2020 2020 2020 2020 2020  06':.           
-00007c70: 2020 2020 2073 6c65 6570 2830 2e31 290a       sleep(0.1).
-00007c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c90: 7365 6c66 2e73 6572 6961 6c2e 7265 7365  self.serial.rese
-00007ca0: 745f 696e 7075 745f 6275 6666 6572 2829  t_input_buffer()
-00007cb0: 0a20 2020 2020 2020 2020 2020 2074 5f63  .            t_c
-00007cc0: 6c65 616e 203d 2074 5b31 3a5d 2e64 6563  lean = t[1:].dec
-00007cd0: 6f64 6528 292e 7374 7269 7028 292e 7265  ode().strip().re
-00007ce0: 706c 6163 6528 275c 725c 6e27 2c20 2727  place('\r\n', ''
-00007cf0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00007d00: 2074 5f63 6c65 616e 2069 7320 4e6f 6e65   t_clean is None
-00007d10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007d20: 2020 7265 7475 726e 204e 6f6e 652c 2065    return None, e
-00007d30: 6c61 7073 6564 5f74 696d 655f 6d73 0a20  lapsed_time_ms. 
-00007d40: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00007d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007d60: 2072 6574 7572 6e20 745f 636c 6561 6e2c   return t_clean,
-00007d70: 2065 6c61 7073 6564 5f74 696d 655f 6d73   elapsed_time_ms
-00007d80: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00007d90: 2020 2020 2020 2020 2020 2023 7072 696e             #prin
-00007da0: 7428 2757 6172 6e69 6e67 202d 206e 6f74  t('Warning - not
-00007db0: 2072 6563 6569 7665 6420 4143 4b20 6672   received ACK fr
-00007dc0: 6f6d 2062 6172 636f 6465 2073 6361 6e6e  om barcode scann
-00007dd0: 6572 2e27 290a 2020 2020 2020 2020 2020  er.').          
-00007de0: 2020 7265 7475 726e 204e 6f6e 652c 2065    return None, e
-00007df0: 6c61 7073 6564 5f74 696d 655f 6d73 0a0a  lapsed_time_ms..
-00007e00: 2020 2020 6465 6620 7363 616e 5f65 7874      def scan_ext
-00007e10: 5f69 6428 7365 6c66 293a 0a20 2020 2020  _id(self):.     
-00007e20: 2020 2062 6172 636f 6465 5f72 6561 6420     barcode_read 
-00007e30: 3d20 2727 0a20 2020 2020 2020 2073 7461  = ''.        sta
-00007e40: 7274 5f74 696d 6520 3d20 7469 6d65 2829  rt_time = time()
-00007e50: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-00007e60: 2020 2020 2020 2020 2020 6261 7263 6f64            barcod
-00007e70: 655f 7265 6164 2c20 656c 6170 7365 645f  e_read, elapsed_
-00007e80: 7469 6d65 5f6d 7320 3d20 7365 6c66 2e73  time_ms = self.s
-00007e90: 6361 6e5f 616e 645f 666c 7573 6828 290a  can_and_flush().
-00007ea0: 2020 2020 2020 2020 2020 2020 6966 2062              if b
-00007eb0: 6172 636f 6465 5f72 6561 6420 6973 204e  arcode_read is N
-00007ec0: 6f6e 6520 6f72 2062 6172 636f 6465 5f72  one or barcode_r
-00007ed0: 6561 6420 3d3d 2727 3a0a 2020 2020 2020  ead =='':.      
-00007ee0: 2020 2020 2020 2020 2020 6261 7263 6f64            barcod
-00007ef0: 655f 7265 6164 203d 2027 270a 2020 2020  e_read = ''.    
-00007f00: 2020 2020 2020 2020 2020 2020 6675 6c6c              full
-00007f10: 5f64 6174 6120 3d20 6375 725f 6964 203d  _data = cur_id =
-00007f20: 2072 6565 6c5f 6964 203d 2067 7469 6e20   reel_id = gtin 
-00007f30: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-00007f40: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00007f50: 2020 2020 2020 2020 2066 756c 6c5f 6461           full_da
-00007f60: 7461 2c20 6375 725f 6964 2c20 7265 656c  ta, cur_id, reel
-00007f70: 5f69 642c 2067 7469 6e20 3d20 7365 6c66  _id, gtin = self
-00007f80: 2e72 6561 645f 6261 7263 6f64 6528 6261  .read_barcode(ba
-00007f90: 7263 6f64 655f 7265 6164 290a 2020 2020  rcode_read).    
-00007fa0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00007fb0: 7772 6974 655f 746f 5f6c 6f67 3a0a 2020  write_to_log:.  
-00007fc0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-00007fd0: 7468 206f 7065 6e28 7365 6c66 2e6c 6f67  th open(self.log
-00007fe0: 5f66 696c 656e 616d 652c 2027 6127 2920  _filename, 'a') 
-00007ff0: 6173 2066 3a0a 2020 2020 2020 2020 2020  as f:.          
-00008000: 2020 2020 2020 2020 2020 7469 6d65 7374            timest
-00008010: 616d 7020 3d20 6461 7465 7469 6d65 2e6e  amp = datetime.n
-00008020: 6f77 2829 2e73 7472 6674 696d 6528 2225  ow().strftime("%
-00008030: 592d 256d 2d25 6420 2548 3a25 4d3a 2553  Y-%m-%d %H:%M:%S
-00008040: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00008050: 2020 2020 2020 206c 6f67 5f6d 6573 7361         log_messa
-00008060: 6765 203d 2066 227b 7469 6d65 7374 616d  ge = f"{timestam
-00008070: 707d 202d 207b 6675 6c6c 5f64 6174 617d  p} - {full_data}
-00008080: 202d 2045 6c61 7073 6564 2054 696d 653a   - Elapsed Time:
-00008090: 207b 656c 6170 7365 645f 7469 6d65 5f6d   {elapsed_time_m
-000080a0: 733a 2e32 667d 206d 735c 6e22 0a20 2020  s:.2f} ms\n".   
-000080b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080c0: 2066 2e77 7269 7465 286c 6f67 5f6d 6573   f.write(log_mes
-000080d0: 7361 6765 290a 0a20 2020 2020 2020 2020  sage)..         
-000080e0: 2020 2072 6574 7572 6e20 6675 6c6c 5f64     return full_d
-000080f0: 6174 612c 2063 7572 5f69 642c 2072 6565  ata, cur_id, ree
-00008100: 6c5f 6964 2c20 6774 696e 0a20 2020 2020  l_id, gtin.     
-00008110: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00008120: 696f 6e20 6173 2065 3a0a 2020 2020 2020  ion as e:.      
-00008130: 2020 2020 2020 7072 696e 7428 6529 0a20        print(e). 
-00008140: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00008150: 6e20 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f  n None, None, No
-00008160: 6e65 2c20 4e6f 6e65 0a0a 2020 2020 6465  ne, None..    de
-00008170: 6620 7265 6164 5f62 6172 636f 6465 2873  f read_barcode(s
-00008180: 656c 662c 2062 6172 636f 6465 5f72 6561  elf, barcode_rea
-00008190: 6429 3a0a 2020 2020 2020 2020 7472 793a  d):.        try:
-000081a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000081b0: 2728 3031 2927 2069 6e20 6261 7263 6f64  '(01)' in barcod
-000081c0: 655f 7265 6164 3a0a 2020 2020 2020 2020  e_read:.        
-000081d0: 2020 2020 2020 2020 6261 7263 6f64 6573          barcodes
-000081e0: 203d 2062 6172 636f 6465 5f72 6561 642e   = barcode_read.
-000081f0: 7370 6c69 7428 2228 3031 2922 290a 2020  split("(01)").  
-00008200: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00008210: 7220 692c 2073 696e 676c 655f 6261 7263  r i, single_barc
-00008220: 6f64 6520 696e 2065 6e75 6d65 7261 7465  ode in enumerate
-00008230: 2862 6172 636f 6465 735b 313a 5d2c 2031  (barcodes[1:], 1
-00008240: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00008250: 2020 2020 2020 2066 756c 6c5f 6461 7461         full_data
-00008260: 203d 2066 2228 3031 297b 7369 6e67 6c65   = f"(01){single
-00008270: 5f62 6172 636f 6465 7d22 0a20 2020 2020  _barcode}".     
-00008280: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-00008290: 7469 6e20 3d20 2729 272e 6a6f 696e 2866  tin = ')'.join(f
-000082a0: 756c 6c5f 6461 7461 2e73 706c 6974 2827  ull_data.split('
-000082b0: 2927 295b 3a32 5d29 202b 2027 2927 0a20  )')[:2]) + ')'. 
-000082c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082d0: 2020 2074 6167 5f64 6174 6120 3d20 6675     tag_data = fu
-000082e0: 6c6c 5f64 6174 612e 7370 6c69 7428 2729  ll_data.split(')
-000082f0: 2729 5b32 5d0a 2020 2020 2020 2020 2020  ')[2].          
-00008300: 2020 2020 2020 2020 2020 6375 725f 6964            cur_id
-00008310: 203d 2074 6167 5f64 6174 612e 7370 6c69   = tag_data.spli
-00008320: 7428 2754 2729 5b31 5d2e 7374 7269 7028  t('T')[1].strip(
-00008330: 2227 2022 292e 7370 6c69 7428 2728 2729  "' ").split('(')
-00008340: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-00008350: 2020 2020 2020 2020 7265 656c 5f69 6420          reel_id 
-00008360: 3d20 7461 675f 6461 7461 2e73 706c 6974  = tag_data.split
-00008370: 2827 5427 295b 305d 2e73 7472 6970 2822  ('T')[0].strip("
-00008380: 2720 2229 0a0a 2020 2020 2020 2020 2020  ' ")..          
-00008390: 2020 2020 2020 2020 2020 6966 2066 756c            if ful
-000083a0: 6c5f 6461 7461 2061 6e64 2063 7572 5f69  l_data and cur_i
-000083b0: 6420 616e 6420 7265 656c 5f69 6420 616e  d and reel_id an
-000083c0: 6420 6774 696e 3a0a 2020 2020 2020 2020  d gtin:.        
-000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083e0: 7265 7475 726e 2066 756c 6c5f 6461 7461  return full_data
-000083f0: 2c20 6375 725f 6964 2c20 7265 656c 5f69  , cur_id, reel_i
-00008400: 642c 2067 7469 6e0a 2020 2020 2020 2020  d, gtin.        
-00008410: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00008420: 2020 2020 2020 2020 2020 6675 6c6c 5f64            full_d
-00008430: 6174 6120 3d20 6375 725f 6964 203d 2072  ata = cur_id = r
-00008440: 6565 6c5f 6964 203d 2067 7469 6e20 3d20  eel_id = gtin = 
-00008450: 6261 7263 6f64 655f 7265 6164 0a20 2020  barcode_read.   
-00008460: 2020 2020 2020 2020 2020 2020 2067 7469               gti
-00008470: 6e5f 7661 6c20 3d20 5472 7565 2069 6620  n_val = True if 
-00008480: 6c65 6e28 6675 6c6c 5f64 6174 6129 203d  len(full_data) =
-00008490: 3d20 7365 6c66 2e73 6774 696e 5f6c 656e  = self.sgtin_len
-000084a0: 6774 6820 656c 7365 2046 616c 7365 0a20  gth else False. 
-000084b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000084c0: 6620 6774 696e 5f76 616c 3a0a 2020 2020  f gtin_val:.    
-000084d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084e0: 6375 725f 6964 203d 2066 756c 6c5f 6461  cur_id = full_da
-000084f0: 7461 2e73 706c 6974 2827 5427 295b 315d  ta.split('T')[1]
-00008500: 2e73 7472 6970 2822 2720 2229 2e73 706c  .strip("' ").spl
-00008510: 6974 2827 2827 295b 305d 0a20 2020 2020  it('(')[0].     
-00008520: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00008530: 6565 6c5f 6964 203d 2066 756c 6c5f 6461  eel_id = full_da
-00008540: 7461 2e73 706c 6974 2827 5427 295b 305d  ta.split('T')[0]
-00008550: 2e73 7472 6970 2822 2720 2229 5b2d 343a  .strip("' ")[-4:
-00008560: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00008570: 2020 2020 2020 6774 696e 203d 2066 756c        gtin = ful
-00008580: 6c5f 6461 7461 2e73 706c 6974 2827 5427  l_data.split('T'
-00008590: 295b 305d 2e73 7472 6970 2822 2720 2229  )[0].strip("' ")
-000085a0: 5b3a 2d34 5d0a 2020 2020 2020 2020 2020  [:-4].          
-000085b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000085c0: 2066 756c 6c5f 6461 7461 2c20 6375 725f   full_data, cur_
-000085d0: 6964 2c20 7265 656c 5f69 642c 2067 7469  id, reel_id, gti
-000085e0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-000085f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00008600: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00008610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008620: 2020 2020 2020 2020 2069 6620 6675 6c6c           if full
-00008630: 5f64 6174 6120 3d3d 2027 4627 3a0a 2020  _data == 'F':.  
-00008640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008650: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00008660: 274e 6f20 6261 7263 6f64 6520 6465 7465  'No barcode dete
-00008670: 6374 6564 2729 0a20 2020 2020 2020 2020  cted').         
-00008680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008690: 2020 2072 6574 7572 6e20 4e6f 6e65 2c20     return None, 
-000086a0: 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65  None, None, None
-000086b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000086c0: 2020 2020 2020 2020 2065 6c69 6620 6675           elif fu
-000086d0: 6c6c 5f64 6174 6120 3d3d 2027 273a 0a20  ll_data == '':. 
-000086e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086f0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00008700: 2045 7863 6570 7469 6f6e 2827 5072 6f62   Exception('Prob
-00008710: 6c65 6d20 7769 7468 2062 6172 636f 6465  lem with barcode
-00008720: 2073 6361 6e6e 6572 2729 0a20 2020 2020   scanner').     
-00008730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008740: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00008750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008760: 2020 2020 2063 7572 5f69 6420 3d20 6675       cur_id = fu
-00008770: 6c6c 5f64 6174 612e 7370 6c69 7428 2754  ll_data.split('T
-00008780: 2729 5b31 5d0a 2020 2020 2020 2020 2020  ')[1].          
-00008790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087a0: 2020 7265 656c 5f69 6420 3d20 6675 6c6c    reel_id = full
-000087b0: 5f64 6174 612e 7370 6c69 7428 2754 2729  _data.split('T')
-000087c0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-000087d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087e0: 6774 696e 203d 2027 270a 0a20 2020 2020  gtin = ''..     
-000087f0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00008800: 7863 6570 7420 4578 6365 7074 696f 6e3a  xcept Exception:
-00008810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008820: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-00008830: 4e6f 7420 5769 6c69 6f74 2062 6172 636f  Not Wiliot barco
-00008840: 6465 2729 0a0a 2020 2020 2020 2020 2020  de')..          
-00008850: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00008860: 2066 756c 6c5f 6461 7461 2c20 6375 725f   full_data, cur_
-00008870: 6964 2c20 7265 656c 5f69 642c 2067 7469  id, reel_id, gti
-00008880: 6e0a 0a20 2020 2020 2020 2065 7863 6570  n..        excep
-00008890: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-000088a0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-000088b0: 696e 7428 6622 4572 726f 7220 6475 7269  int(f"Error duri
-000088c0: 6e67 2072 6561 6469 6e67 2057 696c 696f  ng reading Wilio
-000088d0: 7420 6261 7263 6f64 653a 207b 657d 2229  t barcode: {e}")
-000088e0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-000088f0: 7365 2045 7863 6570 7469 6f6e 0a0a 2020  se Exception..  
-00008900: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-00008910: 652c 204e 6f6e 652c 204e 6f6e 652c 204e  e, None, None, N
-00008920: 6f6e 650a 0a20 2020 2064 6566 2061 7574  one..    def aut
-00008930: 6f5f 7363 616e 2873 656c 6629 3a0a 2020  o_scan(self):.  
-00008940: 2020 2020 2020 7365 6c66 2e73 6572 6961        self.seria
-00008950: 6c2e 7772 6974 6528 6222 5c78 3162 5c78  l.write(b"\x1b\x
-00008960: 3332 2229 0a0a 2020 2020 2020 2020 7420  32")..        t 
-00008970: 3d20 7365 6c66 2e73 6572 6961 6c2e 7265  = self.serial.re
-00008980: 6164 5f61 6c6c 2829 0a20 2020 2020 2020  ad_all().       
-00008990: 2070 7269 6e74 2866 2761 7574 6f20 7363   print(f'auto sc
-000089a0: 616e 3a20 676f 7420 6d73 6720 7b74 7d27  an: got msg {t}'
-000089b0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000089c0: 2074 0a0a 2020 2020 6465 6620 7472 6967   t..    def trig
-000089d0: 6765 725f 7374 6f70 5f73 6574 7469 6e67  ger_stop_setting
-000089e0: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-000089f0: 2073 6c65 6570 2830 2e30 3529 0a20 2020   sleep(0.05).   
-00008a00: 2020 2020 2074 203d 2073 656c 662e 7365       t = self.se
-00008a10: 7269 616c 2e72 6561 645f 616c 6c28 290a  rial.read_all().
-00008a20: 2020 2020 2020 2020 2320 7072 696e 7428          # print(
-00008a30: 6627 656e 6420 636f 6e66 6967 3a20 676f  f'end config: go
-00008a40: 7420 6d73 6720 7b74 7d27 290a 2020 2020  t msg {t}').    
-00008a50: 2020 2020 736c 6565 7028 302e 3035 290a      sleep(0.05).
-00008a60: 2020 2020 2020 2020 2320 7072 696e 7428          # print(
-00008a70: 7429 0a20 2020 2020 2020 2061 636b 7320  t).        acks 
-00008a80: 3d20 7374 7228 7429 2e73 706c 6974 2827  = str(t).split('
-00008a90: 3b27 295b 3a2d 315d 0a20 2020 2020 2020  ;')[:-1].       
-00008aa0: 2069 7353 7563 6365 7373 203d 2061 6c6c   isSuccess = all
-00008ab0: 285b 5472 7565 2069 6620 6163 6b2e 656e  ([True if ack.en
-00008ac0: 6473 7769 7468 2827 5c5c 7830 3627 290a  dswith('\\x06').
-00008ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ae0: 2020 2020 2020 2020 2065 6c73 6520 4661           else Fa
-00008af0: 6c73 6520 666f 7220 6163 6b20 696e 2061  lse for ack in a
-00008b00: 636b 735d 290a 2020 2020 2020 2020 7265  cks]).        re
-00008b10: 7475 726e 2074 2c20 6973 5375 6363 6573  turn t, isSucces
-00008b20: 730a 0a0a 636c 6173 7320 596f 6374 6f54  s...class YoctoT
-00008b30: 656d 7065 7261 7475 7265 5365 6e73 6f72  emperatureSensor
-00008b40: 286f 626a 6563 7429 3a0a 2020 2020 6465  (object):.    de
-00008b50: 6620 5f5f 696e 6974 5f5f 2873 656c 6629  f __init__(self)
-00008b60: 3a0a 2020 2020 2020 2020 7365 6c66 2e73  :.        self.s
-00008b70: 656e 736f 7220 3d20 4e6f 6e65 0a20 2020  ensor = None.   
-00008b80: 2020 2020 2065 7272 6d73 6720 3d20 5952       errmsg = YR
-00008b90: 6566 5061 7261 6d28 290a 2020 2020 2020  efParam().      
-00008ba0: 2020 2320 5365 7475 7020 7468 6520 4150    # Setup the AP
-00008bb0: 4920 746f 2075 7365 206c 6f63 616c 2055  I to use local U
-00008bc0: 5342 2064 6576 6963 6573 0a20 2020 2020  SB devices.     
-00008bd0: 2020 2069 6620 5941 5049 2e52 6567 6973     if YAPI.Regis
-00008be0: 7465 7248 7562 2822 7573 6222 2c20 6572  terHub("usb", er
-00008bf0: 726d 7367 2920 213d 2059 4150 492e 5355  rmsg) != YAPI.SU
-00008c00: 4343 4553 533a 0a20 2020 2020 2020 2020  CCESS:.         
-00008c10: 2020 2072 6169 7365 2045 7175 6970 6d65     raise Equipme
-00008c20: 6e74 4572 726f 7228 2779 6f63 746f 2074  ntError('yocto t
-00008c30: 656d 7065 7261 7475 7265 2073 656e 736f  emperature senso
-00008c40: 7220 676f 7420 696e 6974 2065 7272 6f72  r got init error
-00008c50: 3a20 7b7d 272e 666f 726d 6174 2865 7272  : {}'.format(err
-00008c60: 6d73 672e 7661 6c75 6529 290a 0a20 2020  msg.value))..   
-00008c70: 2064 6566 2063 6f6e 6e65 6374 2873 656c   def connect(sel
-00008c80: 662c 2074 6172 6765 743d 2761 6e79 2729  f, target='any')
-00008c90: 3a0a 2020 2020 2020 2020 6966 2074 6172  :.        if tar
-00008ca0: 6765 7420 3d3d 2027 616e 7927 3a0a 2020  get == 'any':.  
-00008cb0: 2020 2020 2020 2020 2020 2320 7265 7472            # retr
-00008cc0: 6965 7665 2061 6e79 2074 656d 7065 7261  ieve any tempera
-00008cd0: 7475 7265 2073 656e 736f 720a 2020 2020  ture sensor.    
-00008ce0: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
-00008cf0: 736f 7220 3d20 5954 656d 7065 7261 7475  sor = YTemperatu
-00008d00: 7265 2e46 6972 7374 5465 6d70 6572 6174  re.FirstTemperat
-00008d10: 7572 6528 290a 2020 2020 2020 2020 656c  ure().        el
-00008d20: 6966 2074 6172 6765 7420 3d3d 2027 273a  if target == '':
-00008d30: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00008d40: 6e74 2827 7370 6563 6966 6965 6420 696e  nt('specified in
-00008d50: 7661 6c69 6420 7461 7267 6574 2729 0a20  valid target'). 
-00008d60: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00008d70: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
-00008d80: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00008d90: 2020 7365 6c66 2e73 656e 736f 7220 3d20    self.sensor = 
-00008da0: 5954 656d 7065 7261 7475 7265 2e46 696e  YTemperature.Fin
-00008db0: 6454 656d 7065 7261 7475 7265 2874 6172  dTemperature(tar
-00008dc0: 6765 7420 2b20 272e 7465 6d70 6572 6174  get + '.temperat
-00008dd0: 7572 6527 290a 2020 2020 2020 2020 6966  ure').        if
-00008de0: 2073 656c 662e 7365 6e73 6f72 2069 7320   self.sensor is 
-00008df0: 4e6f 6e65 206f 7220 7365 6c66 2e67 6574  None or self.get
-00008e00: 5f73 656e 736f 725f 6e61 6d65 2829 203d  _sensor_name() =
-00008e10: 3d20 2775 6e72 6573 6f6c 7665 6427 3a0a  = 'unresolved':.
-00008e20: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00008e30: 7428 274e 6f20 6d6f 6475 6c65 2063 6f6e  t('No module con
-00008e40: 6e65 6374 6564 2729 0a20 2020 2020 2020  nected').       
-00008e50: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00008e60: 650a 2020 2020 2020 2020 656c 7365 3a0a  e.        else:.
-00008e70: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00008e80: 726e 2054 7275 650a 0a20 2020 2064 6566  rn True..    def
-00008e90: 2067 6574 5f73 656e 736f 725f 6e61 6d65   get_sensor_name
-00008ea0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00008eb0: 6966 2073 656c 662e 7365 6e73 6f72 2069  if self.sensor i
-00008ec0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00008ed0: 2020 2020 7072 696e 7428 276e 6f20 7365      print('no se
-00008ee0: 6e73 6f72 2069 7320 636f 6e6e 6563 7465  nsor is connecte
-00008ef0: 642e 2074 7279 2074 6f20 6361 6c6c 2063  d. try to call c
-00008f00: 6f6e 6e65 6374 2829 2066 6972 7374 2729  onnect() first')
-00008f10: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00008f20: 7572 6e20 2727 0a0a 2020 2020 2020 2020  urn ''..        
-00008f30: 7365 6e73 6f72 5f73 7472 203d 2073 656c  sensor_str = sel
-00008f40: 662e 7365 6e73 6f72 2e64 6573 6372 6962  f.sensor.describ
-00008f50: 6528 290a 2020 2020 2020 2020 6e61 6d65  e().        name
-00008f60: 5f73 7472 203d 2073 656e 736f 725f 7374  _str = sensor_st
-00008f70: 722e 7370 6c69 7428 273d 2729 5b31 5d2e  r.split('=')[1].
-00008f80: 7370 6c69 7428 272e 2729 5b30 5d0a 2020  split('.')[0].  
-00008f90: 2020 2020 2020 7265 7475 726e 206e 616d        return nam
-00008fa0: 655f 7374 720a 0a20 2020 2064 6566 2067  e_str..    def g
-00008fb0: 6574 5f74 656d 7065 7261 7475 7265 2873  et_temperature(s
-00008fc0: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
-00008fd0: 2073 656c 662e 7365 6e73 6f72 2069 7320   self.sensor is 
-00008fe0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00008ff0: 2020 7072 696e 7428 2773 656e 736f 7220    print('sensor 
-00009000: 6973 206e 6f74 2063 6f6e 6e65 6374 6564  is not connected
-00009010: 2e20 7472 7920 746f 2063 616c 6c20 636f  . try to call co
-00009020: 6e6e 6563 7428 2920 6669 7273 7427 290a  nnect() first').
-00009030: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00009040: 726e 2066 6c6f 6174 2827 6e61 6e27 290a  rn float('nan').
-00009050: 2020 2020 2020 2020 6966 206e 6f74 2028          if not (
-00009060: 7365 6c66 2e73 656e 736f 722e 6973 4f6e  self.sensor.isOn
-00009070: 6c69 6e65 2829 293a 0a20 2020 2020 2020  line()):.       
-00009080: 2020 2020 2070 7269 6e74 2827 7365 6e73       print('sens
-00009090: 6f72 2069 7320 6e6f 7420 636f 6e6e 6563  or is not connec
-000090a0: 7465 6420 6f72 2064 6973 636f 6e6e 6563  ted or disconnec
-000090b0: 7465 6420 6475 7269 6e67 2072 756e 2729  ted during run')
-000090c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000090d0: 7572 6e20 666c 6f61 7428 276e 616e 2729  urn float('nan')
-000090e0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000090f0: 2073 656c 662e 7365 6e73 6f72 2e67 6574   self.sensor.get
-00009100: 5f63 7572 7265 6e74 5661 6c75 6528 290a  _currentValue().
-00009110: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-00009120: 6f64 0a20 2020 2064 6566 2065 7869 745f  od.    def exit_
-00009130: 6170 7028 293a 0a20 2020 2020 2020 2059  app():.        Y
-00009140: 4150 492e 4672 6565 4150 4928 290a       API.FreeAPI().
+000036c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000036d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036e0: 7061 7373 0a20 2020 2020 2020 2020 2020  pass.           
+000036f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00003700: 2020 2020 2020 2073 656c 662e 7320 3d20         self.s = 
+00003710: 7365 7269 616c 2e53 6572 6961 6c28 636f  serial.Serial(co
+00003720: 6d70 6f72 742c 2073 656c 662e 6261 7564  mport, self.baud
+00003730: 7261 7465 2c20 7469 6d65 6f75 743d 302e  rate, timeout=0.
+00003740: 3529 0a20 2020 2020 2020 2020 2020 2020  5).             
+00003750: 2020 2073 6c65 6570 2831 290a 2020 2020     sleep(1).    
+00003760: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003770: 2e73 2e77 7269 7465 2822 434f 4e53 4f4c  .s.write("CONSOL
+00003780: 4520 4449 5341 424c 455c 725c 6e22 2e65  E DISABLE\r\n".e
+00003790: 6e63 6f64 6528 2929 0a20 2020 2020 2020  ncode()).       
+000037a0: 2020 2020 2020 2020 2023 2046 6c75 7368           # Flush
+000037b0: 2074 6865 2062 7566 6665 7273 0a20 2020   the buffers.   
+000037c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000037d0: 662e 732e 666c 7573 6828 290a 2020 2020  f.s.flush().    
+000037e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000037f0: 2e73 2e66 6c75 7368 496e 7075 7428 290a  .s.flushInput().
+00003800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003810: 7365 6c66 2e73 2e66 6c75 7368 4f75 7470  self.s.flushOutp
+00003820: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
+00003830: 2020 2020 2073 656c 662e 5175 6572 7928       self.Query(
+00003840: 222a 4944 4e3f 5c72 5c6e 2229 0a20 2020  "*IDN?\r\n").   
+00003850: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00003860: 7020 3d20 7365 6c66 2e51 7565 7279 2822  p = self.Query("
+00003870: 2a49 444e 3f5c 725c 6e22 290a 2020 2020  *IDN?\r\n").    
+00003880: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003890: 2e6d 6f64 656c 203d 2072 6573 700a 2020  .model = resp.  
+000038a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000038b0: 2028 2241 6572 6f66 6c65 7822 2069 6e20   ("Aeroflex" in 
+000038c0: 7265 7370 2920 6f72 2028 2234 3230 3522  resp) or ("4205"
+000038d0: 2069 6e20 7265 7370 293a 0a20 2020 2020   in resp):.     
+000038e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000038f0: 7269 6e74 2827 466f 756e 6420 2720 2b20  rint('Found ' + 
+00003900: 7265 7370 2e73 7472 6970 2827 5c72 5c6e  resp.strip('\r\n
+00003910: 2729 202b 2027 206f 6e20 706f 7274 3a20  ') + ' on port: 
+00003920: 2720 2b20 636f 6d70 6f72 7429 0a20 2020  ' + comport).   
+00003930: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00003940: 6620 2738 3331 3127 2069 6e20 7265 7370  f '8311' in resp
+00003950: 206f 7220 2738 3333 3127 2069 6e20 7265   or '8331' in re
+00003960: 7370 3a0a 2020 2020 2020 2020 2020 2020  sp:.            
+00003970: 2020 2020 2020 2020 7072 696e 7428 2746          print('F
+00003980: 6f75 6e64 2027 202b 2072 6573 702e 7374  ound ' + resp.st
+00003990: 7269 7028 275c 725c 6e27 2920 2b20 2720  rip('\r\n') + ' 
+000039a0: 6f6e 2070 6f72 743a 2027 202b 2063 6f6d  on port: ' + com
+000039b0: 706f 7274 290a 2020 2020 2020 2020 2020  port).          
+000039c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000039d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039e0: 7365 6c66 2e63 6c6f 7365 5f70 6f72 7428  self.close_port(
+000039f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003a00: 2020 2020 2020 7072 696e 7428 2741 6572        print('Aer
+00003a10: 6f66 6c65 7820 4174 7465 6e75 6174 6f72  oflex Attenuator
+00003a20: 206e 6f74 2066 6f75 6e64 206f 6e20 7365   not found on se
+00003a30: 6c65 6374 6564 2070 6f72 742c 2063 6865  lected port, che
+00003a40: 636b 2063 6f6e 6e65 6374 696f 6e27 2c20  ck connection', 
+00003a50: 6669 6c65 3d73 7973 2e73 7464 6572 7229  file=sys.stderr)
+00003a60: 0a0a 2020 2020 2020 2020 6465 6620 5772  ..        def Wr
+00003a70: 6974 6528 7365 6c66 2c20 636d 642c 2077  ite(self, cmd, w
+00003a80: 6169 743d 4661 6c73 6529 3a0a 2020 2020  ait=False):.    
+00003a90: 2020 2020 2020 2020 2222 2253 656e 6420          """Send 
+00003aa0: 7468 6520 696e 7075 7420 636d 6420 7374  the input cmd st
+00003ab0: 7269 6e67 2076 6961 2043 4f4d 2053 6f63  ring via COM Soc
+00003ac0: 6b65 7422 2222 0a20 2020 2020 2020 2020  ket""".         
+00003ad0: 2020 2069 6620 7365 6c66 2e73 2e69 734f     if self.s.isO
+00003ae0: 7065 6e28 293a 0a20 2020 2020 2020 2020  pen():.         
+00003af0: 2020 2020 2020 2070 6173 730a 2020 2020         pass.    
+00003b00: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00003b10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003b20: 6c66 2e73 2e6f 7065 6e28 290a 2020 2020  lf.s.open().    
+00003b30: 2020 2020 2020 2020 7365 6c66 2e73 2e66          self.s.f
+00003b40: 6c75 7368 496e 7075 7428 290a 2020 2020  lushInput().    
+00003b50: 2020 2020 2020 2020 736c 6565 7028 3129          sleep(1)
+00003b60: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+00003b70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00003b80: 2020 7365 6c66 2e73 2e77 7269 7465 2873    self.s.write(s
+00003b90: 7472 2e65 6e63 6f64 6528 636d 6429 290a  tr.encode(cmd)).
+00003ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bb0: 736c 6565 7028 302e 3129 2020 2320 436f  sleep(0.1)  # Co
+00003bc0: 6d6d 616e 6473 206d 6179 2062 6520 6c6f  mmands may be lo
+00003bd0: 7374 2077 6865 6e20 7772 6974 696e 6720  st when writing 
+00003be0: 746f 6f20 6661 7374 0a0a 2020 2020 2020  too fast..      
+00003bf0: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+00003c00: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00003c10: 7373 0a20 2020 2020 2020 2020 2020 2023  ss.            #
+00003c20: 2073 656c 662e 732e 636c 6f73 6528 290a   self.s.close().
+00003c30: 0a20 2020 2020 2020 2064 6566 2051 7565  .        def Que
+00003c40: 7279 2873 656c 662c 2063 6d64 293a 0a20  ry(self, cmd):. 
+00003c50: 2020 2020 2020 2020 2020 2022 2222 5365             """Se
+00003c60: 6e64 2074 6865 2069 6e70 7574 2063 6d64  nd the input cmd
+00003c70: 2073 7472 696e 6720 7669 6120 434f 4d20   string via COM 
+00003c80: 536f 636b 6574 2061 6e64 2072 6574 7572  Socket and retur
+00003c90: 6e20 7468 6520 7265 706c 7920 7374 7269  n the reply stri
+00003ca0: 6e67 2222 220a 2020 2020 2020 2020 2020  ng""".          
+00003cb0: 2020 6966 2073 656c 662e 732e 6973 4f70    if self.s.isOp
+00003cc0: 656e 2829 3a0a 2020 2020 2020 2020 2020  en():.          
+00003cd0: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
+00003ce0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00003cf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00003d00: 662e 732e 6f70 656e 2829 0a20 2020 2020  f.s.open().     
+00003d10: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
+00003d20: 2830 2e31 290a 2020 2020 2020 2020 2020  (0.1).          
+00003d30: 2020 2320 7365 6c66 2e73 2e66 6c75 7368    # self.s.flush
+00003d40: 496e 7075 7428 290a 2020 2020 2020 2020  Input().        
+00003d50: 2020 2020 736c 6565 7028 3129 0a20 2020      sleep(1).   
+00003d60: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+00003d70: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003d80: 6c66 2e73 2e77 7269 7465 2863 6d64 2e65  lf.s.write(cmd.e
+00003d90: 6e63 6f64 6528 2929 0a20 2020 2020 2020  ncode()).       
+00003da0: 2020 2020 2020 2020 2073 6c65 6570 2830           sleep(0
+00003db0: 2e31 290a 2020 2020 2020 2020 2020 2020  .1).            
+00003dc0: 2020 2020 6966 2073 656c 662e 732e 696e      if self.s.in
+00003dd0: 5f77 6169 7469 6e67 203e 2030 3a0a 2020  _waiting > 0:.  
+00003de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003df0: 2020 6461 7461 203d 2073 656c 662e 732e    data = self.s.
+00003e00: 7265 6164 6c69 6e65 2829 2e64 6563 6f64  readline().decod
+00003e10: 6528 2275 7466 2d38 2229 0a20 2020 2020  e("utf-8").     
+00003e20: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00003e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003e40: 2020 2020 2064 6174 6120 3d20 2727 0a20       data = ''. 
+00003e50: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00003e60: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00003e70: 2020 2064 6174 6120 3d20 2727 0a20 2020     data = ''.   
+00003e80: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
+00003e90: 732e 636c 6f73 6528 290a 2020 2020 2020  s.close().      
+00003ea0: 2020 2020 2020 7265 7475 726e 2064 6174        return dat
+00003eb0: 610a 0a20 2020 2020 2020 2064 6566 2063  a..        def c
+00003ec0: 6c6f 7365 5f70 6f72 7428 7365 6c66 293a  lose_port(self):
+00003ed0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00003ee0: 7365 6c66 2e73 2069 7320 6e6f 7420 4e6f  self.s is not No
+00003ef0: 6e65 2061 6e64 2073 656c 662e 732e 6973  ne and self.s.is
+00003f00: 4f70 656e 2829 3a0a 2020 2020 2020 2020  Open():.        
+00003f10: 2020 2020 2020 2020 7365 6c66 2e73 2e63          self.s.c
+00003f20: 6c6f 7365 2829 0a0a 2020 2020 2020 2020  lose()..        
+00003f30: 6465 6620 6973 5f6f 7065 6e28 7365 6c66  def is_open(self
+00003f40: 2c20 6368 6563 6b5f 706f 7274 3d46 616c  , check_port=Fal
+00003f50: 7365 293a 0a20 2020 2020 2020 2020 2020  se):.           
+00003f60: 2069 6620 7365 6c66 2e73 2069 7320 6e6f   if self.s is no
+00003f70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00003f80: 2020 2020 2020 2020 6966 2063 6865 636b          if check
+00003f90: 5f70 6f72 743a 0a20 2020 2020 2020 2020  _port:.         
+00003fa0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+00003fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fc0: 2020 2020 2020 2020 7365 6c66 2e51 7565          self.Que
+00003fd0: 7279 2822 2a49 444e 3f5c 725c 6e22 290a  ry("*IDN?\r\n").
+00003fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ff0: 2020 2020 2020 2020 7265 7370 203d 2073          resp = s
+00004000: 656c 662e 5175 6572 7928 222a 4944 4e3f  elf.Query("*IDN?
+00004010: 5c72 5c6e 2229 0a20 2020 2020 2020 2020  \r\n").         
+00004020: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004030: 656c 662e 6d6f 6465 6c20 3d20 7265 7370  elf.model = resp
+00004040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004050: 2020 2020 2020 2020 2069 6620 2822 4165           if ("Ae
+00004060: 726f 666c 6578 2220 696e 2072 6573 7029  roflex" in resp)
+00004070: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004080: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00004090: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+000040a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040b0: 2020 656c 6966 2027 3833 3131 2720 696e    elif '8311' in
+000040c0: 2072 6573 7020 6f72 2027 3833 3331 2720   resp or '8331' 
+000040d0: 696e 2072 6573 703a 0a20 2020 2020 2020  in resp:.       
+000040e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040f0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00004100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004110: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
+00004120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004130: 2020 2020 2073 656c 662e 636c 6f73 655f       self.close_
+00004140: 706f 7274 2829 0a20 2020 2020 2020 2020  port().         
+00004150: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00004160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004170: 2072 6574 7572 6e20 7365 6c66 2e73 2e69   return self.s.i
+00004180: 734f 7065 6e28 290a 2020 2020 2020 2020  sOpen().        
+00004190: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+000041a0: 0a0a 2020 2020 2020 2020 6465 6620 5365  ..        def Se
+000041b0: 7461 7474 6e28 7365 6c66 2c20 6174 746e  tattn(self, attn
+000041c0: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+000041d0: 6d64 203d 2022 4154 544e 207b 3a2e 3266  md = "ATTN {:.2f
+000041e0: 7d5c 725c 6e22 2e66 6f72 6d61 7428 6174  }\r\n".format(at
+000041f0: 746e 290a 2020 2020 2020 2020 2020 2020  tn).            
+00004200: 7365 6c66 2e57 7269 7465 2863 6d64 290a  self.Write(cmd).
+00004210: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00004220: 6520 3d20 7365 6c66 2e47 6574 6174 746e  e = self.Getattn
+00004230: 2829 0a20 2020 2020 2020 2020 2020 2076  ().            v
+00004240: 616c 7565 203d 2066 6c6f 6174 2876 616c  alue = float(val
+00004250: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+00004260: 6966 2076 616c 7565 2021 3d20 6174 746e  if value != attn
+00004270: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004280: 2020 7072 696e 7428 6627 4572 726f 7220    print(f'Error 
+00004290: 7365 7474 696e 6720 6174 7465 6e75 6174  setting attenuat
+000042a0: 696f 6e3a 206e 6577 203a 207b 6174 746e  ion: new : {attn
+000042b0: 7d20 6375 7272 656e 743a 207b 7661 6c75  } current: {valu
+000042c0: 657d 2729 0a20 2020 2020 2020 2020 2020  e}').           
+000042d0: 2072 6574 7572 6e20 7661 6c75 650a 0a20   return value.. 
+000042e0: 2020 2020 2020 2064 6566 2047 6574 6174         def Getat
+000042f0: 746e 2873 656c 6629 3a0a 2020 2020 2020  tn(self):.      
+00004300: 2020 2020 2020 636d 6420 3d20 2241 5454        cmd = "ATT
+00004310: 4e3f 5c72 5c6e 220a 2020 2020 2020 2020  N?\r\n".        
+00004320: 2020 2020 7661 6c75 6520 3d20 7365 6c66      value = self
+00004330: 2e51 7565 7279 2863 6d64 290a 2020 2020  .Query(cmd).    
+00004340: 2020 2020 2020 2020 7265 7475 726e 2076          return v
+00004350: 616c 7565 0a0a 0a63 6c61 7373 2054 6573  alue...class Tes
+00004360: 636f 6d3a 0a20 2020 2022 2222 0a20 2020  com:.    """.   
+00004370: 2043 6f6e 7472 6f6c 2054 4553 434f 4d20   Control TESCOM 
+00004380: 7465 7374 696e 6720 6368 616d 6265 7273  testing chambers
+00004390: 0a20 2020 2022 2222 0a20 2020 206f 7065  .    """.    ope
+000043a0: 6e5f 636d 6420 3d20 6227 4f50 454e 5c72  n_cmd = b'OPEN\r
+000043b0: 270a 2020 2020 636c 6f73 655f 636d 6420  '.    close_cmd 
+000043c0: 3d20 6227 434c 4f53 455c 7227 0a20 2020  = b'CLOSE\r'.   
+000043d0: 2063 6f6d 5f70 6f72 745f 6f62 6a20 3d20   com_port_obj = 
+000043e0: 4e6f 6e65 0a20 2020 206d 6f64 656c 735f  None.    models_
+000043f0: 6c69 7374 203d 205b 2754 432d 3530 3634  list = ['TC-5064
+00004400: 4327 2c20 2754 412d 3730 3131 4150 272c  C', 'TA-7011AP',
+00004410: 2027 5443 2d35 3036 3341 272c 2027 5443   'TC-5063A', 'TC
+00004420: 2d35 3937 3043 5027 5d0a 0a20 2020 2064  -5970CP']..    d
+00004430: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00004440: 2c20 706f 7274 3d4e 6f6e 6529 3a0a 2020  , port=None):.  
+00004450: 2020 2020 2020 7365 6c66 2e70 6f72 7420        self.port 
+00004460: 3d20 706f 7274 0a20 2020 2020 2020 2074  = port.        t
+00004470: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00004480: 6966 2070 6f72 7420 6973 206e 6f74 204e  if port is not N
+00004490: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000044a0: 2020 2020 2073 656c 662e 636f 6e6e 6563       self.connec
+000044b0: 7428 706f 7274 290a 0a20 2020 2020 2020  t(port)..       
+000044c0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+000044d0: 6e20 6173 2065 3a0a 2020 2020 2020 2020  n as e:.        
+000044e0: 2020 2020 7072 696e 7428 6529 0a20 2020      print(e).   
+000044f0: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+00004500: 5465 7363 6f6d 202d 2043 6f6e 6e65 6374  Tescom - Connect
+00004510: 696f 6e20 6661 696c 6564 2229 0a0a 2020  ion failed")..  
+00004520: 2020 6465 6620 636f 6e6e 6563 7428 7365    def connect(se
+00004530: 6c66 2c20 706f 7274 293a 0a20 2020 2020  lf, port):.     
+00004540: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00004550: 7061 7261 6d20 706f 7274 3a20 636f 6d20  param port: com 
+00004560: 706f 7274 2074 6f20 636f 6e6e 6563 740a  port to connect.
+00004570: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00004580: 2063 6f6d 2070 6f72 7420 6f62 6a0a 2020   com port obj.  
+00004590: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000045a0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+000045b0: 2020 2063 6f6d 5f70 6f72 745f 6f62 6a20     com_port_obj 
+000045c0: 3d20 7365 6c66 2e63 6f6d 5f70 6f72 745f  = self.com_port_
+000045d0: 6f62 6a20 3d20 7365 7269 616c 2e53 6572  obj = serial.Ser
+000045e0: 6961 6c28 706f 7274 3d70 6f72 742c 2062  ial(port=port, b
+000045f0: 6175 6472 6174 653d 3936 3030 2c20 7469  audrate=9600, ti
+00004600: 6d65 6f75 743d 3129 0a20 2020 2020 2020  meout=1).       
+00004610: 2020 2020 2069 6620 636f 6d5f 706f 7274       if com_port
+00004620: 5f6f 626a 2069 7320 6e6f 7420 4e6f 6e65  _obj is not None
+00004630: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004640: 2020 7365 6c66 2e64 6f6f 725f 636d 6420    self.door_cmd 
+00004650: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+00004660: 2020 2020 2020 2073 656c 662e 636f 6d5f         self.com_
+00004670: 706f 7274 5f6f 626a 2e77 7269 7465 2862  port_obj.write(b
+00004680: 274d 4f44 454c 3f5c 7227 290a 2020 2020  'MODEL?\r').    
+00004690: 2020 2020 2020 2020 2020 2020 736c 6565              slee
+000046a0: 7028 302e 3129 0a20 2020 2020 2020 2020  p(0.1).         
+000046b0: 2020 2020 2020 206d 6f64 656c 203d 2073         model = s
+000046c0: 7472 2873 656c 662e 636f 6d5f 706f 7274  tr(self.com_port
+000046d0: 5f6f 626a 2e72 6561 6428 3134 2929 0a20  _obj.read(14)). 
+000046e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000046f0: 6172 7473 203d 205b 7020 666f 7220 7020  arts = [p for p 
+00004700: 696e 206d 6f64 656c 2e73 706c 6974 2822  in model.split("
+00004710: 2722 295d 0a20 2020 2020 2020 2020 2020  '")].           
+00004720: 2020 2020 2070 6172 7473 203d 205b 7020       parts = [p 
+00004730: 666f 7220 7020 696e 2070 6172 7473 5b31  for p in parts[1
+00004740: 5d2e 7370 6c69 7428 2220 2229 5d0a 2020  ].split(" ")].  
+00004750: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004760: 6c66 2e6d 6f64 656c 203d 2070 6172 7473  lf.model = parts
+00004770: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+00004780: 2020 2020 6966 206c 656e 2873 656c 662e      if len(self.
+00004790: 6d6f 6465 6c29 203e 2030 3a0a 2020 2020  model) > 0:.    
+000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047b0: 7072 696e 7428 2252 4620 6368 616d 6265  print("RF chambe
+000047c0: 7220 636f 6e6e 6563 7465 6420 746f 2070  r connected to p
+000047d0: 6f72 7420 2220 2b20 7374 7228 706f 7274  ort " + str(port
+000047e0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+000047f0: 2020 2020 2020 2070 7269 6e74 2822 5465         print("Te
+00004800: 7363 6f6d 202d 2043 6861 6d62 6572 206d  scom - Chamber m
+00004810: 6f64 656c 3a22 2c20 7365 6c66 2e6d 6f64  odel:", self.mod
+00004820: 656c 290a 2020 2020 2020 2020 2020 2020  el).            
+00004830: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00004840: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00004850: 696e 7428 2254 6573 636f 6d20 2d20 4572  int("Tescom - Er
+00004860: 726f 7221 204e 6f20 6368 616d 6265 7220  ror! No chamber 
+00004870: 666f 756e 6422 290a 2020 2020 2020 2020  found").        
+00004880: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00004890: 726e 0a20 2020 2020 2020 2020 2020 2020  rn.             
+000048a0: 2020 2069 6620 7365 6c66 2e6d 6f64 656c     if self.model
+000048b0: 2069 6e20 7365 6c66 2e6d 6f64 656c 735f   in self.models_
+000048c0: 6c69 7374 3a0a 2020 2020 2020 2020 2020  list:.          
+000048d0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+000048e0: 6f6f 725f 636d 6420 3d20 6227 444f 4f52  oor_cmd = b'DOOR
+000048f0: 3f5c 7227 0a20 2020 2020 2020 2020 2020  ?\r'.           
+00004900: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00004910: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004920: 656c 662e 646f 6f72 5f63 6d64 203d 2062  elf.door_cmd = b
+00004930: 274c 4944 3f5c 7227 0a20 2020 2020 2020  'LID?\r'.       
+00004940: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00004950: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00004960: 2045 7863 6570 7469 6f6e 0a20 2020 2020   Exception.     
+00004970: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00004980: 696f 6e20 6173 2065 3a0a 2020 2020 2020  ion as e:.      
+00004990: 2020 2020 2020 2320 7072 696e 7428 6529        # print(e)
+000049a0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+000049b0: 6e74 2828 2254 6573 636f 6d20 2d20 436f  nt(("Tescom - Co
+000049c0: 756c 6420 6e6f 7420 636f 6e6e 6563 7420  uld not connect 
+000049d0: 746f 2070 6f72 7420 2220 2b20 706f 7274  to port " + port
+000049e0: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
+000049f0: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
+00004a00: 6465 6620 636c 6f73 655f 706f 7274 2873  def close_port(s
+00004a10: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00004a20: 220a 2020 2020 2020 2020 636c 6f73 6573  ".        closes
+00004a30: 2063 6f6d 2070 6f72 740a 2020 2020 2020   com port.      
+00004a40: 2020 2222 220a 2020 2020 2020 2020 7472    """.        tr
+00004a50: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+00004a60: 656c 662e 636f 6d5f 706f 7274 5f6f 626a  elf.com_port_obj
+00004a70: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
+00004a80: 2020 2020 2070 7269 6e74 2822 5246 2063       print("RF c
+00004a90: 6861 6d62 6572 2064 6973 636f 6e6e 6563  hamber disconnec
+00004aa0: 7465 6420 6672 6f6d 2070 6f72 743a 2022  ted from port: "
+00004ab0: 202b 2073 7472 2873 656c 662e 706f 7274   + str(self.port
+00004ac0: 2929 0a20 2020 2020 2020 2065 7863 6570  )).        excep
+00004ad0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00004ae0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00004af0: 696e 7428 2243 6f75 6c64 206e 6f74 2064  int("Could not d
+00004b00: 6973 636f 6e6e 6563 7422 290a 0a20 2020  isconnect")..   
+00004b10: 2064 6566 206f 7065 6e5f 6368 616d 6265   def open_chambe
+00004b20: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
+00004b30: 2022 2222 0a20 2020 2020 2020 206f 7065   """.        ope
+00004b40: 6e73 2063 6861 6d62 6572 0a20 2020 2020  ns chamber.     
+00004b50: 2020 203a 7265 7475 726e 3a20 224f 4b22     :return: "OK"
+00004b60: 2069 6620 636f 6d6d 616e 6420 7761 7320   if command was 
+00004b70: 7375 6363 6573 7366 756c 0a20 2020 2020  successful.     
+00004b80: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00004b90: 6620 7365 6c66 2e69 735f 646f 6f72 5f6f  f self.is_door_o
+00004ba0: 7065 6e28 293a 0a20 2020 2020 2020 2020  pen():.         
+00004bb0: 2020 2070 7269 6e74 2822 4368 616d 6265     print("Chambe
+00004bc0: 7220 6973 206f 7065 6e22 290a 2020 2020  r is open").    
+00004bd0: 2020 2020 2020 2020 7265 7475 726e 2027          return '
+00004be0: 4f4b 270a 2020 2020 2020 2020 7472 793a  OK'.        try:
+00004bf0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00004c00: 6e74 2866 2243 6861 6d62 6572 207b 7365  nt(f"Chamber {se
+00004c10: 6c66 2e70 6f72 747d 2069 7320 6f70 656e  lf.port} is open
+00004c20: 696e 6722 290a 2020 2020 2020 2020 2020  ing").          
+00004c30: 2020 7365 6c66 2e63 6f6d 5f70 6f72 745f    self.com_port_
+00004c40: 6f62 6a2e 7265 7365 745f 696e 7075 745f  obj.reset_input_
+00004c50: 6275 6666 6572 2829 0a20 2020 2020 2020  buffer().       
+00004c60: 2020 2020 2073 656c 662e 636f 6d5f 706f       self.com_po
+00004c70: 7274 5f6f 626a 2e72 6573 6574 5f6f 7574  rt_obj.reset_out
+00004c80: 7075 745f 6275 6666 6572 2829 0a20 2020  put_buffer().   
+00004c90: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00004ca0: 6d5f 706f 7274 5f6f 626a 2e77 7269 7465  m_port_obj.write
+00004cb0: 2873 656c 662e 6f70 656e 5f63 6d64 290a  (self.open_cmd).
+00004cc0: 2020 2020 2020 2020 2020 2020 7265 7320              res 
+00004cd0: 3d20 2727 0a20 2020 2020 2020 2020 2020  = ''.           
+00004ce0: 2077 6169 745f 636f 756e 7465 7220 3d20   wait_counter = 
+00004cf0: 300a 2020 2020 2020 2020 2020 2020 7768  0.            wh
+00004d00: 696c 6520 274f 4b27 206e 6f74 2069 6e20  ile 'OK' not in 
+00004d10: 7265 733a 0a20 2020 2020 2020 2020 2020  res:.           
+00004d20: 2020 2020 2069 6620 7761 6974 5f63 6f75       if wait_cou
+00004d30: 6e74 6572 203e 3d20 3135 3a0a 2020 2020  nter >= 15:.    
+00004d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d50: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
+00004d60: 6622 4572 726f 7220 696e 206f 7065 6e69  f"Error in openi
+00004d70: 6e67 2063 6861 6d62 6572 207b 7365 6c66  ng chamber {self
+00004d80: 2e70 6f72 747d 2229 0a20 2020 2020 2020  .port}").       
+00004d90: 2020 2020 2020 2020 2072 6573 203d 2073           res = s
+00004da0: 656c 662e 636f 6d5f 706f 7274 5f6f 626a  elf.com_port_obj
+00004db0: 2e72 6561 6428 3134 292e 6465 636f 6465  .read(14).decode
+00004dc0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00004dd0: 2020 2020 2020 2775 7466 2d38 2729 2e75        'utf-8').u
+00004de0: 7070 6572 2829 2e72 7374 7269 7028 275c  pper().rstrip('\
+00004df0: 7227 290a 2020 2020 2020 2020 2020 2020  r').            
+00004e00: 2020 2020 6966 206c 656e 2873 7472 2872      if len(str(r
+00004e10: 6573 2929 203e 2030 3a0a 2020 2020 2020  es)) > 0:.      
+00004e20: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00004e30: 696e 7428 6627 4368 616d 6265 7220 7b73  int(f'Chamber {s
+00004e40: 656c 662e 706f 7274 7d20 7374 6174 7573  elf.port} status
+00004e50: 3a20 2720 2b20 7374 7228 7265 7329 290a  : ' + str(res)).
+00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e70: 7761 6974 5f63 6f75 6e74 6572 202b 3d20  wait_counter += 
+00004e80: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+00004e90: 2020 736c 6565 7028 302e 3129 0a20 2020    sleep(0.1).   
+00004ea0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00004eb0: 7365 6c66 2e69 735f 646f 6f72 5f6f 7065  self.is_door_ope
+00004ec0: 6e28 293a 0a20 2020 2020 2020 2020 2020  n():.           
+00004ed0: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
+00004ee0: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+00004ef0: 2020 2020 2020 2020 2020 6622 7b73 656c            f"{sel
+00004f00: 662e 706f 7274 7d20 446f 6f72 2073 7461  f.port} Door sta
+00004f10: 7475 7320 646f 6573 6e27 7420 6d61 7463  tus doesn't matc
+00004f20: 6820 636f 6d6d 616e 6420 7365 6e74 2122  h command sent!"
+00004f30: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+00004f40: 696e 7428 6622 4368 616d 6265 7220 7b73  int(f"Chamber {s
+00004f50: 656c 662e 706f 7274 7d20 6973 206f 7065  elf.port} is ope
+00004f60: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
+00004f70: 7265 7475 726e 2027 4f4b 270a 2020 2020  return 'OK'.    
+00004f80: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+00004f90: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
+00004fa0: 2020 2020 2020 2070 7269 6e74 2865 290a         print(e).
+00004fb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00004fc0: 726e 2022 4641 494c 220a 0a20 2020 2064  rn "FAIL"..    d
+00004fd0: 6566 2063 6c6f 7365 5f63 6861 6d62 6572  ef close_chamber
+00004fe0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00004ff0: 2222 220a 2020 2020 2020 2020 636c 6f73  """.        clos
+00005000: 6573 2063 6861 6d62 6572 0a20 2020 2020  es chamber.     
+00005010: 2020 203a 7265 7475 726e 3a20 224f 4b22     :return: "OK"
+00005020: 2069 6620 636f 6d6d 616e 6420 7761 7320   if command was 
+00005030: 7375 6363 6573 7366 756c 0a20 2020 2020  successful.     
+00005040: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00005050: 6620 7365 6c66 2e69 735f 646f 6f72 5f63  f self.is_door_c
+00005060: 6c6f 7365 6428 293a 0a20 2020 2020 2020  losed():.       
+00005070: 2020 2020 2070 7269 6e74 2822 4368 616d       print("Cham
+00005080: 6265 7220 636c 6f73 6564 2229 0a20 2020  ber closed").   
+00005090: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000050a0: 274f 4b27 0a20 2020 2020 2020 2074 7279  'OK'.        try
+000050b0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+000050c0: 696e 7428 6622 4348 414d 4245 5220 7b73  int(f"CHAMBER {s
+000050d0: 656c 662e 706f 7274 7d20 4953 2043 4c4f  elf.port} IS CLO
+000050e0: 5349 4e47 2c20 434c 4541 5220 4841 4e44  SING, CLEAR HAND
+000050f0: 5321 2121 2229 0a20 2020 2020 2020 2020  S!!!").         
+00005100: 2020 2073 6c65 6570 2832 290a 2020 2020     sleep(2).    
+00005110: 2020 2020 2020 2020 7365 6c66 2e63 6f6d          self.com
+00005120: 5f70 6f72 745f 6f62 6a2e 7772 6974 6528  _port_obj.write(
+00005130: 7365 6c66 2e63 6c6f 7365 5f63 6d64 290a  self.close_cmd).
+00005140: 2020 2020 2020 2020 2020 2020 7265 7320              res 
+00005150: 3d20 2727 0a20 2020 2020 2020 2020 2020  = ''.           
+00005160: 2077 6169 745f 636f 756e 7465 7220 3d20   wait_counter = 
+00005170: 300a 2020 2020 2020 2020 2020 2020 7768  0.            wh
+00005180: 696c 6520 2752 4541 4459 2720 6e6f 7420  ile 'READY' not 
+00005190: 696e 2072 6573 3a0a 2020 2020 2020 2020  in res:.        
+000051a0: 2020 2020 2020 2020 6966 2077 6169 745f          if wait_
+000051b0: 636f 756e 7465 7220 3e3d 2032 303a 0a20  counter >= 20:. 
+000051c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051d0: 2020 2072 6169 7365 2045 7863 6570 7469     raise Excepti
+000051e0: 6f6e 2866 2245 7272 6f72 2069 6e20 636c  on(f"Error in cl
+000051f0: 6f73 696e 6720 6368 616d 6265 7220 7b73  osing chamber {s
+00005200: 656c 662e 706f 7274 7d22 290a 2020 2020  elf.port}").    
+00005210: 2020 2020 2020 2020 2020 2020 7265 7320              res 
+00005220: 3d20 7365 6c66 2e63 6f6d 5f70 6f72 745f  = self.com_port_
+00005230: 6f62 6a2e 7265 6164 2831 3429 2e64 6563  obj.read(14).dec
+00005240: 6f64 6528 0a20 2020 2020 2020 2020 2020  ode(.           
+00005250: 2020 2020 2020 2020 2027 7574 662d 3827           'utf-8'
+00005260: 292e 7570 7065 7228 292e 7273 7472 6970  ).upper().rstrip
+00005270: 2827 5c72 2729 0a20 2020 2020 2020 2020  ('\r').         
+00005280: 2020 2020 2020 2069 6620 2745 5252 2720         if 'ERR' 
+00005290: 696e 2072 6573 206f 7220 2752 4541 4459  in res or 'READY
+000052a0: 2720 696e 2072 6573 206f 7220 274f 4b27  ' in res or 'OK'
+000052b0: 2069 6e20 7265 733a 0a20 2020 2020 2020   in res:.       
+000052c0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+000052d0: 6e74 2866 2743 6861 6d62 6572 207b 7365  nt(f'Chamber {se
+000052e0: 6c66 2e70 6f72 747d 2073 7461 7475 733a  lf.port} status:
+000052f0: 2027 202b 2073 7472 2872 6573 2929 0a20   ' + str(res)). 
+00005300: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00005310: 6620 2745 5252 2720 696e 2072 6573 3a0a  f 'ERR' in res:.
+00005320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005330: 2020 2020 7265 7475 726e 2022 4641 494c      return "FAIL
+00005340: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00005350: 2020 7761 6974 5f63 6f75 6e74 6572 202b    wait_counter +
+00005360: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
+00005370: 2020 2020 736c 6565 7028 302e 3129 0a20      sleep(0.1). 
+00005380: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00005390: 7420 7365 6c66 2e69 735f 646f 6f72 5f63  t self.is_door_c
+000053a0: 6c6f 7365 6428 293a 0a20 2020 2020 2020  losed():.       
+000053b0: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
+000053c0: 7863 6570 7469 6f6e 280a 2020 2020 2020  xception(.      
+000053d0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+000053e0: 7b73 656c 662e 706f 7274 7d20 446f 6f72  {self.port} Door
+000053f0: 2073 7461 7475 7320 646f 6573 6e27 7420   status doesn't 
+00005400: 6d61 7463 6820 636f 6d6d 616e 6420 7365  match command se
+00005410: 6e74 2122 290a 2020 2020 2020 2020 2020  nt!").          
+00005420: 2020 7072 696e 7428 6622 4368 616d 6265    print(f"Chambe
+00005430: 7220 7b73 656c 662e 706f 7274 7d20 636c  r {self.port} cl
+00005440: 6f73 6564 2229 0a20 2020 2020 2020 2020  osed").         
+00005450: 2020 2072 6574 7572 6e20 274f 4b27 0a20     return 'OK'. 
+00005460: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+00005470: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
+00005480: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00005490: 6622 4572 726f 7220 696e 2063 6c6f 7369  f"Error in closi
+000054a0: 6e67 2063 6861 6d62 6572 207b 7365 6c66  ng chamber {self
+000054b0: 2e70 6f72 747d 2229 0a20 2020 2020 2020  .port}").       
+000054c0: 2020 2020 2070 7269 6e74 2865 290a 2020       print(e).  
+000054d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000054e0: 2022 4641 494c 220a 0a20 2020 2064 6566   "FAIL"..    def
+000054f0: 2069 735f 636f 6e6e 6563 7465 6428 7365   is_connected(se
+00005500: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+00005510: 7365 6c66 2e63 6f6d 5f70 6f72 745f 6f62  self.com_port_ob
+00005520: 6a20 6973 204e 6f6e 653a 0a20 2020 2020  j is None:.     
+00005530: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00005540: 6c73 650a 2020 2020 2020 2020 7265 7475  lse.        retu
+00005550: 726e 2073 656c 662e 636f 6d5f 706f 7274  rn self.com_port
+00005560: 5f6f 626a 2e69 734f 7065 6e28 290a 0a20  _obj.isOpen().. 
+00005570: 2020 2064 6566 2067 6574 5f73 7461 7465     def get_state
+00005580: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00005590: 7365 6c66 2e63 6f6d 5f70 6f72 745f 6f62  self.com_port_ob
+000055a0: 6a2e 7265 7365 745f 696e 7075 745f 6275  j.reset_input_bu
+000055b0: 6666 6572 2829 0a20 2020 2020 2020 2073  ffer().        s
+000055c0: 6c65 6570 2830 2e31 290a 2020 2020 2020  leep(0.1).      
+000055d0: 2020 7365 6c66 2e63 6f6d 5f70 6f72 745f    self.com_port_
+000055e0: 6f62 6a2e 7772 6974 6528 7365 6c66 2e64  obj.write(self.d
+000055f0: 6f6f 725f 636d 6429 0a20 2020 2020 2020  oor_cmd).       
+00005600: 2073 6c65 6570 2830 2e31 290a 2020 2020   sleep(0.1).    
+00005610: 2020 2020 7374 6174 6520 3d20 7365 6c66      state = self
+00005620: 2e63 6f6d 5f70 6f72 745f 6f62 6a2e 7265  .com_port_obj.re
+00005630: 6164 2831 3429 2e64 6563 6f64 6528 2775  ad(14).decode('u
+00005640: 7466 2d38 2729 2e75 7070 6572 2829 2e72  tf-8').upper().r
+00005650: 7374 7269 7028 275c 7227 290a 2020 2020  strip('\r').    
+00005660: 2020 2020 7265 7475 726e 2073 7461 7465      return state
+00005670: 0a0a 2020 2020 6465 6620 6973 5f64 6f6f  ..    def is_doo
+00005680: 725f 6f70 656e 2873 656c 6629 3a0a 2020  r_open(self):.  
+00005690: 2020 2020 2020 7374 6174 6520 3d20 7365        state = se
+000056a0: 6c66 2e67 6574 5f73 7461 7465 2829 0a20  lf.get_state(). 
+000056b0: 2020 2020 2020 2069 6620 274f 5045 4e27         if 'OPEN'
+000056c0: 2069 6e20 7374 6174 653a 0a20 2020 2020   in state:.     
+000056d0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+000056e0: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
+000056f0: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
+00005700: 2069 735f 646f 6f72 5f63 6c6f 7365 6428   is_door_closed(
+00005710: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+00005720: 7461 7465 203d 2073 656c 662e 6765 745f  tate = self.get_
+00005730: 7374 6174 6528 290a 2020 2020 2020 2020  state().        
+00005740: 6966 2027 434c 4f53 4527 2069 6e20 7374  if 'CLOSE' in st
+00005750: 6174 653a 0a20 2020 2020 2020 2020 2020  ate:.           
+00005760: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+00005770: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00005780: 650a 0a0a 636c 6173 7320 4261 7263 6f64  e...class Barcod
+00005790: 6553 6361 6e6e 6572 286f 626a 6563 7429  eScanner(object)
+000057a0: 3a0a 2020 2020 7072 6566 6978 203d 2027  :.    prefix = '
+000057b0: 7e01 3030 3030 4027 0a20 2020 2073 7566  ~.0000@'.    suf
+000057c0: 6669 7820 3d20 273b 0327 0a20 2020 2063  fix = ';.'.    c
+000057d0: 6f6d 203d 2027 270a 2020 2020 7365 7269  om = ''.    seri
+000057e0: 616c 203d 204e 6f6e 650a 0a20 2020 2064  al = None..    d
+000057f0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00005800: 2c20 636f 6d3d 4e6f 6e65 2c20 6261 7564  , com=None, baud
+00005810: 3d31 3135 3230 302c 2063 6f6e 6669 673d  =115200, config=
+00005820: 5472 7565 2c20 6c6f 675f 7479 7065 3d27  True, log_type='
+00005830: 4e4f 5f4c 4f47 2729 3a0a 2020 2020 2020  NO_LOG'):.      
+00005840: 2020 7365 6c66 2e6c 6f67 5f74 7970 6520    self.log_type 
+00005850: 3d20 6c6f 675f 7479 7065 0a20 2020 2020  = log_type.     
+00005860: 2020 2069 6620 636f 6d20 213d 204e 6f6e     if com != Non
+00005870: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00005880: 656c 662e 6f70 656e 5f70 6f72 7428 636f  elf.open_port(co
+00005890: 6d2c 2062 6175 643d 6261 7564 2c20 636f  m, baud=baud, co
+000058a0: 6e66 6967 3d63 6f6e 6669 6729 0a20 2020  nfig=config).   
+000058b0: 2020 2020 2023 2065 6c73 653a 0a20 2020       # else:.   
+000058c0: 2020 2020 2023 2020 2020 2073 656c 662e       #     self.
+000058d0: 7365 7269 616c 203d 2073 6572 203d 2053  serial = ser = S
+000058e0: 6572 6961 6c28 290a 0a20 2020 2064 6566  erial()..    def
+000058f0: 206f 7065 6e5f 706f 7274 2873 656c 662c   open_port(self,
+00005900: 2063 6f6d 2c20 6261 7564 3d31 3135 3230   com, baud=11520
+00005910: 302c 2063 6f6e 6669 673d 5472 7565 293a  0, config=True):
+00005920: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00005930: 2e73 6572 6961 6c20 213d 204e 6f6e 6520  .serial != None 
+00005940: 616e 6420 7365 6c66 2e73 6572 6961 6c2e  and self.serial.
+00005950: 6973 5f6f 7065 6e28 293a 0a20 2020 2020  is_open():.     
+00005960: 2020 2020 2020 2073 656c 662e 7365 7269         self.seri
+00005970: 616c 2e63 6c6f 7365 506f 7274 2829 0a20  al.closePort(). 
+00005980: 2020 2020 2020 2073 656c 662e 7365 7269         self.seri
+00005990: 616c 203d 2073 6572 203d 2073 6572 6961  al = ser = seria
+000059a0: 6c2e 5365 7269 616c 2863 6f6d 2c20 6261  l.Serial(com, ba
+000059b0: 7564 2c20 7469 6d65 6f75 743d 302e 3529  ud, timeout=0.5)
+000059c0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000059d0: 7365 6c66 2e63 6865 636b 5f63 6f6d 5f70  self.check_com_p
+000059e0: 6f72 7428 293a 0a20 2020 2020 2020 2020  ort():.         
+000059f0: 2020 2070 7269 6e74 2866 277b 636f 6d7d     print(f'{com}
+00005a00: 2069 7320 6e6f 7420 6261 7263 6f64 6520   is not barcode 
+00005a10: 7363 616e 6e65 7227 290a 2020 2020 2020  scanner').      
+00005a20: 2020 6966 2073 6572 2021 3d20 4e6f 6e65    if ser != None
+00005a30: 2061 6e64 2073 656c 662e 6c6f 675f 7479   and self.log_ty
+00005a40: 7065 2021 3d20 274e 4f5f 4c4f 4727 3a0a  pe != 'NO_LOG':.
+00005a50: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00005a60: 7428 6627 4261 7263 6f64 6520 7363 616e  t(f'Barcode scan
+00005a70: 6e65 7220 287b 636f 6d7d 2920 636f 6e6e  ner ({com}) conn
+00005a80: 6563 7465 642e 2729 0a20 2020 2020 2020  ected.').       
+00005a90: 2065 6c69 6620 7365 7220 3d3d 204e 6f6e   elif ser == Non
+00005aa0: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+00005ab0: 7269 6e74 2866 2742 6172 636f 6465 2073  rint(f'Barcode s
+00005ac0: 6361 6e6e 6572 202d 2050 726f 626c 656d  canner - Problem
+00005ad0: 2063 6f6e 6e65 6374 696e 6720 7b63 6f6d   connecting {com
+00005ae0: 7d27 290a 2020 2020 2020 2020 7365 6c66  }').        self
+00005af0: 2e63 6f6d 203d 2063 6f6d 0a20 2020 2020  .com = com.     
+00005b00: 2020 2073 6572 2e74 696d 6572 6f75 7420     ser.timerout 
+00005b10: 3d20 3120 2023 2072 6561 6420 7469 6d65  = 1  # read time
+00005b20: 206f 7574 0a20 2020 2020 2020 2073 6572   out.        ser
+00005b30: 2e77 7269 7465 5469 6d65 6f75 7420 3d20  .writeTimeout = 
+00005b40: 302e 3520 2023 2077 7269 7465 2074 696d  0.5  # write tim
+00005b50: 6520 6f75 742e 0a20 2020 2020 2020 2069  e out..        i
+00005b60: 6620 636f 6e66 6967 3a0a 2020 2020 2020  f config:.      
+00005b70: 2020 2020 2020 7365 6c66 2e63 6f6e 6669        self.confi
+00005b80: 6775 7265 2829 0a0a 2020 2020 6465 6620  gure()..    def 
+00005b90: 6669 6e64 5f61 6e64 5f6f 7065 6e5f 706f  find_and_open_po
+00005ba0: 7274 2873 656c 662c 2062 6175 643d 3131  rt(self, baud=11
+00005bb0: 3532 3030 2c20 636f 6e66 6967 3d54 7275  5200, config=Tru
+00005bc0: 6529 3a0a 2020 2020 2020 2020 636f 6d20  e):.        com 
+00005bd0: 3d20 7365 6c66 2e66 696e 645f 636f 6d5f  = self.find_com_
+00005be0: 706f 7274 2862 6175 6429 0a20 2020 2020  port(baud).     
+00005bf0: 2020 2069 6620 636f 6d20 6973 206e 6f74     if com is not
+00005c00: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00005c10: 2020 2073 656c 662e 6f70 656e 5f70 6f72     self.open_por
+00005c20: 7428 636f 6d2c 2062 6175 642c 2063 6f6e  t(com, baud, con
+00005c30: 6669 6729 0a20 2020 2020 2020 2020 2020  fig).           
+00005c40: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+00005c50: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00005c60: 650a 0a20 2020 2064 6566 2066 696e 645f  e..    def find_
+00005c70: 636f 6d5f 706f 7274 2873 656c 662c 2062  com_port(self, b
+00005c80: 6175 643d 3131 3532 3030 293a 0a20 2020  aud=115200):.   
+00005c90: 2020 2020 2063 6f6d 506f 7274 7320 3d20       comPorts = 
+00005ca0: 7365 7269 616c 5f70 6f72 7473 2829 0a20  serial_ports(). 
+00005cb0: 2020 2020 2020 2063 6f6d 7320 3d20 5b5d         coms = []
+00005cc0: 0a20 2020 2020 2020 2066 6f72 2063 6f6d  .        for com
+00005cd0: 2069 6e20 636f 6d50 6f72 7473 3a0a 2020   in comPorts:.  
+00005ce0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00005cf0: 662e 6368 6563 6b5f 636f 6d5f 706f 7274  f.check_com_port
+00005d00: 2863 6f6d 2c20 6261 7564 293a 0a20 2020  (com, baud):.   
+00005d10: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
+00005d20: 732e 6170 7065 6e64 2863 6f6d 290a 2020  s.append(com).  
+00005d30: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00005d40: 206c 656e 2863 6f6d 7329 203e 2031 3a0a   len(coms) > 1:.
+00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d60: 2020 2020 7072 696e 7428 0a20 2020 2020      print(.     
+00005d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d80: 2020 2027 5761 726e 696e 6720 2d20 6d6f     'Warning - mo
+00005d90: 7265 2074 6861 6e20 6f6e 6520 6261 7263  re than one barc
+00005da0: 6f64 6520 7363 616e 6e65 7220 666f 756e  ode scanner foun
+00005db0: 642c 2075 7369 6e67 2074 6865 2066 6972  d, using the fir
+00005dc0: 7374 2062 6172 636f 6465 2073 6361 6e6e  st barcode scann
+00005dd0: 6572 2e27 290a 0a20 2020 2020 2020 2069  er.')..        i
+00005de0: 6620 6c65 6e28 636f 6d73 2920 3e20 303a  f len(coms) > 0:
+00005df0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00005e00: 7572 6e20 636f 6d73 5b30 5d0a 2020 2020  urn coms[0].    
+00005e10: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00005e20: 2020 2020 2020 7072 696e 7428 2745 7272        print('Err
+00005e30: 6f72 202d 2063 6f75 6c64 206e 6f74 2066  or - could not f
+00005e40: 696e 6420 6261 7263 6f64 6520 7363 616e  ind barcode scan
+00005e50: 6e65 722e 2729 0a20 2020 2020 2020 2020  ner.').         
+00005e60: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
+00005e70: 2020 2020 6465 6620 6368 6563 6b5f 636f      def check_co
+00005e80: 6d5f 706f 7274 2873 656c 662c 2063 6f6d  m_port(self, com
+00005e90: 3d4e 6f6e 652c 2062 6175 643d 3131 3532  =None, baud=1152
+00005ea0: 3030 293a 0a20 2020 2020 2020 2069 735f  00):.        is_
+00005eb0: 6261 725f 7363 616e 203d 2054 7275 650a  bar_scan = True.
+00005ec0: 2020 2020 2020 2020 636c 6f73 655f 706f          close_po
+00005ed0: 7274 203d 2046 616c 7365 0a20 2020 2020  rt = False.     
+00005ee0: 2020 2069 6620 6e6f 7420 7365 6c66 2e69     if not self.i
+00005ef0: 735f 6f70 656e 2829 2061 6e64 2063 6f6d  s_open() and com
+00005f00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00005f10: 2020 2020 2020 2020 2020 636c 6f73 655f            close_
+00005f20: 706f 7274 203d 2054 7275 650a 2020 2020  port = True.    
+00005f30: 2020 2020 2020 2020 7365 6c66 2e73 6572          self.ser
+00005f40: 6961 6c20 3d20 7365 7269 616c 2e53 6572  ial = serial.Ser
+00005f50: 6961 6c28 636f 6d2c 2062 6175 642c 2074  ial(com, baud, t
+00005f60: 696d 656f 7574 3d30 2e35 290a 2020 2020  imeout=0.5).    
+00005f70: 2020 2020 656c 6966 206e 6f74 2073 656c      elif not sel
+00005f80: 662e 6973 5f6f 7065 6e28 293a 0a20 2020  f.is_open():.   
+00005f90: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+00005fa0: 4261 7263 6f64 6553 6361 6e6e 6572 202d  BarcodeScanner -
+00005fb0: 2063 6865 636b 5f63 6f6d 5f70 6f72 743a   check_com_port:
+00005fc0: 204d 6973 7369 6e67 2063 6f6d 2070 6f72   Missing com por
+00005fd0: 7427 290a 2020 2020 2020 2020 2020 2020  t').            
+00005fe0: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
+00005ff0: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
+00006000: 6d61 6e75 616c 5f63 6f6e 6669 6775 7265  manual_configure
+00006010: 285b 2751 5259 5044 4e27 5d29 0a20 2020  (['QRYPDN']).   
+00006020: 2020 2020 2069 6620 6e6f 7420 274e 4c53       if not 'NLS
+00006030: 2d4e 3127 2069 6e20 7374 7228 7265 7329  -N1' in str(res)
+00006040: 3a0a 2020 2020 2020 2020 2020 2020 6973  :.            is
+00006050: 5f62 6172 5f73 6361 6e20 3d20 4661 6c73  _bar_scan = Fals
+00006060: 650a 2020 2020 2020 2020 6966 2063 6c6f  e.        if clo
+00006070: 7365 5f70 6f72 743a 0a20 2020 2020 2020  se_port:.       
+00006080: 2020 2020 2073 656c 662e 7365 7269 616c       self.serial
+00006090: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
+000060a0: 2020 2020 2073 656c 662e 7365 7269 616c       self.serial
+000060b0: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
+000060c0: 2072 6574 7572 6e20 6973 5f62 6172 5f73   return is_bar_s
+000060d0: 6361 6e0a 0a20 2020 2064 6566 2063 6c6f  can..    def clo
+000060e0: 7365 5f70 6f72 7428 7365 6c66 293a 0a20  se_port(self):. 
+000060f0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00006100: 6572 6961 6c2e 6973 4f70 656e 2829 3a0a  erial.isOpen():.
+00006110: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006120: 2e73 6572 6961 6c2e 636c 6f73 6528 290a  .serial.close().
+00006130: 0a20 2020 2064 6566 2069 735f 6f70 656e  .    def is_open
+00006140: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00006150: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00006160: 2072 6573 203d 2073 656c 662e 6d61 6e75   res = self.manu
+00006170: 616c 5f63 6f6e 6669 6775 7265 285b 2751  al_configure(['Q
+00006180: 5259 5044 4e27 5d29 0a20 2020 2020 2020  RYPDN']).       
+00006190: 2020 2020 2069 6620 274e 4c53 2d4e 3127       if 'NLS-N1'
+000061a0: 2069 6e20 7374 7228 7265 7329 3a0a 2020   in str(res):.  
+000061b0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000061c0: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+000061d0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+000061e0: 7365 0a20 2020 2020 2020 2065 7863 6570  se.        excep
+000061f0: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
+00006200: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+00006210: 2064 6566 2063 6f6e 6669 6775 7265 2873   def configure(s
+00006220: 656c 662c 2069 6c6c 5363 6e3d 2731 272c  elf, illScn='1',
+00006230: 2061 6d6c 456e 613d 2730 272c 2067 7262   amlEna='0', grb
+00006240: 456e 613d 2730 272c 2067 7262 566c 6c3d  Ena='0', grbVll=
+00006250: 2732 272c 2061 7473 456e 613d 2730 272c  '2', atsEna='0',
+00006260: 2061 7473 4475 723d 2733 3630 3030 272c   atsDur='36000',
+00006270: 2073 636e 4d6f 643d 2730 272c 0a20 2020   scnMod='0',.   
+00006280: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00006290: 7762 456e 613d 2730 2729 3a0a 2020 2020  wbEna='0'):.    
+000062a0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+000062b0: 696c 6c53 636e 202d 2069 6c6c 756d 696e  illScn - illumin
+000062c0: 6174 696f 6e3a 2020 2020 302d 6f66 662c  ation:    0-off,
+000062d0: 2031 2d6e 6f72 6d61 6c2c 2032 2d61 6c77   1-normal, 2-alw
+000062e0: 6179 7320 6f6e 0a20 2020 2020 2020 2061  ays on.        a
+000062f0: 6d6c 456e 6120 2d20 6169 6d69 6e67 3a20  mlEna - aiming: 
+00006300: 2020 2020 2020 2020 2030 2d6f 6666 2c20           0-off, 
+00006310: 312d 6e6f 726d 616c 2c20 322d 616c 7761  1-normal, 2-alwa
+00006320: 7973 206f 6e0a 2020 2020 2020 2020 7077  ys on.        pw
+00006330: 6245 6e61 202d 2070 6f77 6572 206f 6e20  bEna - power on 
+00006340: 6265 6570 2020 2020 302d 6f66 662c 2031  beep    0-off, 1
+00006350: 2d6f 6e0a 2020 2020 2020 2020 6772 6245  -on.        grbE
+00006360: 6e61 202d 2067 6f6f 6420 7265 6164 2062  na - good read b
+00006370: 6565 7020 2020 302d 6f66 662c 2031 2d6f  eep   0-off, 1-o
+00006380: 6e0a 2020 2020 2020 2020 6174 7345 6e61  n.        atsEna
+00006390: 202d 2061 7574 6f20 736c 6565 7020 2020   - auto sleep   
+000063a0: 2020 2020 302d 6469 7361 626c 652c 2031      0-disable, 1
+000063b0: 2d65 6e61 626c 650a 2020 2020 2020 2020  -enable.        
+000063c0: 6174 7344 7572 202d 2073 6c65 6570 2064  atsDur - sleep d
+000063d0: 7572 6174 696f 6e20 2020 312d 3336 3030  uration   1-3600
+000063e0: 3020 5b73 6563 5d0a 2020 2020 2020 2020  0 [sec].        
+000063f0: 7363 6e4d 6f64 202d 2073 6361 6e20 6d6f  scnMod - scan mo
+00006400: 6465 2020 2020 2020 2020 302d 6c65 7665  de        0-leve
+00006410: 6c20 6d6f 6465 2c20 322d 7365 6e73 6520  l mode, 2-sense 
+00006420: 6d6f 6465 2c20 332d 636f 6e74 696e 756f  mode, 3-continuo
+00006430: 7573 206d 6f64 652c 2037 2d62 6174 6368  us mode, 7-batch
+00006440: 206d 6f64 650a 2020 2020 2020 2020 2727   mode.        ''
+00006450: 270a 2020 2020 2020 2020 736c 6565 7028  '.        sleep(
+00006460: 302e 3129 0a20 2020 2020 2020 2070 6172  0.1).        par
+00006470: 616d 7320 3d20 7b27 494c 4c53 434e 273a  ams = {'ILLSCN':
+00006480: 2069 6c6c 5363 6e2c 2027 414d 4c45 4e41   illScn, 'AMLENA
+00006490: 273a 2061 6d6c 456e 612c 2027 4752 4245  ': amlEna, 'GRBE
+000064a0: 4e41 273a 2067 7262 456e 612c 2027 4154  NA': grbEna, 'AT
+000064b0: 5345 4e41 273a 2061 7473 456e 612c 0a20  SENA': atsEna,. 
+000064c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064d0: 2027 4752 4256 4c4c 273a 2067 7262 566c   'GRBVLL': grbVl
+000064e0: 6c2c 2027 4154 5344 5552 273a 2061 7473  l, 'ATSDUR': ats
+000064f0: 4475 722c 2027 5343 4e4d 4f44 273a 2073  Dur, 'SCNMOD': s
+00006500: 636e 4d6f 642c 2027 5057 4245 4e41 273a  cnMod, 'PWBENA':
+00006510: 2070 7762 456e 617d 0a20 2020 2020 2020   pwbEna}.       
+00006520: 2070 6172 616d 7320 3d20 5b6b 6579 202b   params = [key +
+00006530: 2076 616c 7565 2066 6f72 206b 6579 2c20   value for key, 
+00006540: 7661 6c75 6520 696e 2070 6172 616d 732e  value in params.
+00006550: 6974 656d 7328 295d 0a20 2020 2020 2020  items()].       
+00006560: 2074 2c20 6973 5375 6363 6573 7320 3d20   t, isSuccess = 
+00006570: 7365 6c66 2e6d 616e 7561 6c5f 636f 6e66  self.manual_conf
+00006580: 6967 7572 6528 7061 7261 6d73 290a 2020  igure(params).  
+00006590: 2020 2020 2020 6966 2069 7353 7563 6365        if isSucce
+000065a0: 7373 2061 6e64 2073 656c 662e 6c6f 675f  ss and self.log_
+000065b0: 7479 7065 2021 3d20 274e 4f5f 4c4f 4727  type != 'NO_LOG'
+000065c0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+000065d0: 696e 7428 6627 4261 7263 6f64 6520 7363  int(f'Barcode sc
+000065e0: 616e 6e65 7220 287b 7365 6c66 2e63 6f6d  anner ({self.com
+000065f0: 7d29 2063 6f6e 6669 6775 7265 6420 7375  }) configured su
+00006600: 6363 6573 7366 756c 6c79 2e27 290a 2020  ccessfully.').  
+00006610: 2020 2020 2020 656c 6966 206e 6f74 2069        elif not i
+00006620: 7353 7563 6365 7373 3a0a 2020 2020 2020  sSuccess:.      
+00006630: 2020 2020 2020 7072 696e 7428 6627 4261        print(f'Ba
+00006640: 7263 6f64 6520 7363 616e 6e65 7220 287b  rcode scanner ({
+00006650: 7365 6c66 2e63 6f6d 7d29 2063 6f6e 6669  self.com}) confi
+00006660: 6775 7261 7469 6f6e 2066 6169 6c65 642e  guration failed.
+00006670: 2729 0a0a 2020 2020 6465 6620 7265 7374  ')..    def rest
+00006680: 6f72 655f 616c 6c5f 6661 6374 6f72 795f  ore_all_factory_
+00006690: 6465 6661 756c 7473 2873 656c 6629 3a0a  defaults(self):.
+000066a0: 2020 2020 2020 2020 736c 6565 7028 302e          sleep(0.
+000066b0: 3129 0a20 2020 2020 2020 2070 6172 616d  1).        param
+000066c0: 7320 3d20 7b27 4641 4344 4546 273a 2027  s = {'FACDEF': '
+000066d0: 277d 0a20 2020 2020 2020 2070 6172 616d  '}.        param
+000066e0: 7320 3d20 5b6b 6579 202b 2076 616c 7565  s = [key + value
+000066f0: 2066 6f72 206b 6579 2c20 7661 6c75 6520   for key, value 
+00006700: 696e 2070 6172 616d 732e 6974 656d 7328  in params.items(
+00006710: 295d 0a20 2020 2020 2020 2074 2c20 6973  )].        t, is
+00006720: 5375 6363 6573 7320 3d20 7365 6c66 2e6d  Success = self.m
+00006730: 616e 7561 6c5f 636f 6e66 6967 7572 6528  anual_configure(
+00006740: 7061 7261 6d73 290a 2020 2020 2020 2020  params).        
+00006750: 6966 2069 7353 7563 6365 7373 2061 6e64  if isSuccess and
+00006760: 2073 656c 662e 6c6f 675f 7479 7065 2021   self.log_type !
+00006770: 3d20 274e 4f5f 4c4f 4727 3a0a 2020 2020  = 'NO_LOG':.    
+00006780: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
+00006790: 4261 7263 6f64 6520 7363 616e 6e65 7220  Barcode scanner 
+000067a0: 287b 7365 6c66 2e63 6f6d 7d29 2072 6573  ({self.com}) res
+000067b0: 746f 7265 6420 6661 6374 6f72 7920 6465  tored factory de
+000067c0: 6661 756c 7420 7375 6363 6573 7366 756c  fault successful
+000067d0: 6c79 2e27 290a 2020 2020 2020 2020 656c  ly.').        el
+000067e0: 6966 206e 6f74 2069 7353 7563 6365 7373  if not isSuccess
+000067f0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00006800: 696e 7428 6627 4261 7263 6f64 6520 7363  int(f'Barcode sc
+00006810: 616e 6e65 7220 287b 7365 6c66 2e63 6f6d  anner ({self.com
+00006820: 7d29 2072 6573 746f 7265 6420 6661 6374  }) restored fact
+00006830: 6f72 7920 6465 6661 756c 7420 6661 696c  ory default fail
+00006840: 6564 2e27 290a 0a20 2020 2064 6566 206d  ed.')..    def m
+00006850: 616e 7561 6c5f 636f 6e66 6967 7572 6528  anual_configure(
+00006860: 7365 6c66 2c20 7061 7261 6d73 293a 0a20  self, params):. 
+00006870: 2020 2020 2020 2073 6c65 6570 2830 2e31         sleep(0.1
+00006880: 290a 2020 2020 2020 2020 636f 6e66 6967  ).        config
+00006890: 7320 3d20 7365 6c66 2e70 7265 6669 7820  s = self.prefix 
+000068a0: 2b20 273b 272e 6a6f 696e 2870 6172 616d  + ';'.join(param
+000068b0: 7329 202b 2073 656c 662e 7375 6666 6978  s) + self.suffix
+000068c0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+000068d0: 7269 616c 2e66 6c75 7368 496e 7075 7428  rial.flushInput(
+000068e0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+000068f0: 6572 6961 6c2e 666c 7573 684f 7574 7075  erial.flushOutpu
+00006900: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+00006910: 2e73 6572 6961 6c2e 7772 6974 6528 7374  .serial.write(st
+00006920: 722e 656e 636f 6465 2863 6f6e 6669 6773  r.encode(configs
+00006930: 2929 0a20 2020 2020 2020 2073 6c65 6570  )).        sleep
+00006940: 2830 2e31 290a 2020 2020 2020 2020 742c  (0.1).        t,
+00006950: 2069 7353 7563 6365 7373 203d 2073 656c   isSuccess = sel
+00006960: 662e 7472 6967 6765 725f 7374 6f70 5f73  f.trigger_stop_s
+00006970: 6574 7469 6e67 7328 290a 2020 2020 2020  ettings().      
+00006980: 2020 2320 7072 696e 7428 7429 0a20 2020    # print(t).   
+00006990: 2020 2020 2072 6574 7572 6e20 742c 2069       return t, i
+000069a0: 7353 7563 6365 7373 0a0a 2020 2020 6465  sSuccess..    de
+000069b0: 6620 7363 616e 2873 656c 6629 3a0a 2020  f scan(self):.  
+000069c0: 2020 2020 2020 2320 7072 696e 7428 2261        # print("a
+000069d0: 6e61 6c6f 675f 7472 6967 6765 725f 7365  nalog_trigger_se
+000069e0: 7474 696e 6722 290a 2020 2020 2020 2020  tting").        
+000069f0: 7365 6c66 2e73 6572 6961 6c2e 7772 6974  self.serial.writ
+00006a00: 6528 6222 5c78 3162 5c78 3331 2229 0a20  e(b"\x1b\x31"). 
+00006a10: 2020 2020 2020 2073 6c65 6570 2830 2e31         sleep(0.1
+00006a20: 290a 2020 2020 2020 2020 2320 7420 3d20  ).        # t = 
+00006a30: 7365 722e 7265 6164 2873 6572 2e69 6e5f  ser.read(ser.in_
+00006a40: 7761 6974 696e 6729 0a20 2020 2020 2020  waiting).       
+00006a50: 2074 203d 2073 656c 662e 7365 7269 616c   t = self.serial
+00006a60: 2e72 6561 645f 616c 6c28 290a 2020 2020  .read_all().    
+00006a70: 2020 2020 2320 7072 696e 7428 7429 0a20      # print(t). 
+00006a80: 2020 2020 2020 2072 6574 7572 6e20 740a         return t.
+00006a90: 0a20 2020 2064 6566 2073 6361 6e5f 616e  .    def scan_an
+00006aa0: 645f 666c 7573 6828 7365 6c66 293a 0a20  d_flush(self):. 
+00006ab0: 2020 2020 2020 2073 656c 662e 7365 7269         self.seri
+00006ac0: 616c 2e66 6c75 7368 496e 7075 7428 290a  al.flushInput().
+00006ad0: 2020 2020 2020 2020 7365 6c66 2e73 6572          self.ser
+00006ae0: 6961 6c2e 666c 7573 684f 7574 7075 7428  ial.flushOutput(
+00006af0: 290a 2020 2020 2020 2020 7420 3d20 7365  ).        t = se
+00006b00: 6c66 2e73 6361 6e28 290a 2020 2020 2020  lf.scan().      
+00006b10: 2020 7365 6c66 2e73 6572 6961 6c2e 666c    self.serial.fl
+00006b20: 7573 6849 6e70 7574 2829 0a20 2020 2020  ushInput().     
+00006b30: 2020 2073 656c 662e 7365 7269 616c 2e66     self.serial.f
+00006b40: 6c75 7368 4f75 7470 7574 2829 0a20 2020  lushOutput().   
+00006b50: 2020 2020 2074 436c 6561 6e20 3d20 7374       tClean = st
+00006b60: 7228 7429 2e73 706c 6974 2827 5c5c 7827  r(t).split('\\x'
+00006b70: 295b 2d31 5d0a 2020 2020 2020 2020 6966  )[-1].        if
+00006b80: 2074 436c 6561 6e2e 7374 6172 7473 7769   tClean.startswi
+00006b90: 7468 2827 3036 2729 3a0a 2020 2020 2020  th('06'):.      
+00006ba0: 2020 2020 2020 7443 6c65 616e 203d 2074        tClean = t
+00006bb0: 436c 6561 6e5b 323a 5d0a 2020 2020 2020  Clean[2:].      
+00006bc0: 2020 2020 2020 7443 6c65 616e 203d 2074        tClean = t
+00006bd0: 436c 6561 6e2e 7374 7269 7028 2227 5c5c  Clean.strip("'\\
+00006be0: 6e5c 5c72 2229 0a20 2020 2020 2020 2020  n\\r").         
+00006bf0: 2020 2074 436c 6561 6e20 3d20 7443 6c65     tClean = tCle
+00006c00: 616e 2e73 706c 6974 2827 5c5c 6e27 295b  an.split('\\n')[
+00006c10: 2d31 5d0a 2020 2020 2020 2020 2020 2020  -1].            
+00006c20: 7443 6c65 616e 203d 2074 436c 6561 6e2e  tClean = tClean.
+00006c30: 7370 6c69 7428 275c 5c72 2729 5b2d 315d  split('\\r')[-1]
+00006c40: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00006c50: 7572 6e20 7443 6c65 616e 0a20 2020 2020  urn tClean.     
+00006c60: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00006c70: 2020 2020 2070 7269 6e74 2827 5761 726e       print('Warn
+00006c80: 696e 6720 2d20 6e6f 7420 7265 6365 6976  ing - not receiv
+00006c90: 6564 2041 434b 2066 726f 6d20 6261 7263  ed ACK from barc
+00006ca0: 6f64 6520 7363 616e 6e65 722e 2729 0a20  ode scanner.'). 
+00006cb0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00006cc0: 6e20 7374 7228 7429 2e73 706c 6974 2827  n str(t).split('
+00006cd0: 5c5c 7827 295b 2d31 5d0a 0a20 2020 2064  \\x')[-1]..    d
+00006ce0: 6566 2073 6361 6e5f 6578 745f 6964 2873  ef scan_ext_id(s
+00006cf0: 656c 662c 2073 6361 6e44 7572 3d30 2e35  elf, scanDur=0.5
+00006d00: 2c20 5661 6c69 6461 7465 436e 743d 3329  , ValidateCnt=3)
+00006d10: 3a0a 2020 2020 2020 2020 6261 7263 6f64  :.        barcod
+00006d20: 6552 6561 6420 3d20 2727 0a20 2020 2020  eRead = ''.     
+00006d30: 2020 2062 6172 636f 6465 7320 3d20 5b5d     barcodes = []
+00006d40: 0a20 2020 2020 2020 2073 7461 7274 5469  .        startTi
+00006d50: 6d65 203d 2074 696d 6528 290a 2020 2020  me = time().    
+00006d60: 2020 2020 7768 696c 6520 2828 7469 6d65      while ((time
+00006d70: 2829 202d 2073 7461 7274 5469 6d65 2920  () - startTime) 
+00006d80: 3c20 7363 616e 4475 7229 3a0a 2020 2020  < scanDur):.    
+00006d90: 2020 2020 2020 2020 6261 7263 6f64 6552          barcodeR
+00006da0: 6561 6420 3d20 7365 6c66 2e73 6361 6e5f  ead = self.scan_
+00006db0: 616e 645f 666c 7573 6828 290a 2020 2020  and_flush().    
+00006dc0: 2020 2020 2020 2020 2320 6261 7263 6f64          # barcod
+00006dd0: 6552 6561 6420 3d20 7374 7228 7429 0a20  eRead = str(t). 
+00006de0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00006df0: 6e28 6261 7263 6f64 6552 6561 6429 203c  n(barcodeRead) <
+00006e00: 2038 3a0a 2020 2020 2020 2020 2020 2020   8:.            
+00006e10: 2020 2020 6261 7263 6f64 6552 6561 6420      barcodeRead 
+00006e20: 3d20 2727 0a20 2020 2020 2020 2020 2020  = ''.           
+00006e30: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
+00006e40: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00006e50: 6e28 6261 7263 6f64 6573 2920 3c20 5661  n(barcodes) < Va
+00006e60: 6c69 6461 7465 436e 743a 0a20 2020 2020  lidateCnt:.     
+00006e70: 2020 2020 2020 2020 2020 2062 6172 636f             barco
+00006e80: 6465 732e 6170 7065 6e64 2862 6172 636f  des.append(barco
+00006e90: 6465 5265 6164 290a 2020 2020 2020 2020  deRead).        
+00006ea0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00006eb0: 0a0a 2020 2020 2020 2020 2020 2020 6261  ..            ba
+00006ec0: 7263 6f64 6552 6561 6420 3d20 6d6f 6465  rcodeRead = mode
+00006ed0: 2862 6172 636f 6465 7329 0a20 2020 2020  (barcodes).     
+00006ee0: 2020 2020 2020 2066 756c 6c44 6174 6120         fullData 
+00006ef0: 3d20 6375 7249 6420 3d20 7265 656c 4964  = curId = reelId
+00006f00: 203d 2067 7469 6e20 3d20 6261 7263 6f64   = gtin = barcod
+00006f10: 6552 6561 640a 2020 2020 2020 2020 2020  eRead.          
+00006f20: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00006f30: 2020 2020 2020 2069 6620 2729 2720 696e         if ')' in
+00006f40: 2066 756c 6c44 6174 613a 0a20 2020 2020   fullData:.     
+00006f50: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00006f60: 7469 6e20 3d20 2729 272e 6a6f 696e 2866  tin = ')'.join(f
+00006f70: 756c 6c44 6174 612e 7370 6c69 7428 2729  ullData.split(')
+00006f80: 2729 5b3a 325d 2920 2b20 2729 270a 2020  ')[:2]) + ')'.  
+00006f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fa0: 2020 7461 6744 6174 6120 3d20 6675 6c6c    tagData = full
+00006fb0: 4461 7461 2e73 706c 6974 2827 2927 295b  Data.split(')')[
+00006fc0: 325d 0a20 2020 2020 2020 2020 2020 2020  2].             
+00006fd0: 2020 2065 6c73 653a 2020 2320 6774 696e     else:  # gtin
+00006fe0: 2077 6974 686f 7574 2070 6172 656e 7468   without parenth
+00006ff0: 6573 6973 0a20 2020 2020 2020 2020 2020  esis.           
+00007000: 2020 2020 2020 2020 2067 7469 6e20 3d20           gtin = 
+00007010: 6675 6c6c 4461 7461 5b30 3a31 385d 0a20  fullData[0:18]. 
+00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007030: 2020 2074 6167 4461 7461 203d 2066 756c     tagData = ful
+00007040: 6c44 6174 615b 3138 3a5d 0a20 2020 2020  lData[18:].     
+00007050: 2020 2020 2020 2020 2020 2063 7572 4964             curId
+00007060: 203d 2074 6167 4461 7461 2e73 706c 6974   = tagData.split
+00007070: 2827 5427 295b 315d 2e73 7472 6970 2822  ('T')[1].strip("
+00007080: 2720 2229 2e73 706c 6974 2827 2827 295b  ' ").split('(')[
+00007090: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
+000070a0: 2020 2072 6565 6c49 6420 3d20 7461 6744     reelId = tagD
+000070b0: 6174 612e 7370 6c69 7428 2754 2729 5b30  ata.split('T')[0
+000070c0: 5d2e 7374 7269 7028 2227 2022 290a 2020  ].strip("' ").  
+000070d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000070e0: 7475 726e 2066 756c 6c44 6174 612c 2063  turn fullData, c
+000070f0: 7572 4964 2c20 7265 656c 4964 2c20 6774  urId, reelId, gt
+00007100: 696e 0a20 2020 2020 2020 2020 2020 2065  in.            e
+00007110: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
+00007120: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+00007130: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00007140: 6675 6c6c 4461 7461 2c20 6375 7249 642c  fullData, curId,
+00007150: 2072 6565 6c49 642c 2067 7469 6e0a 0a20   reelId, gtin.. 
+00007160: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00007170: 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20  ne, None, None, 
+00007180: 4e6f 6e65 0a0a 2020 2020 6465 6620 6175  None..    def au
+00007190: 746f 5f73 6361 6e28 7365 6c66 293a 0a20  to_scan(self):. 
+000071a0: 2020 2020 2020 2023 2070 7269 6e74 2822         # print("
+000071b0: 4175 746f 6d61 7469 6320 7265 6164 696e  Automatic readin
+000071c0: 6720 7365 7474 696e 6773 2229 0a20 2020  g settings").   
+000071d0: 2020 2020 2073 656c 662e 7365 7269 616c       self.serial
+000071e0: 2e77 7269 7465 2862 225c 7831 625c 7833  .write(b"\x1b\x3
+000071f0: 3222 290a 2020 2020 2020 2020 736c 6565  2").        slee
+00007200: 7028 302e 3129 0a20 2020 2020 2020 2074  p(0.1).        t
+00007210: 203d 2073 656c 662e 7365 7269 616c 2e72   = self.serial.r
+00007220: 6561 645f 616c 6c28 290a 2020 2020 2020  ead_all().      
+00007230: 2020 2320 7072 696e 7428 7429 0a20 2020    # print(t).   
+00007240: 2020 2020 2072 6574 7572 6e20 740a 0a20       return t.. 
+00007250: 2020 2064 6566 2074 7269 6767 6572 5f73     def trigger_s
+00007260: 746f 705f 7365 7474 696e 6773 2873 656c  top_settings(sel
+00007270: 6629 3a0a 2020 2020 2020 2020 2320 7072  f):.        # pr
+00007280: 696e 7428 2254 7269 6767 6572 5f73 746f  int("Trigger_sto
+00007290: 705f 7365 7474 696e 6773 2229 0a20 2020  p_settings").   
+000072a0: 2020 2020 2023 2073 6c65 6570 2830 2e31       # sleep(0.1
+000072b0: 290a 2020 2020 2020 2020 2320 7420 3d20  ).        # t = 
+000072c0: 7365 722e 7265 6164 2873 6572 2e69 6e5f  ser.read(ser.in_
+000072d0: 7761 6974 696e 6729 0a20 2020 2020 2020  waiting).       
+000072e0: 2073 6c65 6570 2830 2e31 290a 2020 2020   sleep(0.1).    
+000072f0: 2020 2020 7420 3d20 7365 6c66 2e73 6572      t = self.ser
+00007300: 6961 6c2e 7265 6164 5f61 6c6c 2829 0a20  ial.read_all(). 
+00007310: 2020 2020 2020 2073 6c65 6570 2830 2e31         sleep(0.1
+00007320: 290a 2020 2020 2020 2020 2320 7072 696e  ).        # prin
+00007330: 7428 7429 0a20 2020 2020 2020 2061 636b  t(t).        ack
+00007340: 7320 3d20 7374 7228 7429 2e73 706c 6974  s = str(t).split
+00007350: 2827 3b27 295b 3a2d 315d 0a20 2020 2020  (';')[:-1].     
+00007360: 2020 2069 7353 7563 6365 7373 203d 2061     isSuccess = a
+00007370: 6c6c 285b 5472 7565 2069 6620 6163 6b2e  ll([True if ack.
+00007380: 656e 6473 7769 7468 2827 5c5c 7830 3627  endswith('\\x06'
+00007390: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000073a0: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
+000073b0: 4661 6c73 6520 666f 7220 6163 6b20 696e  False for ack in
+000073c0: 2061 636b 735d 290a 2020 2020 2020 2020   acks]).        
+000073d0: 7265 7475 726e 2074 2c20 6973 5375 6363  return t, isSucc
+000073e0: 6573 730a 0a0a 636c 6173 7320 596f 6374  ess...class Yoct
+000073f0: 6f54 656d 7065 7261 7475 7265 5365 6e73  oTemperatureSens
+00007400: 6f72 286f 626a 6563 7429 3a0a 2020 2020  or(object):.    
+00007410: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00007420: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+00007430: 2e73 656e 736f 7220 3d20 4e6f 6e65 0a20  .sensor = None. 
+00007440: 2020 2020 2020 2065 7272 6d73 6720 3d20         errmsg = 
+00007450: 5952 6566 5061 7261 6d28 290a 2020 2020  YRefParam().    
+00007460: 2020 2020 2320 5365 7475 7020 7468 6520      # Setup the 
+00007470: 4150 4920 746f 2075 7365 206c 6f63 616c  API to use local
+00007480: 2055 5342 2064 6576 6963 6573 0a20 2020   USB devices.   
+00007490: 2020 2020 2069 6620 5941 5049 2e52 6567       if YAPI.Reg
+000074a0: 6973 7465 7248 7562 2822 7573 6222 2c20  isterHub("usb", 
+000074b0: 6572 726d 7367 2920 213d 2059 4150 492e  errmsg) != YAPI.
+000074c0: 5355 4343 4553 533a 0a20 2020 2020 2020  SUCCESS:.       
+000074d0: 2020 2020 2072 6169 7365 2045 7175 6970       raise Equip
+000074e0: 6d65 6e74 4572 726f 7228 2779 6f63 746f  mentError('yocto
+000074f0: 2074 656d 7065 7261 7475 7265 2073 656e   temperature sen
+00007500: 736f 7220 676f 7420 696e 6974 2065 7272  sor got init err
+00007510: 6f72 3a20 7b7d 272e 666f 726d 6174 2865  or: {}'.format(e
+00007520: 7272 6d73 672e 7661 6c75 6529 290a 0a20  rrmsg.value)).. 
+00007530: 2020 2064 6566 2063 6f6e 6e65 6374 2873     def connect(s
+00007540: 656c 662c 2074 6172 6765 743d 2761 6e79  elf, target='any
+00007550: 2729 3a0a 2020 2020 2020 2020 6966 2074  '):.        if t
+00007560: 6172 6765 7420 3d3d 2027 616e 7927 3a0a  arget == 'any':.
+00007570: 2020 2020 2020 2020 2020 2020 2320 7265              # re
+00007580: 7472 6965 7665 2061 6e79 2074 656d 7065  trieve any tempe
+00007590: 7261 7475 7265 2073 656e 736f 720a 2020  rature sensor.  
+000075a0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000075b0: 656e 736f 7220 3d20 5954 656d 7065 7261  ensor = YTempera
+000075c0: 7475 7265 2e46 6972 7374 5465 6d70 6572  ture.FirstTemper
+000075d0: 6174 7572 6528 290a 2020 2020 2020 2020  ature().        
+000075e0: 656c 6966 2074 6172 6765 7420 3d3d 2027  elif target == '
+000075f0: 273a 0a20 2020 2020 2020 2020 2020 2070  ':.            p
+00007600: 7269 6e74 2827 7370 6563 6966 6965 6420  rint('specified 
+00007610: 696e 7661 6c69 6420 7461 7267 6574 2729  invalid target')
+00007620: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00007630: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+00007640: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00007650: 2020 2020 7365 6c66 2e73 656e 736f 7220      self.sensor 
+00007660: 3d20 5954 656d 7065 7261 7475 7265 2e46  = YTemperature.F
+00007670: 696e 6454 656d 7065 7261 7475 7265 2874  indTemperature(t
+00007680: 6172 6765 7420 2b20 272e 7465 6d70 6572  arget + '.temper
+00007690: 6174 7572 6527 290a 2020 2020 2020 2020  ature').        
+000076a0: 6966 2073 656c 662e 7365 6e73 6f72 2069  if self.sensor i
+000076b0: 7320 4e6f 6e65 206f 7220 7365 6c66 2e67  s None or self.g
+000076c0: 6574 5f73 656e 736f 725f 6e61 6d65 2829  et_sensor_name()
+000076d0: 203d 3d20 2775 6e72 6573 6f6c 7665 6427   == 'unresolved'
+000076e0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+000076f0: 696e 7428 274e 6f20 6d6f 6475 6c65 2063  int('No module c
+00007700: 6f6e 6e65 6374 6564 2729 0a20 2020 2020  onnected').     
+00007710: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00007720: 6c73 650a 2020 2020 2020 2020 656c 7365  lse.        else
+00007730: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00007740: 7475 726e 2054 7275 650a 0a20 2020 2064  turn True..    d
+00007750: 6566 2067 6574 5f73 656e 736f 725f 6e61  ef get_sensor_na
+00007760: 6d65 2873 656c 6629 3a0a 2020 2020 2020  me(self):.      
+00007770: 2020 6966 2073 656c 662e 7365 6e73 6f72    if self.sensor
+00007780: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00007790: 2020 2020 2020 7072 696e 7428 276e 6f20        print('no 
+000077a0: 7365 6e73 6f72 2069 7320 636f 6e6e 6563  sensor is connec
+000077b0: 7465 642e 2074 7279 2074 6f20 6361 6c6c  ted. try to call
+000077c0: 2063 6f6e 6e65 6374 2829 2066 6972 7374   connect() first
+000077d0: 2729 0a20 2020 2020 2020 2020 2020 2072  ').            r
+000077e0: 6574 7572 6e20 2727 0a0a 2020 2020 2020  eturn ''..      
+000077f0: 2020 7365 6e73 6f72 5f73 7472 203d 2073    sensor_str = s
+00007800: 656c 662e 7365 6e73 6f72 2e64 6573 6372  elf.sensor.descr
+00007810: 6962 6528 290a 2020 2020 2020 2020 6e61  ibe().        na
+00007820: 6d65 5f73 7472 203d 2073 656e 736f 725f  me_str = sensor_
+00007830: 7374 722e 7370 6c69 7428 273d 2729 5b31  str.split('=')[1
+00007840: 5d2e 7370 6c69 7428 272e 2729 5b30 5d0a  ].split('.')[0].
+00007850: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+00007860: 616d 655f 7374 720a 0a20 2020 2064 6566  ame_str..    def
+00007870: 2067 6574 5f74 656d 7065 7261 7475 7265   get_temperature
+00007880: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00007890: 6966 2073 656c 662e 7365 6e73 6f72 2069  if self.sensor i
+000078a0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+000078b0: 2020 2020 7072 696e 7428 2773 656e 736f      print('senso
+000078c0: 7220 6973 206e 6f74 2063 6f6e 6e65 6374  r is not connect
+000078d0: 6564 2e20 7472 7920 746f 2063 616c 6c20  ed. try to call 
+000078e0: 636f 6e6e 6563 7428 2920 6669 7273 7427  connect() first'
+000078f0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00007900: 7475 726e 2066 6c6f 6174 2827 6e61 6e27  turn float('nan'
+00007910: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+00007920: 2028 7365 6c66 2e73 656e 736f 722e 6973   (self.sensor.is
+00007930: 4f6e 6c69 6e65 2829 293a 0a20 2020 2020  Online()):.     
+00007940: 2020 2020 2020 2070 7269 6e74 2827 7365         print('se
+00007950: 6e73 6f72 2069 7320 6e6f 7420 636f 6e6e  nsor is not conn
+00007960: 6563 7465 6420 6f72 2064 6973 636f 6e6e  ected or disconn
+00007970: 6563 7465 6420 6475 7269 6e67 2072 756e  ected during run
+00007980: 2729 0a20 2020 2020 2020 2020 2020 2072  ').            r
+00007990: 6574 7572 6e20 666c 6f61 7428 276e 616e  eturn float('nan
+000079a0: 2729 0a0a 2020 2020 2020 2020 7265 7475  ')..        retu
+000079b0: 726e 2073 656c 662e 7365 6e73 6f72 2e67  rn self.sensor.g
+000079c0: 6574 5f63 7572 7265 6e74 5661 6c75 6528  et_currentValue(
+000079d0: 290a 0a20 2020 2040 7374 6174 6963 6d65  )..    @staticme
+000079e0: 7468 6f64 0a20 2020 2064 6566 2065 7869  thod.    def exi
+000079f0: 745f 6170 7028 293a 0a20 2020 2020 2020  t_app():.       
+00007a00: 2059 4150 492e 4672 6565 4150 4928 290a   YAPI.FreeAPI().
```

### Comparing `wiliot-testers-4.0.11/wiliot_testers/tester_utils.py` & `wiliot-testers-4.0.6/wiliot_testers/tester_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -140,26 +140,15 @@
                 s.close()
         except (OSError, serial.SerialException):
             pass
         except Exception as e:
             raise (e)
     return device_ports
 
-def dict_to_csv(dict_in, path, append=False, only_titles=False):
-    if append:
-        method = 'a'
-    else:
-        method = 'w'
-    with open(path, method, newline='') as f:
-        dict_writer = DictWriter(f, fieldnames=dict_in.keys())
-        if not append:
-            dict_writer.writeheader()
-        if not only_titles:
-            dict_writer.writerow(dict_in)
-        f.close()
+
 def set_temperature():
     """
     initialize yocto temperature sensor
     :return: current temperature
     """
     # object tenp sens
     errmsg = YRefParam()
@@ -754,14 +743,205 @@
     window2.close()
 
 
 ###########################################
 #              Cloud Functions            #
 ###########################################
 
+def upload_to_cloud_api(batch_name, tester_type, run_data_csv_name=None, tags_data_csv_name=None, to_logging=False,
+                        env='', is_batch_name_inside_logs_folder=True, logger_=None, is_path=False,
+                        client=None, packets_instead_tags=False, owner_id='wiliot-ops'):
+    """
+    uploads a tester log to Wiliot cloud
+    :type batch_name: string
+    :param batch_name: folder name of the relevant log
+    :type run_data_csv_name: string
+    :param run_data_csv_name: name of desired run_data log to upload,
+                              should contain 'run_data' and end with .csv
+    :type tags_data_csv_name: string
+    :param tags_data_csv_name: name of desired tags_data log to upload,
+                               should contain 'tags_data' and end with .csv
+    :type tester_type: string
+    :param tester_type: name of the tester the run was made on (offline, tal15k, conversion, yield)
+    :type to_logging: bool
+    :param to_logging: if true, write to logging.debug the result of the upload
+    :type env: string (prod, dev, test)
+    :param env: to what cloud environment should we upload the files
+    :type is_batch_name_inside_logs_folder: bool
+    :param is_batch_name_inside_logs_folder: flag to indicate if the batch_name is the regular run folder (logs) or
+                                             this function is being used in a way we will need the full path
+    :return: True for successful upload, False otherwise
+    """
+    if logger_ is None:
+        logger = logging.getLogger()
+    else:
+        logger = logging.getLogger(logger_)
+    tester_type_name = tester_type.split('-')[0]
+    if tester_type_name not in ['offline', 'tal15k', 'conversion', 'yield', 'sample']:
+        logger.warning('Unsupported tester_type inserted to upload_to_cloud_api()\nPlease change it and retry')
+        return
+    if run_data_csv_name is not None and 'run_data' not in run_data_csv_name:
+        logger.warning('Unsupported run_data_csv_name inserted to upload_to_cloud_api()\nPlease change it and retry')
+        return
+    if tags_data_csv_name is not None and 'packets_data' not in tags_data_csv_name and \
+            'tags_data' not in tags_data_csv_name:
+        logger.warning('Unsupported tags_data_csv_name inserted to upload_to_cloud_api()\nPlease change it and retry')
+        return
+
+    file_path, api_key, is_successful = check_user_config_is_ok(env=env, owner_id=owner_id)
+    if env == 'prod':
+        env = ''
+    if not is_successful:
+        logger.warning('could not extract user credentials. please check warnings')
+        return
+    if client is None:
+        client = ManufacturingClient(api_key=api_key, env=env, logger_=logger.name)
+    else:
+        client = client
+    
+    logger.info('Upload to cloud has began\nWaiting for the server response, please wait...')
+    conn = http.client.HTTPSConnection("api.wiliot.com")
+    boundary = 'wL36Yn8afVp8Ag7AmP8qZ0SA4n1v9T'
+    headers = {
+        'Authorization': 'Bearer ' + client.auth_obj.get_token(),
+        'Content-type': 'multipart/form-data; boundary={}'.format(boundary)
+    }
+    
+    if env == 'prod' or env == '':
+        url = "/v1/manufacturing/upload/testerslogs/"
+    elif env == 'test' or env == '/test':
+        url = "/test/v1/manufacturing/upload/testerslogs/"
+    elif env == 'dev':
+        url = "/dev/v1/manufacturing/upload/testerslogs/"
+    else:
+        print('unsupported env value was inserted (env = ' + str(env) + ')')
+        return False
+    
+    url += tester_type
+    
+    if run_data_csv_name is not None:
+        # run_url = url + '-tester-runs-indicators'
+        run_url = url + '/runs-indicators'
+        logger.info("Run data csv upload to {} started".format(run_url))
+        data_list = [encode('--' + boundary)]
+        if is_batch_name_inside_logs_folder:
+            run_data_path = 'logs/' + batch_name
+        else:
+            run_data_path = batch_name
+        run_data_path = os.path.join(run_data_path, run_data_csv_name)
+        
+        if not os.path.exists(run_data_path):
+            exception_string = str(run_data_path) + ' run_data_path could not be found \n' + \
+                               'please find it and try to upload again'
+            raise Exception(exception_string)
+        if is_path:
+            run_data_path = run_data_csv_name
+        data_list.append(encode('Content-Disposition: form-data; name=file; filename={0}'.format(run_data_path)))
+        file_type = mimetypes.guess_type(run_data_path)[0] or 'application/octet-stream'
+        data_list.append(encode('Content-Type: {}'.format(file_type)))
+        data_list.append(encode(''))
+        with open(run_data_path, 'rb') as f:
+            data_list.append(f.read())
+        data_list.append(encode('--' + boundary + '--'))
+        data_list.append(encode(''))
+        body = b'\r\n'.join(data_list)
+        payload = body
+        
+        conn.request("POST", run_url, payload, headers)
+        run_data_res = conn.getresponse()
+        run_data_data = run_data_res.read()
+        logger.info("answer from cloud is:")
+        run_data_data_decoded = run_data_data.decode('utf-8')
+        run_data_data_decoded_convert = ast.literal_eval(run_data_data_decoded)
+        try:
+            logger.info(run_data_data_decoded_convert['data'])
+        
+        except Exception:
+            logger.warning('Problem with cloud upload')
+            logger.warning(run_data_data_decoded_convert['error'])
+        
+        if str(run_data_res.status) == '500':
+            logger.info(
+                'There was a problem at the Server side (status 500), please try to upload again or reach Wiliot')
+            return False
+        elif str(run_data_res.status) in ['401', '400']:
+            client.auth_obj.get_token()
+            return False
+        elif str(run_data_res.status)[0:2] == '40':
+            logger.info('There was a problem with the request (status 40*), please try to upload again or reach Wiliot')
+            logger.info('Status code is: ' + str(run_data_res.status))
+            if run_data_data_decoded_convert['error'] != 'This CSV file already uploaded':
+                return False
+        elif str(run_data_res.status) == '200':
+            logger.info('The file "' + run_data_csv_name + '" was uploaded successfully to Wiliot cloud')
+    
+    if tags_data_csv_name is not None:
+        # tags_url = url + '-tester-tags-indicators'
+        if packets_instead_tags:
+            tags_url = url + '/packets-indicators'
+            logger.info("Packet data csv upload to {} started".format(tags_url))
+        else:
+            tags_url = url + '/tags-indicators'
+            logger.info("Tags data csv upload to {} started".format(tags_url))
+        data_list = []
+        data_list.append(encode('--' + boundary))
+        if is_batch_name_inside_logs_folder:
+            tags_data_path = 'logs/' + batch_name
+        else:
+            tags_data_path = batch_name
+        tags_data_path = os.path.join(tags_data_path, tags_data_csv_name)
+        if not os.path.exists(tags_data_path):
+            exception_string = str(tags_data_path) + ' tags_data_path could not be found \n' + \
+                               'please find it and try to upload again'
+            raise Exception(exception_string)
+        
+        if is_path:
+            tags_data_path = tags_data_csv_name
+        data_list.append(encode('Content-Disposition: form-data; name=file; filename={0}'.format(tags_data_path)))
+        file_type = mimetypes.guess_type(tags_data_path)[0] or 'application/octet-stream'
+        data_list.append(encode('Content-Type: {}'.format(file_type)))
+        data_list.append(encode(''))
+        with open(tags_data_path, 'rb') as f:
+            data_list.append(f.read())
+        data_list.append(encode('--' + boundary + '--'))
+        data_list.append(encode(''))
+        body = b'\r\n'.join(data_list)
+        payload = body
+        
+        conn.request("POST", tags_url, payload, headers)
+        tags_data_res = conn.getresponse()
+        tags_data_data = tags_data_res.read()
+        logger.info("answer from cloud is:")
+        tags_data_data_decoded = tags_data_data.decode('utf-8')
+        tags_data_data_decoded_convert = ast.literal_eval(tags_data_data_decoded)
+        try:
+            logger.info(tags_data_data_decoded_convert['data'])
+        
+        except Exception:
+            logger.warning('Problem with cloud upload')
+        
+        if str(tags_data_res.status) == '500':
+            logger.info(
+                'There was a problem at the Server side (status 500), please try to upload again or reach Wiliot')
+            return False
+        elif str(tags_data_res.status) in ['401', '400']:
+            client.auth_obj.get_token()
+            return False
+        elif str(tags_data_res.status)[0:2] == '40':
+            logger.info(
+                'There was a problem at the request side (status 40*), please try to upload again or reach Wiliot')
+            logger.info('Status code is: ' + str(tags_data_res.status))
+            return False
+        elif str(tags_data_res.status) == '200':
+            logger.info('The file "' + tags_data_csv_name + '" was uploaded successfully to Wiliot cloud')
+    logger.info('-----------------------------------------------------------------------\n'
+                'upload to cloud is finished successfully\n'
+                '-----------------------------------------------------------------------')
+    return True
+
 
 def get_cloud_error_message(status_code):
     if status_code is None:
         message = 'upload failed with unknown error code, please look inside log and reach wiliot'
     elif status_code == 500:
         message = 'There was a problem at the Server side (status 500), ' \
                   'please try to upload again or reach Wiliot'
```

### Comparing `wiliot-testers-4.0.11/wiliot_testers/upload_testers_data_to_cloud.py` & `wiliot-testers-4.0.6/wiliot_testers/upload_testers_data_to_cloud.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,23 +57,53 @@
 #     (B) EVEN IF ANYONE IS ADVISED OF THE POSSIBILITY OF ANY DAMAGES, LOSSES, OR COSTS; AND
 #     (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 #  """
 import logging
 import os.path
 import PySimpleGUI as Sg
 import datetime
+import numpy as np
 import csv
 import shutil
+
 from wiliot_core import WiliotDir
-from wiliot_testers.utils.upload_to_cloud_api import upload_to_cloud_api
+from wiliot_testers.tester_utils import upload_to_cloud_api
 
 
 MAX_FILE_SIZE = 15 * 10**6  # 15 Mb
 
 
+def get_files_path():
+    """
+    opens GUI for selecting a file and returns it
+    """
+    # Define the window's contents
+    layout = [[Sg.Text('Choose run data file that you want to upload:'), Sg.Input(key="run_data_file"),
+               Sg.FileBrowse()],
+              [Sg.Text('Choose packets data file that you want to upload:'), Sg.Input(key="tags_data_file"),
+               Sg.FileBrowse()],
+              [Sg.Text('environment:'),
+               Sg.InputCombo(('prod', 'test'), default_value="prod", key='env')],
+              [Sg.Text('Tester type:'),
+               Sg.InputCombo(('offline-tester', 'sample-test'), default_value="offline-tester", key='tester_type')],
+              [Sg.Button('Select')]]
+
+    # Create the window
+    window = Sg.Window('upload to Cloud', layout)
+
+    event, values = window.read()
+    # See if user wants to quit or window was closed
+    if event == 'Select' and (values['run_data_file'] != '' or values['tags_data_file'] != ''):
+        window.close()
+        return values
+    else:
+        window.close()
+        return None
+
+
 def create_summary_message(is_upload=True, data_folder_name=''):
     """
     summary log
     :param is_upload:
     :type is_upload: bool or None
     :return:
     :rtype:
@@ -109,108 +139,102 @@
         self.set_logging()
         file_status = self.check_files()
         if not file_status:
             return
 
         # check file size:
         self.all_run_names = [self.values['run_data_file']]
-        self.all_packets_names = [self.values['packets_data_file']]
+        self.all_packets_names = [self.values['tags_data_file']]
         self.tester_type = self.values['tester_type']
-        file_size = os.stat(self.values['packets_data_file']).st_size
+        file_size = os.stat(self.values['tags_data_file']).st_size
         if file_size > MAX_FILE_SIZE and 'offline' in self.tester_type:
-            self.split_large_file(run_data=self.values['run_data_file'], packet_data=self.values['packets_data_file'],
+            self.split_large_file(run_data=self.values['run_data_file'], packet_data=self.values['tags_data_file'],
                                   size=file_size)
 
     def get_files_path(self):
         """
-        opens GUI for selecting a file and returns it
-        """
-        layout = [
-            [Sg.Text('Choose run data file that you want to upload:', font=("Helvetica", 11)),
-             Sg.Input(key="run_data_file", font=("Helvetica", 11)),
-             Sg.FileBrowse(font=("Helvetica", 11))],
-            [Sg.Text('Choose packets data file that you want to upload:', font=("Helvetica", 11)),
-             Sg.Input(key="packets_data_file", font=("Helvetica", 11)),
-             Sg.FileBrowse(font=("Helvetica", 11))],
-            [Sg.Text('Environment:', font=("Helvetica", 11)),
-             Sg.InputCombo(('prod', 'test'), default_value="prod", key='env', font=("Helvetica", 11))],
-            [Sg.Text('Owner id:', font=("Helvetica", 11)),
-             Sg.Input('852213717688', key='owner_id', font=("Helvetica", 11))],
-            [Sg.Text('Tester type:', font=("Helvetica", 11)),
-             Sg.InputCombo(('offline-tester', 'sample-test'), default_value="offline-tester", key='tester_type',
-                           font=("Helvetica", 11))],
-            [Sg.Button('Select', font=("Helvetica", 11))]
-        ]
+            opens GUI for selecting a file and returns it
+            """
+        # Define the window's contents
+        layout = [[Sg.Text('Choose run data file that you want to upload:'), Sg.Input(key="run_data_file"),
+                   Sg.FileBrowse()],
+                  [Sg.Text('Choose packets data file that you want to upload:'), Sg.Input(key="tags_data_file"),
+                   Sg.FileBrowse()],
+                  [Sg.Text('environment:'),
+                   Sg.InputCombo(('prod', 'test'), default_value="prod", key='env')],
+                  [Sg.Text('owner id:'),
+                   Sg.Input('wiliot-ops', key='owner_id')],
+                  [Sg.Text('Tester type:'),
+                   Sg.InputCombo(('offline-tester', 'sample-test'), default_value="offline-tester", key='tester_type')],
+                  [Sg.Button('Select')]]
 
-        window = Sg.Window('upload to Cloud', layout, size=(800, 190), font=("Helvetica", 11))
+        # Create the window
+        window = Sg.Window('upload to Cloud', layout)
 
         event, values = window.read()
-        if event == 'Select' and (values['run_data_file'] != '' or values['packets_data_file'] != ''):
+        # See if user wants to quit or window was closed
+        if event == 'Select' and (values['run_data_file'] != '' or values['tags_data_file'] != ''):
             window.close()
             self.values = values
         else:
             window.close()
             self.values = None
 
     def set_logging(self):
-        """
-        Sets up logging for the object, creating a log file with the current date and time as part of the filename.
-        Returns: None
-        """
-        #  get()dirname from run_data or packets_data
-        files_dir = os.path.dirname(self.values.get('run_data_file', self.values.get('packets_data_file')))
-        if not files_dir:
-            files_dir = os.path.join(WiliotDir().get_tester_dir("upload_to_cloud"), "logs")
-            os.makedirs(files_dir, exist_ok=True)
+
+        # set log path
+        if os.path.isfile(self.values['run_data_file']):
+            files_dir = os.path.dirname(self.values['run_data_file'])
+        elif os.path.isfile(self.values['tags_data_file']):
+            files_dir = os.path.dirname(self.values['run_data_file'])
+        else:
+            env_dir = WiliotDir()
+            files_dir = os.path.join(env_dir.get_tester_dir("upload_to_cloud"), "logs")
+            if not os.path.isdir(files_dir):
+                env_dir.create_dir(files_dir)
         log_path = os.path.join(files_dir,
                                 datetime.datetime.now().strftime("%d-%m-%Y_%H-%M-%S") + 'upload_to_cloud.log')
-        logger = logging.getLogger('Manual Upload')
-        logger.setLevel(logging.DEBUG)
-        formatter = logging.Formatter('%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s', '%H:%M:%S')
+
+        # set logger:
         file_handler = logging.FileHandler(log_path)
-        file_handler.setFormatter(formatter)
+        file_handler.setFormatter(
+            logging.Formatter('%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s', '%H:%M:%S'))
+        file_handler.setLevel(logging.DEBUG)
         stream_handler = logging.StreamHandler()
-        stream_handler.setFormatter(formatter)
+        stream_handler.setFormatter(
+            logging.Formatter('%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s', '%H:%M:%S'))
         stream_handler.setLevel(logging.DEBUG)
+        logger = logging.getLogger('Manual Upload')
+        logger.setLevel(logging.DEBUG)
         logger.addHandler(file_handler)
         logger.addHandler(stream_handler)
         self.logger = logger
 
     def check_files(self):
-        """
-        Checks if the run_data_file and packets_data_file are valid CSV files.
-        Returns True if both files are valid, False otherwise.
-        """
         if not os.path.isfile(self.values['run_data_file']) or not self.values['run_data_file'].endswith('.csv'):
             self.logger.warning('UPLOAD: run_data file format is not csv, please insert a csv file')
             self.logger.info(create_summary_message(False))
             return False
-        if not os.path.isfile(self.values['packets_data_file']) or not self.values['packets_data_file'].endswith('.csv'):
-            self.logger.warning('UPLOAD: packets_data file format is not csv, please insert a csv file')
+        if not os.path.isfile(self.values['tags_data_file']) or not self.values['tags_data_file'].endswith('.csv'):
+            self.logger.warning('UPLOAD: tags_data file format is not csv, please insert a csv file')
             self.logger.info(create_summary_message(False))
             return False
         return True
 
     def split_large_file(self, run_data, packet_data, size):
 
-        """
-        Splits a large packet_data CSV file into smaller parts that are each under the maximum allowed size.
-        Duplicates the corresponding run_data CSV file for each part. Returns a list of file paths for each split part.
-        """
-        # Define a helper function to generate new file paths.
         def get_new_path_name(original_path, k, total, file_str):
             new_folder_name = os.path.dirname(original_path) + f'_{k}_out_of_{n_splits}'
             new_file_name = os.path.basename(original_path).replace(f'@{file_str}_data.csv',
                                                                     f'_{k}_out_of_{total}@{file_str}_data.csv')
             if not os.path.isdir(new_folder_name):
                 os.makedirs(new_folder_name)
             return os.path.join(new_folder_name, new_file_name)
 
-        # Split the file into smaller parts.
-        n_splits = -(-size // MAX_FILE_SIZE)
+        n_splits = int(np.ceil(size / MAX_FILE_SIZE))
         part = 1
         all_packets_path = []
         all_run_path = []
         # read
         f_read = open(packet_data, 'r')
         reader = csv.DictReader(f_read, delimiter=',')
         col_names = reader.fieldnames
@@ -237,49 +261,46 @@
                 last_loc = int(row['tag_run_location'])
         f_write.close()
         if part > n_splits:
             self.logger.info(
                 f'Since the file cannot be split in the middle of location data, a mismatch happened and '
                 f'the number of parts is bigger than the number of split (i.e you will have a file with '
                 f'the suufix {part}_out_of{n_splits}')
-        # Duplicate the run data for each part.
+        # duplicate run data:
         for i in range(part):
-            new_run_path = get_new_path_name(run_data, i + 1, n_splits, 'run')
+            new_run_path = get_new_path_name(run_data, i+1, n_splits, 'run')
             all_run_path.append(new_run_path)
             shutil.copyfile(run_data, new_run_path)
 
         self.all_run_names = all_run_path
         self.all_packets_names = all_packets_path
 
     def upload_to_cloud(self):
-        """
-        Uploads files to a cloud API
-        Returns True if all uploads were successful
-        """
         if self.tester_type == 'offline-tester':
             self.tester_type = 'offline-test'
 
         all_status = []
         for run_path, packet_path in zip(self.all_run_names, self.all_packets_names):
             try:
                 upload_success = upload_to_cloud_api(batch_name=os.path.dirname(run_path),
                                                      tester_type=self.tester_type,
-                                                     run_data_csv_name=os.path.basename(run_path),
-                                                     packets_data_csv_name=os.path.basename(packet_path),
-                                                     env=self.values['env'],
+                                                     run_data_csv_name=run_path,
+                                                     tags_data_csv_name=packet_path,
+                                                     to_logging=True, env=self.values['env'],
                                                      is_batch_name_inside_logs_folder=False,
-                                                     logger_=self.logger.name, owner_id=self.values['owner_id'])
+                                                     logger_=self.logger.name, packets_instead_tags=True,
+                                                     owner_id=self.values['owner_id'],
+                                                     is_path=True)
             except Exception as e:
                 self.logger.warning(f'UPLOAD: during upload_to_cloud_api an error occurred: {e}')
                 upload_success = False
 
-            message = create_summary_message(is_upload=upload_success, data_folder_name=os.path.dirname(run_path))
-            self.logger.info(message)
+            self.logger.info(
+                create_summary_message(is_upload=upload_success, data_folder_name=os.path.dirname(run_path)))
             all_status.append(upload_success)
-
         return all(all_status)
 
 
 if __name__ == '__main__':
     # upload to cloud
     upload_obj = UploadTestersData()
     status = upload_obj.upload_to_cloud()
```

### Comparing `wiliot-testers-4.0.11/wiliot_testers/utils/get_version.py` & `wiliot-testers-4.0.6/wiliot_testers/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/wiliot_tester_log.py` & `wiliot-testers-4.0.6/wiliot_testers/wiliot_tester_log.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.11/wiliot_testers/wiliot_tester_tag_result.py` & `wiliot-testers-4.0.6/wiliot_testers/wiliot_tester_tag_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,21 +81,14 @@
     DUPLICATION_OFFLINE = 14  # Duplicate offline - tag was found as duplicate during offline tester run (ADVA duplicate)
     DUPLICATION_POST_PROCESS = 15  # Duplicate post process - tag was found as duplicate in post process (UID duplicate)
     GW_ERROR = 16  # GW error
     STOP_BY_USER = 17  # test stopped by the user
     SEVERAL_TAGS_UNDER_TEST = 18  # Cannot decided which tag is under test
     FAILED_QUALITY_TEST = 19  # Failed Quality Test according to the specified statistics limits.
     NOT_PRINTED = 20  # tag was not printed due to printing offset
-    CORRUPTED_PACKET_POST_PROCESS = 21  # post process - corrupted packet detection
-    DIFF_TAG_ID_WITH_SAME_ADVA_POST_PROCESS = 22  # post process - same adva but different tag id
-    SHIPMENT_INTERNAL_ID_DUPLICATION = 90  # shipment API error - decided over the cloud
-    SHIPMENT_EXTERNAL_ID_DUPLICATION = 91  # shipment API error - decided over the cloud
-    SHIPMENT_TAG_NOT_EXIST = 92  # shipment API error - decided over the cloud
-    SHIPMENT_OWNER_NOT_WILIOT_OPS = 93  # shipment API error - decided over the cloud
-    SHIPMENT_SERIALIZATION_ISSUE = 94  # shipment API error - decided over the cloud
 
 
 class ConversionTypes(Enum):
     NOT_CONVERTED = 'Unconverted'
     STANDARD = 'Regular Conversion'
     DURABLE = 'Durable Conversion'
```

### Comparing `wiliot-testers-4.0.11/wiliot_testers/wiliot_tester_tag_test.py` & `wiliot-testers-4.0.6/wiliot_testers/wiliot_tester_tag_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
         return True
 
     def gw_init(self):
         """
         initialize gw and the data listener thread
         """
         if self.GwObj is None:
-            self.GwObj = WiliotGateway(auto_connect=True, logger_name=self.logger_gw.name, is_multi_processes=True,
+            self.GwObj = WiliotGateway(auto_connect=True, logger_name=self.logger_gw.name,
                                        lock_print=threading.Lock())
         try:
             if self.GwObj.connected:
                 self.GwObj.reset_buffer()
                 self.GwObj.start_continuous_listener()
                 if self.check_gw_version():
                     self._printing_func('GW obj initialized')
@@ -881,17 +881,15 @@
                                         logger_name=LoggerName.RESULTS)
                     self.tag_results.test_status = FailureCodes.PASS
                     self.tag_results.is_test_passed = True
                     self.test_results.append(self.tag_results)
 
             elif self.test_end:
                 selected_tag = self.select_tag_under_test(optional_tags=tags_reached_criteria)  # Get the best tag
-                all_selected_tags = self.test_results.get_test_unique_adva()
-                is_diff_tag_btwn_sub_tests = selected_tag not in all_selected_tags if len(all_selected_tags) > 0 else False
-                if selected_tag is not None and not is_diff_tag_btwn_sub_tests:
+                if selected_tag is not None:
                     self._printing_func('Tag {} was selected'.format(selected_tag[0].packet_data['adv_address']))
                     # selected tag performance:
                     self.tag_results.is_test_passed = self.statistics_analyzer(test_param=sub_test, test_num=test_num)
                     if self.tag_results.is_test_passed:
                         self.tag_results.test_status = FailureCodes.PASS
                         self._printing_func('Stage {} out of {} Passed'.format(test_num + 1, num_of_tests),
                                             logger_name=LoggerName.RESULTS)
```

### Comparing `wiliot-testers-4.0.11/wiliot_testers/yield/arduino_counter/arduino_counter.ino` & `wiliot-testers-4.0.6/wiliot_testers/yield/arduino_counter/arduino_counter.ino`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 
 const int input = 2; // This is where the input is fed.
 int pulse = 0; // Variable for saving pulses count.
 int var = 0;
 
 void setup(){
   pinMode(input, INPUT);
-
+ 
   Serial.begin(9600);
   Serial.println(F("No pulses yet...")); // Message to send initially (no pulses detected yet).
 }
 
-void loop(){
+void loop(){ 
   if(digitalRead(input) > var)
   {
     var = 1;
     pulse++;
-
+   
     Serial.print(pulse);
     Serial.print(F(" pulse"));
 
     // Put an "s" if the amount of pulses is greater than 1.
     if(pulse > 1) {Serial.print(F("s"));}
-
+   
     Serial.println(F(" detected."));
   }
-
+ 
   if(digitalRead(input) == 0) {var = 0;}
-
+ 
   delay(1); // Delay for stability.
 }
```

### Comparing `wiliot-testers-4.0.11/wiliot_testers/yield/configs/inlay_data.py` & `wiliot-testers-4.0.6/wiliot_testers/yield/configs/inlay_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 csv_dictionary = {
     'TEO_086': {'inlay': 'TEO_086', 'number': '086', 'number_of_rows': 1, 'received_channel': '37',
-                'energy_pattern_val': 18, 'time_profile_val': [5, 40]},
+                'energy_pattern_val': 18, 'time_profile_val': [5, 15]},
     'TIKI_096': {'inlay': 'TIKI_096', 'number': '096', 'number_of_rows': 2, 'received_channel': '37',
-                 'energy_pattern_val': 51, 'time_profile_val': [5, 40]},
+                 'energy_pattern_val': 51, 'time_profile_val': [5, 15]},
     'TIKI_099': {'inlay': 'TIKI_099', 'number': '099', 'number_of_rows': 3, 'received_channel': '37',
-                 'energy_pattern_val': 51, 'time_profile_val': [5, 40]},
+                 'energy_pattern_val': 51, 'time_profile_val': [5, 15]},
     'BATTERY_107': {'inlay': 'BATTERY_107', 'number': '107', 'number_of_rows': 4, 'received_channel': '37',
-                    'energy_pattern_val': 17, 'time_profile_val': [5, 40]},
+                    'energy_pattern_val': 17, 'time_profile_val': [5, 15]},
     'TIKI_117': {'inlay': 'TIKI_117', 'number': '117', 'number_of_rows': 5, 'received_channel': '37',
-                 'energy_pattern_val': 51, 'time_profile_val': [5, 40]},
+                 'energy_pattern_val': 51, 'time_profile_val': [5, 15]},
     'TIKI_121': {'inlay': 'TIKI_121', 'number': '121', 'number_of_rows': 6, 'received_channel': '37',
-                 'energy_pattern_val': 51, 'time_profile_val': [5, 40]},
+                 'energy_pattern_val': 51, 'time_profile_val': [5, 15]},
     'TIKI_122': {'inlay': 'TIKI_122', 'number': '122', 'number_of_rows': 7, 'received_channel': '37',
-                 'energy_pattern_val': 51, 'time_profile_val': [5, 40]},
+                 'energy_pattern_val': 51, 'time_profile_val': [5, 15]},
     '': {'inlay': '', 'number': '', 'number_of_rows': 0, 'received_channel': '', 'energy_pattern_val': 0,
          'time_profile_val': [0, 0]}}
```

### Comparing `wiliot-testers-4.0.11/wiliot_testers/yield/yield_tester.py` & `wiliot-testers-4.0.6/wiliot_testers/yield/yield_tester.py`

 * *Files 23% similar despite different names*

```diff
@@ -65,50 +65,48 @@
 at the same time
 4)Calculating the Yield fraction according to the results we got from the instances
 5)Creating two threads in MainWindow class in order to calculate the fraction by MultiThreadingCalculation instance
 and to run the GUI function (open_session) at the same time.
 """
 
 from wiliot_core import *
+import csv
 import serial.tools.list_ports
 import PySimpleGUI as sg
 from configs.inlay_data import *
+from wiliot_testers.tester_utils import *
 from wiliot_testers.utils.get_version import *
-from wiliot_testers.utils.upload_to_cloud_api import *
 import serial
-import matplotlib.pyplot as plt
-from wiliot_testers.tester_utils import dict_to_csv
+
 
 inlay_types_dict = {item.name: item.value for item in InlayTypes}
 today = datetime.date.today()
 formatted_today = today.strftime("%Y%m%d")  # without -
 formatted_date = today.strftime("%Y-%m-%d")
 current_time = datetime.datetime.now()
 cur_time_formatted = current_time.strftime("%I%M%S")  # without :
 time_formatted = current_time.strftime("%I:%M:%S")
 
 
-class AdvaProcess(object):
+class AdvaProcess(threading.Thread):
     """
     Counting the number of unique advas
     """
 
-    def __init__(self, stop_event, received_channel, time_profile_val, energy_pattern_val, inlay_type):
-        self.gw_instance = WiliotGateway(auto_connect=True,
-                                         is_multi_processes=True)  # gw object, in order to connect with gw
-        self.all_tags = set()
+    def __init__(self, stop_event, received_channel, time_profile_val, energy_pattern_val):
+        threading.Thread.__init__(self, daemon=True)
+        self.gw_instance = WiliotGateway(auto_connect=True)  # gw object, in order to connect with gw
+        self.all_tags = TagCollection()  # tagcollection object, in order to check packets in prepared list
         self.gw_init()
         self.stop = stop_event
         self.received_channel = received_channel
         self.time_profile_val = time_profile_val
         self.energy_pattern_val = energy_pattern_val
         self.gw_reset_config()
         self.number_of_unq_adva = 0
-        self.packets_queue = Queue(maxsize=1000)
-        self.inlay_type = inlay_type
 
     def gw_init(self):
         """
         Initialize the gateway
         """
         if self.gw_instance.connected:
             self.gw_instance.reset_buffer()
@@ -120,455 +118,356 @@
 
     def gw_reset_config(self):
         """
         Configs the gateway
         """
         if self.gw_instance.connected:
             self.gw_instance.start_continuous_listener()
-            self.gw_instance.reset_gw(reset_port=False)
-            self.gw_instance.reset_listener()
-            if not self.gw_instance.is_gw_alive():
-                print('gw_reset_and_config: wait more time since gw did not respond')
-                time.sleep(5)
             self.gw_instance.write('!set_tester_mode 1', with_ack=True)
             self.gw_instance.write('!listen_to_tag_only 1', with_ack=True)
-            self.gw_instance.write('!sub1g_sync 1', with_ack=True)
             self.gw_instance.config_gw(received_channel=self.received_channel, time_profile_val=self.time_profile_val,
                                        energy_pattern_val=self.energy_pattern_val,
                                        start_gw_app=False, with_ack=True,
                                        effective_output_power_val=22, sub1g_output_power_val=29)
         else:
             raise Exception('Could NOT connect to GW')
 
     def run(self):
         """
         Receives available data then counts and returns the number of unique advas
         """
         self.gw_instance.config_gw(start_gw_app=True)
+        self.number_of_unq_adva = 0
         while not self.stop.is_set():
             time.sleep(0)
             if self.gw_instance.is_data_available():
-                packet_list_in = self.gw_instance.get_packets(action_type=ActionType.ALL_SAMPLE,
-                                                              tag_inlay=self.inlay_type)
+                packet_list_in = self.gw_instance.get_packets(action_type=ActionType.ALL_SAMPLE)
                 for packet in packet_list_in:
-                    adva = packet.get_adva()
-                    self.all_tags.add(adva)
-                self.packets_queue.put(packet_list_in)
+                    self.all_tags.append(packet)
             else:
                 continue
-            self.number_of_unq_adva = len(self.all_tags)
-            # check gw connection
-            if not self.gw_instance.is_connected():
-                print('GW was disconnected. trying to initiate connection...')
-            if self.gw_instance.get_read_error_status():
-                print('A GW reading Error was detected')
 
+            self.number_of_unq_adva = len(self.all_tags.tags)
         self.gw_instance.exit_gw_api()
 
     def get_unq_advas(self):
         """
         returns the number of unique advas
         """
         return self.number_of_unq_adva
 
-    def get_packets_queue(self):
-        """
-        Returns the packet queue that is created above
-        """
-        return self.packets_queue
-
 
-class CountThread(object):
+class CountThread(threading.Thread):
     """
     Counting the number of tags
     """
 
     def __init__(self, stop_event, rows=1):
+        threading.Thread.__init__(self, daemon=True)
         self.available_ports = [s.device for s in serial.tools.list_ports.comports()]
-        self.get_ports_of_arduino(self)
+        self.get_ports_of_arduino()
         self.baud = '9600'
-        self.ports = self.get_ports_of_arduino(self)
+        self.ports = self.get_ports_of_arduino()
         try:
             self.comPortObj = serial.Serial(self.ports[0], self.baud, timeout=0.1)
         except serial.SerialException:
             print("NO ARDUINO")
         self.rows = rows
         self.stop = stop_event
         self.tested = 0
 
-    @staticmethod
     def get_ports_of_arduino(self):
         """
         Gets all the ports we have, then chooses Arduino's ports
         """
+
         arduino_ports = []
         for p in serial.tools.list_ports.comports():
             if 'Arduino' in p.description:
                 arduino_ports.append(p.device)
         if not arduino_ports:
             print('NO ARDUINO')
+
         return arduino_ports
 
     def run(self):
         """
         Tries to read data and then counts the number of tags
         """
+
         while not self.stop.is_set():
             time.sleep(1)
             data = ''
             try:
                 data = self.comPortObj.readline()
-            except Exception as e:
-                print(f"NO READLINE: {e}")
+
+            except e:
+                print("NO READLINE")
             buf = b''
             if data.__len__() > 0:
                 buf += data
                 if b'\n' in buf:
                     try:
                         tmp = buf.decode().strip(' \t\n\r')
                         if "pulses detected" in tmp:
                             self.tested += self.rows
 
-                    except Exception as e:
-                        print(f'Warning: Could not decode counter data or Warning: {e}')
+                    except e:
+                        print('Warning: Could not decode counter data or Warning: Could not decode counter data')
                         continue
         self.comPortObj.close()
 
     def get_tested(self):
         """
         returns the number of tags
         """
         return self.tested
 
 
+class MultithreadedCalculation(threading.Thread):
+    """
+    Calculating the yield fraction by multi-threading process
+    """
+
+    def __init__(self, stop_event, received_channel, time_profile_val, energy_pattern_val, rows=1):
+        threading.Thread.__init__(self, daemon=True)
+        self.rows = rows
+        self.adva_process = AdvaProcess(stop_event, received_channel, time_profile_val, energy_pattern_val)
+        self.count_thread = CountThread(stop_event, self.rows)
+        self.stop = stop_event
+        self.result = 0
+
+    def run(self):
+        """
+        The multi-threading process
+        """
+        self.adva_process.start()
+        self.count_thread.start()
+        while not self.stop.is_set():
+            time.sleep(3)
+
+            unq_advas = self.adva_process.get_unq_advas()
+            tags_num = self.count_thread.get_tested()
+            if tags_num > 0:
+                self.result = unq_advas / tags_num
+                print(self.result)
+
+        self.adva_process.stop.set()
+        self.count_thread.stop.set()
+        self.adva_process.join()
+        self.count_thread.join()
+
+    def get_result(self):
+        return self.result
+
+
 class MainWindow:
     """
     The main class the runs the GUI and supervise the multi-threading process of fraction's calculation and GUI viewing
     """
 
     def __init__(self):
-        self.adva_process = None
-        self.adva_process_thread = None
-        self.count_process = None
-        self.count_process_thread = None
-        self.folder_path = None
-        self.py_wiliot_version = None
-        self.d = None
-        self.yield_test_app_data = None
-        self.run_path = None
-        self.final_path_run_data = None
-        self.run_data_dict = None
-        self.tags_num = 0
+        self.multi = None
         self.stop = threading.Event()
-        self.neg_col = 0
         self.selected = ''
         self.wafer_lot = ''
         self.wafer_number = ''
         self.operator = ''
         self.run_start_time = ''
+        self.run_end_time = ''
         self.tester_type = 'yield-test'
         self.tester_station_name = ''
         self.comments = ''
         self.gw_version = ''
+        self.advas = 0
+        self.run_responsive_tags_yield = 0  # still don't have a pass criteria
+        self.result = 0
+        self.run_passed_tags_yield = 0  # still don't have a pass criteria
         self.rows_number = 1
         self.upload_flag = True
-        self.cmn = ''
-        self.final_path_packets_data = ''
-        self.seen_advas = set()
-        self.result = 0
-        self.update_packet_data_flag = False
-
-    def get_result(self):
-        """
-        Calculates the yield fraction
-        """
-        unq_advas = self.adva_process.get_unq_advas()
-        tags_num = self.count_process.get_tested()
-        if tags_num > 0:
-            self.result = (unq_advas / tags_num) * 100
-        return self.result
 
     def run(self):
         """
         Viewing the window and checking if the process stops
         """
+
         self.open_session()
         self.overlay_window()
+        self.multi.stop.set()
+        self.multi.join()
 
-    def init_run_data(self):
-        self.py_wiliot_version = get_version()
-        self.d = WiliotDir()
-        self.d.create_tester_dir(tester_name='yield_tester')
-        self.yield_test_app_data = self.d.get_tester_dir('yield_tester')
-        self.cmn = self.wafer_lot + '.' + self.wafer_number
-        self.run_path = os.path.join(self.yield_test_app_data, self.cmn)
-        if not os.path.exists(self.run_path):
-            os.makedirs(self.run_path)
-        self.cmn = self.wafer_lot + '.' + self.wafer_number + '_' + formatted_today + '_' + cur_time_formatted
-        self.folder_path = os.path.join(self.run_path, self.cmn)
-        if not os.path.exists(self.folder_path):
-            os.makedirs(self.folder_path)
-        self.final_path_run_data = os.path.join(self.folder_path, self.cmn + '@run_data.csv')
-        self.gw_version = self.adva_process.gw_instance.get_gw_version()[0]
-        start_time = datetime.datetime.now()
-        self.run_start_time = start_time.strftime("%I:%M:%S")
-        value = csv_dictionary[self.selected]
-        self.run_data_dict = {'common_run_name': self.cmn, 'tester_station_name': self.tester_station_name,
-                              'operator': self.operator,
-                              'run_start_time': formatted_date + ' ' + self.run_start_time, 'run_end_time': '',
-                              'wafer_lot': self.wafer_lot, 'wafer_number': self.wafer_number,
-                              'tester_type': self.tester_type,
-                              'comments': self.comments, 'inlay': self.selected, 'total_run_tested': 0,
-                              'total_run_responding_tags': 0,
-                              'gw_version': self.gw_version,
-                              'py_wiliot_version': self.py_wiliot_version,
-                              'upload_date': formatted_date + ' ' + time_formatted,
-                              'number_of_rows': value['number_of_rows'],
-                              'received_channel': value['received_channel'],
-                              'energy_pattern_val': value['energy_pattern_val'],
-                              'time_profile_val': value['time_profile_val']}
-
-    @staticmethod
-    def update_run_data_file(run_data_path, run_data_dict, run_end_time, tags_num, advas, result):
-        """
-        Updates the run_data CSV file while running the program
-        """
-        run_data_dict['run_end_time'] = run_end_time
-        run_data_dict['total_run_tested'] = tags_num
-        run_data_dict['total_run_responding_tags'] = advas
-        run_data_dict['yield'] = result
-        dict_to_csv(dict_in=run_data_dict, path=run_data_path)
-
-    def update_packet_data(self):
-        """
-        Updates the run_data CSV file while running the program
-        """
-        packets_queue = self.adva_process.get_packets_queue()
-        if not packets_queue.empty():
-            cur_p = PacketList()
-            for _ in range(packets_queue.qsize()):
-                cur_p.__add__(packets_queue.get())
-            cur_p_df = cur_p.get_df()
-            cur_p_df = cur_p_df.drop_duplicates(subset=['adv_address'])
-            cur_p_df = cur_p_df.loc[~cur_p_df['adv_address'].isin(list(self.seen_advas))]
-
-            for i in cur_p_df['adv_address']:
-                self.seen_advas.add(i)
-            if not self.update_packet_data_flag:
-                # Initializing the packets_data file
-                try:
-                    cur_p_df.insert(loc=len(cur_p_df.columns), column='common_run_name', value=self.cmn)
-                    self.final_path_packets_data = os.path.join(self.folder_path, self.cmn + '@packets_data.csv')
-                    if "index" in cur_p_df:
-                        cur_p_df.drop("index", axis=1, inplace=True)
-                    cur_p_df.to_csv(self.final_path_packets_data, index=False)
-                    self.update_packet_data_flag = True
-                except Exception as e:
-                    print(e)
-            else:
-                # updating packets_data_file
-                cur_p_df.insert(loc=len(cur_p_df.columns), column='common_run_name', value=self.cmn)
-                cur_p_df.to_csv(self.final_path_packets_data, mode='a', index=False, header=False)
-
-    def stop_button(self, window, run_end_time, tags_num, advas, result):
-        """
-        Finishing the program and saves the last changes after pressing Stop in the second window
-        """
-        self.stop.set()
-        window.close()
-        plt.close()
-        self.adva_process_thread.join()
-        self.count_process_thread.join()
-
-        self.update_run_data_file(self.final_path_run_data, self.run_data_dict,
-                                  formatted_date + ' ' + run_end_time,
-                                  tags_num, advas, result)
-        self.update_packet_data()
-
-        if self.upload_flag:
-            try:
-                is_uploaded = upload_to_cloud_api(self.cmn, self.tester_type,
-                                                  run_data_csv_name=self.final_path_run_data,
-                                                  packets_data_csv_name=self.final_path_packets_data,
-                                                  env='test', is_path=True)
-                if is_uploaded:
-                    print("Successful upload")
-                else:
-                    print("Unsuccessful upload")
-            except Exception as e:
-                print(e)
-
-    def init_processes(self, rec_channel, time_pro, energy_pat, inlay_select):
+    def run_data_to_csv(self, csv_dict, file_path, cmn_r_name, run_end_time, total_run_tested,
+                        total_run_responding_tags, total_run_passed_tags, py_wiliot_version):
         """
-        Initializing the two main instances and threads in order to start working
+        Saves a csv file with all the needed features
         """
-        self.adva_process = AdvaProcess(self.stop, rec_channel, time_pro, energy_pat,
-                                        inlay_select)
-        self.adva_process_thread = threading.Thread(target=self.adva_process.run, args=())
-        self.count_process = CountThread(self.stop, self.rows_number)
-        self.count_process_thread = threading.Thread(target=self.count_process.run, args=())
-
-    def start_processes(self):
-        """
-        Starting the work of the both threads
-        """
-        self.adva_process_thread.start()
-        self.count_process_thread.start()
+        with open(file_path, 'w', newline='') as file:
+            csv_writer = csv.writer(file)
+            csv_writer.writerow([
+                'common_run_name', 'tester_station_name', 'operator',
+                'run_start_time', 'run_end_time', 'wafer_lot', 'wafer_number', 'tester_type',
+                'comments', 'inlay', 'total_run_tested', 'total_run_responding_tags',
+                'total_run_passed_tags', 'run_responsive_tags_yield', 'run_passed_tags_yield',
+                'gw_version',
+                'py_wiliot_version', 'upload_date', 'number_of_rows', 'received_channel', 'energy_pattern_val',
+                'time_profile_val', ])
+            if self.selected == '':
+                # exit()
+                pass
+            value = csv_dict[self.selected]
+            csv_writer.writerow(
+                [
+                    cmn_r_name, self.tester_station_name, self.operator,
+                    formatted_date + ' ' + self.run_start_time,
+                    formatted_date + ' ' + run_end_time,
+                    self.wafer_lot, self.wafer_number, self.tester_type, self.comments, self.selected, total_run_tested,
+                    total_run_responding_tags, total_run_passed_tags, self.run_responsive_tags_yield,
+                    self.run_passed_tags_yield, self.gw_version, py_wiliot_version,
+                    formatted_date + ' ' + time_formatted,
+                    value['number_of_rows'], value['received_channel'], value['energy_pattern_val'],
+                    value['time_profile_val'],
+                ])
 
     def overlay_window(self):
         """
         The small window open session
         """
 
+        start_time = datetime.datetime.now()
+        self.run_start_time = start_time.strftime("%I:%M:%S")
         yes_or_no = ['Yes', 'No']
         layout = [
-            [sg.Text('Number of tags:', font=4), sg.Text(key='num_rows', font=4)],
-            [sg.Text('Number of advas:', font=4), sg.Text(key='num_advas', font=4)],
+            [sg.Text('YIELD Fraction is :', font=4)],
+            [sg.Output(key='yield', font=4, size=(60, 7))],
             [sg.Text('Do you want to stop or upload?')],
             [sg.Button('Stop'), [sg.Text('Upload:', font=6)],
-             [sg.Combo(values=yes_or_no, default_value=yes_or_no[0], key='upload', font=4, enable_events=True)]],
-            [sg.Canvas(key='-CANVAS-', size=(10, 100))],
+             [sg.Combo(values=yes_or_no, default_value=yes_or_no[0], key='upload', font=4, enable_events=True)]]
         ]
-
         sub = False
-        window = sg.Window('Upload CSV files', layout, modal=True, finalize=True, location=(870, 200))
-
-        # initialize num_advas and num_rows
-        num_rows_text_elem = window['num_rows']
-        num_advas_text_elem = window['num_advas']
-        num_rows = (self.rows_number * self.neg_col)
-        num_advas = self.adva_process.get_unq_advas()
-        num_rows_text_elem.update(f"{num_rows}")
-        num_advas_text_elem.update(f"{num_advas}")
-        # initialize the graph
-        plt.rcParams['axes.prop_cycle'] = plt.cycler(color=['red'])
-        fig, ax = plt.subplots()
-        ax.set_xlabel('Number of tags')
-        ax.set_ylabel('Yield %')
-        ax.set_ylim([-2, 112])
-        plt.ion()
-        plt.show()
-        prev_tests = 0
-        prev_val = 0
-        text_box = ax.text(0.68, 1.05, f"Yield: {prev_val:.2f} %", transform=ax.transAxes)
-
+        window = sg.Window('Upload CSV files', layout, modal=True)
         while True:
-            event, values = window.read(timeout=100)
-
-            new_num_rows = self.count_process.get_tested() + (self.rows_number * self.neg_col)
-            new_num_advas = self.adva_process.get_unq_advas()
-            # updating number of rows
-            if new_num_rows != num_rows:
-                num_rows = new_num_rows
-                num_rows_text_elem.update(f"{num_rows}")
-            # updating number of advas
-            if new_num_advas != num_advas:
-                num_advas = new_num_advas
-                num_advas_text_elem.update(f"{num_advas}")
-            # updating the graph
-            curr_tests = new_num_rows
-            curr_val = self.get_result()
-            plt.pause(0.01)
-            if curr_val > 100:
-                curr_val = 110
-            ax.plot([prev_tests, curr_tests], [prev_val, curr_val], color='red')
-            prev_tests = curr_tests
-            prev_val = curr_val
-            text_box.set_text(f"Yield : {curr_val:.2f} %")
-            # updating run_data_file
-            end_time = datetime.datetime.now()
-            run_end_time = end_time.strftime("%I:%M:%S")
-            advas = self.adva_process.get_unq_advas()
-            tags_num = self.count_process.get_tested()
-            result = self.get_result()
-            self.update_run_data_file(self.final_path_run_data, self.run_data_dict, formatted_date + ' ' + run_end_time,
-                                      tags_num, advas, result)
-            self.update_packet_data()
-
+            event, values = window.read()
             if event == sg.WIN_CLOSED or event in ('Stop', 'upload'):
                 if event == 'upload':
                     if values['upload'] == 'No':
                         self.upload_flag = False
                     else:
                         self.upload_flag = True  # if we press No then yes
                 if event == 'Stop':
-                    self.stop_button(window, run_end_time, tags_num, advas, result)
+                    self.stop.set()
+                    end_time = datetime.datetime.now()
+                    run_end_time = end_time.strftime("%I:%M:%S")
+                    advas = self.multi.adva_process.get_unq_advas()
+                    tags_num = self.multi.count_thread.get_tested()
+                    result = self.multi.get_result()
+                    cmn = self.wafer_lot + '.' + self.wafer_number + '_' + formatted_today + '_' + cur_time_formatted
+                    py_wiliot_version = get_version()
+                    d = WiliotDir()
+                    d.create_tester_dir(tester_name='yield_tester')
+                    yield_test_app_data = d.get_tester_dir('yield_tester')
+                    run_path = os.path.join(yield_test_app_data, cmn)
+                    if not os.path.exists(run_path):
+                        os.makedirs(run_path)
+                    final_path_run_data = os.path.join(run_path, cmn + '@run_data.csv')
+
+                    try:
+                        self.run_data_to_csv(csv_dictionary, final_path_run_data, cmn, run_end_time,
+                                             tags_num, advas, result, py_wiliot_version)
+                    except Exception as e:
+                        print(e)
+                    try:
+                        tag_df = self.multi.adva_process.all_tags.get_df()
+                        tag_df.insert(loc=len(tag_df.columns), column='common_run_name', value=cmn)
+                        final_path_packets_data = os.path.join(run_path, cmn + '@packets_data.csv')
+                        tag_df.to_csv(final_path_packets_data, index=False)
+                        if self.upload_flag:
+                            try:
+                                is_uploaded = upload_to_cloud_api(cmn, self.tester_type,
+                                                                  run_data_csv_name=final_path_run_data,
+                                                                  tags_data_csv_name=final_path_packets_data,
+                                                                  env='test',
+                                                                  packets_instead_tags=True, is_path=True)
+                                if is_uploaded:
+                                    print("Successful upload")
+                                else:
+                                    print("Unsuccessful upload")
+                            except Exception as e:
+                                print(e)
+                                print("Upload function failure")
+
+                    except Empty:
+                        print("NO PACKETS RECEIVED")
+
                     sub = True
                     break
                 if sub:
                     break
 
+        window.close()
         return sub
 
     def open_session(self):
         """
         opening a session for the process
         """
-        # save data to configs file
         if os.path.exists("configs/gui_input_do_not_delete.json"):
             with open("configs/gui_input_do_not_delete.json", "r") as f:
                 previous_input = json.load(f)
 
         else:
             previous_input = {'inlay': '', 'number': '', 'number_of_rows': '', 'received_channel': '',
                               'energy_pattern_val': '', 'time_profile_val': '', 'tester_station_name': '',
                               'comments': '', 'operator': '', 'wafer_lot': '', 'wafer_num': ''}
-        # update fields from configs
         selected_inlay = csv_dictionary[previous_input['inlay']]
         self.rows_number = selected_inlay['number_of_rows']
         energy_pat = selected_inlay['energy_pattern_val']
         time_pro = selected_inlay['time_profile_val']
         rec_channel = selected_inlay['received_channel']
         lst_inlay_options = list(inlay_types_dict.keys())
-
-
         layout = [
 
             [sg.Text('Wafer Lot:', font=4)],
-            [sg.InputText(previous_input['wafer_lot'], key='wafer_lot', font=4)],
+            [sg.InputText(key='wafer_lot', default_text=previous_input['wafer_lot'], font=4)],
 
             [sg.Text('Wafer Number:', font=4)],
-            [sg.InputText(previous_input['wafer_num'], key='wafer_num', font=4)],
-
-            [sg.Text('Number of neglected columns:', font=4)],
-            [sg.InputText(key='neg_col', font=4)],
+            [sg.InputText(key='wafer_num', default_text=previous_input['wafer_num'], font=4)],
 
             [sg.Text('Inlay:', font=4)],
             [sg.Combo(values=lst_inlay_options, default_value=previous_input['inlay'], key='inlay', font=4,
                       enable_events=True)],
 
             [
                 sg.Column([[sg.Text('Energy Pattern:', font=4),
                             sg.Text(energy_pat, key='energy_pattern_val', font=4)]]),
                 sg.Column([[sg.Text('Time Profile:', font=4),
                             sg.Text(time_pro, key='time_profile_val', font=4)]]),
                 sg.Column([[sg.Text('Number of rows:', font=4), sg.Text(self.rows_number, key='rows', font=4)]]),
                 sg.Column([[sg.Text('Received Channel:', font=4),
-                            sg.Text(rec_channel, key='received_channel', font=4)]])],
+                            sg.Text(rec_channel, key='received_channel', font=4)]])
+            ],
 
             [sg.Text('Tester Station Name:', font=4)],
             [sg.InputText(previous_input['tester_station_name'], key='tester_station_name', font=4)],
             [sg.Text('Comments:', font=4)],
             [sg.InputText(previous_input['comments'], key='comments', font=4)],
 
             [sg.Text('Operator:', font=4)],
             [sg.InputText(previous_input['operator'], key='operator', font=4)],
 
             [sg.Submit()]]
 
         window = sg.Window('WILIOT Yield Tester', layout, finalize=True)
 
-        inlay_select = ''
         while True:
-            event, values = window.read(timeout=100)
-            inlay_select = values['inlay']
-            self.selected = values['inlay']
+            event, values = window.read()
             if event == 'inlay':
                 inlay_select = values['inlay']
                 self.selected = values['inlay']
+                self.wafer_lot = values['wafer_lot']
+                self.wafer_number = values['wafer_num']
 
                 if inlay_select in csv_dictionary:
                     selected_inlay = csv_dictionary[inlay_select]
                     self.rows_number = selected_inlay['number_of_rows']
                     energy_pat = selected_inlay['energy_pattern_val']
                     time_pro = selected_inlay['time_profile_val']
                     rec_channel = selected_inlay['received_channel']
@@ -580,33 +479,26 @@
                     rec_channel = 'Invalid Selection'
 
                 window.find_element('rows').Update(value=self.rows_number)
                 window.find_element('energy_pattern_val').Update(value=energy_pat)
                 window.find_element('time_profile_val').Update(value=time_pro)
                 window.find_element('received_channel').Update(value=rec_channel)
             if event == 'Submit':  # Button clicked
-                if (values['neg_col']) == '':
-                    self.neg_col = 0
-                else:
-                    self.neg_col = int(values['neg_col'])
-                self.wafer_lot = values['wafer_lot']
-                self.wafer_number = values['wafer_num']
                 self.comments = values['comments']
                 self.tester_station_name = values['tester_station_name']
                 self.operator = values['operator']
-
-                self.init_processes(rec_channel, time_pro, energy_pat, inlay_select)
-                self.init_run_data()
-                self.start_processes()
-
+                self.multi = MultithreadedCalculation(self.stop, rec_channel,
+                                                      time_pro, energy_pat, self.rows_number)
+                self.gw_version = self.multi.adva_process.gw_instance.get_gw_version()[0]
+                self.multi.start()
                 with open("configs/gui_input_do_not_delete.json", "w") as f:
                     json.dump(values, f)
                 break
             elif event == sg.WIN_CLOSED:
                 exit()
 
         window.close()
 
 
 if __name__ == '__main__':
     m = MainWindow()
-    m.run()
+    m.run()
```

### Comparing `wiliot-testers-4.0.11/wiliot_testers.egg-info/PKG-INFO` & `wiliot-testers-4.0.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: wiliot-testers
-Version: 4.0.11
-Summary: A library for interacting with Wiliot's Testers app
-Home-page: UNKNOWN
-Author: Wiliot
-Author-email: support@wiliot.com
-License: MIT
-Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyWiliot: wiliot-testers #
 
 wiliot-testers is a python library for accessing Wiliot's Testers scripts
 
 ## Public Library
 
 ### MAC Installation
@@ -56,29 +39,15 @@
 * [Sample Test](wiliot_testers/sample/sample_test.py)
 * [Yield Tester](wiliot_testers/yield/yield_tester.py)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
-Version 4.0.11:
------------------
-* offline tester:
-    * fix bug when several tags under test and test status is still pass
-    * support 8 characters barcode label
-    * Support label scanner for both barcode and QR
-    * check printer communication during the run
-    
-* upload data:
-    * fix .bat file for upload data to the cloud
-    
-* sample test:
-    * fix script error when installing on a clean environment
-    
-    
+
 Version 4.0.6:
 -----------------
 * offline tester:
     *  update test suite.
     *  enable line selection using text communication with the printing (currently available only if printing offset > 0 and no QR check.
     *  add tag reel location to packet data csv (i.e. the location on the reel even if multiple runs were done on the same reel)
     *  check gw trigger (optic sensor signal) and apply printing validation, right after a trigger was received (or missing label was decided)
@@ -117,9 +86,7 @@
 Version 4.0.0:
 -----------------
 * First version
 
 
 The package previous content was published under the name 'wiliot' package.
 for more information please read 'wiliot' package's release notes
-
-
```

### Comparing `wiliot-testers-4.0.11/wiliot_testers.egg-info/SOURCES.txt` & `wiliot-testers-4.0.6/wiliot_testers.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,19 @@
 wiliot_testers/docs/__init__.py
 wiliot_testers/docs/tester_api_flow.pdf
 wiliot_testers/docs/wiliot_logo.png
 wiliot_testers/examples/__init__.py
 wiliot_testers/examples/wiliot_tester_example.py
 wiliot_testers/offline/README.md
 wiliot_testers/offline/__init__.py
-wiliot_testers/offline/barcode_test.py
 wiliot_testers/offline/env_install.bat
 wiliot_testers/offline/env_install.py
 wiliot_testers/offline/offline_tester.py
 wiliot_testers/offline/offline_utils.py
 wiliot_testers/offline/requirements.txt
-wiliot_testers/offline/run_barcode_testing.bat
 wiliot_testers/offline/run_offline_tester.bat
 wiliot_testers/offline/tadbik_r2r_controller.py
 wiliot_testers/offline/configs/__init__.py
 wiliot_testers/offline/configs/test_configs.json
 wiliot_testers/offline/configs/tests_suites.json
 wiliot_testers/offline/docs/__init__.py
 wiliot_testers/offline/docs/example_of_timing_diagram.jpg
@@ -76,15 +74,14 @@
 wiliot_testers/sample/utils/save.png
 wiliot_testers/sample/utils/wiliot3.gif
 wiliot_testers/system_test/__init__.py
 wiliot_testers/system_test/harvester_test.py
 wiliot_testers/system_test/system_test_example.py
 wiliot_testers/utils/__init__.py
 wiliot_testers/utils/get_version.py
-wiliot_testers/utils/upload_to_cloud_api.py
 wiliot_testers/yield/__init__.py
 wiliot_testers/yield/run_yield_tester.bat
 wiliot_testers/yield/yield_tester.py
 wiliot_testers/yield/arduino_counter/__init__.py
 wiliot_testers/yield/arduino_counter/arduino_counter.ino
 wiliot_testers/yield/configs/.default_configs.json
 wiliot_testers/yield/configs/__init__.py
```

