# Comparing `tmp/wmwpy-0.3.0b0.tar.gz` & `tmp/wmwpy-0.4.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wmwpy-0.3.0b0.tar", last modified: Tue May 23 20:25:37 2023, max compression
+gzip compressed data, was "wmwpy-0.4.0b0.tar", last modified: Tue May 30 20:42:16 2023, max compression
```

## Comparing `wmwpy-0.3.0b0.tar` & `wmwpy-0.4.0b0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:25:37.018346 wmwpy-0.3.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42049 2023-05-23 20:25:37.018346 wmwpy-0.3.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:25:37.018346 wmwpy-0.3.0b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:25:37.010346 wmwpy-0.3.0b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:25:37.014346 wmwpy-0.3.0b0/src/wmwpy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:25:37.014346 wmwpy-0.3.0b0/src/wmwpy/Font/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Font/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:25:37.014346 wmwpy-0.3.0b0/src/wmwpy/Utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:25:37.014346 wmwpy-0.3.0b0/src/wmwpy/Utils/Types/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/Types/Documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/Types/Images.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/Types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/XMLTools.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21854 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/textures.py
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/waltex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:25:37.014346 wmwpy-0.3.0b0/src/wmwpy/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/Widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    22504 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/imagelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    14141 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/level.py
--rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/sprite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:25:37.018346 wmwpy-0.3.0b0/src/wmwpy/classes/widget/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_CANVAS.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_FINGER_CATCHER.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_GROUP.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_ICON_LIST.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_LABEL.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_PROGRESS_BAR.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_PUSH_BUTTON.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_SCROLLABLE_CAMERA.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_SCROLLABLE_SET.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_SLIDER.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_TOGGLE.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/game.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/gameobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/gametemplate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:25:37.014346 wmwpy-0.3.0b0/src/wmwpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42049 2023-05-23 20:25:37.000000 wmwpy-0.3.0b0/src/wmwpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-23 20:25:37.000000 wmwpy-0.3.0b0/src/wmwpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:25:37.000000 wmwpy-0.3.0b0/src/wmwpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:25:37.000000 wmwpy-0.3.0b0/src/wmwpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 20:25:37.000000 wmwpy-0.3.0b0/src/wmwpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:42:16.723925 wmwpy-0.4.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    49356 2023-05-30 20:42:16.723925 wmwpy-0.4.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8230 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 20:42:16.723925 wmwpy-0.4.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:42:16.711925 wmwpy-0.4.0b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:42:16.715925 wmwpy-0.4.0b0/src/wmwpy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:42:16.715925 wmwpy-0.4.0b0/src/wmwpy/Font/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Font/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:42:16.715925 wmwpy-0.4.0b0/src/wmwpy/Utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:42:16.715925 wmwpy-0.4.0b0/src/wmwpy/Utils/Types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/Types/Documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/Types/Images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/Types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/XMLTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22603 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/gif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/textures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/waltex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:42:16.719925 wmwpy-0.4.0b0/src/wmwpy/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/Widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26480 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/imagelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23989 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25624 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/sprite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:42:16.723925 wmwpy-0.4.0b0/src/wmwpy/classes/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_CANVAS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_FINGER_CATCHER.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_GROUP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_ICON_LIST.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_LABEL.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_PROGRESS_BAR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_PUSH_BUTTON.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_SCROLLABLE_CAMERA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_SCROLLABLE_SET.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_SLIDER.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_TOGGLE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/gameobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/gametemplate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:42:16.715925 wmwpy-0.4.0b0/src/wmwpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49356 2023-05-30 20:42:16.000000 wmwpy-0.4.0b0/src/wmwpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-30 20:42:16.000000 wmwpy-0.4.0b0/src/wmwpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:42:16.000000 wmwpy-0.4.0b0/src/wmwpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 20:42:16.000000 wmwpy-0.4.0b0/src/wmwpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 20:42:16.000000 wmwpy-0.4.0b0/src/wmwpy.egg-info/top_level.txt
```

### Comparing `wmwpy-0.3.0b0/LICENSE` & `wmwpy-0.4.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `wmwpy-0.3.0b0/PKG-INFO` & `wmwpy-0.4.0b0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmwpy
-Version: 0.3.0b0
+Version: 0.4.0b0
 Summary: Python module to work with Where's My...? games files.
 Author: ego-lay-atman-bay
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -685,23 +685,336 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wmwpy
- Python module for working with Where's My...? game files.
+Python module for working with Where's My...? game files.
 
- <!-- Note: using https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/ for distributing.-->
+<!-- Note: using https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/ for distributing.-->
 
- This is going to be used in Where's My Editor, a level editor for the Where's My...? series.
+This is being used in [Where's My Editor](https://github.com/wmw-modding/wheres-my-editor), a level editor for the Where's My...? series.
+
+
+# Table of contents
+
+- [wmwpy](#wmwpy)
+- [Table of contents](#table-of-contents)
+- [Installation](#installation)
+- [Usage](#usage)
+  - [Get game folder](#get-game-folder)
+  - [Loading the game](#loading-the-game)
+  - [Main classes](#main-classes)
+    - [Level](#level)
+      - [Challenges](#challenges)
+    - [Object](#object)
+- [Building package](#building-package)
+- [Building docs](#building-docs)
+- [Credits](#credits)
+
+# Installation
+To install `wmwpy`, run
+
+```
+pip install wmwpy
+```
+
+or
+
+```
+python -m pip install wmwpy
+```
+
+You can also install it from the source, which may be needed because it is frequently being updated, although you need to make sure `git` is installed.
+
+```
+pip install wmwpy@git+https://github.com/wmw-modding/wmwpy
+```
+
+# Usage
+## Get game folder
+To get started, you need to have a Where's My Water? game folder, either an extracted apk, ipa, or on a rooted / jailbroken device (for editing the game files directly). The game must be extracted like this.
+
+```
+- root
+ - assets
+  - ...
+```
+ 
+The assets folder can be specified in `wmwpy`.
+
+## Loading the game
+Start by loading the game inside `wmwpy`
+
+```python
+import wmwpy
+game = wmwpy.load('game/wmw')
+```
+
+You can specify the assets folder
+
+```python
+game = wmwpy.load('game/wmw', assets = '/assets')
+```
+
+You can set `assets = '.'` if you have the gamepath (first parameter) set to the assets folder (such as on a rooted / jailbroken device).
+
+Alternately, you can specify the platform.
+
+```python
+game = wmwpy.load('game/wmw', platform = 'android')
+```
+
+This automatically sets the assets folder to what it is on the platform.
+
+| Platform | assets folder |
+| -------- | ------------- |
+| android  | /assets       |
+| ios      | /Content      |
+
+You can also specify the game, which sets things up for that game.
+
+```python
+game = wmwpy.load('game/wmp', game = 'WMP')
+```
+
+Currently all the games are
+
+| Game                                   | Code      |
+| ----                                   | ----      |
+| Where's My Water?                      | 'WMW'     |
+| Where's My Water? Free                 | 'WMWF'    |
+| Where's My Perry?                      | 'WMP'     |
+| Where's My Perry? Free                 | 'WMPF'    |
+| Where's My Mickey?                     | 'WMM'     |
+| Where's My Mickey? XL                  | 'WMMXL'   |
+| Where's My Mickey? Free                | 'WMMF'    |
+| Where's My XiYangYang?                 | 'WMXYY'   |
+| Where's My Water? Featuring XiYangYang | 'WMWFXYY' |
+| Where's My Water? 2                    | 'WMW2'    |
+| Where's My Holiday?                    | 'WMH'     |
+| Where's My Valentine?                  | 'WMV'     |
+| Where's My Summer?                     | 'WMS'     |
+
+You can also specify the base assets path, the folder within the assets folder that contains all the assets. For example, Where's My Perry? has all the data within `/assets/Perry`.
+
+```python
+game = wmwpy.load('game/wmp', baseassets = '/Perry')
+```
+
+Each game has the database in a different location, so you can specify it.
+
+```python
+game = wmwpy.load('game/wmp', db = '/Perry/Data/perry.db')
+```
+
+Since Where's My Water? 2 uses a profile instead of a database for the save data, you can also specify that.
+
+```python
+game = wmwpy.load('game/wmw2', profile = '/Water/Data/factory_profile.json')
+```
+
+You can also provide a function to be called during the loading, so you can keep track of the current progress, e.g. in a gui application with a progress bar.
+
+```python
+game = wmwpy.load('game/wmw', load_hook = lambda progress, text, max : print(f'({progress}/{max}) {text}'))
+```
+
+The inputs for the function are
+```
+(
+   progress : int,
+   text : str,
+   max : int,
+)
+```
+
+Once you're done editing all the files, you need to dump the all the assets.
+
+```python
+game.dump()
+```
+
+This will save all the files in the game inside the assets folder. You can customize this if you want them saved in a different location.
+
+```python
+game.dump(folder = 'path/to/output')
+```
+
+## Main classes
+
+### Level
+To load a level from within a game, use the `.Level()` method.
+
+```python
+level = game.Level('first_dig')
+```
+
+The first input can be the name of a level inside the `/Levels` folder (`first_dig`), an absolute path to the level (`/Levels/first_dig`), or the path to an xml file (`/Levels/first_dig.xml`).
+
+You can also specify the xml and image separately.
+
+```python
+level = game.Level(xmlPath = '/Levels/first_dig.xml', imagePath = '/Levels/first_dig.png')
+```
+
+Some levels include objects that wmwpy fails to load, so you can use the `ignore_errors` parameter to ignore them.
+
+```python
+level = game.Level('first_dig', ignore_errors = True)
+```
+
+You can also use the HD or TabHD textures for the objects.
+
+```python
+level = game.Level('first_dig', HD = True, TabHD = True)
+```
+
+If both are specified, TabHD will get priority. If it can't load TabHD textures. See hierarchy.
+
+```
+- TabHD
+ - HD
+  - Low Quality
+```
+
+You can also provide a function to run while loading to see the current progress.
+
+```python
+level = game.Level('first_dig', load_callback = lambda progress, text, max : print(f'({progress}/{max}) {text}'))
+```
+
+The inputs for the function are
+```
+(
+   progress : int,
+   text : str,
+   max : int,
+)
+```
+
+The objects in the level are all accessible in a list
+
+```python
+>> level.objects
+[
+   <wmwpy.classes.object.Object object at 0x000001C7627FE850>,
+   ...
+]
+```
+
+See [Object](#Object)
+
+The level properties are also accessible as a dictionary
+
+```python
+>> level.properties
+{'HeavyIntro': '1'}
+```
+
+WMW2 challenges are also accessible in a list
+
+```python
+>> level.challenges
+[<wmwpy.classes.level.Level.Challenge object at 0x000001C72176ADD0>]
+```
+
+Once you're finished editing the level, you can get the xml.
+
+```python
+xml = level.export(filename = '/Levels/first_dig.xml',)
+```
+
+This returns the xml file as `bytes`, but also saves the file to the game filesystem.
+
+#### Challenges
+Each challenge has requirements in a dictionary
+```python
+>> level.challenges[0].requirements
+{
+    'WinWait': {
+        'seconds': ''
+    },
+    'Duck': {
+        'count': '2'
+    }
+}
+```
+
+### Object
+To load an object within a game, use the `.Object()` method.
+
+```python
+obj = game.Object('/Objects/broken_pipe.hs')
+```
+
+You can also use the HD or TabHD textures for the objects.
+
+```python
+level = game.Level('first_dig', HD = True, TabHD = True)
+```
+
+If both are specified, TabHD will get priority. If it can't load TabHD textures. See hierarchy.
+
+```
+- TabHD
+ - HD
+  - Low Quality
+```
+
+An object has many properties
+
+```python
+>> obj.properties
+{
+    'Type' : 'spout',
+    'SpoutType' : 'DrainSpout',
+    'Goal' : '1',
+    'GoalPreset', : 'Swampy',
+}
+```
+
+An object also has many [Sprites](#Sprite)
+
+```python
+>> obj.sprites
+[<wmwpy.classes.sprite.Sprite object>]
+```
+
+The object image is a `PIL` image.
+
+```python
+>> obj.image
+<PIL.Image.Image image mode=RGBA size=300x300>
+```
+
+The image scale can be set
+
+```python
+obj.scale = 20
+```
+
+You can also save a GIF of the object animations
+
+```python
+obj.saveGIF('broken_pipe.gif')
+```
+
+Once you're finished editing the object, you can get the xml.
+
+```python
+xml = export('/Objects/broken_pipe.hs',)
+```
+
+This returns the xml file as `bytes`, but also saves the file to the game filesystem.
 
 # Building package
- To build the package, install `build`
- ```
+To build the package, install `build`
+```
 pip install build
  ```
  Then run
  ```
 py -m build
  ```
```

### Comparing `wmwpy-0.3.0b0/pyproject.toml` & `wmwpy-0.4.0b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wmwpy-0.3.0b0/src/wmwpy/Utils/Types/Documents.py` & `wmwpy-0.4.0b0/src/wmwpy/Utils/Types/Documents.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.3.0b0/src/wmwpy/Utils/Types/Images.py` & `wmwpy-0.4.0b0/src/wmwpy/Utils/Types/Images.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.3.0b0/src/wmwpy/Utils/XMLTools.py` & `wmwpy-0.4.0b0/src/wmwpy/Utils/XMLTools.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.3.0b0/src/wmwpy/Utils/filesystem.py` & `wmwpy-0.4.0b0/src/wmwpy/Utils/filesystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import io
 from filetype import filetype
 from PIL import Image
 import zipfile
 import natsort
 import typing
 import fnmatch
+import logging
 
 from .path import joinPath
 # from . import Waltex
 # from . import ImageUtils
 # from ..classes import sprite
 # from ..classes import Object
 
@@ -92,15 +93,15 @@
         """
         return this.root.remove(path)
     
     def getAssets(
         this,
         extract_zip = False,
         split_imagelist = False,
-        hook : typing.Callable[[int, str, int], typing.Any] = None
+        load_callback : typing.Callable[[int, str, int], typing.Any] = None,
     ):
         """Scans the assets directory and loads all files into the filesystem. This is so wmwpy can modify files without modifying the actual files.
 
         Args:
             extract_zip (bool, optional): Extrack zip files? Defaults to False.
             split_imagelist (bool, optional): Split imagelist files? Defaults to False.
             hook (Callable[[int, str, int], Any], optional): Hook for loading assets, useful for guis. The function gets called with the paramaters `(progress : int, current : str, max : int)`. Defaults to None.
@@ -134,23 +135,27 @@
         current = 0
         
         for dir, subdir, files in os.walk(assets):
             for file in files:
                 path = pathlib.Path('/', os.path.relpath(os.path.join(dir, file), assets)).as_posix()
                 # print(path)
                 
