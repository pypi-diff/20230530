# Comparing `tmp/ffmpeg-progress-yield-0.7.6.tar.gz` & `tmp/ffmpeg-progress-yield-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg-progress-yield-0.7.6.tar", last modified: Tue May 30 07:05:57 2023, max compression
+gzip compressed data, was "ffmpeg-progress-yield-0.7.7.tar", last modified: Tue May 30 14:51:49 2023, max compression
```

## Comparing `ffmpeg-progress-yield-0.7.6.tar` & `ffmpeg-progress-yield-0.7.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 07:05:57.176997 ffmpeg-progress-yield-0.7.6/
--rw-r--r--   0 werner     (501) staff       (20)     2473 2023-05-30 07:05:56.000000 ffmpeg-progress-yield-0.7.6/CHANGELOG.md
--rw-r--r--   0 werner     (501) staff       (20)     1086 2023-05-05 06:38:37.000000 ffmpeg-progress-yield-0.7.6/LICENSE
--rw-r--r--   0 werner     (501) staff       (20)    10022 2023-05-30 07:05:57.177096 ffmpeg-progress-yield-0.7.6/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)     6773 2023-05-05 06:38:38.000000 ffmpeg-progress-yield-0.7.6/README.md
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 07:05:57.175205 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield/
--rw-r--r--   0 werner     (501) staff       (20)      103 2023-05-30 07:05:55.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield/__init__.py
--rw-r--r--   0 werner     (501) staff       (20)     1283 2023-05-30 06:56:19.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield/__main__.py
--rw-r--r--   0 werner     (501) staff       (20)     7903 2023-05-30 07:05:38.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield/ffmpeg_progress_yield.py
--rw-r--r--   0 werner     (501) staff       (20)        0 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield/py.typed
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 07:05:57.176051 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield.egg-info/
--rw-r--r--   0 werner     (501) staff       (20)    10022 2023-05-30 07:05:57.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield.egg-info/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)      494 2023-05-30 07:05:57.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield.egg-info/SOURCES.txt
--rw-r--r--   0 werner     (501) staff       (20)        1 2023-05-30 07:05:57.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield.egg-info/dependency_links.txt
--rw-r--r--   0 werner     (501) staff       (20)       78 2023-05-30 07:05:57.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield.egg-info/entry_points.txt
--rw-r--r--   0 werner     (501) staff       (20)        1 2021-03-01 12:51:44.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield.egg-info/not-zip-safe
--rw-r--r--   0 werner     (501) staff       (20)       22 2023-05-30 07:05:57.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield.egg-info/top_level.txt
--rw-r--r--   0 werner     (501) staff       (20)      279 2023-05-30 07:05:57.177518 ffmpeg-progress-yield-0.7.6/setup.cfg
--rw-r--r--   0 werner     (501) staff       (20)     1748 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.6/setup.py
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 07:05:57.176776 ffmpeg-progress-yield-0.7.6/test/
--rw-r--r--   0 werner     (501) staff       (20)    37351 2022-12-11 11:53:49.000000 ffmpeg-progress-yield-0.7.6/test/test.mp4
--rw-r--r--   0 werner     (501) staff       (20)     4235 2023-05-30 07:03:53.000000 ffmpeg-progress-yield-0.7.6/test/test.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 14:51:49.009763 ffmpeg-progress-yield-0.7.7/
+-rw-r--r--   0 werner     (501) staff       (20)     2473 2023-05-30 14:51:48.000000 ffmpeg-progress-yield-0.7.7/CHANGELOG.md
+-rw-r--r--   0 werner     (501) staff       (20)     1086 2023-05-05 06:38:37.000000 ffmpeg-progress-yield-0.7.7/LICENSE
+-rw-r--r--   0 werner     (501) staff       (20)    10022 2023-05-30 14:51:49.009870 ffmpeg-progress-yield-0.7.7/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)     6773 2023-05-05 06:38:38.000000 ffmpeg-progress-yield-0.7.7/README.md
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 14:51:49.007881 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield/
+-rw-r--r--   0 werner     (501) staff       (20)      103 2023-05-30 14:51:46.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield/__init__.py
+-rw-r--r--   0 werner     (501) staff       (20)     1283 2023-05-30 06:56:19.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield/__main__.py
+-rw-r--r--   0 werner     (501) staff       (20)     7903 2023-05-30 07:05:38.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield/ffmpeg_progress_yield.py
+-rw-r--r--   0 werner     (501) staff       (20)        0 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield/py.typed
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 14:51:49.008745 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield.egg-info/
+-rw-r--r--   0 werner     (501) staff       (20)    10022 2023-05-30 14:51:48.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield.egg-info/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)      494 2023-05-30 14:51:48.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield.egg-info/SOURCES.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2023-05-30 14:51:48.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield.egg-info/dependency_links.txt
+-rw-r--r--   0 werner     (501) staff       (20)       78 2023-05-30 14:51:48.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield.egg-info/entry_points.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2021-03-01 12:51:44.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield.egg-info/not-zip-safe
+-rw-r--r--   0 werner     (501) staff       (20)       22 2023-05-30 14:51:48.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield.egg-info/top_level.txt
+-rw-r--r--   0 werner     (501) staff       (20)      279 2023-05-30 14:51:49.010215 ffmpeg-progress-yield-0.7.7/setup.cfg
+-rw-r--r--   0 werner     (501) staff       (20)     1748 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.7/setup.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 14:51:49.009508 ffmpeg-progress-yield-0.7.7/test/
+-rw-r--r--   0 werner     (501) staff       (20)    37351 2022-12-11 11:53:49.000000 ffmpeg-progress-yield-0.7.7/test/test.mp4
+-rw-r--r--   0 werner     (501) staff       (20)     4235 2023-05-30 07:03:53.000000 ffmpeg-progress-yield-0.7.7/test/test.py
```

### Comparing `ffmpeg-progress-yield-0.7.6/CHANGELOG.md` & `ffmpeg-progress-yield-0.7.7/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.6/LICENSE` & `ffmpeg-progress-yield-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.6/PKG-INFO` & `ffmpeg-progress-yield-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-progress-yield
-Version: 0.7.6
+Version: 0.7.7
 Summary: Run an ffmpeg command with progress
 Home-page: https://github.com/slhck/ffmpeg-progress-yield
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Keywords: ffmpeg
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ffmpeg-progress-yield-0.7.6/README.md` & `ffmpeg-progress-yield-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield/__main__.py` & `ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield/__main__.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield/ffmpeg_progress_yield.py` & `ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield/ffmpeg_progress_yield.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield.egg-info/PKG-INFO` & `ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-progress-yield
-Version: 0.7.6
+Version: 0.7.7
 Summary: Run an ffmpeg command with progress
 Home-page: https://github.com/slhck/ffmpeg-progress-yield
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Keywords: ffmpeg
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ffmpeg-progress-yield-0.7.6/setup.py` & `ffmpeg-progress-yield-0.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.6/test/test.mp4` & `ffmpeg-progress-yield-0.7.7/test/test.mp4`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.6/test/test.py` & `ffmpeg-progress-yield-0.7.7/test/test.py`

 * *Files identical despite different names*

