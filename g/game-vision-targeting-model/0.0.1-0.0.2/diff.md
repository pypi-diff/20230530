# Comparing `tmp/game-vision-targeting-model-0.0.1.tar.gz` & `tmp/game-vision-targeting-model-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "game-vision-targeting-model-0.0.1.tar", last modified: Tue May 30 17:20:07 2023, max compression
+gzip compressed data, was "game-vision-targeting-model-0.0.2.tar", last modified: Tue May 30 19:12:46 2023, max compression
```

## Comparing `game-vision-targeting-model-0.0.1.tar` & `game-vision-targeting-model-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 17:20:07.987691 game-vision-targeting-model-0.0.1/
--rw-rw-rw-   0        0        0      599 2023-05-30 17:20:07.986664 game-vision-targeting-model-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-30 17:20:07.984667 game-vision-targeting-model-0.0.1/game_vision_targeting_model.egg-info/
--rw-rw-rw-   0        0        0      599 2023-05-30 17:20:07.000000 game-vision-targeting-model-0.0.1/game_vision_targeting_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-05-30 17:20:07.000000 game-vision-targeting-model-0.0.1/game_vision_targeting_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 17:20:07.000000 game-vision-targeting-model-0.0.1/game_vision_targeting_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 17:20:07.000000 game-vision-targeting-model-0.0.1/game_vision_targeting_model.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      577 2023-05-30 17:19:25.000000 game-vision-targeting-model-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 17:20:07.987980 game-vision-targeting-model-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:46.512616 game-vision-targeting-model-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-30 19:12:46.512616 game-vision-targeting-model-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-30 19:12:28.000000 game-vision-targeting-model-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:12:46.512616 game-vision-targeting-model-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:46.512616 game-vision-targeting-model-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:46.512616 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:28.000000 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:46.512616 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:28.000000 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-30 19:12:28.000000 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/models/map_classifier_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:46.512616 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:28.000000 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:46.512616 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:28.000000 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-30 19:12:28.000000 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/variables/model_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:28.000000 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/variables/training_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-30 19:12:28.000000 game-vision-targeting-model-0.0.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:46.512616 game-vision-targeting-model-0.0.2/src/game_vision_targeting_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-30 19:12:45.000000 game-vision-targeting-model-0.0.2/src/game_vision_targeting_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-30 19:12:46.000000 game-vision-targeting-model-0.0.2/src/game_vision_targeting_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:12:45.000000 game-vision-targeting-model-0.0.2/src/game_vision_targeting_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 19:12:46.000000 game-vision-targeting-model-0.0.2/src/game_vision_targeting_model.egg-info/top_level.txt
```

### Comparing `game-vision-targeting-model-0.0.1/PKG-INFO` & `game-vision-targeting-model-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1
-Name: game-vision-targeting-model
-Version: 0.0.1
-Summary: A small example package
-Home-page: https://github.com/KentVejrupMadsen/gv-targeting-model
-Author-email: Kent vejrup Madsen <kent.vejrup.madsen@outlook.com>
-License: UNKNOWN
-Project-URL: Homepage, https://github.com/KentVejrupMadsen/gv-targeting-model
-Project-URL: Bug Tracker, https://github.com/KentVejrupMadsen/gv-targeting-model/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-# ML: Game targeting model
-
-
-
-
+Metadata-Version: 2.1
+Name: game-vision-targeting-model
+Version: 0.0.2
+Summary: A small example package
+Home-page: https://github.com/KentVejrupMadsen/gv-targeting-model
+Author-email: Kent vejrup Madsen <kent.vejrup.madsen@outlook.com>
+License: UNKNOWN
+Project-URL: Homepage, https://github.com/KentVejrupMadsen/gv-targeting-model
+Project-URL: Bug Tracker, https://github.com/KentVejrupMadsen/gv-targeting-model/issues
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+# ML: Game targeting model
+
+
+
+
```

### Comparing `game-vision-targeting-model-0.0.1/game_vision_targeting_model.egg-info/PKG-INFO` & `game-vision-targeting-model-0.0.2/src/game_vision_targeting_model.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1
-Name: game-vision-targeting-model
-Version: 0.0.1
-Summary: A small example package
-Home-page: https://github.com/KentVejrupMadsen/gv-targeting-model
-Author-email: Kent vejrup Madsen <kent.vejrup.madsen@outlook.com>
-License: UNKNOWN
-Project-URL: Homepage, https://github.com/KentVejrupMadsen/gv-targeting-model
-Project-URL: Bug Tracker, https://github.com/KentVejrupMadsen/gv-targeting-model/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-# ML: Game targeting model
-
-
-
-
+Metadata-Version: 2.1
+Name: game-vision-targeting-model
+Version: 0.0.2
+Summary: A small example package
+Home-page: https://github.com/KentVejrupMadsen/gv-targeting-model
+Author-email: Kent vejrup Madsen <kent.vejrup.madsen@outlook.com>
+License: UNKNOWN
+Project-URL: Homepage, https://github.com/KentVejrupMadsen/gv-targeting-model
+Project-URL: Bug Tracker, https://github.com/KentVejrupMadsen/gv-targeting-model/issues
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+# ML: Game targeting model
+
+
+
+
```