-                if hook:
+                if callable(load_callback):
                     current += 1
-                    hook(current, path, total)
+                    load_callback(current, path, total)
                 
                 fileobj : File = this.add(path, os.path.join(dir, file))
                 
                 if fileobj.extension == 'zip' and extract_zip:
                     fileobj.read()
         
+        
+        if callable(load_callback):
+            load_callback(current, 'Finished loading game', total)
+        
         return this
     
     def exists(this, fp : str) -> bool:
         """Test if file path exists.
 
         Args:
             fp (str): File path.
@@ -168,49 +173,65 @@
             recursive (bool, optional): Whether to include subfolders. Defaults to False.
 
         Returns:
             list: List of files and subfolders.
         """
         return this.get(path).listdir(recursive = recursive, search = search)
     
-    def dump(this, output : str = None):
+    def dump(
+        this,
+        folder : str = None,
+        callback : typing.Callable[[int, str, int], typing.Any] = None,
+    ):
         """Dump the contents of the filesystem to the specified directory
 
         Args:
-            output (str, optional): Path to output directory. Defaults to original path.
+            folder (str, optional): Path to output directory. Defaults to original path.
+            callback (Callable[[int, str, int], Any], optional): A callback function to be ran while dumping the filesystem. Defaults to None.
         """
-        if output == None:
-            output = joinPath(this.gamepath, this.assets)
+        if folder == None:
+            folder = joinPath(this.gamepath, this.assets)
         
         # print(f'output: {output}')
         
         files = this.listdir(recursive=True)
+        total = len(files)
+        progress = 0
+        
         for path in files:
             file = this.get(path)
+            
+            
+            progress += 1
+            
+            if callable(callback):
+                callback(progress, path, total)
+            
             if file.is_dir():
                 continue
             parts = pathlib.Path(path).parts
             
             if parts[0] in ['/', '\\', '']:
                 parts = parts[1::]
             
             # print(f'new: {parts}')
             
-            newpath = pathlib.Path(output, *parts)
+            newpath = pathlib.Path(folder, *parts)
             
             # print(f'writing: {newpath.as_posix()}')
             
             newpath.parent.mkdir(exist_ok=True)
             
             data = file.rawdata.getvalue()
             
             with open(newpath, 'wb') as f:
                 f.write(data)
-        
-        
+            
+        if callable(callback):
+            callback(progress, 'Done!', total)
     
 # Filesystem helpers
 class FileBase():
     name = ''
     
     def __init__(this, parent, path : str):
         """File Base
@@ -551,15 +572,20 @@
         if not path:
             path = '/'
         
         super().__init__(parent, path)
         this._type.value = this._Type.FOLDER
         this.files = []
         
-    def add(this, path : str, content : bytes, replace = False) -> File:
+    def add(
+        this,
+        path : str,
+        content : bytes,
+        replace = False,
+    ) -> File:
         """Add file to folder.
 
         Args:
             path (str): New file path.
             content (bytes): Content of file in bytes.
             replace (bool, optional): Whether to replace any conflicting file.. Defaults to False.
 
@@ -601,15 +627,15 @@
             path (str): Path to File or Folder.
 
         Returns:
             File or Folder: File or Folder.
         """
         parts = pathlib.Path(path).parts
         file = None
-        if parts[0] == '\\':
+        if parts[0] in ['\\', '/']:
             file = this.root
         elif parts[0] == '..':
             file = this.parent
         else:
             for f in this.files:
                 if f.name == parts[0]:
                     file = f
```

### Comparing `wmwpy-0.3.0b0/src/wmwpy/Utils/path.py` & `wmwpy-0.4.0b0/src/wmwpy/Utils/path.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.3.0b0/src/wmwpy/Utils/rotate.py` & `wmwpy-0.4.0b0/src/wmwpy/Utils/rotate.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.3.0b0/src/wmwpy/Utils/waltex.py` & `wmwpy-0.4.0b0/src/wmwpy/Utils/waltex.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.3.0b0/src/wmwpy/__init__.py` & `wmwpy-0.4.0b0/src/wmwpy/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-__version__ = "0.3.0-beta"
+__version__ = "0.4.0-beta"
 __author__ = 'ego-lay-atman-bay'
 
 import typing
+import logging
 
 from .game import Game
+from . import Utils
 from . import classes
 from . import Font
 from .classes import widget
-from . import Utils
 from .gametemplate import GAMES
 from .Utils import filesystem
 
+__all__ = ['load', 'Game', 'Utils', 'classes', 'GAMES', 'filesystem']
+
 def load(
     gamepath : str,
     platform : typing.Literal['android', 'ios'] = 'android',
     game : str = 'WMW',
     assets : str = None,
     db : str = None,
     profile : str = None,
     baseassets : str = None,
-    hook : typing.Callable[[int, str, int], typing.Any] = None,
+    load_callback : typing.Callable[[int, str, int], typing.Any] = None,
 ) -> Game:
     """load game
 
     Args:
         gamepath (str): Folder to extracted game.
         platform (Literal['android', 'ios'], optional): What platform this game is for. Can be 'android' or 'ios'. Defaults to 'android'.
         game (str, optional): Which game is being loaded. A full list of games is in the `gametemplate.GAMES` variable. Defaults to 'WMW'. 
@@ -47,23 +50,23 @@
     }
     
     if assets == None:
         assets = platforms[platform]['assets']
     
     try:
         return GAMES[game](
-            gamepath=gamepath,
-            assets=assets,
-            db=db,
-            profile=profile,
-            hook = hook,
-            baseassets=baseassets
+            gamepath = gamepath,
+            assets = assets,
+            db = db,
+            profile = profile,
+            load_callback = load_callback,
+            baseassets = baseassets,
         )
     except:
         return Game(
-            gamepath=gamepath,
-            assets=assets,
-            db=db,
-            profile=profile,
-            hook = hook,
-            baseassets=baseassets
+            gamepath = gamepath,
+            assets = assets,
+            db = db,
+            profile = profile,
+            load_callback = load_callback,
+            baseassets = baseassets,
         )
```

### Comparing `wmwpy-0.3.0b0/src/wmwpy/classes/Widgets.py` & `wmwpy-0.4.0b0/src/wmwpy/classes/Widgets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import lxml
 from lxml import etree
-from PIL import Image, ImageTk
+from PIL import Image
 from ..Utils.waltex import WaltexImage
 from .widget import Widget
 
 class Widgets():
     def __init__(this, element : etree.Element, gamePath : str, screenSize = (), texturePath : str = None, baseLayoutFile : str = None) -> None:
         this.element = element
```

### Comparing `wmwpy-0.3.0b0/src/wmwpy/classes/curves.py` & `wmwpy-0.4.0b0/src/wmwpy/classes/curves.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.3.0b0/src/wmwpy/classes/imagelist.py` & `wmwpy-0.4.0b0/src/wmwpy/classes/imagelist.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,78 +13,112 @@
 
 class Imagelist(GameObject):
     TEMPLATE = b"""<?xml version="1.0"?>
     <ImageList imgSize="512 512" file="" textureBasePath="/Textures/">
     </ImageList>
     """
     
-    class Type():
+    class Format():
         IMAGELIST = 0
         PAGES = 1
     
     def __init__(
         this,
         file : str | bytes | File = None,
         filesystem : Filesystem | Folder = None,
         gamepath : str = None, assets : str = '/assets',
         baseassets : str = '/',
         HD : bool = False,
+        TabHD : bool = False,
+        save_images : bool = False
     ) -> None:
-        """
-        Get imagelist from file
+        """Get imagelist from file
+        
         Args:
-            file (str | bytes | File): File to read.
+            file (str | bytes | File, optional): File to read. Defaults to None.
             filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
