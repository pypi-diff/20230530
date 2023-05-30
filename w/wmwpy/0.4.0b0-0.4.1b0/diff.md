# Comparing `tmp/wmwpy-0.4.0b0.tar.gz` & `tmp/wmwpy-0.4.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wmwpy-0.4.0b0.tar", last modified: Tue May 30 20:42:16 2023, max compression
+gzip compressed data, was "wmwpy-0.4.1b0.tar", last modified: Tue May 30 21:22:02 2023, max compression
```

## Comparing `wmwpy-0.4.0b0.tar` & `wmwpy-0.4.1b0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:42:16.723925 wmwpy-0.4.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    49356 2023-05-30 20:42:16.723925 wmwpy-0.4.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8230 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 20:42:16.723925 wmwpy-0.4.0b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:42:16.711925 wmwpy-0.4.0b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:42:16.715925 wmwpy-0.4.0b0/src/wmwpy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:42:16.715925 wmwpy-0.4.0b0/src/wmwpy/Font/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Font/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:42:16.715925 wmwpy-0.4.0b0/src/wmwpy/Utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:42:16.715925 wmwpy-0.4.0b0/src/wmwpy/Utils/Types/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/Types/Documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/Types/Images.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/Types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/XMLTools.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22603 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/gif.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/textures.py
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/Utils/waltex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:42:16.719925 wmwpy-0.4.0b0/src/wmwpy/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/Widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    26480 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/imagelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/level.py
--rw-r--r--   0 runner    (1001) docker     (123)    23989 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    25624 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/sprite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:42:16.723925 wmwpy-0.4.0b0/src/wmwpy/classes/widget/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_CANVAS.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_FINGER_CATCHER.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_GROUP.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_ICON_LIST.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_LABEL.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_PROGRESS_BAR.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_PUSH_BUTTON.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_SCROLLABLE_CAMERA.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_SCROLLABLE_SET.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_SLIDER.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/WT_TOGGLE.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/classes/widget/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/game.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/gameobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-30 20:42:04.000000 wmwpy-0.4.0b0/src/wmwpy/gametemplate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:42:16.715925 wmwpy-0.4.0b0/src/wmwpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    49356 2023-05-30 20:42:16.000000 wmwpy-0.4.0b0/src/wmwpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-30 20:42:16.000000 wmwpy-0.4.0b0/src/wmwpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:42:16.000000 wmwpy-0.4.0b0/src/wmwpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 20:42:16.000000 wmwpy-0.4.0b0/src/wmwpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 20:42:16.000000 wmwpy-0.4.0b0/src/wmwpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:22:02.055078 wmwpy-0.4.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    49356 2023-05-30 21:22:02.055078 wmwpy-0.4.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8230 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:22:02.055078 wmwpy-0.4.1b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:22:02.043078 wmwpy-0.4.1b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:22:02.043078 wmwpy-0.4.1b0/src/wmwpy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:22:02.047078 wmwpy-0.4.1b0/src/wmwpy/Font/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Font/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:22:02.047078 wmwpy-0.4.1b0/src/wmwpy/Utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:22:02.047078 wmwpy-0.4.1b0/src/wmwpy/Utils/Types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/Types/Documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/Types/Images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/Types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/XMLTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22603 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/gif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/textures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/waltex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:22:02.051078 wmwpy-0.4.1b0/src/wmwpy/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/Widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26480 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/imagelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23989 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25624 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/sprite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:22:02.055078 wmwpy-0.4.1b0/src/wmwpy/classes/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_CANVAS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_FINGER_CATCHER.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_GROUP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_ICON_LIST.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_LABEL.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_PROGRESS_BAR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_PUSH_BUTTON.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_SCROLLABLE_CAMERA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_SCROLLABLE_SET.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_SLIDER.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_TOGGLE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/gameobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/gametemplate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:22:02.047078 wmwpy-0.4.1b0/src/wmwpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49356 2023-05-30 21:22:02.000000 wmwpy-0.4.1b0/src/wmwpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-30 21:22:02.000000 wmwpy-0.4.1b0/src/wmwpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:22:02.000000 wmwpy-0.4.1b0/src/wmwpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:22:02.000000 wmwpy-0.4.1b0/src/wmwpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 21:22:02.000000 wmwpy-0.4.1b0/src/wmwpy.egg-info/top_level.txt
```

### Comparing `wmwpy-0.4.0b0/LICENSE` & `wmwpy-0.4.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/PKG-INFO` & `wmwpy-0.4.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmwpy
-Version: 0.4.0b0
+Version: 0.4.1b0
 Summary: Python module to work with Where's My...? games files.
 Author: ego-lay-atman-bay
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `wmwpy-0.4.0b0/README.md` & `wmwpy-0.4.1b0/README.md`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/pyproject.toml` & `wmwpy-0.4.1b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/Utils/Types/Documents.py` & `wmwpy-0.4.1b0/src/wmwpy/Utils/Types/Documents.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/Utils/Types/Images.py` & `wmwpy-0.4.1b0/src/wmwpy/Utils/Types/Images.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/Utils/XMLTools.py` & `wmwpy-0.4.1b0/src/wmwpy/Utils/XMLTools.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/Utils/filesystem.py` & `wmwpy-0.4.1b0/src/wmwpy/Utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/Utils/gif.py` & `wmwpy-0.4.1b0/src/wmwpy/Utils/gif.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/Utils/path.py` & `wmwpy-0.4.1b0/src/wmwpy/Utils/path.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/Utils/rotate.py` & `wmwpy-0.4.1b0/src/wmwpy/Utils/rotate.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/Utils/textures.py` & `wmwpy-0.4.1b0/src/wmwpy/Utils/textures.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/Utils/waltex.py` & `wmwpy-0.4.1b0/src/wmwpy/Utils/waltex.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/__init__.py` & `wmwpy-0.4.1b0/src/wmwpy/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4.0-beta"
+__version__ = "0.4.1-beta"
 __author__ = 'ego-lay-atman-bay'
 
 import typing
 import logging
 
 from .game import Game
 from . import Utils
