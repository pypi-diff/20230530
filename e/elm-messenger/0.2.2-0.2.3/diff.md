# Comparing `tmp/elm-messenger-0.2.2.tar.gz` & `tmp/elm-messenger-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm-messenger-0.2.2.tar", last modified: Tue May 30 00:47:58 2023, max compression
+gzip compressed data, was "elm-messenger-0.2.3.tar", last modified: Tue May 30 01:24:28 2023, max compression
```

## Comparing `elm-messenger-0.2.2.tar` & `elm-messenger-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-30 00:47:58.096549 elm-messenger-0.2.2/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.2.2/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-30 00:47:58.096549 elm-messenger-0.2.2/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.2.2/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-30 00:47:58.096549 elm-messenger-0.2.2/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-30 00:47:58.000000 elm-messenger-0.2.2/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      392 2023-05-30 00:47:58.000000 elm-messenger-0.2.2/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-30 00:47:58.000000 elm-messenger-0.2.2/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-30 00:47:58.000000 elm-messenger-0.2.2/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       16 2023-05-30 00:47:58.000000 elm-messenger-0.2.2/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-30 00:47:58.000000 elm-messenger-0.2.2/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-30 00:47:58.096549 elm-messenger-0.2.2/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.2.2/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.2.2/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)    18539 2023-05-30 00:30:00.000000 elm-messenger-0.2.2/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      771 2023-05-27 16:23:18.000000 elm-messenger-0.2.2/messengercli/patcher.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.2.2/messengercli/updater.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      418 2023-05-30 00:47:58.096549 elm-messenger-0.2.2/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.2.2/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-30 01:24:28.690950 elm-messenger-0.2.3/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.2.3/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-30 01:24:28.690950 elm-messenger-0.2.3/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.2.3/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-30 01:24:28.690950 elm-messenger-0.2.3/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-30 01:24:28.000000 elm-messenger-0.2.3/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      392 2023-05-30 01:24:28.000000 elm-messenger-0.2.3/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-30 01:24:28.000000 elm-messenger-0.2.3/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-30 01:24:28.000000 elm-messenger-0.2.3/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       16 2023-05-30 01:24:28.000000 elm-messenger-0.2.3/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-30 01:24:28.000000 elm-messenger-0.2.3/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-30 01:24:28.690950 elm-messenger-0.2.3/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.2.3/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.2.3/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)    18539 2023-05-30 01:23:48.000000 elm-messenger-0.2.3/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      771 2023-05-27 16:23:18.000000 elm-messenger-0.2.3/messengercli/patcher.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.2.3/messengercli/updater.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      418 2023-05-30 01:24:28.690950 elm-messenger-0.2.3/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.2.3/setup.py
```

### Comparing `elm-messenger-0.2.2/messengercli/messenger.py` & `elm-messenger-0.2.3/messengercli/messenger.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import os
 import shutil
 import json
 from .updater import Updater
 from .patcher import patch
 
 app = typer.Typer(add_completion=False, help="Messenger CLI")
-API_VERSION = "0.2.2"
+API_VERSION = "0.2.3"
 
 
 class Messenger:
     config = None
 
     def __init__(self) -> None:
         """
@@ -48,34 +48,34 @@
 
         Updater(
             [
                 ".messenger/scene/Sample/Export.elm",
                 ".messenger/scene/Sample/Global.elm",
                 ".messenger/scene/Sample/Model.elm",
                 ".messenger/scene/Sample/LayerBase.elm",
-                ".messenger/scene/Sample/LayerInit.elm",
+                ".messenger/scene/Sample/SceneInit.elm",
             ],
             [
                 f"src/Scenes/{scene}/Export.elm",
                 f"src/Scenes/{scene}/Global.elm",
                 f"src/Scenes/{scene}/Model.elm",
                 f"src/Scenes/{scene}/LayerBase.elm",
-                f"src/Scenes/{scene}/LayerInit.elm",
+                f"src/Scenes/{scene}/SceneInit.elm",
             ],
         ).rep(scene)
 
         # Modify Scene
         with open("src/Lib/Scene/Base.elm", "r") as f:
             scenebase = f.read()
         new_scenebase = scenebase.replace(
             "type SceneInitData\n    =",
             f"type SceneInitData\n    = {scene}InitData {scene}Init\n    |",
         ).replace(
             "import Lib.Env.Env exposing (Env)",
-            f"import Lib.Env.Env exposing (Env)\nimport Scenes.{scene}.LayerInit exposing ({scene}Init)",
+            f"import Lib.Env.Env exposing (Env)\nimport Scenes.{scene}.SceneInit exposing ({scene}Init)",
         )
         with open("src/Lib/Scene/Base.elm", "w") as f:
             f.write(new_scenebase)
 
     def update_scenes(self):
         """
         Update scene settings (AllScenes and SceneSettings)
@@ -145,38 +145,38 @@
 
         Updater(
             [
                 ".messenger/sceneproto/scene/Export.elm",
                 ".messenger/sceneproto/scene/Global.elm",
                 ".messenger/sceneproto/scene/Model.elm",
                 ".messenger/sceneproto/scene/LayerBase.elm",
-                ".messenger/sceneproto/scene/LayerInit.elm",
+                ".messenger/sceneproto/scene/SceneInit.elm",
                 ".messenger/sceneproto/gamecomponent/Base.elm",
                 ".messenger/sceneproto/gamecomponent/Handler.elm",
             ],
             [
                 f"src/SceneProtos/{scene}/Export.elm",
                 f"src/SceneProtos/{scene}/Global.elm",
                 f"src/SceneProtos/{scene}/Model.elm",
                 f"src/SceneProtos/{scene}/LayerBase.elm",
-                f"src/SceneProtos/{scene}/LayerInit.elm",
+                f"src/SceneProtos/{scene}/SceneInit.elm",
                 f"src/SceneProtos/{scene}/GameComponent/Base.elm",
                 f"src/SceneProtos/{scene}/GameComponent/Handler.elm",
             ],
         ).rep(scene)
 
         # Modify Scene
         with open("src/Lib/Scene/Base.elm", "r") as f:
             scenebase = f.read()
         new_scenebase = scenebase.replace(
             "type SceneInitData\n    =",
             f"type SceneInitData\n    = {scene}InitData {scene}Init\n    |",
         ).replace(
             "import Lib.Env.Env exposing (Env)",
-            f"import Lib.Env.Env exposing (Env)\nimport SceneProtos.{scene}.LayerInit exposing ({scene}Init)",
+            f"import Lib.Env.Env exposing (Env)\nimport SceneProtos.{scene}.SceneInit exposing ({scene}Init)",
         )
         with open("src/Lib/Scene/Base.elm", "w") as f:
             f.write(new_scenebase)
 
     def add_sceneproto_layer(self, sceneproto: str, layer: str):
         """
         Add a layer in one sceneproto
```

### Comparing `elm-messenger-0.2.2/messengercli/patcher.py` & `elm-messenger-0.2.3/messengercli/patcher.py`

 * *Files identical despite different names*

### Comparing `elm-messenger-0.2.2/messengercli/updater.py` & `elm-messenger-0.2.3/messengercli/updater.py`

 * *Files identical despite different names*