-            HD (bool, optional): Whether to use HD textures. Defaults to False.
-            gamepath (str, optional): Path to game. Only is used when filesystem is `Folder` or `None`. Defaults to None.
+            gamepath (str, optional): Game path. Only used if filesystem not specified. Defaults to None.
+            assets (str, optional): Assets path relative to game path. Only used if filesystem not specified. Defaults to '/assets'.
             baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`
-            assets (str, optional): Path to assets relative to gamepath. Defaults to '/assets'.
+            HD (bool, optional): Use HD images. Defaults to False.
+            TabHD (bool, optional): Use TabHD images. Defaults to False.
+        
         Raises:
             FileNotFoundError: Filesystem is not usable and no gamepath.
         """
         
         super().__init__(filesystem, gamepath, assets, baseassets)
         
+        this.HD = HD
+        this.TabHD = TabHD
+        
+        if isinstance(file, str):
+            file = getHDFile(
+                file,
+                HD = this.HD,
+                TabHD = this.TabHD,
+                filesystem = this.filesystem,
+                gamepath = this.gamepath,
+                assets = this.assets,
+                baseassets = this.baseassets,
+            )
+        elif isinstance(file, File):
+            file = getHDFile(
+                file.path,
+                HD = this.HD,
+                TabHD = this.TabHD,
+                filesystem = this.filesystem,
+                gamepath = this.gamepath,
+                assets = this.assets,
+                baseassets = this.baseassets,
+            )
+        
+        if isinstance(file, str):
+            file = this.filesystem.get(file)
+        
         this.file = super().get_file(file, template = this.TEMPLATE)
 
-        this.HD = HD
         this.xml : etree.ElementBase = etree.parse(this.file).getroot()
-        this.textureBasePath : str = '/Textures/'
+        
         this.pages : list[Imagelist.Page] = []
-        this.type = this.Type.IMAGELIST
+        this.format = this.Format.IMAGELIST
         this.filename = ''
 
         # this.images = {}
 
-        this.read()
+        this.read(save_images = save_images)
     
-    def read(this):
+    def read(this, save_images : bool = False):
         """Read the imagelist xml.
         """
-        this.type = this.Type.IMAGELIST
+        this.format = this.Format.IMAGELIST
         
         for element in this.xml:
             if element is etree.Comment:
                 continue
             
             if element.tag == 'Page':
-                this.type = this.Type.PAGES
+                this.format = this.Format.PAGES
                 page = this.Page(
                     element,
                     filesystem = this.filesystem,
                     HD = this.HD,
+                    TabHD = this.TabHD,
+                    save_images = save_images,
                 )
                 
                 this.pages.append(page)
         
-        if this.type == this.Type.IMAGELIST:
+        if this.format == this.Format.IMAGELIST:
             page = this.Page(
                 this.xml,
                 filesystem = this.filesystem,
                 HD = this.HD,
+                TabHD = this.TabHD,
+                save_images = save_images,
             )
             
             this.pages.append(page)
     
     def export(
         this,
         path : str = None,
@@ -113,41 +147,41 @@
             this.filename = path
         
         if removeImageFiles:
             this.removeImageFiles()
         
         if path != None:
             if exportImage:
-                if this.type == this.Type.PAGES:
+                if this.format == this.Format.PAGES:
                     index = 0
                     for page in this.pages:
                         index += 1
                         
                         filename = os.path.splitext(path)[0]
                         filename = f'{filename}_split_{str(index)}.{imageFormat}'
                         
                         page.file = filename
-                        page.exportAtlas(filename = filename, format = imageFormat)
+                        page.exportAtlas(filename = getHDFile(filename, this.HD, this.TabHD), format = imageFormat)
                         
                 else:
-                    page : this.Page = this.pages[0]
+                    page = this.pages[0]
                     
                     filename = os.path.splitext(path)[0]
                     filename = f'{filename}.{imageFormat}'
                     
                     page.file = filename
-                    page.exportAtlas(filename = filename, format = imageFormat)
+                    page.exportAtlas(filename = getHDFile(filename, this.HD, this.TabHD), format = imageFormat)
         
-        if this.type == this.Type.IMAGELIST:
+        if this.format == this.Format.IMAGELIST:
             page = this.pages[0]
-            xml = page.getXML(type = this.type)
+            xml = page.getXML(type = this.format)
         else:
             xml = etree.Element('Imagelist')
             for page in this.pages:
-                xml.append(page.getXML(type = this.type))
+                xml.append(page.getXML(type = this.format))
             
         output = etree.tostring(xml, pretty_print=True, xml_declaration=True, encoding='utf-8')
         
         if path != None:
             if (file := this.filesystem.get(path)) != None:
                 if isinstance(file, Folder):
                     raise TypeError(f'Path {path} is not a file.')
@@ -159,15 +193,15 @@
         
         
         return output
     
     def combinePages(this):
         """Combine all the pages in this Imagelist into 1 Page
         """
-        if this.type == this.Type.IMAGELIST:
+        if this.format == this.Format.IMAGELIST:
             return
         
         main = this.pages[0]
         for i in range(len(this.pages) - 1):
             page : this.Page = this.pages[i + 1]
             for name in page.images:
                 image = page.images[name]
@@ -177,277 +211,205 @@
                     image.properties,
                     replace = False
                 )
                 
         main.id = None
         main.exportAtlas()
         
-        this.type = this.Type.IMAGELIST
+        this.format = this.Format.IMAGELIST
         
         this.pages = [main]
                 
     
-    def getImage(this, name : str):
+    def get(this, name : str):
         """Get image from imagelist.
 
         Args:
             name (str): Name of image.
 
         Returns:
             Imagelist.Page.Image: Imagelist Image.
         """
         for page in this.pages:
-            image = page.getImage(name)
+            image = page.get(name)
             if image:
                 return image
             
         return None
         
         # return this.filesystem.get(os.path.join(this.textureBasePath, name))
     
     def removeImageFiles(this):
         """Remove all image files in imagelist from filesystem.
         """
         for page in this.pages:
             page.removeImageFiles()
     
     class Page(GameObject):
-        HD = False
-        id = None
-        imgSize = (1,1)
-        textureBasePath = '/Textures/'
-        file = ''
-
         def __init__(
             this,
             element : etree.ElementBase,
             filesystem: Filesystem | Folder = None,
             gamepath: str = None,
             assets: str = '/assets',
-            HD = False,
+            HD : bool = False,
+            TabHD : bool = False,
+            save_images : bool = False,
         ) -> None:
             """Page for Imagelist. This is also used when imagelist is not in pages format.
 
             Args:
                 element (etree.Element): lxml elment
                 filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
                 gamepath (str, optional): Gamepath used if filesystem is not specified. Defaults to None.
                 assets (str, optional): Assets path relative to gamepath. Only used if filesystem is not specified. Defaults to '/assets'.
                 HD (bool, optional): Use HD graphics. Defaults to False.
             """
             super().__init__(filesystem, gamepath, assets)
             
-            this.HD : bool = HD
+            this.HD = HD
+            this.TabHD = TabHD
             
             this.xml : etree.ElementBase = element
             
             this.atlas = None
-            this.images : dict[str, Imagelist.Page.Image] = {}
-            
-            this.read()
-        
-        class Image(GameObject):
-            def __init__(
-                this,
-                atlas : PIL.Image.Image,
-                properties : dict,
-                textureBasePath = '/Textures',
-                filesystem: Filesystem | Folder = None,
-                gamepath: str = None,
-                assets: str = '/assets'
-            ) -> None:
-                """Image for Imagelist
-
-                Args:
-                    atlas (PIL.Image.Image): Atlas file containing all images
-                    properties (dict): Properties for Image
-                    filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
-                    gamepath (str, optional): Game path. Only used if filesystem not specified. Defaults to None.
-                    assets (str, optional): Assets path relative to game path. Only used if filesystem not specified. Defaults to '/assets'.
-                """
-                super().__init__(filesystem, gamepath, assets)
-
-                this.atlas = atlas
-                this.properties = deepcopy(properties)
-
-                this.size : tuple[int,int] = (1,1)
-                this.offset : tuple[float,float] = (0,0)
-                this.rect : tuple[int,int,int,int] = (0,0,0,0)
-                this.name : str = ''
-                this.textureBasePath : str = textureBasePath
-
-                this.image = PIL.Image.new('RGBA', this.size)
-
-                this.rawdata = io.BytesIO()
-
-                this.getData()
-                this.getImage()
-
-            def getData(this):
-                """Get properties from xml.
-                """
-                if 'size' in this.properties:
-                    this.size = tuple([int(v) for v in this.properties['size'].split()])
-                if 'offset' in this.properties:
-                    this.offset = tuple([int(v) for v in this.properties['offset'].split()])
-                if 'rect' in this.properties:
-                    this.rect = tuple([int(v) for v in this.properties['rect'].split()])
-                if 'name' in this.properties:
-                    this.name = this.properties['name']
-
-            def getImage(this):
-                """Get image from atlas.
-
-                Returns:
-                    PIL.Image.Image: PIL Image.
-                """
-                this.image = this.atlas.crop(numpy.add(this.rect, (0,0) + this.rect[0:2]))
-                this.image = this.image.resize(this.size)
-                
-                this.image.save(this.rawdata, format = os.path.splitext(this.name)[1][1::])
-                return this.image
-
-            def show(this):
-                """Show image with default image viewer.
-                """
-                this.image.show()
-            
-            def updateProperties(this):
-                """Update properties dict.
-                """
-                this.properties['name'] = this.name
-                this.properties['size'] = ' '.join([str(x) for x in this.size])
-                this.properties['rect'] = ' '.join([str(x) for x in this.rect])
-                this.properties['offset'] = ' '.join([str(x) for x in this.offset])
-            
-            def getXML(this):
-                """Get xml for image.
-
-                Returns:
-                    lxml.etree.Element: lxml element
-                """
-                this.updateProperties()
-                xml : etree.ElementBase = etree.Element('Image', **this.properties)
-                
-                return xml
-            
-            def removeFile(this):
-                """Remove file from filesystem.
-                """
-                return this.filesystem.remove(this.filename)
-                
-            
-            def saveFile(this, replace : bool = False):
-                """Save image to filesystem.
-
-                Args:
-                    replace (bool, optional): Whether to replace any existing file. Defaults to False.
-                """
-                this.image.save(this.rawdata, os.path.splitext(this.name)[1][1::])
-                this.filesystem.add(
-                    this.name,
-                    file = this.rawdata.getvalue(),
-                    replace = replace
-                )
-            
+            this.images : list[Imagelist.Page.Image] = []
+            this.properties : dict[str,str] = {}
             
-            @property
-            def filename(this) -> str:
-                """Image filepath in the Filesystem
-
-                Returns:
-                    str: Full filepath in the Filesystem
-                """
-                return this.filesystem.get(this.name).path
-
+            this.read(save_images = save_images)
         
-        def read(this):
+        def read(this, save_images : bool = False):
             """Read xml.
             """
             this.properties = deepcopy(this.xml.attrib)
-            if 'imgSize' in this.properties:
-                this.size = tuple([int(v) for v in this.properties['imgSize'].split()])
-            if 'textureBasePath' in this.properties:
-                this.textureBasePath = this.properties['textureBasePath']
-            if 'file' in this.properties:
-                this.file = this.properties['file']
-            if 'id' in this.properties:
-                this.id = this.properties['id']
     
-            if this.HD:
-                hd = getHDFile(this.file)
-                if this.filesystem.exists(hd):
-                    this.file = hd
-    
-            this.fullAtlasPath = ''
-    
-            if this.gamepath:
-                this.fullAtlasPath = joinPath(this.gamepath, this.assets, this.file)
+            # if this.gamepath:
+            #     this.fullAtlasPath = joinPath(this.gamepath, this.assets, this.file)
                 # print(this.fullAtlasPath)
     
             this.getAtlas()
-            this.getImages()
+            this.getImages(save_images = save_images)
+        
+        @property
+        def imgSize(this) -> tuple[int,int]:
+            """The size of the image in the properties. Does not have to reflect the size of the atlas.
+
+            Returns:
+                tuple[int,int]: (width,height)
+            """
+            if 'imgSize' in this.properties:
+                return tuple([int(v) for v in this.properties['imgSize'].split()])
+            else:
+                return (1,1)
+        @imgSize.setter
+        def imgSize(this, size : tuple | list | str):
+            if isinstance(size, (list, tuple)):
+                this.properties['imgSize'] = ''.join([str(a) for a in size])
+            elif isinstance(size, str):
+                this.properties['imgSize'] = size
+            else:
+                raise TypeError('size must be a tuple, list, or str')
+    
+        @property
+        def textureBasePath(this) -> str:
+            """The base Textures path, or the place where the files are extracted to.
+
+            Returns:
+                str: The textureBasePath
+            """
+            if 'textureBasePath' in this.properties:
+                return this.properties['textureBasePath']
+            else:
+                this.textureBasePath = joinPath(this.filesystem.baseassets, '/Textures/')
+                return this.textureBasePath
+        @textureBasePath.setter
+        def textureBasePath(this, path):
+            this.properties['textureBasePath'] = path
+        
+        @property
+        def file(this):
+            """The path to the atlas file to use in this ImageList
+
+            Returns:
+                str: Path to atlas file.
+            """
+            if 'file' in this.properties:
+                return getHDFile(
+                    this.properties['file'],
+                    HD = this.HD,
+                    TabHD = this.TabHD,
+                    filesystem = this.filesystem,
+                    assets = this.assets,
+                    baseassets = this.baseassets,
+                )
+            else:
+                return ''
+        @file.setter
+        def file(this, path):
+            this.properties['file'] = path
+        
+        @property
+        def id(this):
+            """Page id
+
+            Returns:
+                str: The id
+            """
+            if 'id' in this.properties:
+                return this.properties['id']
+            else:
+                return None
+        @id.setter
+        def id(this, value : int, str):
+            if isinstance(value, str):
+                this.properties['id'] = value
+            else:
+                this.properties['id'] = str(value)
     
         def getAtlas(this):
             """Get atlas image.
             """
-            if not this.file:
-                image = Texture(PIL.Image.new('RGBA', this.size))
+            if this.file in ['', None]:
+                image = Texture(PIL.Image.new('RGBA', this.imgSize))
                 this.atlas = image.image.copy()
-                return
-            if this.filesystem.exists(this.file):
+                
+            elif this.filesystem.exists(this.file):
                 file = this.filesystem.get(this.file)
                 image = Texture(file.read())
                 this.atlas = image.image.copy()
-            else:
-                this.textureSettings = getTextueSettings(
-                    this.gamepath,
-                    this.assets,
-                    joinPath(os.path.dirname(os.path.dirname(this.textureBasePath)), 'Data/textureSettings.xml'),
-                    this.name
-                )
-    
-                this.atlas = getTexture(this.fullAtlasPath, this.textureSettings, this.size)
     
-        def getImages(this):
+        def getImages(this, save_images = False):
             """Get images from xml.
             """
-            for image in this.xml:
-                if not image.tag is etree.Comment:
-                    if image.tag == 'Image':
-                        texture = this.Image(
-                            this.atlas,
-                            properties = image.attrib,
-                            textureBasePath = this.textureBasePath,
-                            filesystem = this.filesystem.get(this.textureBasePath),
-                        )
-                        this.images[image.get('name')] = texture
-                        
-                        # print(f'{this.textureBasePath = }')
-                        # print(f'{texture.name = }')
-    
-                        this.filesystem.add(
-                            joinPath(this.textureBasePath, texture.name),
-                            texture.rawdata.getvalue(),
-                            replace = True
-                        )
+            for element in this.xml:
+                if element is etree.Comment:
+                    continue
+                
+                if element.tag == 'Image':
+                    image = this.Image(
+                        this.atlas,
+                        properties = element.attrib,
+                        textureBasePath = this.textureBasePath,
+                        filesystem = this.filesystem.get(this.textureBasePath),
+                        save_image = save_images,
+                    )
+                    this.images.append(image)
     
-        def getImage(this, name : str) -> Image:
+        def get(this, name : str) -> 'Imagelist.Page.Image':
             """Get an image from the imagelist
 
             Args:
                 name (str): Name of image.
 
             Returns:
                 Imagelist.Page.Image: Imagelist Image.
             """
-            if name in this.images:
-                return this.images[name]
-            else:
-                return None
+            for image in this.images:
+                if image.name == name:
+                    return image
         
         def add(this,
                 name : str,
                 image : PIL.Image.Image,
                 properties : dict = {},
                 replace = False
             ):
@@ -469,30 +431,30 @@
             properties['name'] = name
             properties['rect'] = ' '.join([str(_) for _ in (0,0) + image.size])
             
             texture = this.Image(
                 image,
                 properties
             )
-            this.images[name] = texture
+            this.images.append(texture)
             
-            this._getrect()
+            this._getRects()
         
         def exportAtlas(this, filename = None, gap : tuple = (1,1), format : str = 'webp', ):
             """Export the atlas image into the Filesystem. This function recreates the imagelist, so you need to also export the xml using `getXML()`.
 
             Args:
                 gap (tuple, optional): Gap between each image. Defaults to (1,1).
                 filename (str, optional): Filename of image. Defaults to `file` property.
                 format (str, optional): Format to save image as. Defaults to 'webp'.
 
             Returns:
                 PIL.Image.Image: PIL Image.
             """
-            this._getrect(gap = gap)
+            this._getRects(gap = gap)
             this._updateAtlas()
             file = io.BytesIO()
             
             this.atlas.save(file, format=format)
             
             if filename == None:
                 filename = f'{os.path.splitext(this.file)[0]}.{format}'
@@ -502,28 +464,14 @@
             if this.filesystem.exists(filename):
                 this.filesystem.get(filename).rawdata = file
             else:
                 this.filesystem.add(filename, file.getvalue())
             
             return this.atlas
         
-        def updateProperties(this):
-            """Updates all the properties dict.
-            """
-            this.properties['textureBasePath'] = this.textureBasePath
-            this.properties['imgSize'] = ' '.join([str(n) for n in this.size])
-            this.properties['file'] = this.file
-            # print(this.properties['file'])
-            if this.id == None:
-                if 'id' in this.properties:
-                   del this.properties['id']
-            else:
-                this.properties['id'] = str(this.id)
-                
-        
         def getXML(this, filename = None, type : int = 1):
             """Generates the xml for the page / imagelist.
 
             Args:
                 filename (str, optional): Name of image. Defaults to file property.
                 type (int, optional): Type of file. 0 for `Page`, 1 for `Imagelist`. Defaults to 1.
 
@@ -531,32 +479,30 @@
                 lxml.etree.Element: lxml Element.
             """
             if filename != None:
                 this.file = filename
             
             tag = 'Page' if type else 'Imagelist'
             
-            this.updateProperties()
             xml : etree.ElementBase = etree.Element(tag, **this.properties)
             
-            for name in this.images:
-                image : this.Image = this.images[name]
+            for image in this.images:
                 xml.append(image.getXML())
             
             this.xml = xml
             return this.xml
         
         def removeImageFiles(this):
             """Remove all image files from filesystem.
             """
             for name in this.images:
-                this.images[name].removeFile()
+                this.images.removeFile()
             
         
-        def _getrect(this, gap : tuple = (1,1)):
+        def _getRects(this, gap : tuple = (1,1)):
             """Update the rect for all images.
 
             Args:
                 gap (tuple, optional): Gap between images. Defaults to (1,1).
             """
             x, y = gap
             maxheight = maxwidth = 0
@@ -568,15 +514,15 @@
                 
                 if x > maxwidth:
                     maxwidth = x
                 
                 x += image.size[0] + gap[0]
                 
                 column += 1
-                if x > this.size[0]:
+                if x > this.imgSize[0]:
                     x = gap[0]
                     y += maxheight + gap[1]
                     maxheight = 0
                     column = 0
                     row += 1
                 
                 if column == 0:
@@ -584,41 +530,212 @@
                     x += image.size[0] + gap[0]
                 
                 if image.size[1] > maxheight:
                     maxheight = image.size[1]
             
             y += maxheight + gap[1]
             
-            if y > this.size[1]:
-                this.size = (this.size[0], y)
+            if y > this.imgSize[1]:
+                this.imgSize = (this.imgSize[0], y)
             
                 
         def _updateAtlas(this):
-            atlas : PIL.Image.Image = PIL.Image.new('RGBA', this.size)
+            atlas : PIL.Image.Image = PIL.Image.new('RGBA', this.imgSize)
             
             for image in this.images:
                 image = this.images[image]
                 image.atlas = atlas
                 atlas.paste(image.image, image.rect[0:2])
             
             this.atlas = atlas
             return this.atlas
     
-        def getNO_TEX(this):
-            """## NEED TO UPDATE
-            """
-            NO_TEX_settings = getTextueSettings(
-                this.gamepath,
-                this.assets,
-                joinPath(os.path.dirname(os.path.dirname(this.textureBasePath)), 'Data/textureSettings.xml'),
-                os.path.join(this.textureBasePath, 'NO_TEX.png')
-            )
-            NO_TEX_image = PIL.Image.open(joinPath(this.gamepath, this.assets, this.textureBasePath, 'NO_TEX.png')).convert('RGBA')
-            this.NO_TEX = this.Image(NO_TEX_image, {
-                'size': ' '.join([str(x) for x in NO_TEX_image.size]),
-                'rect': ' '.join([str(x) for x in (0,0) + NO_TEX_image.size]),
-                'name': 'NO_TEX.png',
-            })
-            # this.Image(this.atlas, image.attrib)
-    
-    
+        class Image(GameObject):
+            def __init__(
+                this,
+                atlas : PIL.Image.Image,
+                properties : dict,
+                textureBasePath = '/Textures',
+                filesystem: Filesystem | Folder = None,
+                gamepath: str = None,
+                assets: str = '/assets',
+                save_image : bool = False,
+            ) -> None:
+                """Image for Imagelist
+
+                Args:
+                    atlas (PIL.Image.Image): Atlas file containing all images
+                    properties (dict): Properties for Image.
+                    filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
+                    gamepath (str, optional): Game path. Only used if filesystem not specified. Defaults to None.
+                    assets (str, optional): Assets path relative to game path. Only used if filesystem not specified. Defaults to '/assets'.
+                """
+                super().__init__(filesystem, gamepath, assets)
+
+                this.atlas = atlas
+                this.properties = deepcopy(properties)
+                this.textureBasePath : str = textureBasePath
+
+                this.image = PIL.Image.new('RGBA', this.size)
+
+                this.rawdata = io.BytesIO()
+                
+                this._image = None
+                
+                if save_image:
+                    this.getImage()
+            
+            @property
+            def size(this) -> tuple[int,int]:
+                """The size of the image.
+
+                Returns:
+                    tuple[int,int]: (width,height)
+                """
+                if 'size' in this.properties:
+                    return tuple([int(v) for v in this.properties['size'].split()])
+                else:
+                    this.size = this.image.size
+                    return this.size
+            @size.setter
+            def size(this, value : tuple | list | str):
+                if isinstance(value, (tuple, list)):
+                    this.properties['size'] = ' '.join([str(v) for v in value])
+                elif isinstance(value, (int, float)):
+                    this.properties['size'] = ' '.join([str(int(value))] * 2)
+                elif isinstance(value, str):
+                    this.properties['size'] = value
+                else:
+                    raise TypeError('value must be tuple, list or str')
+
+            @property
+            def offset(this) -> tuple[int,int]:
+                """The image offset
+
+                Returns:
+                    tuple[int,int]: (x,y)
+                
+                (I have no idea what this is for)
+                """
+                if 'offset' in this.properties:
+                    return tuple([int(v) for v in this.properties['offset'].split()])
+                else:
+                    this.offset = (0,0)
+                    return this.offset
+            @offset.setter
+            def offset(this, value : tuple | list | str):
+                if isinstance(value, (tuple, list)):
+                    this.properties['offset'] = ' '.join([str(v) for v in value])
+                elif isinstance(value, (int, float)):
+                    this.properties['offset'] = ' '.join([str(int(value))] * 2)
+                elif isinstance(value, str):
+                    this.properties['offset'] = value
+                else:
+                    raise TypeError('value must be tuple, list or str')
+
+            @property
+            def rect(this) -> tuple[int,int,int,int]:
+                """The rectangle of this image inside the atlas
+
+                Returns:
+                    tuple[int,int,int,int]: (x,y,width,height)
+                """
+                
+                if 'rect' in this.properties:
+                    return tuple([int(v) for v in this.properties['rect'].split()])
+                else:
+                    this.rect = (0,0) + this.size
+                    return this.rect
+            @rect.setter
+            def rect(this, value : tuple | list | str):
+                if isinstance(value, (tuple, list)):
+                    this.properties['rect'] = ' '.join([str(v) for v in value])
+                elif isinstance(value, (int, float)):
+                    this.properties['rect'] = ' '.join(['0', '0'] + ([str(int(value))] * 2))
+                elif isinstance(value, str):
+                    this.properties['rect'] = value
+                else:
+                    raise TypeError('value must be tuple, list or str')
+            
+            @property
+            def name(this) -> str:
+                """The name of the iamge
+
+                Returns:
+                    str: image name
+                """
+                if 'name' in this.properties:
+                    return this.properties['name']
+                else:
+                    this.name = 'image.png'
+                    return this.name
+            @name.setter
+            def name(this, name : str):
+                this.properties['name'] = str(name)
+            
+            @property
+            def image(this):
+                if this._image == None:
+                    this.getImage()
+                
+                return this._image.copy()
+            
+            @image.setter
+            def image(this, image : PIL.Image.Image):
+                this._image = image.copy()
+
+            def getImage(this) -> PIL.Image.Image:
+                """Get image from atlas.
+
+                Returns:
+                    PIL.Image.Image: PIL Image.
+                """
+                this._image = this.atlas.crop(numpy.add(this.rect, (0,0) + this.rect[0:2]))
+                this._image = this._image.resize(this.size)
+                
+                this._image.save(this.rawdata, format = os.path.splitext(this.name)[1][1::].upper())
+                return this._image
+
+            def show(this):
+                """Show image with default image viewer.
+                """
+                this.image.show()
+            
+            def getXML(this):
+                """Get xml for image.
+
+                Returns:
+                    lxml.etree.Element: lxml element
+                """
+                xml : etree.ElementBase = etree.Element('Image', **this.properties)
+                
+                return xml
+            
+            def removeFile(this):
+                """Remove file from filesystem.
+                """
+                return this.filesystem.remove(this.filename)
+                
+            
+            def saveFile(this, replace : bool = False):
+                """Save image to filesystem.
+
+                Args:
+                    replace (bool, optional): Whether to replace any existing file. Defaults to False.
+                """
+                this.image.save(this.rawdata, os.path.splitext(this.name)[1][1::])
+                this.filesystem.add(
+                    this.name,
+                    content = this.rawdata.getvalue(),
+                    replace = replace,
+                )
+            
+            
+            @property
+            def filename(this) -> str:
+                """Image filepath in the Filesystem
+
+                Returns:
+                    str: Full filepath in the Filesystem
+                """
+                return this.filesystem.get(this.name).path
```

