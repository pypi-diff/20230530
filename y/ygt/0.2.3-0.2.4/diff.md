# Comparing `tmp/ygt-0.2.3.tar.gz` & `tmp/ygt-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ygt-0.2.3.tar", last modified: Fri May 26 02:52:38 2023, max compression
+gzip compressed data, was "ygt-0.2.4.tar", last modified: Tue May 30 21:22:06 2023, max compression
```

## Comparing `ygt-0.2.3.tar` & `ygt-0.2.4.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-26 02:52:38.092718 ygt-0.2.3/
--rw-r--r--   0 peterbaker   (504) staff       (20)    11358 2022-11-11 22:39:04.000000 ygt-0.2.3/LICENSE
--rw-r--r--   0 peterbaker   (504) staff       (20)      181 2023-04-16 16:44:10.000000 ygt-0.2.3/MANIFEST.in
--rw-r--r--   0 peterbaker   (504) staff       (20)     4547 2023-05-26 02:52:38.092592 ygt-0.2.3/PKG-INFO
--rw-r--r--   0 peterbaker   (504) staff       (20)     4151 2023-05-26 02:30:51.000000 ygt-0.2.3/README.md
--rw-r--r--   0 peterbaker   (504) staff       (20)      822 2023-05-26 02:40:12.000000 ygt-0.2.3/pyproject.toml
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-05-26 02:52:38.092750 ygt-0.2.3/setup.cfg
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2022-11-11 22:39:05.000000 ygt-0.2.3/setup.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-26 02:52:38.076929 ygt-0.2.3/src/
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-26 02:52:38.077472 ygt-0.2.3/src/hooks/
--rw-rw-r--   0 peterbaker   (504) staff       (20)      103 2023-05-04 12:22:22.000000 ygt-0.2.3/src/hooks/hook-freetype.py
--rw-r--r--   0 peterbaker   (504) staff       (20)      143 2023-05-07 08:59:05.000000 ygt-0.2.3/src/hooks/hook-xgridfit.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-26 02:52:38.084083 ygt-0.2.3/src/ygt/
--rw-r--r--   0 peterbaker   (504) staff       (20)        1 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/__init__.py
--rw-r--r--   0 peterbaker   (504) staff       (20)       64 2023-04-06 15:04:52.000000 ygt-0.2.3/src/ygt/__main__.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     1673 2023-04-12 11:23:21.000000 ygt-0.2.3/src/ygt/autohint_trash.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     3721 2023-05-04 10:24:55.000000 ygt-0.2.3/src/ygt/cvGuesser.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     6713 2023-05-25 12:17:29.000000 ygt-0.2.3/src/ygt/fontViewDialog.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-26 02:52:38.084929 ygt-0.2.3/src/ygt/fonts/
--rw-rw-r--   0 peterbaker   (504) staff       (20)   119788 2012-09-20 04:00:00.000000 ygt-0.2.3/src/ygt/fonts/SourceCodePro-Regular.ttf
--rw-r--r--   0 peterbaker   (504) staff       (20)    14895 2023-05-25 20:13:01.000000 ygt-0.2.3/src/ygt/freetypeFont.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    12079 2023-05-25 20:16:51.000000 ygt-0.2.3/src/ygt/harfbuzzFont.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-26 02:52:38.092270 ygt-0.2.3/src/ygt/icons/
--rw-r--r--   0 peterbaker   (504) staff       (20)    26646 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/align.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    24080 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/anchor.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15786 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/black_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6769 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/cursor-icon-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6681 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/cursor-icon-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    10657 2022-12-01 22:00:45.000000 ygt-0.2.3/src/ygt/icons/cv.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     9754 2022-12-18 19:55:30.000000 ygt-0.2.3/src/ygt/icons/cv_guess.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15405 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/gray_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6447 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/hand-icon-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6330 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/hand-icon-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7662 2023-01-23 03:27:58.000000 ygt-0.2.3/src/ygt/icons/horizontal-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7714 2023-01-23 03:31:16.000000 ygt-0.2.3/src/ygt/icons/horizontal-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    16295 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/interpolate.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    22063 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/make_set.png
--rw-r--r--   0 peterbaker   (504) staff       (20)   536171 2022-11-12 02:29:09.000000 ygt-0.2.3/src/ygt/icons/program.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    28381 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/shift.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    24089 2023-04-12 17:06:29.000000 ygt-0.2.3/src/ygt/icons/stem_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7025 2023-01-23 03:32:57.000000 ygt-0.2.3/src/ygt/icons/vertical-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6856 2023-01-23 03:32:24.000000 ygt-0.2.3/src/ygt/icons/vertical-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15484 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/white_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6030 2023-05-03 03:10:09.000000 ygt-0.2.3/src/ygt/macfuncDialog.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    61448 2023-05-25 00:47:12.000000 ygt-0.2.3/src/ygt/makeCVDialog.py
--rwxrwxrwx   0 peterbaker   (504) staff       (20)    73281 2023-05-25 21:05:10.000000 ygt-0.2.3/src/ygt/window.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     2052 2023-04-13 13:41:11.000000 ygt-0.2.3/src/ygt/ygError.py
--rw-rw-r--   0 peterbaker   (504) staff       (20)   123606 2023-05-24 11:49:08.000000 ygt-0.2.3/src/ygt/ygHintEditor.py
--rw-rw-r--   0 peterbaker   (504) staff       (20)   142713 2023-05-23 14:04:27.000000 ygt-0.2.3/src/ygt/ygModel.py
--rwxrwxrwx   0 peterbaker   (504) staff       (20)     9038 2023-05-11 15:28:45.000000 ygt-0.2.3/src/ygt/ygPreferences.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    26442 2023-05-25 20:13:17.000000 ygt-0.2.3/src/ygt/ygPreview.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    10146 2023-05-11 03:15:43.000000 ygt-0.2.3/src/ygt/ygSchema.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     5652 2023-05-02 21:03:38.000000 ygt-0.2.3/src/ygt/ygStems.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    13155 2023-05-17 23:57:49.000000 ygt-0.2.3/src/ygt/ygYAMLEditor.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-26 02:52:38.084825 ygt-0.2.3/src/ygt.egg-info/
--rw-r--r--   0 peterbaker   (504) staff       (20)     4547 2023-05-26 02:52:38.000000 ygt-0.2.3/src/ygt.egg-info/PKG-INFO
--rw-r--r--   0 peterbaker   (504) staff       (20)     1335 2023-05-26 02:52:38.000000 ygt-0.2.3/src/ygt.egg-info/SOURCES.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)        1 2023-05-26 02:52:38.000000 ygt-0.2.3/src/ygt.egg-info/dependency_links.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       40 2023-05-26 02:52:38.000000 ygt-0.2.3/src/ygt.egg-info/entry_points.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)      184 2023-05-26 02:52:38.000000 ygt-0.2.3/src/ygt.egg-info/requires.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       27 2023-05-26 02:52:38.000000 ygt-0.2.3/src/ygt.egg-info/top_level.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       54 2023-05-06 10:50:11.000000 ygt-0.2.3/src/ygt.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-30 21:22:06.625563 ygt-0.2.4/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    11358 2022-11-11 22:39:04.000000 ygt-0.2.4/LICENSE
+-rw-r--r--   0 peterbaker   (504) staff       (20)      181 2023-04-16 16:44:10.000000 ygt-0.2.4/MANIFEST.in
+-rw-r--r--   0 peterbaker   (504) staff       (20)     5127 2023-05-30 21:22:06.625450 ygt-0.2.4/PKG-INFO
+-rw-r--r--   0 peterbaker   (504) staff       (20)     4731 2023-05-30 20:24:50.000000 ygt-0.2.4/README.md
+-rw-r--r--   0 peterbaker   (504) staff       (20)      822 2023-05-30 20:34:08.000000 ygt-0.2.4/pyproject.toml
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-05-30 21:22:06.625594 ygt-0.2.4/setup.cfg
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2022-11-11 22:39:05.000000 ygt-0.2.4/setup.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-30 21:22:06.610304 ygt-0.2.4/src/
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-30 21:22:06.611421 ygt-0.2.4/src/hooks/
+-rw-rw-r--   0 peterbaker   (504) staff       (20)      103 2023-05-04 12:22:22.000000 ygt-0.2.4/src/hooks/hook-freetype.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)      104 2023-05-30 15:29:33.000000 ygt-0.2.4/src/hooks/hook-uharfbuzz.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)      143 2023-05-07 08:59:05.000000 ygt-0.2.4/src/hooks/hook-xgridfit.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-30 21:22:06.618259 ygt-0.2.4/src/ygt/
+-rw-r--r--   0 peterbaker   (504) staff       (20)        1 2022-11-11 22:39:05.000000 ygt-0.2.4/src/ygt/__init__.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)       64 2023-04-06 15:04:52.000000 ygt-0.2.4/src/ygt/__main__.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     3721 2023-05-04 10:24:55.000000 ygt-0.2.4/src/ygt/cvGuesser.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6041 2023-05-29 17:51:23.000000 ygt-0.2.4/src/ygt/fontViewDialog.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-30 21:22:06.619146 ygt-0.2.4/src/ygt/fonts/
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   119788 2012-09-20 04:00:00.000000 ygt-0.2.4/src/ygt/fonts/SourceCodePro-Regular.ttf
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15056 2023-05-27 20:14:17.000000 ygt-0.2.4/src/ygt/freetypeFont.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    39388 2023-05-30 17:32:50.000000 ygt-0.2.4/src/ygt/harfbuzzFont.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-30 21:22:06.625165 ygt-0.2.4/src/ygt/icons/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    26646 2022-11-11 22:39:05.000000 ygt-0.2.4/src/ygt/icons/align.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    24080 2022-11-11 22:39:05.000000 ygt-0.2.4/src/ygt/icons/anchor.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15786 2022-11-11 22:39:05.000000 ygt-0.2.4/src/ygt/icons/black_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6769 2022-11-11 22:39:05.000000 ygt-0.2.4/src/ygt/icons/cursor-icon-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6681 2022-11-11 22:39:05.000000 ygt-0.2.4/src/ygt/icons/cursor-icon-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    10657 2022-12-01 22:00:45.000000 ygt-0.2.4/src/ygt/icons/cv.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     9754 2022-12-18 19:55:30.000000 ygt-0.2.4/src/ygt/icons/cv_guess.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15405 2022-11-11 22:39:05.000000 ygt-0.2.4/src/ygt/icons/gray_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6447 2022-11-11 22:39:05.000000 ygt-0.2.4/src/ygt/icons/hand-icon-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6330 2022-11-11 22:39:05.000000 ygt-0.2.4/src/ygt/icons/hand-icon-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7662 2023-01-23 03:27:58.000000 ygt-0.2.4/src/ygt/icons/horizontal-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7714 2023-01-23 03:31:16.000000 ygt-0.2.4/src/ygt/icons/horizontal-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    16295 2022-11-11 22:39:05.000000 ygt-0.2.4/src/ygt/icons/interpolate.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    22063 2022-11-11 22:39:05.000000 ygt-0.2.4/src/ygt/icons/make_set.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)   536171 2022-11-12 02:29:09.000000 ygt-0.2.4/src/ygt/icons/program.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    28381 2022-11-11 22:39:05.000000 ygt-0.2.4/src/ygt/icons/shift.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    24089 2023-04-12 17:06:29.000000 ygt-0.2.4/src/ygt/icons/stem_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7025 2023-01-23 03:32:57.000000 ygt-0.2.4/src/ygt/icons/vertical-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6856 2023-01-23 03:32:24.000000 ygt-0.2.4/src/ygt/icons/vertical-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15484 2022-11-11 22:39:05.000000 ygt-0.2.4/src/ygt/icons/white_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6030 2023-05-03 03:10:09.000000 ygt-0.2.4/src/ygt/macfuncDialog.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    61448 2023-05-25 00:47:12.000000 ygt-0.2.4/src/ygt/makeCVDialog.py
+-rwxrwxrwx   0 peterbaker   (504) staff       (20)    75840 2023-05-30 20:33:48.000000 ygt-0.2.4/src/ygt/window.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2052 2023-04-13 13:41:11.000000 ygt-0.2.4/src/ygt/ygError.py
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   124450 2023-05-30 12:19:12.000000 ygt-0.2.4/src/ygt/ygHintEditor.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)      798 2023-05-27 17:17:12.000000 ygt-0.2.4/src/ygt/ygLabel.py
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   143698 2023-05-29 17:55:08.000000 ygt-0.2.4/src/ygt/ygModel.py
+-rwxrwxrwx   0 peterbaker   (504) staff       (20)     9038 2023-05-11 15:28:45.000000 ygt-0.2.4/src/ygt/ygPreferences.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    27035 2023-05-28 11:47:28.000000 ygt-0.2.4/src/ygt/ygPreview.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    10146 2023-05-11 03:15:43.000000 ygt-0.2.4/src/ygt/ygSchema.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     5652 2023-05-02 21:03:38.000000 ygt-0.2.4/src/ygt/ygStems.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    13155 2023-05-17 23:57:49.000000 ygt-0.2.4/src/ygt/ygYAMLEditor.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-30 21:22:06.619043 ygt-0.2.4/src/ygt.egg-info/
+-rw-r--r--   0 peterbaker   (504) staff       (20)     5127 2023-05-30 21:22:06.000000 ygt-0.2.4/src/ygt.egg-info/PKG-INFO
+-rw-r--r--   0 peterbaker   (504) staff       (20)     1356 2023-05-30 21:22:06.000000 ygt-0.2.4/src/ygt.egg-info/SOURCES.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)        1 2023-05-30 21:22:06.000000 ygt-0.2.4/src/ygt.egg-info/dependency_links.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       40 2023-05-30 21:22:06.000000 ygt-0.2.4/src/ygt.egg-info/entry_points.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)      184 2023-05-30 21:22:06.000000 ygt-0.2.4/src/ygt.egg-info/requires.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       27 2023-05-30 21:22:06.000000 ygt-0.2.4/src/ygt.egg-info/top_level.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       54 2023-05-06 10:50:11.000000 ygt-0.2.4/src/ygt.py
```

### Comparing `ygt-0.2.3/LICENSE` & `ygt-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/PKG-INFO` & `ygt-0.2.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-Metadata-Version: 2.1
-Name: ygt
-Version: 0.2.3
-Summary: A graphical hint editor for TrueType fonts
-Author-email: "Peter S. Baker" <b.tarde@mail.com>
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10.4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Ygt
 
 **Ygt** is a Python app for hinting TrueType fonts. It is built to be fast, flexible, and free:
 
 - it will run equally well under Windows, Mac OS, and Linux;
 - it emphasizes modern requirements for TrueType hinting while deemphasizing the obsolete;
 - the most common commands use unmodified shortcut keys so you can work quickly with one hand on the keyboard and one on the mouse;
 - it will read either a TrueType font or a UFO;
