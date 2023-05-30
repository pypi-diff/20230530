# Comparing `tmp/elm-messenger-0.2.3.tar.gz` & `tmp/elm-messenger-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm-messenger-0.2.3.tar", last modified: Tue May 30 01:24:28 2023, max compression
+gzip compressed data, was "elm-messenger-0.2.4.tar", last modified: Tue May 30 02:10:57 2023, max compression
```

## Comparing `elm-messenger-0.2.3.tar` & `elm-messenger-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-30 01:24:28.690950 elm-messenger-0.2.3/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.2.3/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-30 01:24:28.690950 elm-messenger-0.2.3/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.2.3/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-30 01:24:28.690950 elm-messenger-0.2.3/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-30 01:24:28.000000 elm-messenger-0.2.3/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      392 2023-05-30 01:24:28.000000 elm-messenger-0.2.3/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-30 01:24:28.000000 elm-messenger-0.2.3/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-30 01:24:28.000000 elm-messenger-0.2.3/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       16 2023-05-30 01:24:28.000000 elm-messenger-0.2.3/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-30 01:24:28.000000 elm-messenger-0.2.3/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-30 01:24:28.690950 elm-messenger-0.2.3/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.2.3/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.2.3/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)    18539 2023-05-30 01:23:48.000000 elm-messenger-0.2.3/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      771 2023-05-27 16:23:18.000000 elm-messenger-0.2.3/messengercli/patcher.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.2.3/messengercli/updater.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      418 2023-05-30 01:24:28.690950 elm-messenger-0.2.3/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.2.3/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-30 02:10:57.766738 elm-messenger-0.2.4/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.2.4/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-30 02:10:57.766738 elm-messenger-0.2.4/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.2.4/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-30 02:10:57.766738 elm-messenger-0.2.4/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-30 02:10:57.000000 elm-messenger-0.2.4/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      392 2023-05-30 02:10:57.000000 elm-messenger-0.2.4/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-30 02:10:57.000000 elm-messenger-0.2.4/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-30 02:10:57.000000 elm-messenger-0.2.4/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       16 2023-05-30 02:10:57.000000 elm-messenger-0.2.4/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-30 02:10:57.000000 elm-messenger-0.2.4/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-30 02:10:57.766738 elm-messenger-0.2.4/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.2.4/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.2.4/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)    18770 2023-05-30 02:08:02.000000 elm-messenger-0.2.4/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      771 2023-05-27 16:23:18.000000 elm-messenger-0.2.4/messengercli/patcher.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.2.4/messengercli/updater.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      418 2023-05-30 02:10:57.766738 elm-messenger-0.2.4/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.2.4/setup.py
```

### Comparing `elm-messenger-0.2.3/messengercli/messenger.py` & `elm-messenger-0.2.4/messengercli/messenger.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import os
 import shutil
 import json
 from .updater import Updater
 from .patcher import patch
 
 app = typer.Typer(add_completion=False, help="Messenger CLI")
-API_VERSION = "0.2.3"
+API_VERSION = "0.2.4"
 
 
 class Messenger:
     config = None
 
     def __init__(self) -> None:
         """
@@ -30,14 +30,18 @@
                 raise Exception("Messenger API version not found in the config file.")
             if self.config["version"] != API_VERSION:
                 raise Exception(f"Messenger API version not matched. I'm using v{API_VERSION}. You can edit messenger.json manually to upgrade.")
         else:
             raise Exception(
                 "messenger.json not found. Are you in the project initialized by the Messenger? Try `messenger init <your-project-name>`."
             )
+        if not os.path.exists(".messenger"):
+            print("Messenger files not found. Initializing...")
+            os.system(f"git clone {self.config['template_repo']} .messenger --depth=1")
+
 
     def dump_config(self):
         with open("messenger.json", "w") as f:
             json.dump(self.config, f, indent=4, ensure_ascii=False)
 
     def add_scene(self, scene: str):
         if scene in self.config["scenes"] or scene in self.config["sceneprotos"]:
@@ -410,15 +414,15 @@
 
     os.makedirs("src/Scenes", exist_ok=True)
     os.makedirs("assets", exist_ok=True)
     os.makedirs("src/Components", exist_ok=True)
     os.makedirs("src/SceneProtos", exist_ok=True)
 
     print("Creating elm.json...")
-    initObject = {"version": API_VERSION, "scenes": {}, "sceneprotos": {}}
+    initObject = {"version": API_VERSION, "template_repo" : template_repo, "scenes": {}, "sceneprotos": {}}
     with open("messenger.json", "w") as f:
         json.dump(initObject, f, indent=4, ensure_ascii=False)
     print("Installing dependencies...")
     os.system("elm make")
     print("Done!")
     print(f"Now please go to {name} and add scenes and components.")
```

### Comparing `elm-messenger-0.2.3/messengercli/patcher.py` & `elm-messenger-0.2.4/messengercli/patcher.py`

 * *Files identical despite different names*

### Comparing `elm-messenger-0.2.3/messengercli/updater.py` & `elm-messenger-0.2.4/messengercli/updater.py`

 * *Files identical despite different names*