### Comparing `wmwpy-0.3.0b0/src/wmwpy/classes/layout.py` & `wmwpy-0.4.0b0/src/wmwpy/classes/layout.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.3.0b0/src/wmwpy/classes/level.py` & `wmwpy-0.4.0b0/src/wmwpy/classes/level.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 import io
+import os
 from lxml import etree
-from PIL import Image, ImageTk
+from PIL import Image
 import numpy
 import typing
 import copy
+import logging
+
+LOADED_ImageTk = True
+if LOADED_ImageTk:
+    try:
+        from PIL import ImageTk
+    except:
+        LOADED_ImageTk = False
+
 
 from ..Utils.filesystem import *
 from ..Utils.logging_utils import log_exception
 from .object import Object
 from ..gameobject import GameObject
 
 class Level(GameObject):
@@ -25,44 +35,67 @@
         image : str | bytes | File = None,
         filesystem : Filesystem | Folder = None,
         gamepath : str = None,
         assets : str = '/assets',
         baseassets : str = '/',
         load_callback : typing.Callable[[int, str, int], typing.Any] = None,
         ignore_errors : bool = False,
+        HD : bool = False,
+        TabHD : bool = False,
     ) -> None:
         """Load level
 
         Args:
             xml (str | bytes | File): XML file for level.
             image (str | bytes | File): Image file for level.
             filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
             gamepath (str, optional): Game path. Only used if filesystem not specified. Defaults to None.
             assets (str, optional): Assets path relative to game path. Only used if filesystem not specified. Defaults to '/assets'.
             baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`
+            load_callback (Callable[[int, str, int], Any], optional): A callback function to be ran while loading the level. Defaults to None.
+            ignore_errors (bool, optional): Ignore errors while loading. Defaults to False.
+            HD (bool, optional): Use HD images. Defaults to False.
+            TabHD (bool, optional): Use TabHD images. Defaults to False.
         """
         
         this.gamepath = gamepath
         this.assets = assets
         this.filename = ''
         if this.assets == None:
             this.assets = '/assets'
         
         super().__init__(filesystem, gamepath, assets, baseassets)
         
+        logging.debug(f'Level: xml before: {xml}')
+        
+        if isinstance(xml, File):
+            logging.debug(f'Level: xml path: {xml.path}')
+        
         this.xml_file = super().get_file(xml, template = this.XML_TEMPLATE)
         
+        logging.debug(f'Level: xml after: {this.xml_file}')
+        # try:
+        #     logging.debug(f'Level: raw xml:\n{this.xml_file.getvalue().decode()}')
+        # except:
+        #     logging.debug('Level: file not io.BytesIO')
+        
+        if isinstance(this.xml_file, io.BytesIO):
+            this.xml_file.seek(0)
+        
         this.xml = etree.parse(this.xml_file).getroot()
         
         this.image_file = super().get_file(image)
         if this.image_file == None:
             this.image = this.IMAGE_TEMPLATE.copy()
         else:
             this.image = Image.open(this.image_file).quantize(colors=256)
         
+        this.HD = HD
+        this.TabHD = TabHD
+        
         this.objects : list[Object] = []
         this.properties : dict[str,str] = {}
         this.challenges : list[Level.Challenge] = []
         this.room = (0,0)
         
         this.read(load_callback = load_callback, ignore_errors = ignore_errors)
         
@@ -94,21 +127,25 @@
         return image
         
     @image.setter
     def image(this, value : Image.Image):
         this._image = value
     
     @property
-    def PhotoImage(this) -> ImageTk.PhotoImage:
+    def PhotoImage(this) -> 'ImageTk.PhotoImage':
         """Tkinter PhotoImage of the Level image
 
         Returns:
             ImageTk.PhotoImage: Tkinter PhotoImage
         """
-        this._PhotoImage = ImageTk.PhotoImage(this.image)
+        if LOADED_ImageTk:
+            this._PhotoImage = ImageTk.PhotoImage(this.image)
+        else:
+            this._PhotoImage = this.image.copy()
+            
         return this._PhotoImage
 
     @property
     def scale(this) -> int:
         """Level size scale
         """
         return this._scale
@@ -171,14 +208,16 @@
                     
                     obj = Object(
                         this.filesystem.get(properties['Filename']), # get file because `Object` does not take filepath
                         filesystem = this.filesystem,
                         properties = properties,
                         pos = pos,
                         name = name,
+                        HD = this.HD,
+                        TabHD = this.TabHD,
                     )
                     
                     obj.id = id
                     
                     this.objects.append(obj)
                     
                     id += 1
@@ -224,14 +263,15 @@
                 if not ignore_errors:
                     raise
             
     def export(
         this,
         filename : str = None,
         exportObjects : bool = False,
+        saveImage : bool = True,
     ) -> bytes:
         """Export level
 
         Args:
             filename (str, optional): Path to level. Defaults to Level.filename.
             exportObjects (bool, optional): Whether to export objects. Defaults to False.
 
@@ -282,14 +322,32 @@
                 file.write(output)
             else:
                 raise TypeError(f'Path {filename} is not a file.')
                 
         else:
             this.filesystem.add(filename, output)
         
+        if saveImage:
+            imgFile = io.BytesIO()
+            this._image.save(
+                imgFile,
+                format = this.IMAGE_FORMAT,
+            )
+            
+            filename = os.path.splitext(filename)[0] + f'.{this.IMAGE_FORMAT.lower()}'
+            
+            if (file := this.filesystem.get(filename)) != None:
+                if isinstance(file, File):
+                    file.write(imgFile.getvalue())
+                else:
+                    raise TypeError(f'Path {filename} is not a file.')
+                    
+            else:
+                this.filesystem.add(filename, imgFile.getvalue())
+        
         return output
     
     def addObject(
         this,
         filename : str | Object,
         properties : dict = {},
         pos : tuple[float,float] = (0,0),
```

### Comparing `wmwpy-0.3.0b0/src/wmwpy/classes/object.py` & `wmwpy-0.4.0b0/src/wmwpy/classes/sprite.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,606 +1,739 @@
-import lxml
 from lxml import etree
-import io
-from copy import deepcopy
-from PIL import Image, ImageTk, ImageDraw
+from PIL import Image
 import numpy
+from copy import deepcopy
 import math
+import typing
+import os
 
-from ..gameobject import GameObject
-from .sprite import Sprite
-from ..Utils.filesystem import *
-from ..Utils.rotate import rotate
+LOADED_ImageTk = True
+if LOADED_ImageTk:
+    try:
+        from PIL import ImageTk
+    except:
+        LOADED_ImageTk = False
 
+from .imagelist import Imagelist
+from ..Utils.filesystem import *
+from ..Utils.gif import save_transparent_gif
 from ..Utils.XMLTools import strbool
-class Object(GameObject):
+from ..gameobject import GameObject
+
+class Sprite(GameObject):
     def __init__(
         this,
         file : str | bytes | File,
-        filesystem : Filesystem | Folder = None,
-        gamepath : str = None,
-        assets : str = '/assets',
+        filesystem: Filesystem | Folder = None,
+        gamepath: str = None, assets: str = '/assets',
         baseassets : str = '/',
         properties : dict = {},
-        pos : tuple | str = (0,0),
-        name : str = 'Obj',
-        scale : int = 10,
+        scale : int = 50,
+        HD : bool = False,
+        TabHD : bool = False,
     ) -> None:
-        """Get game object. Game object is `.hs` file.
+        """Game sprite.
 
         Args:
-            file (str | bytes | File): Object file.
+            this (_type_): _description_
+            file (str | bytes | File): Sprite file.
             filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
             gamepath (str, optional): Game path. Only used if filesystem not specified. Defaults to None.
             assets (str, optional): Assets path relative to game path. Only used if filesystem not specified. Defaults to '/assets'.
             baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`
-            properties (dict, optional): Object properties that override default properties. Defaults to {}.
-            pos (tuple | str, optional): Position of object. Defaults to (0,0).
-            name (str, optional): Name of object. Defaults to 'Obj'.
-            scale (int, optional): The image scale. Defaults to 10.
+            properties (dict, optional): Sprite properties. Defaults to {}.
+            scale (int, optional): Sprite image scale. Defaults to 10.
+            HD (bool, optional): Use HD images. Defaults to False.
+            TabHD (bool, optional): Use TabHD images. Defaults to False.
         """
         
         super().__init__(filesystem, gamepath, assets, baseassets)
-        
         this.file = super().get_file(file)
         
-        this._properties = deepcopy(properties)
-        if isinstance(pos, str):
-            this.pos = tuple([float(a) for a in pos.split()])
-        else:
-            this.pos = tuple(pos)
-        
         this.xml : etree.ElementBase = etree.parse(this.file).getroot()
-        this.sprites : list[Sprite] = []
-        this.shapes : list[Shape] = []
-        this.UVs : list[tuple[int,int]] = []
-        this.VertIndices : list[int] = []
-        this.defaultProperties = {}
-        this.properties = {}
-        this.name = name
-        this.size = (0,0)
-        this.id = 0
-        
-        this._background : list[Sprite] = []
-        this._foreground : list[Sprite] = []
-        this._PhotoImage : dict[str, ImageTk.PhotoImage] = {}
         
-        this._offset = [0,0]
+        this.HD = HD
+        this.TabHD = TabHD
+        
+        this.properties = deepcopy(properties)
+        this.animations : list[Sprite.Animation] = []
+        
         this.scale = scale
         
         this.readXML()