@@ -48,25 +48,25 @@
             'assets': '/Content',
         },
     }
     
     if assets == None:
         assets = platforms[platform]['assets']
     
-    try:
-        return GAMES[game](
-            gamepath = gamepath,
-            assets = assets,
-            db = db,
-            profile = profile,
-            load_callback = load_callback,
-            baseassets = baseassets,
-        )
-    except:
-        return Game(
-            gamepath = gamepath,
-            assets = assets,
-            db = db,
-            profile = profile,
-            load_callback = load_callback,
-            baseassets = baseassets,
-        )
+    # try:
+    return GAMES.get(game, Game)(
+        gamepath = gamepath,
+        assets = assets,
+        db = db,
+        profile = profile,
+        load_callback = load_callback,
+        baseassets = baseassets,
+    )
+    # except:
+    #     return Game(
+    #         gamepath = gamepath,
+    #         assets = assets,
+    #         db = db,
+    #         profile = profile,
+    #         load_callback = load_callback,
+    #         baseassets = baseassets,
+    #     )
```

### Comparing `wmwpy-0.4.0b0/src/wmwpy/classes/Widgets.py` & `wmwpy-0.4.1b0/src/wmwpy/classes/Widgets.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/classes/curves.py` & `wmwpy-0.4.1b0/src/wmwpy/classes/curves.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/classes/imagelist.py` & `wmwpy-0.4.1b0/src/wmwpy/classes/imagelist.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/classes/layout.py` & `wmwpy-0.4.1b0/src/wmwpy/classes/layout.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/classes/level.py` & `wmwpy-0.4.1b0/src/wmwpy/classes/level.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/classes/object.py` & `wmwpy-0.4.1b0/src/wmwpy/classes/object.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/classes/sprite.py` & `wmwpy-0.4.1b0/src/wmwpy/classes/sprite.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/classes/widget/__init__.py` & `wmwpy-0.4.1b0/src/wmwpy/classes/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/classes/widget/widget.py` & `wmwpy-0.4.1b0/src/wmwpy/classes/widget/widget.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/game.py` & `wmwpy-0.4.1b0/src/wmwpy/game.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/gameobject.py` & `wmwpy-0.4.1b0/src/wmwpy/gameobject.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.0b0/src/wmwpy/gametemplate.py` & `wmwpy-0.4.1b0/src/wmwpy/gametemplate.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,35 +13,35 @@
     def __init__(
         this,
         gamepath: str,
         assets: str = '/assets',
         db: str = '/Data/water.db',
         profile: str = None,
         baseassets: str = '/',
-        hook: typing.Callable[[int, str, int], typing.Any] = None
+        load_callback: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
         
         
-        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = load_callback)
 
 class WMWF(WMW):
     _DB = '/Data/water-Lite.db'
     
     game = 'WMWF'
     
     def __init__(
         this,
         gamepath: str,
         assets: str = '/assets',
         db: str = '/Data/water-Lite.db',
         profile: str = None,
         baseassets: str = '/',
-        hook: typing.Callable[[int, str, int], typing.Any] = None
+        load_callback: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
-        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, hook = hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = load_callback)
 
 # Where's My Perry?
 class WMP(Game):
     _DB = '/Perry/Data/perry.db'
     _BASEASSETS = '/Perry/'
     
     game = 'WMP'
@@ -49,33 +49,33 @@
     def __init__(
         this,
         gamepath: str,
         assets: str = '/assets',
         db: str = '/Perry/Data/water.db',
         profile: str = None,
         baseassets: str = '/Perry/',
-        hook: typing.Callable[[int, str, int], typing.Any] = None
+        load_callback: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
-        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = load_callback)
 
 class WMPF(WMP):
     _DB = '/Perry/Data/perry-Lite.db'
     
     game = 'WMPF'
     
     def __init__(
         this,
         gamepath: str,
         assets: str = '/assets',
         db: str = '/Perry/Data/water-Lite.db',
         profile: str = None,
         baseassets: str = '/Perry/',
-        hook: typing.Callable[[int, str, int], typing.Any] = None
+        load_callback: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
-        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, hook = hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = load_callback)
 
 # Where's My Mickey?
 class WMM(Game):
     _DB = '/Mickey/Data/perry.db'
     _BASEASSETS = '/Mickey/'
     
     game = 'WMM'
