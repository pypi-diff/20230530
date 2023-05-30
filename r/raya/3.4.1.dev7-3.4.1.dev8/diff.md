# Comparing `tmp/raya-3.4.1.dev7.tar.gz` & `tmp/raya-3.4.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raya-3.4.1.dev7.tar", last modified: Sat May 27 14:43:06 2023, max compression
+gzip compressed data, was "raya-3.4.1.dev8.tar", last modified: Tue May 30 00:10:04 2023, max compression
```

## Comparing `raya-3.4.1.dev7.tar` & `raya-3.4.1.dev8.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-27 14:43:06.965586 raya-3.4.1.dev7/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1074 2023-01-29 19:45:42.000000 raya-3.4.1.dev7/LICENSE
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      579 2023-05-27 14:43:06.965586 raya-3.4.1.dev7/PKG-INFO
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      150 2023-05-15 19:14:17.000000 raya-3.4.1.dev7/README.md
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      103 2023-01-29 19:45:42.000000 raya-3.4.1.dev7/pyproject.toml
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       38 2023-05-27 14:43:06.965586 raya-3.4.1.dev7/setup.cfg
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2752 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/setup.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-27 14:43:06.961586 raya-3.4.1.dev7/src/
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-27 14:43:06.961586 raya-3.4.1.dev7/src/raya/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       38 2023-05-15 19:14:17.000000 raya-3.4.1.dev7/src/raya/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       27 2023-05-27 14:42:25.000000 raya-3.4.1.dev7/src/raya/_version.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     3183 2023-05-27 14:43:05.000000 raya-3.4.1.dev7/src/raya/application_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      664 2023-05-27 14:43:05.000000 raya-3.4.1.dev7/src/raya/constants.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-27 14:43:06.961586 raya-3.4.1.dev7/src/raya/controllers/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-01-29 19:45:42.000000 raya-3.4.1.dev7/src/raya/controllers/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      260 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/controllers/analytics_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)    17375 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/controllers/arms_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      620 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/controllers/base_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       90 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/controllers/base_pseudo_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1222 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/controllers/cameras_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      425 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/controllers/communication_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2838 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/controllers/cv_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1387 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/controllers/fleet_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      523 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/controllers/grasping_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      924 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/controllers/interactions_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1298 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/controllers/leds_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1171 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/controllers/lidar_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     3127 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/controllers/manipulation_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2042 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/controllers/motion_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     7148 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/controllers/navigation_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1367 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/controllers/sensors_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      808 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/controllers/skills_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2590 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/controllers/sound_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     8614 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/controllers/ui_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       59 2023-05-27 14:43:05.000000 raya-3.4.1.dev7/src/raya/entry_point.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     4681 2023-05-27 14:43:05.000000 raya-3.4.1.dev7/src/raya/enumerations.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)    13055 2023-05-27 14:43:05.000000 raya-3.4.1.dev7/src/raya/exceptions.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6274 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/exceptions_handler.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-27 14:43:06.961586 raya-3.4.1.dev7/src/raya/handlers/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-05-15 19:15:31.000000 raya-3.4.1.dev7/src/raya/handlers/__init__.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-27 14:43:06.965586 raya-3.4.1.dev7/src/raya/handlers/cv/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-05-15 19:15:31.000000 raya-3.4.1.dev7/src/raya/handlers/cv/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      877 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/handlers/cv/classifier_handler_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      844 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/handlers/cv/detector_handler_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      743 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/handlers/cv/estimator_handler_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      302 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/handlers/cv/faces_detector_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      831 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/handlers/cv/faces_recognizer_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      305 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/handlers/cv/hand_estimator_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      183 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/handlers/cv/model_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      790 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/handlers/cv/objects_classifier_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      782 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/handlers/cv/objects_detector_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      794 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/handlers/cv/objects_segmentator_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      783 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/handlers/cv/planes_segmentator_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      862 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/handlers/cv/recognizer_handler_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      871 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/handlers/cv/segmentator_handler_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      703 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/handlers/cv/tags_detector_handler.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-27 14:43:06.965586 raya-3.4.1.dev7/src/raya/handlers/general/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-05-15 19:15:31.000000 raya-3.4.1.dev7/src/raya/handlers/general/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      330 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/handlers/general/callback_handler.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-27 14:43:06.965586 raya-3.4.1.dev7/src/raya/listeners/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-01-29 19:45:42.000000 raya-3.4.1.dev7/src/raya/listeners/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       77 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/listeners/lidar_listeners.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      160 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/listeners/sensors_listeners.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      352 2023-05-27 14:43:05.000000 raya-3.4.1.dev7/src/raya/logger.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2055 2023-05-27 14:43:05.000000 raya-3.4.1.dev7/src/raya/raya_interface.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      257 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/standalone_handler.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-27 14:43:06.965586 raya-3.4.1.dev7/src/raya/tools/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-01-29 19:45:42.000000 raya-3.4.1.dev7/src/raya/tools/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      399 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/tools/filesystem.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      984 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/tools/fsm.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      152 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya/tools/image.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-27 14:43:06.961586 raya-3.4.1.dev7/src/raya.egg-info/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      579 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya.egg-info/PKG-INFO
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2314 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya.egg-info/SOURCES.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        1 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya.egg-info/dependency_links.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        5 2023-05-27 14:43:06.000000 raya-3.4.1.dev7/src/raya.egg-info/top_level.txt
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-30 00:10:04.473423 raya-3.4.1.dev8/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1074 2023-01-29 19:45:42.000000 raya-3.4.1.dev8/LICENSE
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      579 2023-05-30 00:10:04.473423 raya-3.4.1.dev8/PKG-INFO
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      150 2023-05-15 19:14:17.000000 raya-3.4.1.dev8/README.md
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      103 2023-01-29 19:45:42.000000 raya-3.4.1.dev8/pyproject.toml
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       38 2023-05-30 00:10:04.473423 raya-3.4.1.dev8/setup.cfg
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2752 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/setup.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-30 00:10:04.469422 raya-3.4.1.dev8/src/
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-30 00:10:04.473423 raya-3.4.1.dev8/src/raya/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       38 2023-05-15 19:14:17.000000 raya-3.4.1.dev8/src/raya/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       27 2023-05-30 00:09:02.000000 raya-3.4.1.dev8/src/raya/_version.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     3183 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/application_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      664 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/constants.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-30 00:10:04.473423 raya-3.4.1.dev8/src/raya/controllers/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-01-29 19:45:42.000000 raya-3.4.1.dev8/src/raya/controllers/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      260 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/controllers/analytics_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)    17485 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/controllers/arms_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      620 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/controllers/base_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       90 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/controllers/base_pseudo_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1222 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/controllers/cameras_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      425 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/controllers/communication_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2838 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/controllers/cv_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1387 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/controllers/fleet_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      523 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/controllers/grasping_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      924 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/controllers/interactions_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1298 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/controllers/leds_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1171 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/controllers/lidar_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     3127 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/controllers/manipulation_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2042 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/controllers/motion_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     7148 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/controllers/navigation_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1367 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/controllers/sensors_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      808 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/controllers/skills_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2590 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/controllers/sound_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     8614 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/controllers/ui_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       59 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/entry_point.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     4681 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/enumerations.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)    13099 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/exceptions.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6272 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/exceptions_handler.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-30 00:10:04.473423 raya-3.4.1.dev8/src/raya/handlers/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-05-15 19:15:31.000000 raya-3.4.1.dev8/src/raya/handlers/__init__.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-30 00:10:04.473423 raya-3.4.1.dev8/src/raya/handlers/cv/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-05-15 19:15:31.000000 raya-3.4.1.dev8/src/raya/handlers/cv/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      877 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/handlers/cv/classifier_handler_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      844 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/handlers/cv/detector_handler_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      743 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/handlers/cv/estimator_handler_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      302 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/handlers/cv/faces_detector_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      831 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/handlers/cv/faces_recognizer_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      305 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/handlers/cv/hand_estimator_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      183 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/handlers/cv/model_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      790 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/handlers/cv/objects_classifier_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      782 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/handlers/cv/objects_detector_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      794 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/handlers/cv/objects_segmentator_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      783 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/handlers/cv/planes_segmentator_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      862 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/handlers/cv/recognizer_handler_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      871 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/handlers/cv/segmentator_handler_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      703 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/handlers/cv/tags_detector_handler.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-30 00:10:04.473423 raya-3.4.1.dev8/src/raya/handlers/general/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-05-15 19:15:31.000000 raya-3.4.1.dev8/src/raya/handlers/general/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      330 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/handlers/general/callback_handler.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-30 00:10:04.473423 raya-3.4.1.dev8/src/raya/listeners/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-01-29 19:45:42.000000 raya-3.4.1.dev8/src/raya/listeners/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       77 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/listeners/lidar_listeners.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      160 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/listeners/sensors_listeners.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      352 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/logger.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2055 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/raya_interface.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      257 2023-05-30 00:10:03.000000 raya-3.4.1.dev8/src/raya/standalone_handler.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-30 00:10:04.473423 raya-3.4.1.dev8/src/raya/tools/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-01-29 19:45:42.000000 raya-3.4.1.dev8/src/raya/tools/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      399 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/tools/filesystem.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      984 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/tools/fsm.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      152 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya/tools/image.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-30 00:10:04.473423 raya-3.4.1.dev8/src/raya.egg-info/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      579 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya.egg-info/PKG-INFO
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2314 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya.egg-info/SOURCES.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        1 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya.egg-info/dependency_links.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        5 2023-05-30 00:10:04.000000 raya-3.4.1.dev8/src/raya.egg-info/top_level.txt
```

### Comparing `raya-3.4.1.dev7/LICENSE` & `raya-3.4.1.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/PKG-INFO` & `raya-3.4.1.dev8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raya
-Version: 3.4.1.dev7
+Version: 3.4.1.dev8
 Summary: Unlimited Robotics - Ra-Ya Python Library
 Home-page: https://documentation.unlimited-robotics.com/
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Platform: UNKNOWN
```

### Comparing `raya-3.4.1.dev7/setup.py` & `raya-3.4.1.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/application_base.py` & `raya-3.4.1.dev8/src/raya/application_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/constants.py` & `raya-3.4.1.dev8/src/raya/constants.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/controllers/arms_controller.py` & `raya-3.4.1.dev8/src/raya/controllers/arms_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,23 @@
 
     def __init__(self, name: str, node: Node, app, extra_info={}):
         pass
 
     def get_list_of_arms(self):
         return
 