-        
-        if isinstance(file, File):
-            this.filename = file.path
+        this.animation = 0
     
-    def getOffset(this) -> tuple[float,float]:
-        """Get the center offset for the Object image
+    def setAnimation(this, animation : str | int):
+        """Set the current animation for the Sprite
 
-        Returns:
-            tuple[float,float]: (x,y)
+        Args:
+            animation (str | int): Animation name or index.
         """
-        rects = []
-        this._background : list[Sprite] = []
-        this._foreground : list[Sprite] = []
-        
-        for sprite in this.sprites:
-            if 'visible' in sprite.properties:
-                if not strbool(sprite.properties['visible']):
-                    continue
-            if ('isBackground' in sprite.properties) and strbool(sprite.properties['isBackground']):
-                this._background.append(sprite)
-            else:
-                this._foreground.append(sprite)
-                
-            pos = numpy.array(sprite.pos)
-            size = (numpy.array(sprite.image.size) / sprite.scale) * [1,-1]
-            
-            rects.append(
-                tuple(pos - (size / 2))
-            )
-            rects.append(
-                tuple(pos + (size / 2))
-            )
-            
-        rects = numpy.array(rects).swapaxes(0,1)
-        
-        min = numpy.array([math.floor(v.min()) for v in rects])
-        max = numpy.array([math.ceil(v.max()) for v in rects])
-        
-        
-        this.size = max - min
-        this._offset = [a.mean() for a in numpy.array([min,max]).swapaxes(0,1)]
-        
-        return this._offset
+        this.animation = animation
     
     @property
-    def background(this) -> Image.Image:
-        """The background image of this Object
+    def image(this) -> Image.Image:
+        """Image of sprite
 
         Returns:
             PIL.Image.Image: PIL Image
         """
-        this.getOffset()
+        image = this.animation.image.copy()
+        gridSize = numpy.array(this.gridSize)
+        size = gridSize * this.scale
+        size = [abs(round(x)) for x in size]
+        image = image.resize(size)
         
-        image = Image.new('RGBA', tuple(this.size * this.scale), (0,0,0,0))
-        
-        for sprite in this._background:
-            size = (numpy.array(sprite.image.size) / sprite.scale) * [1,-1]
-            pos = this.truePos(
-                sprite.pos,
-                size,
-                this.size,
-                scale = this.scale,
-                offset = this._offset
-            )
-            
-            # print(f'{pos = }')
-            
-            image.alpha_composite(
-                sprite.image,
-                tuple([round(x) for x in pos]),
-            )
-        image = this.rotateImage(image)
+        image = image.rotate(this.angle, Image.BILINEAR, expand=True)
         
         return image
     
     @property
-    def background_PhotoImage(this) -> ImageTk.PhotoImage:
-        """Tkinter PhotoImage of this Object
+    def animation(this) -> 'Sprite.Animation':
+        """Returns the current animation
 
         Returns:
-            ImageTk.PhotoImage: Tkinter PhotoImage
+            Sprite.Animation: A Sprite.Animation class
         """
-        this._PhotoImage['background'] = ImageTk.PhotoImage(this.background)
-        return this._PhotoImage['background']
+        return this._currentAnimation
+    @animation.setter
+    def animation(this, animation : str | int):
+        if isinstance(animation, (int, float)):
+            animation = int(animation)
+            this._currentAnimation = this.animations[animation]
+        elif isinstance(animation, str):
+            for a in this.animations:
+                if a.name == animation:
+                    this._currentAnimation = a
+                    break
+        elif isinstance(animation, this.Animation):
+            this._currentAnimation = animation
     
     @property
-    def foreground(this) -> Image.Image:
-        """The foreground of the Object image
+    def frames(this) -> list['Sprite.Animation.Frame']:
+        """Returns the current animation frames.
 
         Returns:
-            PIL.Image.Image: PIL Image
+            list[Sprite.Animation.Frame]: A list of frames.
         """
-        this.getOffset()
-        image = Image.new('RGBA', tuple(this.size * this.scale), (0,0,0,0))
-        
-        for sprite in this._foreground:
-            size = (numpy.array(sprite.image.size) / sprite.scale) * [1,-1]
-            pos = this.truePos(
-                sprite.pos,
-                size,
-                this.size,
-                scale = this.scale,
-                offset = this._offset
-            )
-            
-            # print(f'{pos = }')
-            
-            image.alpha_composite(
-                sprite.image,
-                tuple([round(x) for x in pos]),
-            )
-        image = this.rotateImage(image)
-        
-        return image
+        return this.animation.frames
     
     @property
-    def foreground_PhotoImage(this) -> ImageTk.PhotoImage:
-        """Foregound Tkinter PhotoImage
+    def frame(this) -> int:
+        """The current animation frame.
 
         Returns:
-            ImageTk.PhotoImage: Tkinter PhotoImage
+            int: Current animation frame index.
         """
-        this._PhotoImage['foreground'] = ImageTk.PhotoImage(this.foreground)
-        return this._PhotoImage['foreground']
+        return this.animation.frame
+    @frame.setter
+    def frame(this, value : int):
+        this.animation.frame = value
     
     @property
-    def image(this) -> Image.Image:
-        """Full Object image, with both the background and foreground.
-
-        Returns:
-            PIL.Image.Image: PIL Image
-        """
-        
-        image = this.background
-        image.alpha_composite(this.foreground)
-        
-        return image
+    def fps(this) -> float:
+        return this.animation.fps
     
     @property
-    def offset(this) -> tuple[float,float]:
-        """The center offset of the Object image
-
-        Returns:
-            tuple[float,float]: (x,y)
+    def filename(this) -> str:
+        """Sprite filename
         """
-        this.getOffset()
-        offset = this._offset
-        
-        offset = this.rotatePoint(this._offset)
-        
-        return offset
-    
-    def rotatePoint(this, point : tuple = (0,0), angle : float = None) -> tuple[float,float]:
-        """Rotate a point around (0,0)
-
-        Args:
-            point (tuple, optional): Point to rotate. Defaults to (0,0).
-            angle (float, optional): Angle to rotate. Defaults to Object `Angle` property.
-
-        Returns:
-            tuple[float,float]: (x,y)
-        """
-        if angle == None:
-            if 'Angle' in this.properties:
-                angle = float(this.properties['Angle'])
-            else:
-                angle = 0
-        
-        if angle == 0:
-            return point
-        
-        return rotate(point, degrees=-angle)
-    
-    def rotateImage(this, image : Image.Image) -> Image.Image:
-        """Rotate an image the amount of degrees as the Object `Angle` property
-
-        Args:
-            image (PIL.Image.Image): Image to rotate
-
-        Returns:
-            PIL.Image.Image: Rotated PIL Image
-        """
-        if 'Angle' in this.properties:
-            angle = float(this.properties['Angle'])
-            image = image.rotate(angle, expand = True, resample = Image.BILINEAR)
-        
-        return image
-    
-    @property
-    def PhotoImage(this) -> ImageTk.PhotoImage:
-        """Tkinter PhotoImage of the Object image
-
-        Returns:
-            ImageTk.PhotoImage: Tkinter PhotoImage
-        """
-        this._PhotoImage['image'] = ImageTk.PhotoImage(this.image)
-        return this._PhotoImage['image']
-    
-    @property
-    def scale(this) -> int:
-        """Object image scale
-        """
-        return this._scale
-    @scale.setter
-    def scale(this, value : int):
-        this._scale = value
-        for sprite in this.sprites:
-            sprite.scale = this._scale
+        if 'filename' in this.properties:
+            return this.properties['filename']
+        else:
+            return None
+    @filename.setter
+    def filename(this, value):
+        this.properties['filename'] = value
         
     def readXML(this):
-        """Read object XML
+        """Read Sprite XML
         """
-        
-        # specifically specifying type so it's easier to use in vscode
-        tags = {
-            'Shapes': this._getShapes,
-            'Sprites': this._getSprites,
-            'UVs': this._getUVs,
-            'VertIndices': this._getVertIndices,
-            'DefaultProperties': this._getDefaultProperties,
-        }
-        
+        this.animations = []
         for element in this.xml:
-            if element is etree.Comment:
-                continue
-            if element.tag in tags:
-                tags[element.tag](element)
-        
-        this.getProperties()
+            if (not element is etree.Comment) or element.tag == 'Animation':
+                animation = this.Animation(
+                    element,
+                    this.filesystem,
+                    HD = this.HD,
+                    TabHD = this.TabHD,
+                )
+                
+                this.animations.append(animation)
     
-    def export(this, path : str = None) -> bytes:
-        """Export object XML
+    def export(this, path : str = None):
+        """Export the Sprite XML file
 
         Args:
-            path (str, optional): Filename for object. Defaults to Object.filename.
+            path (str, optional): Path to export into the filesystem. Defaults to the original filename.
 
         Raises:
-            TypeError: Path is not a file
+            TypeError: Path is not a file.
 
         Returns:
-            bytes: XML file.
+            str: Contents of saved file.
         """
-        xml : etree.ElementBase = etree.Element('InteractiveObject')
-        
-        shapes = etree.Element('Shapes')
-        
-        for shape in this.shapes:
-            shape : Shape
-            shapes.append(shape.getXML())
-        
-        if len(shapes) > 0:
-            xml.append(shapes)
-        
-        sprites : etree.ElementBase = etree.Element('Sprites')
-        
-        for sprite in this.sprites:
-            sprite : Sprite
-            sprite.export()
-            etree.SubElement(sprites, 'Sprite', sprite.properties)
-        
-        if len(sprites) > 0:
-            xml.append(sprites)
-        
-        UVs : etree.ElementBase = etree.Element('UVs')
+        xml : etree.ElementBase = etree.Element('Sprite')
         
-        for UV in this.UVs:
-            pos = ' '.join([str(_) for _ in UV])
-            etree.SubElement(UVs, 'UV', {'pos': pos})
-        
-        if len(UVs) > 0:
-            xml.append(UVs)
-        
-        VertIndices : etree.ElementBase = etree.Element('VertIndices')
-        
-        for index in this.VertIndices:
-            etree.SubElement(VertIndices, 'Vert', {'index': str(index)})
-        
-        if len(VertIndices) > 0:
-            xml.append(VertIndices)
-        
-        DefaultProperties : etree.ElementBase = etree.Element('DefaultProperties')
-        
-        for name in this.defaultProperties:
-            etree.SubElement(DefaultProperties, 'Property', {
-                'name': name,
-                'value': this.defaultProperties[name]
-            })
-        
-        if len(DefaultProperties) > 0:
-            xml.append(DefaultProperties)
+        for animation in this.animations:
+            xml.append(animation.getXML())
         
         this.xml = xml
+        
         output = etree.tostring(xml, pretty_print=True, xml_declaration=True, encoding='utf-8')
         
         if path == None:
             if this.filename:
                 path = this.filename
         
         if path != None:
             if (file := this.filesystem.get(path)) != None:
                 if isinstance(file, File):
                     file.write(output)
                 else:
                     raise TypeError(f'Path {path} is not a file.')
-                    
             else:
                 this.filesystem.add(path, output)
         
         return output
     
-    def updateProperties(this):
-        """Update properties. Deletes any properties that are the same as defaultProperties.
-        """
-        properties = list(this.properties.keys())
-        
-        # for property in properties:
-        #     if property in this.defaultProperties:
-        #         if this.properties[property] == this.defaultProperties[property]:
-        #             del this.properties[property]
-        
-        # if this.type != None:
-        #     this.properties['Type'] = this.type
-
-    def getLevelXML(
-        this,
-        filename : str = None,
-    ) -> etree.ElementBase:
-        """Gets XML to be used in levels.
-
-        Args:
-            filename (str, optional): Object filename. Defaults to Object.filename.
-
-        Returns:
-            etree.Element: lxml Element
-        """
-        if filename == None:
-            if this.filename:
-                filename = this.filename
-        else:
-            this.filename = filename
-        
-        xml = etree.Element('Object', name = this.name)
-        etree.SubElement(xml, 'AbsoluteLocation', value = ' '.join([str(_) for _ in this.pos]))
-        
-        properties = etree.SubElement(xml, 'Properties')
-        
-        this.updateProperties()
-        
-        for name in this.properties:
-            value = this.properties[name]
-            
-            etree.SubElement(properties, 'Property', name = name, value = str(value))
-        
-        this.getProperties()
-        
-        return xml
-    
     @property
-    def filename(this) -> str | None:
-        """Object filename based on the `Filename` proprty
+    def visible(this) -> bool:
+        """Whether this Sprite is visible or not
         """
-        if 'Filename' in this.properties:
-            return this.properties['Filename']
-        else:
-            return None
-    @filename.setter
-    def filename(this, value : str):
-        this.properties['Filename'] = value
+        if 'visible' in this.properties:
+            return strbool(this.properties['visible'])
+        return False
+    @visible.setter
+    def visible(this, value : bool | str):
+        this.properties['visible'] = str(strbool(value)).lower()
     
     @property
-    def type(this) -> str | None:
-        """The Object type, based off the `Type` property.
-        """
-        if 'Type' in this.properties:
-            return this.properties['Type']
-        elif 'Type' in this.defaultProperties:
-            return this.defaultProperties['Type']
-        else:
-            return ''
-    @type.setter
-    def type(this, value : str):
-        if not isinstance(value, str):
-            raise TypeError('type is not a string')
-        
-        if not 'Type' in this.defaultProperties:
-            this.defaultProperties['Type'] = value
-        this.properties['Type'] = value
-    
-    def _getShapes(this, xml : etree.ElementBase):
-        for element in xml:
-            shape = Shape(element)
-            this.shapes.append(shape)
-        
-    def _getSprites(this, xml : etree.ElementBase):
-        for element in xml:
-            if element is etree.Comment:
-                continue
-            
-            if element.tag == 'Sprite':
-                attributes = element.attrib
-                sprite = Sprite(
-                    file = this.filesystem.get(attributes['filename']),
-                    filesystem = this.filesystem,
-                    properties = attributes,
-                    scale = this.scale,
-                )
-                this.sprites.append(sprite)
-    
-    def _getUVs(this, xml : etree.ElementBase):
-        for element in xml:
-            if element is etree.Comment:
-                continue
-            if element.tag == 'UV':
-                pos = element.get('pos')
-                this.UVs.append(tuple([float(_) for _ in pos.split()]))
-    
-    def _getVertIndices(this, xml : etree.ElementBase):
-        for element in xml:
-            if element is etree.Comment:
-                continue
-            if element.tag == 'Vert':
-                index = element.get('index')
-                this.VertIndices.append(int(index))
-    
-    def getProperties(this):
-        for prop in this.defaultProperties:
-            this.properties[prop] = this.defaultProperties[prop]
-        for prop in this._properties:
-            this.properties[prop] = this._properties[prop]
-        return this.properties
-    
-    def _getDefaultProperties(this, xml : etree.ElementBase):
-        for element in xml:
-            if element is etree.Comment:
-                continue
-            if element.tag == 'Property':
-                name = element.get('name')
-                value = element.get('value')
-                
-                this.defaultProperties[name] = value
-    
-    def setProperty(this, property : str | dict, value : str = ''):
-        """Set object property.
-
-        Args:
-            property (str | dict): Property name to set. If value is dict, it will combine the properties in the dict with the current properties.
-            value (str, optional): Property value. Defaults to ''.
+    def isBackground(this):
+        """Whether this Sprite is a background
         """