@@ -83,33 +83,33 @@
     def __init__(
         this,
         gamepath: str,
         assets: str = '/assets',
         db: str = '/Mickey/Data/perry.db',
         profile: str = None,
         baseassets: str = '/Mickey/',
-        hook: typing.Callable[[int, str, int], typing.Any] = None
+        load_callback: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
-        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = load_callback)
 
 class WMMF(WMM):
     _DB = '/Mickey/Data/perry-Lite.db'
     
     game = 'WMMF'
     
     def __init__(
         this,
         gamepath: str,
         assets: str = '/assets',
         db: str = '/Mickey/Data/perry-Lite.db',
         profile: str = None,
         baseassets: str = '/Mickey/',
-        hook: typing.Callable[[int, str, int], typing.Any] = None
+        load_callback: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
-        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, hook = hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = load_callback)
 
 # Where's My XiYangYang?
 class WMXYY(Game):
     _DB = '/Perry/Data/perry.db'
     _BASEASSETS = '/Perry/'
     
     game = 'WMXYY'
@@ -117,36 +117,36 @@
     def __init__(
         this,
         gamepath: str,
         assets: str = '/assets',
         db: str = '/Perry/Data/water.db',
         profile: str = None,
         baseassets: str = '/Perry/',
-        hook: typing.Callable[[int, str, int], typing.Any] = None,
+        load_callback: typing.Callable[[int, str, int], typing.Any] = None,
         databasekey = None
     ) -> None:
-        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = load_callback)
 
 class WMWFXYY(Game):
     _DB = '/Perry/Data/perry.db'
     _BASEASSETS = '/Perry/'
     
     game = 'WMWFXYY'
     
     def __init__(
         this,
         gamepath: str,
         assets: str = '/assets',
         db: str = '/Perry/Data/water.db',
         profile: str = None,
         baseassets: str = '/Perry/',
-        hook: typing.Callable[[int, str, int], typing.Any] = None,
+        load_callback: typing.Callable[[int, str, int], typing.Any] = None,
         databasekey = None
     ) -> None:
-        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = load_callback)
 
 # Where's My Water 2?
 class WMW2(Game):
     _DB = '/Water/Data/perry.db'
     _BASEASSETS = '/Water/'
     _PROFILE = '/Water/Data/factory_profile.json'
     
@@ -155,17 +155,17 @@
     def __init__(
         this,
         gamepath: str,
         assets: str = '/assets',
         db: str = '/Water/Data/perry.db',
         profile: str = '/Water/Data/factory_profile.json',
         baseassets: str = '/Water/',
-        hook: typing.Callable[[int, str, int], typing.Any] = None
+        load_callback: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
-        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = load_callback)
 
 # Where's My Holiday?
 class WMH(Game):
     _DB = '/Data/water-Lite.db'
     _BASEASSETS = '/'
     
     game = 'WMH'
@@ -173,17 +173,17 @@
     def __init__(
         this,
         gamepath: str,
         assets: str = '/assets',
         db: str = '/Data/water-Lite.db',
         profile: str = None,
         baseassets: str = '/',
-        hook: typing.Callable[[int, str, int], typing.Any] = None
+        load_callback: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
-        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = load_callback)
     
     def mode(this, mode : typing.Literal['wmw', 'wmp'] = 'wmw'):
         """Switch game mode from 'wmw' to 'wmp' and vice verca.
 
         Args:
             mode (str, optional): Mode. Can be 'wmw' or 'wmp'. Defaults to 'wmw'.
         """
@@ -210,17 +210,17 @@
     def __init__(
         this,
         gamepath: str,
         assets: str = '/Content',
         db: str = '/Perry/Data/water-Lite.db',
         profile: str = None,
         baseassets: str = '/Perry/',
-        hook: typing.Callable[[int, str, int], typing.Any] = None
+        load_callback: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
-        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, hook = hook)
+        super().__init__(gamepath = gamepath, assets = assets, db = db, profile = profile, baseassets = baseassets, load_callback = load_callback)
 
 GAMES : dict[str, Game] = {}
 
 def register_game(name : str, class_ : Game):
     """Register a game template
 
     Args:
```

### Comparing `wmwpy-0.4.0b0/src/wmwpy.egg-info/PKG-INFO` & `wmwpy-0.4.1b0/src/wmwpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmwpy
-Version: 0.4.0b0
+Version: 0.4.1b0
 Summary: Python module to work with Where's My...? games files.
 Author: ego-lay-atman-bay
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `wmwpy-0.4.0b0/src/wmwpy.egg-info/SOURCES.txt` & `wmwpy-0.4.1b0/src/wmwpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