+    def get_list_of_groups(self):
+        return
+
     def get_state_of_arm(self, arm: str):
         return
 
+    def get_list_of_joints(self, arm: str):
+        return
+
     def get_limits_of_joints(self, arm: str, units: ANG_UNIT = ANG_UNIT.DEG):
         return
 
     async def is_any_arm_in_execution(self):
         return
 
     def are_checkings_in_progress(self):
```

### Comparing `raya-3.4.1.dev7/src/raya/controllers/base_controller.py` & `raya-3.4.1.dev8/src/raya/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/controllers/cameras_controller.py` & `raya-3.4.1.dev8/src/raya/controllers/cameras_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/controllers/cv_controller.py` & `raya-3.4.1.dev8/src/raya/controllers/cv_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/controllers/fleet_controller.py` & `raya-3.4.1.dev8/src/raya/controllers/fleet_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/controllers/grasping_controller.py` & `raya-3.4.1.dev8/src/raya/controllers/grasping_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/controllers/interactions_controller.py` & `raya-3.4.1.dev8/src/raya/controllers/interactions_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/controllers/leds_controller.py` & `raya-3.4.1.dev8/src/raya/controllers/leds_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/controllers/lidar_controller.py` & `raya-3.4.1.dev8/src/raya/controllers/lidar_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/controllers/manipulation_controller.py` & `raya-3.4.1.dev8/src/raya/controllers/manipulation_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/controllers/motion_controller.py` & `raya-3.4.1.dev8/src/raya/controllers/motion_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/controllers/navigation_controller.py` & `raya-3.4.1.dev8/src/raya/controllers/navigation_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/controllers/sensors_controller.py` & `raya-3.4.1.dev8/src/raya/controllers/sensors_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/controllers/skills_controller.py` & `raya-3.4.1.dev8/src/raya/controllers/skills_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/controllers/sound_controller.py` & `raya-3.4.1.dev8/src/raya/controllers/sound_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/controllers/ui_controller.py` & `raya-3.4.1.dev8/src/raya/controllers/ui_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/enumerations.py` & `raya-3.4.1.dev8/src/raya/enumerations.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/exceptions.py` & `raya-3.4.1.dev8/src/raya/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 class RayaException(Exception):
 
     def get_raya_file(self):
         return
 
 