-        if isinstance(property, dict):
-            for name in property:
-                this.properties[name] = property[name]
-            return
-        this.properties[property] = value
-
-class Shape(GameObject):
-    def __init__(this, xml : etree.ElementBase = None) -> None:
-        """Shape for Object
-
-        Args:
-            xml (etree.Element, optional): lxml Element. Defaults to None.
-        """
-        this.points : list[tuple[float,float]] = []
-        this.xml = xml
-        
-        this.readXML()
-    
-    def readXML(this):
-        """Read XML if any.
-        """
-        if this.xml == None:
-            return
-        for element in this.xml:
-            if element is etree.Comment:
-                continue
-            if element.tag == 'Point':
-                pos : str = element.get('pos')
-                point = tuple([float(_) for _ in pos.split()])
-                this.points.append(point)
+        if 'isBackground' in this.properties:
+            return strbool(this.properties['isBackground'])
+        return False
+    @isBackground.setter
+    def isBackground(this, value : bool | str):
+        this.properties['isBackground'] = str(strbool(value)).lower()
     
-    def getXML(this) -> etree.ElementBase:
-        """Gets Shape XML for Object.
+    @property
+    def gridSize(this) -> tuple[float,float]:
+        """The gridSize (size) of this Sprite
 
         Returns:
-            etree.Element: lxml Element.
+            tuple[float,float]: (width,height)
         """
-        xml : etree.ElementBase = etree.Element('Shape')
-        for point in this.points:
-            etree.SubElement(xml, 'Point', {'pos': ' '.join([str(_) for _ in point])})
-        this.xml = xml
-        return xml
+        if 'gridSize' in this.properties:
+            return tuple([float(x) for x in this.properties['gridSize'].split()])
+        return (1,1)
+    @gridSize.setter
+    def gridSize(this, value : tuple[int,int] | str):
+        if isinstance(value, str):
+            this.properties['gridSize'] = value
+        elif isinstance(value, (tuple, list)):
+            this.properties['gridSize'] = ' '.join([str(x) for x in value])
     
     @property
-    def image(this) -> Image.Image:
-        """Get the Shape image
+    def pos(this) -> tuple[float,float]:
+        """Position of Sprite relative to the center of the Object
 
         Returns:
-            PIL.Image.Image: PIL Image
+            tuple[float,float]: (x,y)
         """
-        points = numpy.array(this.points).swapaxes(0,1)
-        
-        min = numpy.array([math.floor(v.min()) for v in points])
-        max = numpy.array([math.ceil(v.max()) for v in points])
-        
-        offset = numpy.array([a.mean() for a in numpy.array([min,max]).swapaxes(0,1)])
-        # offset = offset * [1,-1]
-        # print(f'{offset = }')
+        if 'pos' in this.properties:
+            return tuple([float(x) for x in this.properties['pos'].split()])
+        return (0,0)
+    @pos.setter
+    def pos(this, value : tuple[int,int] | str):
+        if isinstance(value, str):
+            this.properties['pos'] = value
+        elif isinstance(value, (tuple, list)):
+            this.properties['pos'] = ' '.join([str(x) for x in value])
+    
+    @property
+    def angle(this) -> float:
+        """Sprite rotation angle
+
+        Returns:
+            float: Angle as degrees
+        """
+        if 'angle' in this.properties:
+            return float(this.properties['angle'])
+        return 0
+    @angle.setter
+    def angle(this, value : int | float):
+        this.properties['angle'] = str(value)
+    
+    def getAnimation(
+        this,
+        duration : int = 0,
+        fps : float = 0,
+    ) -> dict[
+        typing.Literal[
+            'fps',
+            'frame_duration',
+            'frames',
+        ],
+        float |
+        int |
+        list[Image.Image]
+    ]:
         
-        size = max - min
+        """Get the animation of this object
+
+        Args:
+            duration (int, optional): Duration of animation in seconds. If 0, it will try to create a perfect loop. Defaults to 0.
+            fps (float, optional): The fps of the animation. If 0, it will try to detect the fps that works for all the sprites. Defaults to 0.
+
+        Raises:
+            TypeError: 'fps must be an int or float'
+        """
+        return this.animation.getAnimation(
+            duration = duration,
+            fps = fps,
+        )
+    
+    def saveGIF(
+        this,
+        filename : str = None,
+        duration : int = 0,
+        fps : float = 0,
+    ):
         
-        image = Image.new('1', tuple([math.ceil(x) + 1 for x in size]), 1)
-        draw = ImageDraw.Draw(image)
+        """Save current animation as a gif.
+
+        Args:
+            filename (str, optional): The filename to save this animation gif as. Defaults to None.
+            duration (int, optional): The duration of the gif in seconds. If it's 0, it automatically finds a perfect loop. Defaults to 0.
+            fps (float, optional): The frames per second of the animation. If it's 0, it is automatically calculated. Defaults to 0.
+
+        Returns:
+            PIL.Image.Image: The resulting PIL Image object.
+        """
+        if filename in ['', None]:
+            filename = f'{os.path.splitext(os.path.basename(this.filename))[0]}-{this.animation.name}.gif'
+        
+        this.animation.saveGIF(
+            filename = filename,
+            duration = duration,
+            fps = fps,
+        )
+
+    class Animation(GameObject):
+        def __init__(
+            this,
+            xml : str | etree.ElementBase,
+            filesystem: Filesystem | Folder = None,
+            gamepath: str = None,
+            assets: str = '/assets',
+            baseassets: str = '/',
+            HD : bool = False,
+            TabHD : bool = False,
+        ) -> None:
+            """Animation for Sprite.
+
+            Args:
+                xml (str | etree.Element): lxml.etree Element xml element for sprite.
+                filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
+                gamepath (str, optional): Game path. Only used if filesystem not specified. Defaults to None.
+                assets (str, optional): Assets path relative to game path. Only used if filesystem not specified. Defaults to '/assets'.
+                baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`
+                HD (bool, optional): Use HD images. Defaults to False.
+                TabHD (bool, optional): Use TabHD images. Defaults to False.
+            """
+            super().__init__(filesystem, gamepath, assets, baseassets)
+            
+            if isinstance(xml, str):
+                this.xml : etree.ElementBase = etree.parse(xml).getroot()
+            else:
+                this.xml = xml
+            
+            this.HD = HD
+            this.TabHD = TabHD
+            
+            this.properties = {}
+            this.name = ''
+            this.textureBasePath = '/Textures/'
+            this.atlas : Imagelist = None
+            this.fps = 30
+            this.playbackMode = 'ONCE'
+            this.loopCount = 1
+            
+            this._PhotoImage = None
+            
+            this.frames : list[Sprite.Animation.Frame] = []
+            this.frame = 0
+            
+            this.readXML()
+        
+        @property
+        def image(this) -> Image.Image:
+            """Current Animation image
+
+            Returns:
+                PIL.Image.Image: PIL Image
+            """
+            
+            return this.frames[this.frame].image
+        
+        @property
+        def frame(this) -> int:
+            return this._frame
+        @frame.setter
+        def frame(this, value : int):
+            if len(this.frames) > 0:
+                this._frame = int(value) % len(this.frames)
+            else:
+                this._frame = 0
         
-        # size = size * [1,-1]
-        # print(f'{size = }')
-        for n in range(len(this.points)):
-            point = this.points[n]
-            previous = (this.points[(n - 1) % len(this.points)])
+        @property
+        def PhotoImage(this) -> 'ImageTk.PhotoImage':
+            """Tkinter PhotoImage for the Animation
+            """
+            if LOADED_ImageTk:
+                this._PhotoImage = ImageTk.PhotoImage(this.image)
+            else:
+                this._PhotoImage = this.image.copy()
             
-            line = numpy.array([point, previous])
-            # line = line * [1,-1]
-            line = numpy.array(this.truePos(
-                line,
-                (1,1),
-                size,
-                offset,
-            ))
+            return this._PhotoImage
             
-            # print(line)
+        def readXML(this):
+            """Read the xml for this Animation
+            """
+            this.getAttributes()
+            this.getFrames()
+        
+        def getAttributes(this):
+            """Get all the attributes of this Animation
+            """
+            this.properties = this.xml.attrib
+            
+            if 'name' in this.properties:
+                this.name = this.properties['name']
+            if 'textureBasePath' in this.properties:
+                this.textureBasePath = this.properties['textureBasePath']
+            if 'atlas' in this.properties:
+                this.atlasPath = this.properties['atlas']
+                this.atlas = Imagelist(
+                    this.filesystem.get(this.properties['atlas']),
+                    this.filesystem,
+                    HD=this.HD,
+                    TabHD = this.TabHD,
+                )
+                
+                # this.atlasHD = Imagelist(
+                #     this.filesystem.get(this.properties['atlas']),
+                #     this.filesystem,
+                #     HD=True
+                # )
+                
+            if 'playbackMode' in this.properties:
+                this.playbackMode = this.properties['playbackMode']
+            if 'loopCount' in this.properties:
+                this.loopCount = int(this.properties['loopCount'])
+            
+            
+        def getFrames(this) -> list['Sprite.Animation.Frame']:
+            """Get a list of all the Animation `Frame`s
+
+            Returns:
+                list[Sprite.Animation.Frame]: List of all the Frames in this Animation.
+            """
+            this.frames = []
+            
+            if this.xml == None:
+                return None
+            for f in this.xml:
+                if (not f is etree.Comment) and f.tag == 'Frame':
+                    this.frames.append(this.Frame(
+                        f.attrib,
+                        this.atlas,
+                        this.textureBasePath
+                    ))
+            
+            return this.frames
+
+        def updateProperties(this):
+            """Update the Sprite properties
+            """
+            def updateProperty(property : str, value, default = None):
+                if default != None and value == default:
+                    if property in this.properties:
+                        del this.properties[property]
+                else:
+                    this.properties[property] = value
             
-            line = line.flatten()
-            line = tuple([round(x) for x in line])
+            updateProperty('name', this.name)
+            updateProperty('textureBasePath', this.textureBasePath)
+            this.atlas.export(this.atlasPath, exportImage=True)
+            updateProperty('atlas', this.atlasPath)
+            updateProperty('fps', str(this.fps))
+            updateProperty('playbackMode', this.playbackMode)
+            updateProperty('loopCount', str(this.loopCount))
+        
+        def getXML(this):
+            """Get the XML of this Animation
+
+            Returns:
+                etree.Element: etree Element
+            """
+            this.updateProperties()
+            xml : etree.ElementBase = etree.Element('Animation', **this.properties)
+            
+            for frame in this.frames:
+                xml.append(frame.getXML())
+            
+            this.xml = xml
+            return this.xml
+        
+        @property
+        def fps(this):
+            if 'fps' in this.properties:
+                return float(this.properties['fps'])
+            else:
+                this.fps = 30
+                return this.fps
+        @fps.setter
+        def fps(this, value : int | float | str):
+            this.properties['fps'] = str(value)
+        
+        def getAnimation(
+            this,
+            duration : int = 0,
+            fps : float = 0,
+        ) -> dict[
+            typing.Literal[
+                'fps',
+                'frame_duration',
+                'frames',
+            ],
+            float |
+            int |
+            list[Image.Image]
+        ]:
+            """Get the animation of this object
+
+            Args:
+                duration (int, optional): Duration of animation in seconds. If 0, it will try to create a perfect loop. Defaults to 0.
+                fps (float, optional): The fps of the animation. If 0, it will try to detect the fps that works for all the sprites. Defaults to 0.
+
+            Raises:
+                TypeError: 'fps must be an int or float'
+            """
+            if not isinstance(fps, (int, float)) and not fps == None:
+                raise TypeError('fps must be an int or float')
+            
+            if not isinstance(duration, (int, float)) and not duration == None:
+                raise TypeError('duration must be an int or float')
+            
+            if (fps in [0, None]) or (fps <= 0):
+                fps = this.fps
+            
+            frames : list[Image.Image] = []
+            this.frame = 0
+            frame = 0
+            time = 0
+            
+            def check():
+                if duration > 0:
+                    return time <= duration
+                
+                if (time <= 0) or (frame <= 1):
+                    return True
+                if this.frame == 0:
+                    return False
+                
+                return True
+                
+                # print(f'test = {( not ((time > 0) and (duration <= 0) and ((sum([sprite.frame for sprite in this.sprites]) == 0))))}')
+                # print(f'time check = {((time <= duration) and (duration > 0))}')
             
+            while check():
+                this.frame += (frame) % ((fps / this.fps) + 1)
+                
+                frames.append(this.image)
+                
+                frame += 1
+                time += (1000 / fps) / 1000
+            
+            # frames = frames[:-1]
+            
+            return {
+                'fps': fps,
+                'frame_duration' : (1000 / fps) / 1000,
+                'frames' : frames,
+            }
+        
+        def saveGIF(
+            this,
+            filename = None,
+            duration : int = 0,
+            fps : float = 0,
+        ) -> Image.Image:
+            """Save animation as a gif.
+
+            Args:
+                filename (str, optional): The filename to save this animation gif as. Defaults to None.
+                duration (int, optional): The duration of the gif in seconds. If it's 0, it automatically finds a perfect loop. Defaults to 0.
+                fps (float, optional): The frames per second of the animation. If it's 0, it is automatically calculated. Defaults to 0.
+
+            Returns:
+                PIL.Image.Image: The resulting PIL Image object.
+            """
+            if filename == None:
+                filename = this.name
+                filename = os.path.splitext(filename)[0] + '.gif'
+                
+                print(f'{filename = }')
             
-            draw.line(line, fill=0, width=1)
+            animation = this.getAnimation(
+                duration = duration,
+                fps = fps,
+            )
+            
+            return save_transparent_gif(
+                animation['frames'],
+                durations = animation['frame_duration'],
+                save_file = filename,
+            )
         