-- it can save hints in an easily understood and edited YAML file,
+- it saves hints in an easily understood and edited YAML file,
 - which can be compiled to a hinted font either from inside the program or from the command line,
 - or it can save compiled hints to a UFO (from which fontmake can produce a hinted font)
 
 Ygt is in an alpha state, with features yet to be added (especially auto-hinting). But it is already a workable program, which the developer has used to hint thousands of glyphs in several large fonts.
 
-For the time being, Ygt must be launched from a command line. To install, make sure you are running Python 3.10.4 or later and type `pip install ygt` on the command line. Alternatively, download the files from GitHub, navigate to the directory with the file pyproject.toml, and type `pip install .` (don't forget the period!). Then type `ygt` on the command line to start the program.
+Several executable files are available in the “Releases” section of the Ygt GitHub site. If none of these are suitable for your system, Ygt must be launched from a command line. In this case, install from an environment where the version of Python is 3.10.4 or later by typing `pip install ygt` on the command line. Alternatively, download the files from GitHub, navigate to the directory with the file pyproject.toml, and type `pip install .` (don't forget the period!). Then type `ygt <Return>` to start the program.
 
 For more information, see the [documentation](https://github.com/psb1558/ygt/tree/main/docs) or watch a brief [introductory video](https://psb1558.github.io/ygt/index.html).
 
 ## Changes
 
+### Version 0.2.4 (circa 2023-5-31)
+
+Qt was adding extra antialiasing in string/array preview. We now display only FreeType antialiasing.
+
+Harfbuzz metrics updated when instance is changed.
+
+Can now pass indices to cvNN and salt.
+
+Fixed crash on file not found.
+
+Preview->Features launches a dialog with which you can supply values, on, off, or 1-99 to any GSUB feature. Use it (among other things) to turn off features that are on by default.
+
 ### Version 0.2.3 (2023-5-25)
 
 Enable OpenType features in string preview panel (via Harfbuzz).
 
 Better lcd/subpixel rendering in string preview panel.
 
 Touched points are tinted pink.
```

### Comparing `ygt-0.2.3/README.md` & `ygt-0.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,51 @@
+Metadata-Version: 2.1
+Name: ygt
+Version: 0.2.4
+Summary: A graphical hint editor for TrueType fonts
+Author-email: "Peter S. Baker" <b.tarde@mail.com>
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10.4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Ygt
 
 **Ygt** is a Python app for hinting TrueType fonts. It is built to be fast, flexible, and free:
 
 - it will run equally well under Windows, Mac OS, and Linux;
 - it emphasizes modern requirements for TrueType hinting while deemphasizing the obsolete;
 - the most common commands use unmodified shortcut keys so you can work quickly with one hand on the keyboard and one on the mouse;
 - it will read either a TrueType font or a UFO;
-- it can save hints in an easily understood and edited YAML file,
+- it saves hints in an easily understood and edited YAML file,
 - which can be compiled to a hinted font either from inside the program or from the command line,
 - or it can save compiled hints to a UFO (from which fontmake can produce a hinted font)
 
 Ygt is in an alpha state, with features yet to be added (especially auto-hinting). But it is already a workable program, which the developer has used to hint thousands of glyphs in several large fonts.
 
-For the time being, Ygt must be launched from a command line. To install, make sure you are running Python 3.10.4 or later and type `pip install ygt` on the command line. Alternatively, download the files from GitHub, navigate to the directory with the file pyproject.toml, and type `pip install .` (don't forget the period!). Then type `ygt` on the command line to start the program.
+Several executable files are available in the “Releases” section of the Ygt GitHub site. If none of these are suitable for your system, Ygt must be launched from a command line. In this case, install from an environment where the version of Python is 3.10.4 or later by typing `pip install ygt` on the command line. Alternatively, download the files from GitHub, navigate to the directory with the file pyproject.toml, and type `pip install .` (don't forget the period!). Then type `ygt <Return>` to start the program.
 
 For more information, see the [documentation](https://github.com/psb1558/ygt/tree/main/docs) or watch a brief [introductory video](https://psb1558.github.io/ygt/index.html).
 
 ## Changes
 
+### Version 0.2.4 (circa 2023-5-31)
+
+Qt was adding extra antialiasing in string/array preview. We now display only FreeType antialiasing.
+
+Harfbuzz metrics updated when instance is changed.
+
+Can now pass indices to cvNN and salt.
+
+Fixed crash on file not found.
+
+Preview->Features launches a dialog with which you can supply values, on, off, or 1-99 to any GSUB feature. Use it (among other things) to turn off features that are on by default.
+
 ### Version 0.2.3 (2023-5-25)
 
 Enable OpenType features in string preview panel (via Harfbuzz).
 
 Better lcd/subpixel rendering in string preview panel.
 
 Touched points are tinted pink.
```

### Comparing `ygt-0.2.3/pyproject.toml` & `ygt-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ygt"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
     { name="Peter S. Baker", email="b.tarde@mail.com" },
 ]
 description = "A graphical hint editor for TrueType fonts"
 readme = "README.md"
 requires-python = ">=3.10.4"
 classifiers = [
```

### Comparing `ygt-0.2.3/src/ygt/cvGuesser.py` & `ygt-0.2.4/src/ygt/cvGuesser.py`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/fontViewDialog.py` & `ygt-0.2.4/src/ygt/fontViewDialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .freetypeFont import freetypeFont, RENDER_LCD_1, RENDER_GRAYSCALE
 from fontTools import subset
 from .ygModel import ygFont
+from .ygLabel import ygLabel
 from math import ceil
 from PyQt6.QtCore import pyqtSignal
 from PyQt6.QtWidgets import QWidget, QGridLayout, QVBoxLayout, QScrollArea, QLabel
 from PyQt6.QtGui import QPainter, QColor, QPalette, QPixmap
 from tempfile import SpooledTemporaryFile
 import copy
 
@@ -33,28 +34,14 @@
         self.setWindowTitle("Font View")
         self.glyph_name_list = []
         for g in glyph_list:
             self.glyph_name_list.append(g[1])
         self.yg_font = yg_font
         self.face = self.yg_font.freetype_font
         self.face.set_size(24)
-        #if self.yg_font.source_file.source_type == "yaml":
-        #    self.face = freetypeFont(filename, size=24, render_mode=RENDER_LCD_1)
-        #else:
-        #    temp_font = copy.deepcopy(self.yg_font.preview_font)
-        #    tf = SpooledTemporaryFile(max_size=3000000, mode='b')
-        #    options = subset.Options(glyph_names=True)
-        #    options.layout_features = []
-        #    subsetter = subset.Subsetter(options)
-        #    subsetter.populate(glyphs=self.glyph_name_list)
-        #    subsetter.subset(temp_font)
-        #    temp_font.save(tf, 1)
-        #    tf.seek(0)
-        #    self.face = freetypeFont(tf, size=24, render_mode=RENDER_LCD_1)
-        #    tf.close()
         if not self.face.valid:
             self.valid = False
             return
         self.glyph_list = glyph_list
         self.glyph_index = {}
 
         text_hsv_value = self.palette().color(QPalette.ColorRole.WindowText).value()
@@ -109,15 +96,15 @@
                 col = 0
         if dialog.dark_theme:
             self.setStyleSheet("background-color: black;")
         else:
             self.setStyleSheet("background-color: white;")
 
 
-class fontViewCell(QLabel):
+class fontViewCell(ygLabel):
     def __init__(self, dialog: fontViewWindow, glyph: list) -> None:
         super().__init__()
         self.dialog = dialog
         self.glyph = glyph[1]
         self.setFixedSize(36, 36)
         self.has_hints = False
         self.pixmap = None
```

### Comparing `ygt-0.2.3/src/ygt/fonts/SourceCodePro-Regular.ttf` & `ygt-0.2.4/src/ygt/fonts/SourceCodePro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/freetypeFont.py` & `ygt-0.2.4/src/ygt/freetypeFont.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 import freetype as ft # type: ignore
 import numpy
 import copy
 from tempfile import SpooledTemporaryFile
-from PyQt6.QtGui import QColor, QPen, QImage, QRegion, QBitmap, QPixmap, QPainter
-from PyQt6.QtCore import QRect, QLine
+from PyQt6.QtGui import QColor, QPen, QImage, QPainter
+from PyQt6.QtCore import QLine
 
 RENDER_GRAYSCALE = 1
 RENDER_LCD_1 = 2
 RENDER_LCD_2 = 3
 
 
 class ygLetterBox:
@@ -200,15 +200,15 @@
             painter,
             x,
             y,
             spacing_mark = False,
             dark_theme = False,
             is_target = False,
             x_offset = 0,
-            y_offset = 0
+            y_offset = 0,
         ):
         """Draws a bitmap with subpixel rendering (suitable for an lcd screen)
 
         Params:
 
         painter (QPainter): a Qt tool to draw with
 
@@ -249,15 +249,15 @@
         # Get QImage from Z; set composition mode; draw the glyph.
         if have_outline:
             img = QImage(Z.data, width, height, bytesPerLine, QImage.Format.Format_RGB888)
             if dark_theme:
                 painter.setCompositionMode(QPainter.CompositionMode.CompositionMode_Screen)
             else:
                 painter.setCompositionMode(QPainter.CompositionMode.CompositionMode_Multiply)
-            # painter.setRenderHint(QPainter.RenderHint.TextAntialiasing, on=False)
+            painter.setRenderHint(QPainter.RenderHint.TextAntialiasing, on=False)
             painter.drawImage(starting_xpos, starting_ypos, img)
 
         # Draw a red line under target glyph (the one in the current resolution).
         ending_xpos = starting_xpos + round(gdata["advance"])
         ending_ypos = starting_ypos + gdata["rows"]
         if is_target:
             ul_y = ending_ypos + 4
@@ -402,15 +402,14 @@
         return indices
 
     def draw_string(self,
                     painter,
                     s: str | list,
                     x,
                     y,
-                    background_image: QImage,
                     positions: list = [],
                     x_limit = 200,
                     y_increment = 67,
                     dark_theme = False,
         ):
 
         self.last_glyph_index = None
@@ -425,26 +424,32 @@
         ypos = y
         for count, i in enumerate(indices):
             self.set_char(i)
             x_offset = 0
             y_offset = 0
             x_advance = -1
             # If possible, use positions from Harfbuzz. This will include kerning
-            # and correct positioning of diacritics.
+            # and correct positioning of diacritics. These will still be valid
+            # for our mini-font--only we've got to translate gids in Harfbuzz's
+            # cooy of our font to gids in the subsetted font returned by
+            # window.ygPreviewFontMaker. We do this by doing gid-->gname before
+            # running window.ygPreviewFontMaker and gname-->gid afterwards.
             if len(positions):
                 x_offset = self.font_to_pixels(positions[count].x_offset)
                 y_offset = self.font_to_pixels(positions[count].y_offset)
                 x_advance = self.font_to_pixels(positions[count].x_advance)
 
-            #if self.last_glyph_index != None:
-            #    k = self.face.get_kerning(
-            #        self.last_glyph_index, i, ft.FT_KERNING_DEFAULT
-            #    )
-            #    xpos += k.x
-            adv = self.draw_char(painter, xpos, ypos, dark_theme = dark_theme, x_offset = x_offset, y_offset = y_offset)
+            adv = self.draw_char(
+                painter,
+                xpos,
+                ypos,
+                dark_theme = dark_theme,
+                x_offset = x_offset,
+                y_offset = y_offset,
+                )
             if x_advance >= 0:
                 adv = x_advance
             xpos += adv
             if xpos >= x_limit:
                 xpos = x
                 ypos += y_increment
                 self.last_glyph_index = None
```

### Comparing `ygt-0.2.3/src/ygt/icons/align.png` & `ygt-0.2.4/src/ygt/icons/align.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/icons/anchor.png` & `ygt-0.2.4/src/ygt/icons/anchor.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/icons/black_distance.png` & `ygt-0.2.4/src/ygt/icons/black_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/icons/cursor-icon-off.png` & `ygt-0.2.4/src/ygt/icons/cursor-icon-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/icons/cursor-icon-on.png` & `ygt-0.2.4/src/ygt/icons/cursor-icon-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/icons/cv.png` & `ygt-0.2.4/src/ygt/icons/cv.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/icons/cv_guess.png` & `ygt-0.2.4/src/ygt/icons/cv_guess.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/icons/gray_distance.png` & `ygt-0.2.4/src/ygt/icons/gray_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/icons/hand-icon-off.png` & `ygt-0.2.4/src/ygt/icons/hand-icon-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/icons/hand-icon-on.png` & `ygt-0.2.4/src/ygt/icons/hand-icon-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/icons/horizontal-off.png` & `ygt-0.2.4/src/ygt/icons/horizontal-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/icons/horizontal-on.png` & `ygt-0.2.4/src/ygt/icons/horizontal-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/icons/interpolate.png` & `ygt-0.2.4/src/ygt/icons/interpolate.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/icons/make_set.png` & `ygt-0.2.4/src/ygt/icons/make_set.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/icons/program.png` & `ygt-0.2.4/src/ygt/icons/program.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/icons/shift.png` & `ygt-0.2.4/src/ygt/icons/shift.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/icons/stem_distance.png` & `ygt-0.2.4/src/ygt/icons/stem_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/icons/vertical-off.png` & `ygt-0.2.4/src/ygt/icons/vertical-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/icons/vertical-on.png` & `ygt-0.2.4/src/ygt/icons/vertical-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/icons/white_distance.png` & `ygt-0.2.4/src/ygt/icons/white_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/macfuncDialog.py` & `ygt-0.2.4/src/ygt/macfuncDialog.py`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/makeCVDialog.py` & `ygt-0.2.4/src/ygt/makeCVDialog.py`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/window.py` & `ygt-0.2.4/src/ygt/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,20 +51,20 @@
     QUndoGroup,
     QCloseEvent,
     QAction,
     QFontDatabase,
     QPainter,
 )
 from fontTools import ttLib, ufoLib # type: ignore
-from .harfbuzzFont import harfbuzzFont
+from .harfbuzzFont import harfbuzzFont, hbFeatureDialog
 
 # FileNameVar = TypeVar("FileNameVar", str, tuple[str, Any])
 FileNameVar = Union[str, tuple[str, Any]]
 # FileNameVar = Any
-ygt_version = "0.2.3"
+ygt_version = "0.2.4"
 
 
 class ygPreviewFontMaker(QThread):
     """To be run from a QThread. This is because it can take the better
     part of a second to generate a preview, even on a pretty fast
     machine, and we want to be able to run this on a signal without
     making the GUI balky.
@@ -243,14 +243,15 @@
         self.script_actions: list = []
         self.script_menu = None
         self.language_actions: list = []
         self.language_menu = None
         self.feature_actions: list = []
         self.feature_menu = None
         self.feature_reset_action = None
+        self.custom_feature_action = None
         self.window_list: list = []
         self.preview_maker: Optional[ygPreviewFontMaker] = None
         self.font_generator: Optional[ygFontGenerator] = None
         self.auto_preview_update = True
 
         #
         # Build menus and toolbar
@@ -423,14 +424,16 @@
 
         self.script_menu = self.preview_menu.addMenu("Script")
         self.script_menu.setEnabled(False)
         self.language_menu = self.preview_menu.addMenu("Language")
         self.language_menu.setEnabled(False)
         self.feature_menu = self.preview_menu.addMenu("Features")
         self.feature_menu.setEnabled(False)
+        self.custom_feature_action = self.preview_menu.addAction("Feature...")
+        self.custom_feature_action.setEnabled(False)
         self.feature_reset_action = self.preview_menu.addAction("Reset features")
         self.feature_reset_action.setEnabled(False)
 
         self.preview_menu.aboutToShow.connect(self.preview_menu_about_to_show)
 
         #
         # View Menu
@@ -766,14 +769,17 @@
             self.instance_menu.setEnabled(True)
 
     @pyqtSlot(object)
     def update_string_preview(self, s) -> None:
         preview_text = self.yg_string_preview.panel._text
         if preview_text != None and len(preview_text) > 0:
             self.yg_string_preview.set_string_preview()
+            if self.yg_preview.hb_instance_changed:
+                self.yg_preview.hb_instance_changed = False
+                self.yg_string_preview.update_hb_string_data()
         else:
             self.yg_string_preview.set_size_array()
         self.yg_string_preview.set_face(self.yg_preview.face)
         self.yg_string_preview.panel.make_pixmap()
         self.yg_string_preview.update()
 
     #
@@ -817,49 +823,56 @@
     def setup_script_menu(self):
         if not self.yg_font:
             return
         self.script_menu.clear()
         self.script_actions.clear()
         scripts = self.yg_font.harfbuzz_font.sub_scripts
         for s in scripts:
-            sa = self.script_menu.addAction(s)
+            sa = self.script_menu.addAction(harfbuzzFont.expanded_script_name(s))
             sa.setCheckable(True)
             sa.setChecked(s == self.yg_font.harfbuzz_font.current_script_tag)
             sa.triggered.connect(self.set_script)
             self.script_actions.append(sa)
         self.script_menu.setEnabled(len(scripts) > 0)
 
     def setup_language_menu(self):
         if not self.yg_font:
             return
         self.language_menu.clear()
         self.language_actions.clear()
         languages = self.yg_font.harfbuzz_font.sub_languages
         for l in languages:
-            la = self.language_menu.addAction(l)
+            la = self.language_menu.addAction(harfbuzzFont.expanded_language_name(l))
             la.setCheckable(True)
             la.setChecked(l == self.yg_font.harfbuzz_font.current_language_tag)
             la.triggered.connect(self.set_language)
             self.language_actions.append(la)
         self.language_menu.setEnabled(len(languages) > 0)
 
     def setup_feature_menu(self):
         if not self.yg_font:
             return
         self.feature_menu.clear()
         self.feature_actions.clear()
         features = self.yg_font.harfbuzz_font.sub_features
         for f in features:
-            fa = self.feature_menu.addAction(harfbuzzFont.expanded_feature_name(f))
-            fa.setCheckable(True)
-            fa.setChecked(f in self.yg_font.harfbuzz_font._active_features)
-            fa.triggered.connect(self.toggle_feature)
-            self.feature_actions.append(fa)
+            prefix = f[0:2]
+            if not f in harfbuzzFont.DEFAULT_LAYOUT_TAGS:
+                fa = self.feature_menu.addAction(harfbuzzFont.expanded_feature_name(f))
+                fa.setCheckable(True)
+                fa.setChecked(f in self.yg_font.harfbuzz_font._active_features)
+                # fa.setChecked(self.yg_font.harfbuzz_font.feature_is_active(f))
+                if f == "salt" or prefix == "cv":
+                    fa.triggered.connect(self.set_indexed_feature)
+                else:
+                    fa.triggered.connect(self.toggle_feature)
+                self.feature_actions.append(fa)
         self.feature_menu.setEnabled(len(features) > 0)
         self.feature_reset_action.setEnabled(len(features) > 0)
+        self.custom_feature_action.setEnabled(len(features) > 0)
             
 
     @pyqtSlot()
     def view_menu_about_to_show(self) -> None:
         if self.points_as_coords:
             self.index_label_action.setEnabled(True)
             self.coord_label_action.setEnabled(False)
@@ -998,14 +1011,15 @@
         self.pv_mode_3_action.triggered.connect(self.yg_preview.render3)
         self.pv_theme_auto_action.triggered.connect(self.yg_preview.set_theme_auto)
         self.pv_theme_light_action.triggered.connect(self.yg_preview.set_theme_light)
         self.pv_theme_dark_action.triggered.connect(self.yg_preview.set_theme_dark)
         self.pv_show_hints_action.triggered.connect(self.yg_preview.toggle_show_hints)
         self.pv_show_grid_action.triggered.connect(self.yg_preview.toggle_grid)
         self.feature_reset_action.triggered.connect(self.yg_font.harfbuzz_font.reset_features)
+        self.custom_feature_action.triggered.connect(self.hb_custom_feature)
 
     def setup_preview_instance_connections(self) -> None:
         if self.yg_font.is_variable_font and self.instance_actions != None:
             self.prev_instance_action.triggered.connect(self.yg_preview.next_instance)
             self.next_instance_action.triggered.connect(self.yg_preview.prev_instance)
             for i in self.instance_actions:
                 i.triggered.connect(self.yg_preview.set_instance)
@@ -1369,14 +1383,15 @@
         yaml_source["glyphs"] = {}
         return yaml_source
 
     def _open(self, f: FileNameVar) -> int:
         """Returns 0 if file opened in this window
         Returns 1 if this window already has a file open
         Returns 2 if the file is already open (the window is activated and brought to top)
+        Returns 3 if there was an error and the file could not be opened.
 
         f param can be:
         - the name of a .yaml file
         - the name of a .ttf font
         - the name of a .ufo font (treated differently if it contains ygt source)
         """
         # If this window already has content, return 1 as a signal that a new window
@@ -1440,14 +1455,17 @@
             # If opening ttf, we have both yaml_source and ygt_filename
             # If opening ufo, ygt_filename is the same as the font name
             # If opening yaml, we just pass the filename (since font is identified in the file)
             if len(yaml_source) > 0:
                 self.yg_font = ygFont(self, yaml_source, ygt_filename=ygt_filename)
             else:
                 self.yg_font = ygFont(self, filename)
+            if not self.yg_font.load_successful:
+                self.yg_font = None
+                return 3
             self.yg_font.setup_error_signal(self.error_manager.new_message)
 
             self.setup_script_menu()
             self.setup_language_menu()
             self.setup_feature_menu()
 
             self.add_preview()
@@ -1714,36 +1732,71 @@
             "Pixels per em:",
             value = 25,
             min = 10,
             max = 400,
         )
         if ok:
             self.yg_preview.set_size(i)
+
+    @pyqtSlot()
+    def hb_custom_feature(self):
+        d = hbFeatureDialog(self, self.yg_font.harfbuzz_font)
+        d.exec()
+        # We need to launch harfbuzzFont.hbFeatureDialog, passing
+        # ref to self and the current harfbuzzFont.
+        pass
     
     @pyqtSlot()
     def toggle_feature(self):
         f = harfbuzzFont.tag_only(self.sender().text())
         if f in self.yg_font.harfbuzz_font.active_features:
             self.yg_font.harfbuzz_font.deactivate_feature(f)
         else:
             self.yg_font.harfbuzz_font.activate_feature(f)
 
     @pyqtSlot()
+    def set_indexed_feature(self):
+        i = 1
+        f = harfbuzzFont.tag_only(self.sender().text())
+        if f in self.yg_font.harfbuzz_font.active_features:
+            self.yg_font.harfbuzz_font.deactivate_feature(f)
+        else:
+            i, ok = QInputDialog().getInt(
+                self,
+                "Index for " + f,
+                "Index: ",
+                value = 1,
+                min = 1,
+                max = 99,
+            )
+            if ok:
+                if i > 0:
+                    self.yg_font.harfbuzz_font.activate_feature(f, index = i)
+                else:
+                    self.yg_font.harfbuzz_font.deactivate_feature(f)
+            # Do an appropriately titled dialog that only accepts int > 0.
+            # If necessary, alter activate_feature() to accept an int
+            # argument and put that in the _active_features instead of
+            # a bool.
+            # Call activate_feature() if int > 0; else call
+            # deactivate_feature(). ***
+
+    @pyqtSlot()
     def set_script(self):
-        tag = self.sender().text()
+        tag = harfbuzzFont.tag_only(self.sender().text())
         self.yg_font.harfbuzz_font.select_script(tag)
         for s in self.script_actions:
-            s.setChecked(tag == s.text())
+            s.setChecked(tag == harfbuzzFont.tag_only(s.text()))
 
     @pyqtSlot()
     def set_language(self):
-        tag = self.sender().text()
+        tag = harfbuzzFont.tag_only(self.sender().text())
         self.yg_font.harfbuzz_font.select_language(tag)
         for l in self.language_actions:
-            l.setChecked(tag == l.text())
+            l.setChecked(tag == harfbuzzFont.tag_only(l.text()))
 
     #
     # Program exit
     #
 
     def save_query(self) -> int:
         msg_box = QMessageBox()
@@ -1844,17 +1897,21 @@
 
     def set_preferences(self) -> None:
         self.preferences.set_points_as_coords(self.points_as_coords)
         self.preferences.set_zoom_factor(self.zoom_factor)
         self.preferences.set_show_off_curve_points(self.show_off_curve_points)
         self.preferences.set_show_point_numbers(self.show_point_numbers)
 
-    # Could be property
+    @property
     def current_glyph(self):
         return self.glyph_pane.yg_glyph_scene.yg_glyph
+    
+    @property
+    def current_glyph_name(self):
+        return self.current_glyph.gname
 
 
 class mainWinEventFilter(QObject):
     def __init__(self, top_win):
         super().__init__()
         self.top_window = top_win
 
@@ -1864,18 +1921,18 @@
                 self.top_window.preferences["top_window"] = self.top_window
         return super().eventFilter(source, event)
 
 
 def main():
     import uharfbuzz
     #from inspect import getfullargspec, signature
-    print(dir(uharfbuzz._harfbuzz.GlyphPosition))
+    # print(dir(Qt.Key))
     # print(dir(QPainter))
-    #print(dir(hb._harfbuzz.Font))
-    #print(dir(hb._harfbuzz.Buffer))
+    # print(dir(hb._harfbuzz.hb_font_set_var_named_instance))
+    # print(dir(hb._harfbuzz.Buffer))
 
     app = QApplication([])
 
     if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
         font_path = os.path.join(
             sys._MEIPASS,
             "fonts",
```

### Comparing `ygt-0.2.3/src/ygt/ygError.py` & `ygt-0.2.4/src/ygt/ygError.py`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/ygHintEditor.py` & `ygt-0.2.4/src/ygt/ygHintEditor.py`

 * *Files 0% similar despite different names*

```diff
@@ -3202,14 +3202,32 @@
         #    down. For panning the screen.
         # 3. Hyphen (minus) removes a target point from a hint.
         # 4. Plus adds a point to a hint.
         if event.key() in [16777219, 16777223]:
             self.yg_glyph_scene.delete_selected_hints()
         elif event.key() == Qt.Key.Key_Plus:
             self.yg_glyph_scene.add_to_set()
+        elif event.key() == Qt.Key.Key_J:
+            with_ctrl = (
+                QApplication.keyboardModifiers() & Qt.KeyboardModifier.ControlModifier
+            ) == Qt.KeyboardModifier.ControlModifier
+            with_shift = (
+                QApplication.keyboardModifiers() & Qt.KeyboardModifier.ShiftModifier
+            ) == Qt.KeyboardModifier.ShiftModifier
+            if with_ctrl and with_shift:
+                print("========= locals() =========")
+                g = locals()
+                gg = g.keys()
+                for ggg in gg:
+                    print(str(ggg)+ ": " + str(sys.getsizeof(g[ggg])))
+                print("========= globals() =========")
+                g = globals()
+                gg = g.keys()
+                for ggg in gg:
+                    print(str(ggg)+ ": " + str(sys.getsizeof(g[ggg])))
         elif event.key() == Qt.Key.Key_Minus:
             self.yg_glyph_scene.delete_from_set()
         elif event.key() == 32 and not event.isAutoRepeat():
             self.drag_mode_backup = self.dragMode()
             if self.drag_mode_backup == QGraphicsView.DragMode.NoDrag:
                 self.sig_toggle_drag_mode.emit(QGraphicsView.DragMode.ScrollHandDrag)
```

### Comparing `ygt-0.2.3/src/ygt/ygModel.py` & `ygt-0.2.4/src/ygt/ygModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,14 +241,15 @@
         y_doc. If yaml_source is a dict, it is the skeleton yaml source
         generated for a new program. Otherwise, yaml_source will be a
         filename.
 
         yaml_source can be either a dict (containing newly initialized ygt code) or
         the name of either a .yaml file or a ufo.
         """
+        self.load_successful = True
         # Determine the filename
         if type(yaml_source) is str:
             self.filename = yaml_source
         elif len(yaml_filename) > 0:
             self.filename = yaml_filename
         else:
             self.filename = "NewFile.yaml"
@@ -257,30 +258,35 @@
         suff = pathlib.Path(self.filename).suffix
         if suff == ".yaml":
             self.source_type = "yaml"
         elif suff == ".ufo":
             self.source_type = "ufo"
         else:
             # This shouldn't happen.
-            raise Exception("Bad filename " + str(self.filename))
+            self.load_successful = False
+            return
+            #raise Exception("Bad filename " + str(self.filename))
 
         # Read the yaml source. Either the skeleton created earlier (but shouldn't
         # it be here?), a yaml file, or a yaml file in a ufo.
         if type(yaml_source) is dict:
             self.y_doc = copy.deepcopy(yaml_source)
         else:
-            if self.source_type == "yaml":
-                y_stream = open(self.filename, "r")
-                self.y_doc = yaml.safe_load(y_stream)
-                y_stream.close()
-            else:
-                ufo = ufoLib.UFOReader(self.filename)
-                if ufo.formatVersionTuple[0] == 3:
-                    doc = ufo.readData("org.ygthinting/source.yaml")
-                    self.y_doc = yaml.safe_load(doc)
+            try:
+                if self.source_type == "yaml":
+                    y_stream = open(self.filename, "r")
+                    self.y_doc = yaml.safe_load(y_stream)
+                    y_stream.close()
+                else:
+                    ufo = ufoLib.UFOReader(self.filename)
+                    if ufo.formatVersionTuple[0] == 3:
+                        doc = ufo.readData("org.ygthinting/source.yaml")
+                        self.y_doc = yaml.safe_load(doc)
+            except Exception:
+                self.load_successful = False
 
     @property
     def source(self) -> dict:
         return self.y_doc
 
     def save_source(self, top_window: Any = None) -> None:
         yy = yaml.dump(self.y_doc, sort_keys=False, width=float("inf"), Dumper=Dumper)
@@ -338,48 +344,69 @@
     sig_cvt_changed = pyqtSignal()
     sig_error = pyqtSignal(object)
 
     def __init__(
         self, main_window: Any, source_file: Union[str, dict], ygt_filename: str = ""
     ) -> None:
         super().__init__()
+        self.load_successful = True
         self.main_window = main_window
 
         #
         # Set up an undo stack
         #
         self.undo_stack = QUndoStack()
         self.main_window.add_undo_stack(self.undo_stack)
 
         #
-        # Open the font
+        # Open the Ygt source and the font.
         #
         self.source_file = SourceFile(source_file, yaml_filename=ygt_filename)
+        if not self.source_file.load_successful:
+            if self.main_window:
+                self.main_window.show_error_message(
+                    [
+                        "Error",
+                        "File load error",
+                        "Can't load Ygt source, probably because the file can't be found."
+                    ]
+                )
+                self.load_successful = False
+                return
+            else:
+                raise Exception("Can't load Ygt source.")
 
         # Fix directory (change to directory where source file is located)
         d = None
         if isinstance(source_file, str) and source_file:
             d = os.path.dirname(source_file)
         elif ygt_filename:
             d = os.path.dirname(ygt_filename)
         if d and os.path.isdir(d) and d != os.getcwd():
             os.chdir(d)
 
         self.source = self.source_file.source
         self.font_files = FontFiles(self.source)
         fontfile = self.font_files.in_font
         if not fontfile:
-            raise Exception("Need the name of an existing font")
+            if self.main_window:
+                self.main_window.show_error_message(
+                    ["Error", "Font not specified", "Didn't find the name of a font file in the source"]
+                    )
+                self.load_successful = False
+                return
+            else:
+                raise Exception("Need the name of an existing font")
             # Need to let user try again.
         split_fn = os.path.splitext(str(fontfile))
         extension = split_fn[1]
         ft_open_error = False
         # self.freetype_font = None
-        # Here we get *two* copies of the font in memory: one in FontTools format,
-        # the other FreeType.
+        # Here we get *three* copies of the font in memory: one in FontTools format,
+        # one FreeType, one Harfbuzz. Is there any way around this?
         if extension == ".ttf":
             try:
                 self.ft_font = ttLib.TTFont(fontfile)
                 self.freetype_font = freetypeFont(fontfile)
                 self.harfbuzz_font = harfbuzzFont(fontfile, self.freetype_font)
             except FileNotFoundError as ferr:
                 ft_open_error = True
@@ -392,23 +419,29 @@
                 self.freetype_font = freetypeFont(tf, keep_open = True)
                 self.harfbuzz_font = harfbuzzFont(tf, self.freetype_font)
                 # tf.close()
             except Exception as e:
                 print(e)
                 ft_open_error = True
         if ft_open_error:
-            raise Exception("Can't find font file " + str(fontfile))
-            # Fix this! Need a dialog box and a chance to try again for a valid font.
-            #
-            # Do this: open a file dialog for locating the font file, and place this
-            # in the SourceFile object. If user doesn't choose a font, then close
-            # this window (send signal to top_window?). The application can continue
-            # if other windows are open.
+            if self.main_window:
+                self.main_window.show_error_message(
+                    [
+                        "Error",
+                        "Font file not found",
+                        "Can't find font file" + str(fontfile)
+                    ]
+                )
+                self.load_successful = False
+                return
+            else:
+                raise Exception("Can't find font file " + str(fontfile))
+
+        # Make a deepcopy so we can always have a clean copy of the font to work with.
 
-        # Making a deepcopy so we can always have a clean copy of the font to work with.
         self.preview_font = copy.deepcopy(self.ft_font)
 
         #
         # If it's a variable font, get instances and axes
         #
         try:
             self.instances = {}
@@ -427,15 +460,16 @@
             self.masters = ygMasters(self, self.source)
         #
         # Set up access to YAML font data (if there is no cvt table yet, get some
         # values from the font).
         #
         self.glyphs = ygGlyphs(self.source).data
         self.defaults = ygDefaults(self, self.source)
-        self.defaults._set_default({"init-graphics": False, "cleartype": True})
+        if not "defaults" in self.source:
+            self.defaults._set_default({"init-graphics": False, "cleartype": True})
         if not "cvt" in self.source:
             self.source["cvt"] = {}
         if len(self.source["cvt"]) == 0:
             cvt = self.source["cvt"]
             cvt["baseline"] = {"val": 0, "type": "pos", "axis": "y"}
             try:
                 p = self.extreme_points("H")[0]
@@ -580,34 +614,30 @@
 
         # This dict is for using a glyph name to look up a glyph's index.
         self.name_to_index = {}
         raw_order_list = self.ft_font.getGlyphOrder()
         for order_index, gn in enumerate(raw_order_list):
             self.name_to_index[gn] = order_index
 
-        # Get a list of tuples containing unicodes and glyph names (still
-        # omitting composites). Sort first by unicode, then by name. This
-        # is our order for the font.
+        # Get a list of tuples containing unicodes and glyph names.
+        # Sort first by unicode, then by name. This is our order for the font.
         for gn in glyph_names:
             g = self.ft_font["glyf"][gn]
-            # Remove this test if we're going to display composites.
-            # if not g.isComposite():
-            if True:
-                cc = g.getCoordinates(self.ft_font["glyf"])
-                if len(cc) > 0:
-                    self.glyph_list.append((self.get_unicode(gn), gn))
+            cc = g.getCoordinates(self.ft_font["glyf"])
+            if len(cc) > 0:
+                self.glyph_list.append((self.get_unicode(gn), gn))
         self.glyph_list.sort(key=lambda x: x[1])
         self.glyph_list.sort(key=lambda x: x[0])
 
         self.unicode_to_name = {}
         for g in self.glyph_list:
             self.unicode_to_name[g[0]] = g[1]
 
-        # Like name_to_index, but this one looks up the index in a slimmed-down,
-        # non-composite-only list. This is for navigating in this program.
+        # Like name_to_index, but this returns the glyph's index in Ygt order.
+        # This is for navigating in this program.
         self.glyph_index = {}
         for glyph_counter, g in enumerate(self.glyph_list):
             self.glyph_index[g[1]] = glyph_counter
 
         # Track whether signal is connected
         self.signal_connected = False
 
@@ -632,14 +662,17 @@
         def_inst = None
         kk = self.instances.keys()
         for k in kk:
             if self.instances[k] == default_coordinates:
                 def_inst = k
                 break
         return def_inst
+    
+    def instance_coordinates(self, inst: str) -> dict:
+        return self.instances[inst]
 
     @property
     def axis_tags(self) -> list:
         result = []
         for a in self.axes:
             result.append(a.axisTag)
         return result
@@ -711,16 +744,14 @@
                 del self.source["glyphs"][g]
         except Exception as e:
             self.send_error_message(
                 {"msg": "Error in cleanup_font: " + str(e), "mode": "console"}
             )
 
     def is_composite(self, gname: str) -> bool:
-        if not gname in self.name_to_index:
-            return False
         return self.ft_font['glyf'][gname].isComposite()
 
     def has_hints(self, gname: str) -> bool:
         if not gname in self.glyphs:
             return False
         glyph_program = self.glyphs[gname]
         if not ("y" in glyph_program or "x" in glyph_program):
@@ -1184,15 +1215,15 @@
 
 class fontInfoEditCommand(QUndoCommand):
     """Superclass for editing font-level data."""
 
     def __init__(self, yg_font: ygFont) -> None:
         super().__init__()
         self.yg_font = yg_font
-        self.yg_glyph = self.yg_font.main_window.current_glyph()
+        self.yg_glyph = self.yg_font.main_window.current_glyph
         self.undo_state = fontInfoSaver(self.yg_font)
         self.redo_state: Union[fontInfoSaver, None] = None
 
     def send_signal(self) -> None:
         if self.yg_font.signal_connected:
             self.yg_font.sig_cvt_changed.emit()
             self.yg_glyph.sig_hints_changed.emit(self.yg_glyph.hints)
```

### Comparing `ygt-0.2.3/src/ygt/ygPreferences.py` & `ygt-0.2.4/src/ygt/ygPreferences.py`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/ygPreview.py` & `ygt-0.2.4/src/ygt/ygPreview.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     QVBoxLayout,
     QScrollArea,
     QSizePolicy,
 )
 from PyQt6.QtGui import QPainter, QBrush, QColor, QPalette, QPixmap
 from PyQt6.QtCore import Qt, QRect, pyqtSignal, pyqtSlot, QLine
 #import cv2
+from .ygLabel import ygLabel
 
 
 PREVIEW_WIDTH = 450
 PREVIEW_HEIGHT = 500
 STRING_PREVIEW_HEIGHT = 200
 PREVIEW_HORI_MARGIN = 25
 PREVIEW_VERT_MARGIN = 50
@@ -36,15 +37,14 @@
         self._layout = QVBoxLayout()
         self._layout.setSpacing(10)
         self._layout.setContentsMargins(0, 0, 0, 0)
         self._layout.addWidget(preview)
         self._layout.addWidget(string_preview)
         self.setLayout(self._layout)
 
-
 class ygPreview(QLabel):
 
     sig_preview_paint_done = pyqtSignal(object)
 
     def __init__(self, top_window) -> None:
         super().__init__()
         self.top_window = top_window
@@ -86,14 +86,15 @@
         self.top_char_margin = 0
         self.show_grid = True
 
         # Two- or three-dimensional array shaped by numpy.
         self.Z: list = []
         self.instance_dict: Optional[dict] = None
         self.instance: Optional[str] = None
+        self.hb_instance_changed = False
 
         # Figure out if we have a dark or a light theme.
         text_hsv_value = self.palette().color(QPalette.ColorRole.WindowText).value()
         self.background_color = self.default_background = self.palette().color(QPalette.ColorRole.Base)
         bg_hsv_value = self.background_color.value()
         self.dark_theme = text_hsv_value > bg_hsv_value
         self.theme_choice = "auto"
@@ -334,15 +335,21 @@
 
     @pyqtSlot()
     def set_instance(self) -> None:
         self.instance = self.sender().text() # type: ignore
         self._set_instance()
 
     def _set_instance(self) -> None:
+        # Set the instance in the FreeType font
         self.face.set_instance(self.instance)
+        # Set the instance in the harfbuzz font.
+        ygf = self.top_window.yg_font
+        ygf.harfbuzz_font.set_coordinates(ygf.instance_coordinates(self.instance))
+        self.hb_instance_changed = True
+        # Leave the rest of the harfbuzz stuff for updating the string preview.
         self.set_label_text()
         self.make_pixmap()
         self.update()
 
     @pyqtSlot()
     def bigger_one(self) -> None:
         self.resize_by(1)
@@ -547,15 +554,15 @@
         if self.show_grid:
             self.draw_grid(painter)
         painter.end()
         self.setPixmap(self.pixmap)
         self.sig_preview_paint_done.emit(None)
 
 
-class ygStringPreviewPanel(QLabel):
+class ygStringPreviewPanel(ygLabel):
     sig_go_to_glyph = pyqtSignal(object)
 
     def __init__(self, yg_preview: ygPreview, top_window) -> None:
         super().__init__()
         self.yg_preview = yg_preview
         self.top_window = top_window
         self.face = self.yg_preview.face
@@ -665,15 +672,14 @@
             dark_theme = self.yg_preview.dark_theme
         self.rect_list = self.face.draw_string(
             painter,
             # self._text,
             self._full_glyph_list,
             xposition,
             yposition,
-            self.pixmap.toImage(),
             positions = self._full_pos_list,
             x_limit = PREVIEW_WIDTH - 50,
             dark_theme = dark_theme
         )
         painter.end()
         self.setPixmap(self.pixmap)
 
@@ -727,16 +733,20 @@
         self.qle.editingFinished.connect(self.got_string)
 
         self._layout.addWidget(self.panel)
         self._layout.addWidget(self.button_widget)
 
         self.setLayout(self._layout)
 
-        # list of glyph names correspond
-        
+    def update_hb_string_data(self):
+        """Update metrics from harfbuzz font. Call if instance has been changed."""
+        t = self.panel._text
+        l_full, p_full = self.top_window.yg_font.harfbuzz_font.get_shaped_names(t)
+        self.full_pos_list = p_full
+
     @property
     def full_glyph_list(self):
         return self.panel._full_glyph_list
     
     @full_glyph_list.setter
     def full_glyph_list(self, l):
         self.panel._full_glyph_list.clear()
```

### Comparing `ygt-0.2.3/src/ygt/ygSchema.py` & `ygt-0.2.4/src/ygt/ygSchema.py`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/ygStems.py` & `ygt-0.2.4/src/ygt/ygStems.py`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt/ygYAMLEditor.py` & `ygt-0.2.4/src/ygt/ygYAMLEditor.py`

 * *Files identical despite different names*

### Comparing `ygt-0.2.3/src/ygt.egg-info/PKG-INFO` & `ygt-0.2.4/src/ygt.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ygt
-Version: 0.2.3
+Version: 0.2.4
 Summary: A graphical hint editor for TrueType fonts
 Author-email: "Peter S. Baker" <b.tarde@mail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.4
 Description-Content-Type: text/markdown
@@ -14,26 +14,38 @@
 
 **Ygt** is a Python app for hinting TrueType fonts. It is built to be fast, flexible, and free:
 
 - it will run equally well under Windows, Mac OS, and Linux;
 - it emphasizes modern requirements for TrueType hinting while deemphasizing the obsolete;
 - the most common commands use unmodified shortcut keys so you can work quickly with one hand on the keyboard and one on the mouse;
 - it will read either a TrueType font or a UFO;
-- it can save hints in an easily understood and edited YAML file,
+- it saves hints in an easily understood and edited YAML file,
 - which can be compiled to a hinted font either from inside the program or from the command line,
 - or it can save compiled hints to a UFO (from which fontmake can produce a hinted font)
 
 Ygt is in an alpha state, with features yet to be added (especially auto-hinting). But it is already a workable program, which the developer has used to hint thousands of glyphs in several large fonts.
 
-For the time being, Ygt must be launched from a command line. To install, make sure you are running Python 3.10.4 or later and type `pip install ygt` on the command line. Alternatively, download the files from GitHub, navigate to the directory with the file pyproject.toml, and type `pip install .` (don't forget the period!). Then type `ygt` on the command line to start the program.
+Several executable files are available in the “Releases” section of the Ygt GitHub site. If none of these are suitable for your system, Ygt must be launched from a command line. In this case, install from an environment where the version of Python is 3.10.4 or later by typing `pip install ygt` on the command line. Alternatively, download the files from GitHub, navigate to the directory with the file pyproject.toml, and type `pip install .` (don't forget the period!). Then type `ygt <Return>` to start the program.
 
 For more information, see the [documentation](https://github.com/psb1558/ygt/tree/main/docs) or watch a brief [introductory video](https://psb1558.github.io/ygt/index.html).
 
 ## Changes
 
+### Version 0.2.4 (circa 2023-5-31)
+
+Qt was adding extra antialiasing in string/array preview. We now display only FreeType antialiasing.
+
+Harfbuzz metrics updated when instance is changed.
+
+Can now pass indices to cvNN and salt.
+
+Fixed crash on file not found.
+
+Preview->Features launches a dialog with which you can supply values, on, off, or 1-99 to any GSUB feature. Use it (among other things) to turn off features that are on by default.
+
 ### Version 0.2.3 (2023-5-25)
 
 Enable OpenType features in string preview panel (via Harfbuzz).
 
 Better lcd/subpixel rendering in string preview panel.
 
 Touched points are tinted pink.
```

### Comparing `ygt-0.2.3/src/ygt.egg-info/SOURCES.txt` & `ygt-0.2.4/src/ygt.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/ygt.py
 src/hooks/hook-freetype.py
+src/hooks/hook-uharfbuzz.py
 src/hooks/hook-xgridfit.py
 src/ygt/__init__.py
 src/ygt/__main__.py
-src/ygt/autohint_trash.py
 src/ygt/cvGuesser.py
 src/ygt/fontViewDialog.py
 src/ygt/freetypeFont.py
 src/ygt/harfbuzzFont.py
 src/ygt/macfuncDialog.py
 src/ygt/makeCVDialog.py
 src/ygt/window.py
 src/ygt/ygError.py
 src/ygt/ygHintEditor.py
+src/ygt/ygLabel.py
 src/ygt/ygModel.py
 src/ygt/ygPreferences.py
 src/ygt/ygPreview.py
 src/ygt/ygSchema.py
 src/ygt/ygStems.py
 src/ygt/ygYAMLEditor.py
 src/ygt.egg-info/PKG-INFO
```

