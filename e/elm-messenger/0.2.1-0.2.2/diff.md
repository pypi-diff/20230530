# Comparing `tmp/elm-messenger-0.2.1.tar.gz` & `tmp/elm-messenger-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm-messenger-0.2.1.tar", last modified: Sat May 27 16:00:29 2023, max compression
+gzip compressed data, was "elm-messenger-0.2.2.tar", last modified: Tue May 30 00:47:58 2023, max compression
```

## Comparing `elm-messenger-0.2.1.tar` & `elm-messenger-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-27 16:00:29.127185 elm-messenger-0.2.1/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.2.1/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-27 16:00:29.127185 elm-messenger-0.2.1/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.2.1/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-27 16:00:29.123852 elm-messenger-0.2.1/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-27 16:00:29.000000 elm-messenger-0.2.1/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      392 2023-05-27 16:00:29.000000 elm-messenger-0.2.1/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-27 16:00:29.000000 elm-messenger-0.2.1/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-27 16:00:29.000000 elm-messenger-0.2.1/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       16 2023-05-27 16:00:29.000000 elm-messenger-0.2.1/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-27 16:00:29.000000 elm-messenger-0.2.1/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-27 16:00:29.123852 elm-messenger-0.2.1/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.2.1/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.2.1/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)    18588 2023-05-27 15:53:54.000000 elm-messenger-0.2.1/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      771 2023-05-27 15:51:04.000000 elm-messenger-0.2.1/messengercli/patcher.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.2.1/messengercli/updater.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      418 2023-05-27 16:00:29.127185 elm-messenger-0.2.1/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.2.1/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-30 00:47:58.096549 elm-messenger-0.2.2/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.2.2/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-30 00:47:58.096549 elm-messenger-0.2.2/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.2.2/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-30 00:47:58.096549 elm-messenger-0.2.2/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-30 00:47:58.000000 elm-messenger-0.2.2/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      392 2023-05-30 00:47:58.000000 elm-messenger-0.2.2/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-30 00:47:58.000000 elm-messenger-0.2.2/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-30 00:47:58.000000 elm-messenger-0.2.2/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       16 2023-05-30 00:47:58.000000 elm-messenger-0.2.2/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-30 00:47:58.000000 elm-messenger-0.2.2/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-30 00:47:58.096549 elm-messenger-0.2.2/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.2.2/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.2.2/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)    18539 2023-05-30 00:30:00.000000 elm-messenger-0.2.2/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      771 2023-05-27 16:23:18.000000 elm-messenger-0.2.2/messengercli/patcher.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.2.2/messengercli/updater.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      418 2023-05-30 00:47:58.096549 elm-messenger-0.2.2/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.2.2/setup.py
```

### Comparing `elm-messenger-0.2.1/messengercli/messenger.py` & `elm-messenger-0.2.2/messengercli/messenger.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import os
 import shutil
 import json
 from .updater import Updater
 from .patcher import patch
 
 app = typer.Typer(add_completion=False, help="Messenger CLI")
-API_VERSION = "0.2.1"
+API_VERSION = "0.2.2"
 
 
 class Messenger:
     config = None
 
     def __init__(self) -> None:
         """
@@ -229,15 +229,15 @@
                     f"import SceneProtos.{sceneproto}.{l}.Export as {l}\nimport SceneProtos.{sceneproto}.{l}.Global as {l}G"
                     for l in layers
                 ]
             )
         ).rep(
             ",\n".join(
                 [
-                    f"{l}G.getLayerT <| {l}.initLayer (addCommonData nullCommonData env) ({l}.initFromScene env layerInitData)"
+                    f"{l}G.getLayerT <| {l}.initLayer (addCommonData nullCommonData env) layerInitData"
                     for l in layers
                 ]
             )
         )
 
     def add_level(self, sceneproto: str, level: str):
         """
@@ -365,15 +365,15 @@
                     f"import Scenes.{scene}.{l}.Export as {l}\nimport Scenes.{scene}.{l}.Global as {l}G"
                     for l in layers
                 ]
             )
         ).rep(
             ",\n".join(
                 [
-                    f"{l}G.getLayerT <| {l}.initLayer (addCommonData nullCommonData env)  ({l}.initFromScene env layerInitData)"
+                    f"{l}G.getLayerT <| {l}.initLayer (addCommonData nullCommonData env) layerInitData"
                     for l in layers
                 ]
             )
         )
 
 
 @app.command()
```

### Comparing `elm-messenger-0.2.1/messengercli/patcher.py` & `elm-messenger-0.2.2/messengercli/patcher.py`

 * *Files identical despite different names*

### Comparing `elm-messenger-0.2.1/messengercli/updater.py` & `elm-messenger-0.2.2/messengercli/updater.py`

 * *Files identical despite different names*