-        return image
+        # Frame
+        class Frame():
+            _offset = (0,0)
+            _scale = (1,1)
+            _angleDeg = 0
+            _repeat = 1
+            def __init__(
+                this,
+                properties : dict,
+                atlas : Imagelist = None,
+                textureBasePath : str = None,
+            ) -> None:
+                """Frame for Sprite.Animation.
+
+                Args:
+                    this (_type_): _description_
+                    properties (dict): Image properties.
+                    atlas (Imagelist, optional): Image atlas for Image. Defaults to None.
+                    textureBasePath (str, optional): Directory to put image in. Defaults to None.
+                """
+                this.atlas = atlas
+                this.textueBasePath = textureBasePath
+                this.properties = properties
+                
+                this.name = ''
+                this.offset = this._offset
+                this.scale = this._scale
+                this.angleDeg = this._angleDeg
+                this.repeat = this._repeat
+                
+                
+                
+                this.getData()
+                this.getImage()
+            
+            def getData(this):
+                """Get the Frame data
+                """
+                if 'name' in this.properties:
+                    this.name = this.properties['name']
+                if 'offset' in this.properties:
+                    this.offset = tuple([float(x) for x in this.properties['offset'].split()])
+                if 'scale' in this.properties:
+                    this.scale = tuple([float(x) for x in this.properties['scale'].split()])
+                if 'angleDeg' in this.properties:
+                    this.angleDeg = float(this.properties['angleDeg'])
+                if 'repeat' in this.properties:
+                    this.repeat = int(this.properties['repeat'])
+                
+            def getImage(this):
+                this._image = this.atlas.get(this.name)
+            
+            @property
+            def image(this) -> Image.Image:
+                """Image of this Image
+
+                Returns:
+                    PIL.Image.Image: PIL Image
+                """
+                if this._image:
+                    image = this._image.image.copy()
+                    image = image.resize(tuple([round(_) for _ in (numpy.array(this._image.size) * numpy.array(this.scale))]))
+                    image = image.rotate(this.angleDeg, expand = True)
+                else:
+                    image = Image.new('RGBA', (1,1), (0,0,0,0))
+                return image
+            @image.setter
+            def image(this, image : Image.Image):
+                this._image = image
+            
+            def updateProperties(this):
+                """Update Image properties
+                """
+                def updateProperty(property : str, value, default):
+                    if value == default:
+                        if property in this.properties:
+                            del this.properties[property]
+                    else:
+                        this.properties[property] = value
+                
+                this.properties['name'] = this.name
+                
+                updateProperty(
+                    'offset',
+                    ' '.join([str(_) for _ in this.offset]),
+                    ' '.join([str(_) for _ in this._offset])
+                )
+                
+                updateProperty(
+                    'scale',
+                    ' '.join([str(_) for _ in this.scale]),
+                    ' '.join([str(_) for _ in this._scale])
+                )
+                
+                updateProperty(
+                    'angleDeg',
+                    str(this.angleDeg),
+                    str(this._angleDeg)
+                )
+                
+                updateProperty(
+                    'repeat',
+                    str(this.repeat),
+                    str(this._repeat)
+                )
+
+            def getXML(this) -> etree.ElementBase:
+                """Get the XML for the Frame
+
+                Returns:
+                    etree.Element: XML of this Frame
+                """
+                this.updateProperties()
+                return etree.Element('Frame', **this.properties)
+            
+            def show(this, title: str | None = None):
+                """Calls the PIL.Image.Image.show() method.
+                
+                ---
+                #### Description copied from the PIL library
+                
+                Displays this image. This method is mainly intended for debugging purposes.
+
+                This method calls PIL.ImageShow.show internally. You can use
+                PIL.ImageShow.register to override its default behaviour.
+
+                The image is first saved to a temporary file. By default, it will be in PNG format.
+
+                On Unix, the image is then opened using the **display**, **eog** or **xv** utility, depending on which one can be found.
+
+                On macOS, the image is opened with the native Preview application.
+
+                On Windows, the image is opened with the standard PNG display utility.
+
+                Args:
+                    title (str | None, optional): Optional title to use for the image window, where possible.. Defaults to None.
+                """
+                return this.image.show(title = title)
```

### Comparing `wmwpy-0.3.0b0/src/wmwpy/classes/widget/__init__.py` & `wmwpy-0.4.0b0/src/wmwpy/classes/widget/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from PIL import ImageTk
-
 from .widget import Widget, register_widget, WIDGETS, get_widget
 
 from .WT_PUSH_BUTTON import WT_PUSH_BUTTON
 from .WT_LABEL import WT_LABEL
 from .WT_TOGGLE import WT_TOGGLE
 from .WT_SLIDER import WT_SLIDER
 from .WT_PROGRESS_BAR import WT_PROGRESS_BAR
```

### Comparing `wmwpy-0.3.0b0/src/wmwpy/classes/widget/widget.py` & `wmwpy-0.4.0b0/src/wmwpy/classes/widget/widget.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.3.0b0/src/wmwpy/game.py` & `wmwpy-0.4.0b0/src/wmwpy/game.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import typing
+import logging
 
 from .Utils.filesystem import *
 from .Utils import Texture
+from .Utils import path
 from .classes import *
 
 class Game():
     _DB = '/Data/water.db'
     _BASEASSETS = '/'
     _PROFILE = None
     
@@ -15,177 +17,232 @@
     def __init__(
         this,
         gamepath : str, assets : str = '/assets',
         db : str = '/Data/water.db',
         profile : str = None,
         baseassets : str = '/',
         platform : typing.Literal['android', 'ios'] = 'android',
-        hook : typing.Callable[[int, str, int], typing.Any] = None,
+        load_callback : typing.Callable[[int, str, int], typing.Any] = None,
     ) -> None:
         """load game
 
         Args:
             gamepath (str): Folder to extracted game.
             assets (str, optional): Relative path to assets folder. Defaults to '/assets'.
             db (str, optional): Relative path to database file from assets folder. Defaults to '/Data/water.db'.
             profile (str, optional): Relative path to profile file in WMW2. Defaults to `None`
             baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`
             platform (Literal['android', 'ios'], optional): What platform this game is for. Can be 'android' or 'ios'. Defaults to 'android'.
-            hook (Callable[[int, str, int], Any], optional): Hook for loading assets, useful for guis. The function gets called with the paramaters `(progress : int, current : str, max : int)`. Defaults to None.
+            load_callbac (Callable[[int, str, int], Any], optional): (Callable[[int, str, int], Any], optional): A callback function to be ran while loading the game. Defaults to None.
         """
         if gamepath == None:
             return
         
         this.gamepath = os.path.abspath(gamepath)
         # print(f'{gamepath = }\n{this.gamepath = }')
         this.assets = assets
         this.db = db or this._DB
         this.profile = profile or this._PROFILE
         this.baseassets = baseassets or this._BASEASSETS
         this.platform = platform
         
         
-        this.updateFilesystem(hook = hook)
+        this.updateFilesystem(load_callback = load_callback)
         
-    def updateFilesystem(this, hook : typing.Callable[[int, str, int], typing.Any] = None):
+    def updateFilesystem(this, load_callback : typing.Callable[[int, str, int], typing.Any] = None):
         this.filesystem = Filesystem(this.gamepath, this.assets)
-        this.filesystem.getAssets(hook = hook)
+        this.filesystem.getAssets(load_callback = load_callback)
+    
+    def dump(
+        this,
+        folder = None,
+        callback : typing.Callable[[int, str, int], typing.Any] = None,
+    ):
+        """Dump the contents of the filesystem to the specified directory
+
+        Args:
+            folder (str, optional): Path to output directory. Defaults to original path.
+            callback (Callable[[int, str, int], Any], optional): A callback function to be ran while dumping the filesystem. Defaults to None.
+        """
+        this.filesystem.dump(folder = folder, callback = callback)
         
     def Level(
         this,
         xmlPath : str = None,
         imagePath : str = None,
         load_callback : typing.Callable[[int, str, int], typing.Any] = None,
         ignore_errors : bool = False,
+        HD = False,
+        TabHD = False,
     ):
         """
         Load level
 
         Args:
             xmlPath (str, optional): Path to xml file. Defaults to None.
             imagePath (str, optional): Path to image file. Defaults to None.
         """
+        logging.debug(f'Game: xml input: {xmlPath}')
+        
+        levels = this.filesystem.get(path.joinPath(this.baseassets, '/Levels'))
+        
         if isinstance(xmlPath, File):
             xml = xmlPath
+            
+            logging.debug(f'Game: xml path: {xmlPath.path}')
+            
         else:
             xml = None
             if xmlPath:
                 split = os.path.splitext(xmlPath)
                 if split[1] == '':
                     if imagePath in ['', None]:
                         imagePath = '.'.join([split[0], 'png'])
                     xmlPath = '.'.join([split[0], 'xml'])
                 
-                xml = this.filesystem.get(xmlPath)
+                xml = levels.get(xmlPath)
+        
+        logging.debug(f'Game: xml file before {xml}')
+        
+        if isinstance(xml, File):
+            logging.debug(f'Game: xml path: {xml.path}')
         
         if isinstance(imagePath, File):
             image = imagePath
         else:
             image = None
             if imagePath:
-                image = this.filesystem.get(imagePath)
+                image = levels.get(imagePath)
+        
+        logging.debug(f'Game: xml after: {xml}')
+        if isinstance(xml, File):
+            logging.debug(f'Game: xml path: {xml.path}')
         
         level = Level(
             xml = xml,
             image = image,
             filesystem = this.filesystem,
             load_callback = load_callback,
             ignore_errors = ignore_errors,
+            HD = HD,
+            TabHD = TabHD,
         )
         if isinstance(xmlPath, File):
             level.filename = xmlPath.path
         else:
             level.filename = xmlPath
         
         return level
     
     def Object(
         this,
         object : str,
+        HD : bool = False,
+        TabHD : bool = False,
         **kwargs
     ):
         """
-        Loads object
+        Load object
 
         Args:
             object (str): Path to `.hs` object file.
+            HD (bool, optional): Use HD images. Defaults to False.
+            TabHD (bool, optional): Use TabHD images. Defaults to False.
 
         Returns:
             classes.object.Object: Where's My Water? object.
         """
         
+        objects = this.filesystem.get(path.joinPath(this.baseassets, '/Objects'))
         
         if not isinstance(object, File):
-            object = this.filesystem.get(object)
+            object = objects.get(object)
         
         obj = Object(
             object,
             filesystem = this.filesystem,
+            HD = HD,
+            TabHD = TabHD,
             **kwargs
         )
         if isinstance(object, File):
             obj.filename = object.path
         else:
             obj.filename = object
             
         
         return obj
     
     def Imagelist(
         this,
         imagelist : str = None,
         HD = False,
+        TabHD = False,
+        save_images = False
     ):
         """
         Load imagelist
 
         Args:
             imagelist (str): Path to `.imagelist` file. Defaults to None
-            HD (bool, optional): Whether to use HD textures. Defaults to False.
+            HD (bool, optional): Use HD images. Defaults to False.
+            TabHD (bool, optional): Use TabHD images. Defaults to False.
 
         Returns:
             classes.imagelist.Imagelist: Imagelist object.
         """
         
+        textures = this.filesystem.get(path.joinPath(this.baseassets, '/Textures'))
+        
         if not isinstance(imagelist, File):
-            imagelist = this.filesystem.get(imagelist)
+            imagelist = textures.get(imagelist)
         
         imagelistObject = Imagelist(
             imagelist,
             filesystem = this.filesystem,
-            HD = False,
+            HD = HD,
+            TabHD = TabHD,
+            save_images = save_images,
         )
         if isinstance(imagelist, File):
             imagelistObject.filename = imagelist.path
         else:
             imagelistObject.filename = imagelist
         
         return imagelistObject
     
     def Sprite(
         this,
         sprite : str,
+        HD = False,
+        TabHD = False,
         **kwargs
     ):
         """
         Loads sprite.
 
         Args:
-            sprite (str): Path to `.sprite` file.`
+            sprite (str): Path to `.sprite` file.
+            HD (bool, optional): Use HD images. Defaults to False.
+            TabHD (bool, optional): Use TabHD images. Defaults to False.
 
         Returns:
             classes.sprite.Sprite: Sprite object.
         """
         
+        sprites = this.filesystem.get(path.joinPath(this.baseassets, '/Sprites'))
+        
         if not isinstance(sprite, File):
-            sprite = this.filesystem.get(sprite)
+            sprite = sprites.get(sprite)
         
         spriteObject = Sprite(
             sprite,
             filesystem = this.filesystem,
+            HD = HD,
+            TabHD = TabHD,
             **kwargs
         )
         if isinstance(sprite, File):
             spriteObject.filename = sprite.path
         else:
             spriteObject.filename = sprite.path
         
@@ -201,25 +258,27 @@
         Args:
             texture (str): Path to image file.
 
         Returns:
             Utils.textures.Texture: Texture object.
         """
         
+        textures = this.filesystem.get(path.joinPath(this.baseassets, '/Textures'))
+        
         if not isinstance(texture, File):
-            texture = this.filesystem.get(texture)
+            texture = textures.get(texture)
         
         return Texture(
             texture
         )
     
     def Layout(this, layout : str):
         raise NotImplementedError('load layout is not implemented yet.')
     
-    def generateFileManifest(this, writeFile : bool = True, filename : str = '/FileManifest.txt'):
+    def FileManifest(this, writeFile : bool = True, filename : str = '/FileManifest.txt'):
         """Generate the `FileManifest.txt` file needed for some games, such as WMM. This just generates a text file with the paths to every file in the `assets` folder (which includes the `FileManifest.txt` file).
 
         Args:
             writeFile (bool, optional): Write the manifest to the `FileManifest.txt` file. Defaults to True.
             filename (str, optional): Filename for FileManifest.txt. Defaults to 'filename'.
 
         Returns:
```

### Comparing `wmwpy-0.3.0b0/src/wmwpy/gameobject.py` & `wmwpy-0.4.0b0/src/wmwpy/gameobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             
         elif isinstance(this.filesystem, Folder):
             pass
         
         elif hasattr(this.filesystem, 'filesystem'):
             this.filesystem = this.filesystem.filesystem
 