-class RayaAbortException(RayaException):
+class RayaAbortException(Exception):
     pass
 
 
-class RayaNotStarted(RayaException):
+class RayaNotStarted(Exception):
     pass
 
 
-class RayaAppFinished(RayaException):
+class RayaAppFinished(Exception):
     pass
 
 
-class RayaAppAborted(RayaException):
+class RayaAppAborted(Exception):
     pass
 
 
 class RayaCommandException(RayaException):
     pass
 
 
@@ -756,14 +756,18 @@
     pass
 
 
 class RayaArmsNumberOfElementsNotMatch(RayaArmsException):
     pass
 
 
+class RayaArmsInvalidArmName(RayaArmsException):
+    pass
+
+
 class RayaArmsInvalidGroupName(RayaArmsException):
     pass
 
 
 class RayaArmsNotPoseArmDataAvailable(RayaArmsException):
     pass
```

### Comparing `raya-3.4.1.dev7/src/raya/exceptions_handler.py` & `raya-3.4.1.dev8/src/raya/exceptions_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     32: (RayaCVWrongCamera, ''),
     33: (RayaCVWrongCameraDepth, ''),
     34: (RayaCVRunningOtherCamera, ''),
     35: (RayaCVRunningOtherTagSize, '')
 }
 EXCEPTIONS_MAP_ARMS = {
     **EXCEPTIONS_MAP_GENERAL, 20: (RayaAlreadyMoving, ''),
-    21: (RayaArmsInvalidGroupName, ''),
+    21: (RayaArmsInvalidArmName, ''),
     22: (RayaArmsNotPoseArmDataAvailable, ''),
     23: (RayaArmsNotPredefinedPoseAvailable, ''),
     24: (RayaArmsInvalidNumberOfJoints, ''),
     25: (RayaArmsOutOfLimits, ''),
     26: (RayaArmsPredefinedPoseEmptyName, ''),
     27: (RayaArmsPredefinedPoseNameAlreadyExist, ''),
     28: (RayaArmsPredefinedPoseNameNotExist, ''),
```

### Comparing `raya-3.4.1.dev7/src/raya/handlers/cv/classifier_handler_base.py` & `raya-3.4.1.dev8/src/raya/handlers/cv/classifier_handler_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/handlers/cv/detector_handler_base.py` & `raya-3.4.1.dev8/src/raya/handlers/cv/detector_handler_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/handlers/cv/estimator_handler_base.py` & `raya-3.4.1.dev8/src/raya/handlers/cv/estimator_handler_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/handlers/cv/faces_recognizer_handler.py` & `raya-3.4.1.dev8/src/raya/handlers/cv/faces_recognizer_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/handlers/cv/objects_classifier_handler.py` & `raya-3.4.1.dev8/src/raya/handlers/cv/objects_classifier_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/handlers/cv/objects_detector_handler.py` & `raya-3.4.1.dev8/src/raya/handlers/cv/objects_detector_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/handlers/cv/objects_segmentator_handler.py` & `raya-3.4.1.dev8/src/raya/handlers/cv/objects_segmentator_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/handlers/cv/planes_segmentator_handler.py` & `raya-3.4.1.dev8/src/raya/handlers/cv/planes_segmentator_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/handlers/cv/recognizer_handler_base.py` & `raya-3.4.1.dev8/src/raya/handlers/cv/recognizer_handler_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/handlers/cv/segmentator_handler_base.py` & `raya-3.4.1.dev8/src/raya/handlers/cv/segmentator_handler_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/handlers/cv/tags_detector_handler.py` & `raya-3.4.1.dev8/src/raya/handlers/cv/tags_detector_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/raya_interface.py` & `raya-3.4.1.dev8/src/raya/raya_interface.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya/tools/fsm.py` & `raya-3.4.1.dev8/src/raya/tools/fsm.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev7/src/raya.egg-info/PKG-INFO` & `raya-3.4.1.dev8/src/raya.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raya
-Version: 3.4.1.dev7
+Version: 3.4.1.dev8
 Summary: Unlimited Robotics - Ra-Ya Python Library
 Home-page: https://documentation.unlimited-robotics.com/
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Platform: UNKNOWN
```

### Comparing `raya-3.4.1.dev7/src/raya.egg-info/SOURCES.txt` & `raya-3.4.1.dev8/src/raya.egg-info/SOURCES.txt`

 * *Files identical despite different names*