-        else:
+        elif this.gamepath:
             this.filesystem = Filesystem(this.gamepath, this.assets)
             this.filesystem.getAssets()
         # except Exception as e:
         #     print(f'Error: {str(e)}')
         #     raise FileNotFoundError('Must have a valid `filesystem` or `gamepath`')
     
     def get_file(
```

### Comparing `wmwpy-0.3.0b0/src/wmwpy/gametemplate.py` & `wmwpy-0.4.0b0/src/wmwpy/gametemplate.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         db: str = '/Data/water.db',
         profile: str = None,
         baseassets: str = '/',
         hook: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
         
         
-        super().__init__(gamepath, assets, db, profile, baseassets, hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = hook)
 
 class WMWF(WMW):
     _DB = '/Data/water-Lite.db'
     
     game = 'WMWF'
     
     def __init__(
@@ -33,15 +33,15 @@
         gamepath: str,
         assets: str = '/assets',
         db: str = '/Data/water-Lite.db',
         profile: str = None,
         baseassets: str = '/',
         hook: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
-        super().__init__(gamepath, assets, db, profile, baseassets, hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, hook = hook)
 
 # Where's My Perry?
 class WMP(Game):
     _DB = '/Perry/Data/perry.db'
     _BASEASSETS = '/Perry/'
     
     game = 'WMP'
@@ -51,15 +51,15 @@
         gamepath: str,
         assets: str = '/assets',
         db: str = '/Perry/Data/water.db',
         profile: str = None,
         baseassets: str = '/Perry/',
         hook: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
-        super().__init__(gamepath, assets, db, profile, baseassets, hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = hook)
 
 class WMPF(WMP):
     _DB = '/Perry/Data/perry-Lite.db'
     
     game = 'WMPF'
     
     def __init__(
@@ -67,15 +67,15 @@
         gamepath: str,
         assets: str = '/assets',
         db: str = '/Perry/Data/water-Lite.db',
         profile: str = None,
         baseassets: str = '/Perry/',
         hook: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
-        super().__init__(gamepath, assets, db, profile, baseassets, hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, hook = hook)
 
 # Where's My Mickey?
 class WMM(Game):
     _DB = '/Mickey/Data/perry.db'
     _BASEASSETS = '/Mickey/'
     
     game = 'WMM'
@@ -85,15 +85,15 @@
         gamepath: str,
         assets: str = '/assets',
         db: str = '/Mickey/Data/perry.db',
         profile: str = None,
         baseassets: str = '/Mickey/',
         hook: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
-        super().__init__(gamepath, assets, db, profile, baseassets, hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = hook)
 
 class WMMF(WMM):
     _DB = '/Mickey/Data/perry-Lite.db'
     
     game = 'WMMF'
     
     def __init__(
@@ -101,15 +101,15 @@
         gamepath: str,
         assets: str = '/assets',
         db: str = '/Mickey/Data/perry-Lite.db',
         profile: str = None,
         baseassets: str = '/Mickey/',
         hook: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
-        super().__init__(gamepath, assets, db, profile, baseassets, hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, hook = hook)
 
 # Where's My XiYangYang?
 class WMXYY(Game):
     _DB = '/Perry/Data/perry.db'
     _BASEASSETS = '/Perry/'
     
     game = 'WMXYY'
@@ -120,15 +120,15 @@
         assets: str = '/assets',
         db: str = '/Perry/Data/water.db',
         profile: str = None,
         baseassets: str = '/Perry/',
         hook: typing.Callable[[int, str, int], typing.Any] = None,
         databasekey = None
     ) -> None:
-        super().__init__(gamepath, assets, db, profile, baseassets, hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = hook)
 
 class WMWFXYY(Game):
     _DB = '/Perry/Data/perry.db'
     _BASEASSETS = '/Perry/'
     
     game = 'WMWFXYY'
     
@@ -138,15 +138,15 @@
         assets: str = '/assets',
         db: str = '/Perry/Data/water.db',
         profile: str = None,
         baseassets: str = '/Perry/',
         hook: typing.Callable[[int, str, int], typing.Any] = None,
         databasekey = None
     ) -> None:
-        super().__init__(gamepath, assets, db, profile, baseassets, hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = hook)
 
 # Where's My Water 2?
 class WMW2(Game):
     _DB = '/Water/Data/perry.db'
     _BASEASSETS = '/Water/'
     _PROFILE = '/Water/Data/factory_profile.json'
     
@@ -157,15 +157,15 @@
         gamepath: str,
         assets: str = '/assets',
         db: str = '/Water/Data/perry.db',
         profile: str = '/Water/Data/factory_profile.json',
         baseassets: str = '/Water/',
         hook: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
-        super().__init__(gamepath, assets, db, profile, baseassets, hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = hook)
 
 # Where's My Holiday?
 class WMH(Game):
     _DB = '/Data/water-Lite.db'
     _BASEASSETS = '/'
     
     game = 'WMH'
@@ -175,15 +175,15 @@
         gamepath: str,
         assets: str = '/assets',
         db: str = '/Data/water-Lite.db',
         profile: str = None,
         baseassets: str = '/',
         hook: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
-        super().__init__(gamepath, assets, db, profile, baseassets, hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = hook)
     
     def mode(this, mode : typing.Literal['wmw', 'wmp'] = 'wmw'):
         """Switch game mode from 'wmw' to 'wmp' and vice verca.
 
         Args:
             mode (str, optional): Mode. Can be 'wmw' or 'wmp'. Defaults to 'wmw'.
         """
@@ -212,15 +212,15 @@
         gamepath: str,
         assets: str = '/Content',
         db: str = '/Perry/Data/water-Lite.db',
         profile: str = None,
         baseassets: str = '/Perry/',
         hook: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
-        super().__init__(gamepath, assets, db, profile, baseassets, hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, hook = hook)
 
 GAMES : dict[str, Game] = {}
 
 def register_game(name : str, class_ : Game):
     """Register a game template
 
     Args:
```

### Comparing `wmwpy-0.3.0b0/src/wmwpy.egg-info/PKG-INFO` & `wmwpy-0.4.0b0/src/wmwpy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmwpy
-Version: 0.3.0b0
+Version: 0.4.0b0
 Summary: Python module to work with Where's My...? games files.
 Author: ego-lay-atman-bay
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -685,23 +685,336 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wmwpy
- Python module for working with Where's My...? game files.
+Python module for working with Where's My...? game files.
 
- <!-- Note: using https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/ for distributing.-->
+<!-- Note: using https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/ for distributing.-->
 
- This is going to be used in Where's My Editor, a level editor for the Where's My...? series.
+This is being used in [Where's My Editor](https://github.com/wmw-modding/wheres-my-editor), a level editor for the Where's My...? series.
+
+
+# Table of contents
+
+- [wmwpy](#wmwpy)
+- [Table of contents](#table-of-contents)
+- [Installation](#installation)
+- [Usage](#usage)
+  - [Get game folder](#get-game-folder)
+  - [Loading the game](#loading-the-game)
+  - [Main classes](#main-classes)
+    - [Level](#level)
+      - [Challenges](#challenges)
+    - [Object](#object)
+- [Building package](#building-package)
+- [Building docs](#building-docs)
+- [Credits](#credits)
+
+# Installation
+To install `wmwpy`, run
+
+```
+pip install wmwpy
+```
+
+or
+
+```
+python -m pip install wmwpy
+```
+
+You can also install it from the source, which may be needed because it is frequently being updated, although you need to make sure `git` is installed.
+
+```
+pip install wmwpy@git+https://github.com/wmw-modding/wmwpy
+```
+
+# Usage
+## Get game folder
+To get started, you need to have a Where's My Water? game folder, either an extracted apk, ipa, or on a rooted / jailbroken device (for editing the game files directly). The game must be extracted like this.
+
+```
+- root
+ - assets
+  - ...
+```
+ 
+The assets folder can be specified in `wmwpy`.
+
+## Loading the game
+Start by loading the game inside `wmwpy`
+
+```python
+import wmwpy
+game = wmwpy.load('game/wmw')
+```
+
+You can specify the assets folder
+
+```python
+game = wmwpy.load('game/wmw', assets = '/assets')
+```
+
+You can set `assets = '.'` if you have the gamepath (first parameter) set to the assets folder (such as on a rooted / jailbroken device).
+
+Alternately, you can specify the platform.
+
+```python
+game = wmwpy.load('game/wmw', platform = 'android')
+```
+
+This automatically sets the assets folder to what it is on the platform.
+
+| Platform | assets folder |
+| -------- | ------------- |
+| android  | /assets       |
+| ios      | /Content      |
+
+You can also specify the game, which sets things up for that game.
+
+```python
+game = wmwpy.load('game/wmp', game = 'WMP')
+```
+
+Currently all the games are
+
+| Game                                   | Code      |
+| ----                                   | ----      |
+| Where's My Water?                      | 'WMW'     |
+| Where's My Water? Free                 | 'WMWF'    |
+| Where's My Perry?                      | 'WMP'     |
+| Where's My Perry? Free                 | 'WMPF'    |
+| Where's My Mickey?                     | 'WMM'     |
+| Where's My Mickey? XL                  | 'WMMXL'   |
+| Where's My Mickey? Free                | 'WMMF'    |
+| Where's My XiYangYang?                 | 'WMXYY'   |
+| Where's My Water? Featuring XiYangYang | 'WMWFXYY' |
+| Where's My Water? 2                    | 'WMW2'    |
+| Where's My Holiday?                    | 'WMH'     |
+| Where's My Valentine?                  | 'WMV'     |
+| Where's My Summer?                     | 'WMS'     |
+
+You can also specify the base assets path, the folder within the assets folder that contains all the assets. For example, Where's My Perry? has all the data within `/assets/Perry`.
+
+```python
+game = wmwpy.load('game/wmp', baseassets = '/Perry')
+```
+
+Each game has the database in a different location, so you can specify it.
+
+```python
+game = wmwpy.load('game/wmp', db = '/Perry/Data/perry.db')
+```
+
+Since Where's My Water? 2 uses a profile instead of a database for the save data, you can also specify that.
+
+```python
+game = wmwpy.load('game/wmw2', profile = '/Water/Data/factory_profile.json')
+```
+
+You can also provide a function to be called during the loading, so you can keep track of the current progress, e.g. in a gui application with a progress bar.
+
+```python
+game = wmwpy.load('game/wmw', load_hook = lambda progress, text, max : print(f'({progress}/{max}) {text}'))
+```
+
+The inputs for the function are
+```
+(
+   progress : int,
+   text : str,
+   max : int,
+)
+```
+
+Once you're done editing all the files, you need to dump the all the assets.
+
+```python
+game.dump()
+```
+
+This will save all the files in the game inside the assets folder. You can customize this if you want them saved in a different location.
+
+```python
+game.dump(folder = 'path/to/output')
+```
+
+## Main classes
+
+### Level
+To load a level from within a game, use the `.Level()` method.
+
+```python
+level = game.Level('first_dig')
+```
+
+The first input can be the name of a level inside the `/Levels` folder (`first_dig`), an absolute path to the level (`/Levels/first_dig`), or the path to an xml file (`/Levels/first_dig.xml`).
+
+You can also specify the xml and image separately.
+
+```python
+level = game.Level(xmlPath = '/Levels/first_dig.xml', imagePath = '/Levels/first_dig.png')
+```
+
+Some levels include objects that wmwpy fails to load, so you can use the `ignore_errors` parameter to ignore them.
+
+```python
+level = game.Level('first_dig', ignore_errors = True)
+```
+
+You can also use the HD or TabHD textures for the objects.
+
+```python
+level = game.Level('first_dig', HD = True, TabHD = True)
+```
+
+If both are specified, TabHD will get priority. If it can't load TabHD textures. See hierarchy.
+
+```
+- TabHD
+ - HD
+  - Low Quality
+```
+
+You can also provide a function to run while loading to see the current progress.
+
+```python
+level = game.Level('first_dig', load_callback = lambda progress, text, max : print(f'({progress}/{max}) {text}'))
+```
+
+The inputs for the function are
+```
+(
+   progress : int,
+   text : str,
+   max : int,
+)
+```
+
+The objects in the level are all accessible in a list
+
+```python
+>> level.objects
+[
+   <wmwpy.classes.object.Object object at 0x000001C7627FE850>,
+   ...
+]
+```
+
+See [Object](#Object)
+
+The level properties are also accessible as a dictionary
+
+```python
+>> level.properties
+{'HeavyIntro': '1'}
+```
+
+WMW2 challenges are also accessible in a list
+
+```python
+>> level.challenges
+[<wmwpy.classes.level.Level.Challenge object at 0x000001C72176ADD0>]
+```
+
+Once you're finished editing the level, you can get the xml.
+
+```python
+xml = level.export(filename = '/Levels/first_dig.xml',)
+```
+
+This returns the xml file as `bytes`, but also saves the file to the game filesystem.
+
+#### Challenges
+Each challenge has requirements in a dictionary
+```python
+>> level.challenges[0].requirements
+{
+    'WinWait': {
+        'seconds': ''
+    },
+    'Duck': {
+        'count': '2'
+    }
+}
+```
+
+### Object
+To load an object within a game, use the `.Object()` method.
+
+```python
+obj = game.Object('/Objects/broken_pipe.hs')
+```
+
+You can also use the HD or TabHD textures for the objects.
+
+```python
+level = game.Level('first_dig', HD = True, TabHD = True)
+```
+
+If both are specified, TabHD will get priority. If it can't load TabHD textures. See hierarchy.
+
+```
+- TabHD
+ - HD
+  - Low Quality
+```
+
+An object has many properties
+
+```python
+>> obj.properties
+{
+    'Type' : 'spout',
+    'SpoutType' : 'DrainSpout',
+    'Goal' : '1',
+    'GoalPreset', : 'Swampy',
+}
+```
+
+An object also has many [Sprites](#Sprite)
+
+```python
+>> obj.sprites
+[<wmwpy.classes.sprite.Sprite object>]
+```
+
+The object image is a `PIL` image.
+
+```python
+>> obj.image
+<PIL.Image.Image image mode=RGBA size=300x300>
+```
+
+The image scale can be set
+
+```python
+obj.scale = 20
+```
+
+You can also save a GIF of the object animations
+
+```python
+obj.saveGIF('broken_pipe.gif')
+```
+
+Once you're finished editing the object, you can get the xml.
+
+```python
+xml = export('/Objects/broken_pipe.hs',)
+```
+
+This returns the xml file as `bytes`, but also saves the file to the game filesystem.
 
 # Building package
- To build the package, install `build`
- ```
+To build the package, install `build`
+```
 pip install build
  ```
  Then run
  ```
 py -m build
  ```
```

### Comparing `wmwpy-0.3.0b0/src/wmwpy.egg-info/SOURCES.txt` & `wmwpy-0.4.0b0/src/wmwpy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/wmwpy.egg-info/dependency_links.txt
 src/wmwpy.egg-info/requires.txt
 src/wmwpy.egg-info/top_level.txt
 src/wmwpy/Font/__init__.py
 src/wmwpy/Utils/XMLTools.py
 src/wmwpy/Utils/__init__.py
 src/wmwpy/Utils/filesystem.py
+src/wmwpy/Utils/gif.py
 src/wmwpy/Utils/logging_utils.py
 src/wmwpy/Utils/path.py
 src/wmwpy/Utils/rotate.py
 src/wmwpy/Utils/textures.py
 src/wmwpy/Utils/waltex.py
 src/wmwpy/Utils/Types/Documents.py
 src/wmwpy/Utils/Types/Images.py
```

