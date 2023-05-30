# Comparing `tmp/txrm2tiff-2.0.2.tar.gz` & `tmp/txrm2tiff-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/rky95813/Documents/Eclipse2/txrm2tiff/dist/tmp3wl_j0xf/txrm2tiff-2.0.2.tar", last modified: Tue Jan 18 15:39:39 2022, max compression
+gzip compressed data, was "/home/rky95813/Documents/Eclipse2/txrm2tiff/dist/.tmp-yj7778ir/txrm2tiff-2.0.4.tar", last modified: Tue May 30 18:36:48 2023, max compression
```

## Comparing `txrm2tiff-2.0.2.tar` & `txrm2tiff-2.0.4.tar`

### file list

```diff
@@ -1,49 +1,78 @@
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2022-01-18 15:39:39.000000 txrm2tiff-2.0.2/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1533 2020-03-30 17:10:47.000000 txrm2tiff-2.0.2/LICENSE
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7504 2022-01-18 15:39:39.000000 txrm2tiff-2.0.2/PKG-INFO
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6967 2021-11-26 16:04:02.000000 txrm2tiff-2.0.2/README.md
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       38 2022-01-18 15:39:39.000000 txrm2tiff-2.0.2/setup.cfg
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1407 2021-12-02 14:57:04.000000 txrm2tiff-2.0.2/setup.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2022-01-18 15:39:38.000000 txrm2tiff-2.0.2/src/
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2022-01-18 15:39:38.000000 txrm2tiff-2.0.2/src/txrm2tiff/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      181 2021-12-02 15:05:17.000000 txrm2tiff-2.0.2/src/txrm2tiff/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5891 2021-12-02 15:13:07.000000 txrm2tiff-2.0.2/src/txrm2tiff/__main__.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2022-01-18 15:39:38.000000 txrm2tiff-2.0.2/src/txrm2tiff/font/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    42884 2021-02-08 17:40:15.000000 txrm2tiff-2.0.2/src/txrm2tiff/font/CallingCode-Regular.otf
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      145 2021-12-14 14:32:03.000000 txrm2tiff-2.0.2/src/txrm2tiff/info.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6530 2021-12-01 13:13:47.000000 txrm2tiff-2.0.2/src/txrm2tiff/inspector.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7049 2021-12-14 13:07:27.000000 txrm2tiff-2.0.2/src/txrm2tiff/main.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2022-01-18 15:39:39.000000 txrm2tiff-2.0.2/src/txrm2tiff/txrm/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       28 2021-12-01 16:06:26.000000 txrm2tiff-2.0.2/src/txrm2tiff/txrm/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    18789 2021-12-14 14:32:04.000000 txrm2tiff-2.0.2/src/txrm2tiff/txrm/abstract.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    11806 2021-12-02 12:43:42.000000 txrm2tiff-2.0.2/src/txrm2tiff/txrm/annot_mixin.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1357 2021-12-14 13:07:27.000000 txrm2tiff-2.0.2/src/txrm2tiff/txrm/main.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     8432 2021-12-14 13:07:27.000000 txrm2tiff-2.0.2/src/txrm2tiff/txrm/ref_mixin.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2688 2021-12-14 13:07:27.000000 txrm2tiff-2.0.2/src/txrm2tiff/txrm/save_mixin.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1623 2021-12-01 16:29:22.000000 txrm2tiff-2.0.2/src/txrm2tiff/txrm/shifts_mixin.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1560 2021-12-14 13:12:04.000000 txrm2tiff-2.0.2/src/txrm2tiff/txrm/txrm_property.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3158 2021-12-14 13:07:27.000000 txrm2tiff-2.0.2/src/txrm2tiff/txrm/v3.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2928 2021-12-14 13:07:27.000000 txrm2tiff-2.0.2/src/txrm2tiff/txrm/v5.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2022-01-18 15:39:39.000000 txrm2tiff-2.0.2/src/txrm2tiff/txrm_functions/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       45 2021-11-26 16:04:02.000000 txrm2tiff-2.0.2/src/txrm2tiff/txrm_functions/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4668 2021-12-01 16:08:16.000000 txrm2tiff-2.0.2/src/txrm2tiff/txrm_functions/general.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2649 2021-12-01 16:08:13.000000 txrm2tiff-2.0.2/src/txrm2tiff/txrm_functions/images.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2022-01-18 15:39:39.000000 txrm2tiff-2.0.2/src/txrm2tiff/utils/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)        0 2021-11-26 16:04:02.000000 txrm2tiff-2.0.2/src/txrm2tiff/utils/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3923 2021-12-14 13:07:27.000000 txrm2tiff-2.0.2/src/txrm2tiff/utils/file_handler.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      415 2021-11-26 16:04:02.000000 txrm2tiff-2.0.2/src/txrm2tiff/utils/functions.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6020 2021-11-26 16:04:02.000000 txrm2tiff-2.0.2/src/txrm2tiff/utils/image_processing.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      818 2021-11-26 16:04:02.000000 txrm2tiff-2.0.2/src/txrm2tiff/utils/logging.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5618 2021-12-14 14:32:04.000000 txrm2tiff-2.0.2/src/txrm2tiff/utils/metadata.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2570 2021-11-26 16:04:02.000000 txrm2tiff-2.0.2/src/txrm2tiff/utils/shortcut_creation.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2022-01-18 15:39:39.000000 txrm2tiff-2.0.2/src/txrm2tiff/xradia_properties/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       50 2021-11-26 16:04:02.000000 txrm2tiff-2.0.2/src/txrm2tiff/xradia_properties/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1856 2021-11-26 16:04:02.000000 txrm2tiff-2.0.2/src/txrm2tiff/xradia_properties/enums.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3281 2021-12-14 13:07:27.000000 txrm2tiff-2.0.2/src/txrm2tiff/xradia_properties/stream_dtypes.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2022-01-18 15:39:38.000000 txrm2tiff-2.0.2/src/txrm2tiff.egg-info/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7504 2022-01-18 15:39:37.000000 txrm2tiff-2.0.2/src/txrm2tiff.egg-info/PKG-INFO
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1224 2022-01-18 15:39:38.000000 txrm2tiff-2.0.2/src/txrm2tiff.egg-info/SOURCES.txt
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)        1 2022-01-18 15:39:37.000000 txrm2tiff-2.0.2/src/txrm2tiff.egg-info/dependency_links.txt
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       55 2022-01-18 15:39:37.000000 txrm2tiff-2.0.2/src/txrm2tiff.egg-info/entry_points.txt
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      130 2022-01-18 15:39:38.000000 txrm2tiff-2.0.2/src/txrm2tiff.egg-info/requires.txt
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       10 2022-01-18 15:39:38.000000 txrm2tiff-2.0.2/src/txrm2tiff.egg-info/top_level.txt
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-05-30 18:36:48.000000 txrm2tiff-2.0.4/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1272 2021-02-08 17:40:15.000000 txrm2tiff-2.0.4/.gitignore
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-05-30 18:36:47.000000 txrm2tiff-2.0.4/.settings/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       64 2020-03-30 17:10:47.000000 txrm2tiff-2.0.4/.settings/org.eclipse.core.resources.prefs
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-05-30 18:36:47.000000 txrm2tiff-2.0.4/.vscode/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      638 2021-03-02 11:54:13.000000 txrm2tiff-2.0.4/.vscode/launch.json
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      766 2023-05-30 18:11:44.000000 txrm2tiff-2.0.4/.vscode/settings.json
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1533 2020-03-30 17:10:47.000000 txrm2tiff-2.0.4/LICENSE
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7445 2023-05-30 18:36:48.000000 txrm2tiff-2.0.4/PKG-INFO
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6967 2021-11-26 16:04:02.000000 txrm2tiff-2.0.4/README.md
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-05-30 18:36:47.000000 txrm2tiff-2.0.4/conda/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1473 2023-05-30 18:06:49.000000 txrm2tiff-2.0.4/conda/meta.yaml
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1536 2023-05-30 18:36:31.000000 txrm2tiff-2.0.4/pyproject.toml
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       38 2023-05-30 18:36:48.000000 txrm2tiff-2.0.4/setup.cfg
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-05-30 18:36:47.000000 txrm2tiff-2.0.4/src/
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-05-30 18:36:47.000000 txrm2tiff-2.0.4/src/txrm2tiff/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      122 2023-05-30 10:44:58.000000 txrm2tiff-2.0.4/src/txrm2tiff/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5966 2023-05-30 10:44:58.000000 txrm2tiff-2.0.4/src/txrm2tiff/__main__.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-05-30 18:36:47.000000 txrm2tiff-2.0.4/src/txrm2tiff/font/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    42884 2021-02-08 17:40:15.000000 txrm2tiff-2.0.4/src/txrm2tiff/font/CallingCode-Regular.otf
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1554 2021-02-08 17:40:15.000000 txrm2tiff-2.0.4/src/txrm2tiff/font/License.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       89 2023-05-30 10:44:58.000000 txrm2tiff-2.0.4/src/txrm2tiff/info.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6531 2023-05-30 10:44:58.000000 txrm2tiff-2.0.4/src/txrm2tiff/inspector.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7057 2023-05-30 10:44:58.000000 txrm2tiff-2.0.4/src/txrm2tiff/main.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-05-30 18:36:47.000000 txrm2tiff-2.0.4/src/txrm2tiff/txrm/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       28 2021-12-01 16:06:26.000000 txrm2tiff-2.0.4/src/txrm2tiff/txrm/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    18841 2023-05-30 10:44:58.000000 txrm2tiff-2.0.4/src/txrm2tiff/txrm/abstract.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    12824 2023-05-30 15:24:48.000000 txrm2tiff-2.0.4/src/txrm2tiff/txrm/annot_mixin.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1357 2021-12-14 13:07:27.000000 txrm2tiff-2.0.4/src/txrm2tiff/txrm/main.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     8432 2023-05-30 10:24:41.000000 txrm2tiff-2.0.4/src/txrm2tiff/txrm/ref_mixin.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3080 2023-05-30 14:59:57.000000 txrm2tiff-2.0.4/src/txrm2tiff/txrm/save_mixin.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1623 2021-12-01 16:29:22.000000 txrm2tiff-2.0.4/src/txrm2tiff/txrm/shifts_mixin.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1560 2023-05-30 10:24:37.000000 txrm2tiff-2.0.4/src/txrm2tiff/txrm/txrm_property.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3158 2023-05-30 10:24:41.000000 txrm2tiff-2.0.4/src/txrm2tiff/txrm/v3.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2928 2023-05-30 10:24:41.000000 txrm2tiff-2.0.4/src/txrm2tiff/txrm/v5.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-05-30 18:36:47.000000 txrm2tiff-2.0.4/src/txrm2tiff/txrm_functions/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       45 2021-11-26 16:04:02.000000 txrm2tiff-2.0.4/src/txrm2tiff/txrm_functions/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4667 2023-05-30 10:44:58.000000 txrm2tiff-2.0.4/src/txrm2tiff/txrm_functions/general.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2649 2021-12-01 16:08:13.000000 txrm2tiff-2.0.4/src/txrm2tiff/txrm_functions/images.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-05-30 18:36:47.000000 txrm2tiff-2.0.4/src/txrm2tiff/utils/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)        0 2021-11-26 16:04:02.000000 txrm2tiff-2.0.4/src/txrm2tiff/utils/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3915 2023-05-30 10:44:58.000000 txrm2tiff-2.0.4/src/txrm2tiff/utils/file_handler.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      415 2021-11-26 16:04:02.000000 txrm2tiff-2.0.4/src/txrm2tiff/utils/functions.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6400 2023-05-30 10:44:58.000000 txrm2tiff-2.0.4/src/txrm2tiff/utils/image_processing.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      818 2021-11-26 16:04:02.000000 txrm2tiff-2.0.4/src/txrm2tiff/utils/logging.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5618 2023-05-30 10:24:41.000000 txrm2tiff-2.0.4/src/txrm2tiff/utils/metadata.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2570 2021-11-26 16:04:02.000000 txrm2tiff-2.0.4/src/txrm2tiff/utils/shortcut_creation.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-05-30 18:36:47.000000 txrm2tiff-2.0.4/src/txrm2tiff/xradia_properties/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       50 2021-11-26 16:04:02.000000 txrm2tiff-2.0.4/src/txrm2tiff/xradia_properties/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1856 2023-05-30 10:24:41.000000 txrm2tiff-2.0.4/src/txrm2tiff/xradia_properties/enums.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3334 2023-05-30 10:44:58.000000 txrm2tiff-2.0.4/src/txrm2tiff/xradia_properties/stream_dtypes.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-05-30 18:36:47.000000 txrm2tiff-2.0.4/src/txrm2tiff.egg-info/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7445 2023-05-30 18:36:44.000000 txrm2tiff-2.0.4/src/txrm2tiff.egg-info/PKG-INFO
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1853 2023-05-30 18:36:46.000000 txrm2tiff-2.0.4/src/txrm2tiff.egg-info/SOURCES.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)        1 2023-05-30 18:36:44.000000 txrm2tiff-2.0.4/src/txrm2tiff.egg-info/dependency_links.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       54 2023-05-30 18:36:44.000000 txrm2tiff-2.0.4/src/txrm2tiff.egg-info/entry_points.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      170 2023-05-30 18:36:46.000000 txrm2tiff-2.0.4/src/txrm2tiff.egg-info/requires.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       10 2023-05-30 18:36:46.000000 txrm2tiff-2.0.4/src/txrm2tiff.egg-info/top_level.txt
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-05-30 18:36:48.000000 txrm2tiff-2.0.4/tests/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      193 2021-02-08 17:40:15.000000 txrm2tiff-2.0.4/tests/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    11184 2023-05-30 10:44:58.000000 txrm2tiff-2.0.4/tests/test_abstract_txrm.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    10711 2023-05-30 10:44:58.000000 txrm2tiff-2.0.4/tests/test_annotator.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     9650 2023-05-30 10:44:58.000000 txrm2tiff-2.0.4/tests/test_commandline_entrypoint.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4462 2023-05-30 10:24:41.000000 txrm2tiff-2.0.4/tests/test_file_handler.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5849 2023-05-30 10:44:58.000000 txrm2tiff-2.0.4/tests/test_image_processing.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2777 2021-12-01 16:29:22.000000 txrm2tiff-2.0.4/tests/test_inspector.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    14713 2023-05-30 10:44:58.000000 txrm2tiff-2.0.4/tests/test_main.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4036 2023-05-30 10:24:41.000000 txrm2tiff-2.0.4/tests/test_metadata.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3858 2023-05-30 10:24:41.000000 txrm2tiff-2.0.4/tests/test_referencer.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     9936 2023-05-30 16:23:06.000000 txrm2tiff-2.0.4/tests/test_saver.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1455 2021-12-01 16:07:16.000000 txrm2tiff-2.0.4/tests/test_setup_fuctions.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2246 2021-12-01 16:29:22.000000 txrm2tiff-2.0.4/tests/test_shifts.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5057 2021-12-01 16:07:23.000000 txrm2tiff-2.0.4/tests/test_txrm_functions.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2682 2023-05-30 10:44:58.000000 txrm2tiff-2.0.4/tests/test_txrm_property.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3709 2023-05-30 15:25:01.000000 txrm2tiff-2.0.4/tests/test_txrm_v5.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6007 2023-05-30 15:10:23.000000 txrm2tiff-2.0.4/tests/test_txrmv3.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      834 2021-12-01 16:07:35.000000 txrm2tiff-2.0.4/tests/test_util_functions.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7056 2021-12-14 13:07:27.000000 txrm2tiff-2.0.4/tests/test_with_files.py
```

### Comparing `txrm2tiff-2.0.2/LICENSE` & `txrm2tiff-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.2/PKG-INFO` & `txrm2tiff-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: txrm2tiff
-Version: 2.0.2
-Summary: A converter for Zeiss txrm and xrm files, created from B24 of Diamond Light Source
-Home-page: https://github.com/DiamondLightSource/txrm2tiff
-Author: Thomas Fish
-Author-email: thomas.fish@diamond.ac.uk
-License: BSD 3-Clause
-Platform: UNKNOWN
+Version: 2.0.4
+Summary: A converter for Zeiss txrm and xrm files, created by & for B24 of Diamond Light Source
+Author-email: Thomas Fish <thomas.fish@diamond.ac.uk>
+License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >3.6
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # txrm2tiff
 
 Converts TXRM/XRM files to OME-TIFF files.
 
 Txrm2tiff was created for users of beamline B24 of Diamond Light Source by Thomas Fish. This has been adapted from, and is used by, B24's the automatic processing pipeline. Parts of this code were originally written by Kevin Savage, with further additions and amendments by Peter Chang, Victoria Beilsten-Edmands.
@@ -118,9 +116,7 @@
 * Any annotations from XRM/TXRM v5.0 files can be exported and saved (along with a scale bar).
 * Data type of the output image can be specified (warnings will be given if the data type limits off the dynamic range of the image, also values are rounded before casting float -> integer).
 * Metadata will be added in OME XML format to the header.
 * Batch convert options.
 * Inspector (can extract any information from XRM/TXRM files).
 * Within Python, XRM/TXRM files can be opened and interacted with using the function `open_txrm` (`from txrm2tiff import open_txrm`), which returns a `Txrm` object of the correct version. Recomended usage: `with open_txrm(...) as txrm:`.
 * Within Python, XRM/TXRM files can quickly be converted and saved using `convert_and_save` (`from txrm2tiff import convert_and_save`).
-
-
```

### Comparing `txrm2tiff-2.0.2/README.md` & `txrm2tiff-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/__main__.py` & `txrm2tiff-2.0.4/src/txrm2tiff/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 #!/usr/bin/python
 import argparse
 import sys
+import os
+if os.name == "nt":
+    sys.stdout.reconfigure(encoding="utf-8")
 
 from .info import __version__
 
 parser = argparse.ArgumentParser(
     prog="txrm2tiff",
     description="Converter of txrm/xrm files to OME tif/tiff files",
     add_help=False,
```

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/font/CallingCode-Regular.otf` & `txrm2tiff-2.0.4/src/txrm2tiff/font/CallingCode-Regular.otf`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/inspector.py` & `txrm2tiff-2.0.4/src/txrm2tiff/inspector.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
                                 dtype,
                                 strict=True,
                             )
                             values_str = ", ".join([str(i) for i in values])
                             self._output_text += f"\t{values_str} (stored as {dtype})"
                         except (ValueError, TypeError) as e:
                             self._output_text += (
-                                f"\tWARNING: Expected data type unsucessful:\t{e}\n"
+                                f"\tWARNING: Expected data type unsuccessful:\t{e}\n"
                             )
                             self.inspect_unknown_dtype_stream(key)
                     else:
                         self._output_text += f"\nUnknown data type. "
                         self.inspect_unknown_dtype_stream(key)
                 else:
                     self._output_text += f"\nStream '{key}' does not exist.\n"
```

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/main.py` & `txrm2tiff-2.0.4/src/txrm2tiff/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -171,20 +171,20 @@
         output_path = input_path
     else:
         if output_path.suffix == "" or output_path.is_dir():
             output_path = output_path / input_path.name
         else:
             # If a valid filepath was given, just return that (avoids double .ome)
             return output_path
-    return _set_output_suffix(output_path, curent_suffix=input_path.suffix)
+    return _set_output_suffix(output_path, current_suffix=input_path.suffix)
 
 
-def _set_output_suffix(filepath: Path, curent_suffix: Optional[str] = None) -> Path:
-    if curent_suffix is None:
-        curent_suffix = filepath.suffix
-    if curent_suffix == ".txrm":
+def _set_output_suffix(filepath: Path, current_suffix: Optional[str] = None) -> Path:
+    if current_suffix is None:
+        current_suffix = filepath.suffix
+    if current_suffix == ".txrm":
         return filepath.with_suffix(".ome.tiff")
-    elif curent_suffix == ".xrm":
+    elif current_suffix == ".xrm":
         return filepath.with_suffix(".ome.tif")
     else:
-        logging.error("Invalid file extension: %s", curent_suffix)
-        raise NameError(f"Invalid file extension: {curent_suffix}")
+        logging.error("Invalid file extension: %s", current_suffix)
+        raise NameError(f"Invalid file extension: {current_suffix}")
```

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/txrm/abstract.py` & `txrm2tiff-2.0.4/src/txrm2tiff/txrm/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                 self.ole = OleFileIO(f)
             else:
                 raise IOError("'%s' is not a valid xrm/txrm file" % self.name)
             if self.ole.fp is None:
                 raise IOError("'%s' failed to open for unknown reasons" % self.name)
 
     def close(self) -> None:
-        """Closes txrm file. Can be reoped using open_file."""
+        """Closes txrm file. Can be reopened using open_file."""
         if not self.file_is_open:
             logging.info("File %s is already closed", self.name)
             return
         logging.debug("Closing file %s", self.name)
         self.ole.close()
 
     def clear_all(self):
@@ -241,15 +241,15 @@
                         self.image_dtype,
                     )
             if imgdata is None:  # if dtype was not given or that method failed
                 img_size = np.prod(self.shape)
                 imgdata = txrm_functions.fallback_image_interpreter(
                     img_stream_bytes, img_size, self.strict
                 )
-            if imgdata.size:
+            if imgdata.size > 0:
                 imgdata.shape = self.shape  # Resize if not empty
             return imgdata
         except Exception:
             if strict:
                 raise
             return np.asarray([])
 
@@ -382,15 +382,16 @@
             self.image_info["MosiacRows"][0],
         ]
 
     @txrm_property(fallback=[])
     def energies(self) -> typing.List[float]:
         energies = self.image_info["Energy"]
         if not np.sum(energies):
-            energies = self.position_info["Energy"]
+            # position_info includes units
+            energies = self.position_info["Energy"][0]
         if np.sum(energies):
             return energies
         raise ValueError("Could not get energies")
 
     @txrm_property(fallback=[])
     def exposures(self) -> typing.List[float]:
         """Returns list of exposures"""
```

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/txrm/annot_mixin.py` & `txrm2tiff-2.0.4/src/txrm2tiff/txrm/annot_mixin.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from collections import defaultdict
 from typing import Iterable, Optional, Tuple
 
 import numpy as np
 from PIL import Image, ImageDraw, ImageFont
 from PIL.ImageOps import autocontrast
 
+from ..utils.file_handler import manual_annotation_save
 from ..xradia_properties import AnnotationTypes, XrmDataTypes as XDT
 
 font_path = Path(__file__).parent.parent / "font" / "CallingCode-Regular.otf"
 
 
 class AnnotatorMixin:
     def __new__(cls, *args, **kwargs):
@@ -30,17 +31,17 @@
                 AnnotationTypes.ANN_CIRCLE: cls._plot_ellipse,
                 AnnotationTypes.ANN_POLYGON: cls._plot_polygon,
                 AnnotationTypes.ANN_POLYLINE: cls._plot_polyline,
                 AnnotationTypes.ANN_FREE_HAND_SKETCH: cls._plot_freehand,
             },
         )
 
-    def annotate(self) -> Optional[np.ndarray]:
+    def annotate(self, scale_bar=True) -> Optional[np.ndarray]:
         """Annotate output image. Please ensure that the image has been referenced first, if applicable."""
-        annotations = self.extract_annotations(scale_bar=True)
+        annotations = self.extract_annotations(scale_bar=scale_bar)
         # Checks if anything has been added
         if annotations is None:
             logging.warning("No annotations to apply")
             self.annotated_image = None
         else:
             # Annotations will be in the wrong place if flipped
             images = self.get_output(flip=False, clear_images=False)
@@ -132,33 +133,31 @@
                 tmp_bar_length = (
                     self.output_shape[2] / 5.0
                 )  # Get initial bar length based on image width
                 tmp_bar_size = tmp_bar_length * pixel_size  # Calculate physical size
 
                 # Round to nearest multiple of the order of magnitude
                 exponent = math.floor(math.log10(tmp_bar_size))
-                step_size = 10.0 ** exponent
+                step_size = 10.0**exponent
                 bar_size = round(
                     round(tmp_bar_size / step_size)
                     * step_size,  # Find nearest multiple of step_size
                     -exponent,
                 )  # round to -exponent decimal places (to mitigate rounding errors)
                 bar_length = (
                     bar_size / pixel_size
                 )  # Calculate number of pixels that wide new bar size bar should be
 
                 # Set text and calculate text positions:
                 text = "%gμm" % bar_size
-                text_width, text_height = draw.textsize(text, font=f)
-                text_x = round(
-                    x0 + bar_length / 2 - (text_width / 2)
-                )  # Centre text above bar
-                text_y = y0 - bar_width - text_height
+                text_xy = (x0 + bar_length / 2, y0 - bar_width)
                 # Draw:
-                draw.text((text_x, text_y), text, font=f, fill=colour)
+                draw.text(
+                    text_xy, text, font=f, fill=colour, anchor="mb"
+                )  # anchor: middle-bottom
                 draw.line((x0, y0, x0 + bar_length, y0), fill=colour, width=bar_width)
                 return True
             except Exception:
                 logging.error(
                     "Exception occurred while drawing scale bar", exc_info=True
                 )
         return False
@@ -176,62 +175,66 @@
         return (*colours[2::-1], colours[3])
 
     @staticmethod
     def _not_implemented(*args):
         """Do nothing"""
         pass
 
-    def _plot_line(self, draw: ImageDraw, stream_stem: str):
+    def _plot_line(self, draw: ImageDraw, stream_stem: str) -> None:
         colour = self._get_colour(stream_stem)
         thickness = self._get_thickness(stream_stem)
         x1 = self.read_stream(f"{stream_stem}/X1", XDT.XRM_DOUBLE, strict=True)[0]
         x2 = self.read_stream(f"{stream_stem}/X2", XDT.XRM_DOUBLE, strict=True)[0]
         y1 = self.read_stream(f"{stream_stem}/Y1", XDT.XRM_DOUBLE, strict=True)[0]
         y2 = self.read_stream(f"{stream_stem}/Y2", XDT.XRM_DOUBLE, strict=True)[0]
 
         draw.line(self._flip_y((x1, y1), (x2, y2)), fill=colour, width=thickness)
 
-    def _plot_rect(self, draw: ImageDraw, stream_stem: str):
+    def __extract_rectangle_coords(self, stream_stem: str) -> Tuple[Tuple[int]]:
+        x = []
+        y = []
+        x.append(
+            self.read_stream(f"{stream_stem}/Rectangle/Left", XDT.XRM_INT, strict=True)[
+                0
+            ]
+        )
+        y.append(
+            self.read_stream(
+                f"{stream_stem}/Rectangle/Bottom", XDT.XRM_INT, strict=True
+            )[0]
+        )
+        x.append(
+            self.read_stream(
+                f"{stream_stem}/Rectangle/Right", XDT.XRM_INT, strict=True
+            )[0]
+        )
+        y.append(
+            self.read_stream(f"{stream_stem}/Rectangle/Top", XDT.XRM_INT, strict=True)[
+                0
+            ]
+        )
+        x.sort()
+        y.sort(reverse=True)
+        # Values in the first tuple must be smaller than their respective second tuple value.
+        # Therefore y1 must be first and y0 second because they are flipped.
+        return self._flip_y(*zip(x, y))
+
+    def _plot_rect(self, draw: ImageDraw, stream_stem: str) -> None:
         colour = self._get_colour(stream_stem)
         thickness = self._get_thickness(stream_stem)
-        x0 = self.read_stream(
-            f"{stream_stem}/Rectangle/Left", XDT.XRM_INT, strict=True
-        )[0]
-        y0 = self.read_stream(
-            f"{stream_stem}/Rectangle/Bottom", XDT.XRM_INT, strict=True
-        )[0]
-        x1 = self.read_stream(
-            f"{stream_stem}/Rectangle/Right", XDT.XRM_INT, strict=True
-        )[0]
-        y1 = self.read_stream(f"{stream_stem}/Rectangle/Top", XDT.XRM_INT, strict=True)[
-            0
-        ]
+        xy = self.__extract_rectangle_coords(stream_stem)
 
-        draw.rectangle(
-            self._flip_y((x0, y0), (x1, y1)), outline=colour, width=thickness
-        )
+        draw.rectangle(xy, outline=colour, width=thickness)
 
-    def _plot_ellipse(self, draw: ImageDraw, stream_stem: str):
+    def _plot_ellipse(self, draw: ImageDraw, stream_stem: str) -> None:
         colour = self._get_colour(stream_stem)
         thickness = self._get_thickness(stream_stem)
-        x0 = self.read_stream(
-            f"{stream_stem}/Rectangle/Left", XDT.XRM_INT, strict=True
-        )[0]
-        y0 = self.read_stream(
-            f"{stream_stem}/Rectangle/Bottom", XDT.XRM_INT, strict=True
-        )[0]
-        x1 = self.read_stream(
-            f"{stream_stem}/Rectangle/Right", XDT.XRM_INT, strict=True
-        )[0]
-        y1 = self.read_stream(f"{stream_stem}/Rectangle/Top", XDT.XRM_INT, strict=True)[
-            0
-        ]
-        # Values in the first tuple must be smaller than their respective second tuple value.
-        # Therefore y1 must be first and y0 second because they are flipped.
-        draw.ellipse(self._flip_y((x0, y1), (x1, y0)), outline=colour, width=thickness)
+        xy = self.__extract_rectangle_coords(stream_stem)
+
+        draw.ellipse(xy, outline=colour, width=thickness)
 
     def _plot_polygon(self, draw: ImageDraw, stream_stem: str) -> None:
         colour = self._get_colour(stream_stem)
         thickness = self._get_thickness(stream_stem)
         total_points = self.read_stream(f"{stream_stem}/TotalPts", np.uintc)[0]
         xs = self.read_stream(f"{stream_stem}/PointX", XDT.XRM_DOUBLE, strict=True)[
             :total_points
@@ -259,20 +262,53 @@
             width=thickness,
             joint=joint,
         )
 
     def _plot_freehand(self, draw: ImageDraw, stream_stem: str) -> None:
         self._plot_polyline(draw, stream_stem, joint="curve")
 
-    def _flip_y(self, *xys: Iterable[Number]) -> Tuple[Tuple[Number, Number]]:
+    def _flip_y(self, *xys: Iterable[Number]) -> Tuple[Tuple[Number]]:
         """
         Stored x-y coordinates are assuming 0 is bottom left, whereas PIL assumes 0 is top left
         This flips any list of coordinates that alternate x, y
 
         Args:
             *xys: n args assuming the form (x0, y0), (x1, y1), ... (xn, yn)
 
         Returns:
-            tuple of tuples: x-y coordinates with a flipped y
+            Tuple of tuples: x-y coordinates with a flipped y
         """
-        xys = tuple((x, self.output_shape[1] - 1 - y) for (x, y) in xys)
-        return xys
+        return tuple((x, self.output_shape[1] - 1 - y) for x, y in xys)
+
+    def save_annotations(
+        self,
+        filepath: Optional[Path] = None,
+        mkdir: bool = False,
+        strict: Optional[bool] = None,
+    ) -> bool:
+        """Saves images (if available) returning True if successful."""
+        if strict is None:
+            strict = self.strict
+        try:
+            if self.annotated_image is None:
+                raise AttributeError("No annotated image to save")
+            if filepath is None:
+                if self.path is None:
+                    raise ValueError(
+                        "An output filepath must be given if an input path was not given."
+                    )
+                filepath = self.path.resolve()
+                filepath = filepath.parent / f"{filepath.stem}_Annotated.tiff"
+
+            if mkdir:
+                filepath.parent.mkdir(parents=True, exist_ok=True)
+
+            manual_annotation_save(
+                filepath,
+                self.annotated_image,
+            )
+            return True
+        except Exception:
+            logging.error("Saving failed", exc_info=not strict)
+            if strict:
+                raise
+            return False
```

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/txrm/main.py` & `txrm2tiff-2.0.4/src/txrm2tiff/txrm/main.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/txrm/ref_mixin.py` & `txrm2tiff-2.0.4/src/txrm2tiff/txrm/ref_mixin.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/txrm/save_mixin.py` & `txrm2tiff-2.0.4/src/txrm2tiff/txrm/save_mixin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 import logging
 
-import numpy as np
 from pathlib import Path
 from typing import Optional
+import numpy as np
 from numpy.typing import DTypeLike
 
 from ..utils.metadata import create_ome_metadata, dtype_dict
-from ..utils.file_handler import manual_save, manual_annotation_save
+from ..utils.file_handler import manual_save
 
 
 class SaveMixin:
     def save_images(
         self,
         filepath: Optional[Path] = None,
         datatype: Optional[DTypeLike] = None,
         shifts: bool = True,
         flip: bool = False,
         clear_images: bool = False,
         mkdir: bool = False,
+        save_annotations: bool = True,
+        annotated_path: Optional[Path] = None,
+        strict: Optional[bool] = None,
     ) -> bool:
         """Saves images (if available) returning True if successful."""
+        if strict is None:
+            strict = self.strict
         try:
             if filepath is None:
                 if self.path is None:
                     raise ValueError(
                         "An output filepath must be given if an input path was not given."
                     )
-                filepath = self.path.with_suffix(".ome.tiff")
+                filepath = self.path.resolve().with_suffix(".ome.tiff")
             if not self.referenced:
                 logging.info("Saving without reference")
 
             im = self.get_output(
                 load=True, shifts=shifts, flip=flip, clear_images=clear_images
             )
             if im is None:
@@ -44,29 +49,34 @@
                         datatype,
                         ", ".join(dtype_dict.keys()),
                         str(im.dtype),
                     )
             metadata = self.create_metadata(filepath)
 
             if mkdir:
-                tiff_dir = filepath.resolve().parent
-                tiff_dir.mkdir(parents=True, exist_ok=True)
+                filepath.parent.mkdir(parents=True, exist_ok=True)
 
             manual_save(filepath, im, datatype, metadata)
-            if self.annotated_image is not None:
-                stem = filepath.stem
-                suffix = filepath.suffix
-                if stem.lower().endswith(".ome") and suffix.lower() == ".tiff":
-                    # Special case for ome.tiff
-                    suffix = f"{stem[-4:]}{suffix}"
-                    stem = stem[:-4]
-                manual_annotation_save(
-                    filepath.parent / f"{stem}_Annotated{suffix}",
-                    self.annotated_image,
-                )
+            if (
+                save_annotations
+                and hasattr(self, "annotate")
+                and self.annotated_image is not None
+            ):
+                if annotated_path is None:
+                    # Generate default path
+                    filename = filepath.name
+                    if filename.lower().endswith(".ome.tiff"):
+                        # Special case for ome.tiff
+                        stem, suffix = filename.rsplit(".ome.")
+                    else:
+                        stem, suffix = filename.rsplit(".")
+                    annotated_path = filepath.parent / f"{stem}_Annotated.{suffix}"
+                self.save_annotations(annotated_path, mkdir=mkdir, strict=strict)
             return True
         except Exception:
-            logging.error("Saving failed", exc_info=True)
+            logging.error("Saving failed", exc_info=not strict)
+            if strict:
+                raise
             return False
 
     def create_metadata(self, filepath: Path):
         return create_ome_metadata(self, filepath.stem)
```

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/txrm/shifts_mixin.py` & `txrm2tiff-2.0.4/src/txrm2tiff/txrm/shifts_mixin.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/txrm/txrm_property.py` & `txrm2tiff-2.0.4/src/txrm2tiff/txrm/txrm_property.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/txrm/v3.py` & `txrm2tiff-2.0.4/src/txrm2tiff/txrm/v3.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/txrm/v5.py` & `txrm2tiff-2.0.4/src/txrm2tiff/txrm/v5.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/txrm_functions/general.py` & `txrm2tiff-2.0.4/src/txrm2tiff/txrm_functions/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         logging.error(
             "Error occurred reading stream '%s' as %s", key, dtype, exc_info=True
         )
         return []
 
 
 def get_stream_from_bytes(stream_bytes: bytes, dtype: npt.DTypeLike) -> np.ndarray:
-    """Converts olefile bytes to np.ndarray of valuess of type dtype."""
+    """Converts olefile bytes to np.ndarray of values of type dtype."""
     return np.frombuffer(stream_bytes, dtype)
 
 
 def _read_number_stream_to_list(
     ole: of.OleFileIO, key: str, dtype: typing.Union[npt.DTypeLike, None]
 ) -> typing.List[typing.Union[numbers.Number, bytes]]:
     """Reads olefile stream and returns to list of values of type dtype."""
@@ -101,15 +101,15 @@
     return image_info
 
 
 def get_position_dict(
     ole: of.OleFileIO,
 ) -> typing.Dict[str, typing.Tuple[typing.Union[typing.List, str]]]:
     """
-    Gets dictionary of motor posisions.
+    Gets dictionary of motor positions.
 
     Args:
         ole (of.OleFileIO)
 
     Returns:
         typing.Dict[str, typing.Tuple[typing.Union[typing.List, str]]]: all positions for each motor in the form: {motor name string: ([values], unit string)}.
     """
```

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/txrm_functions/images.py` & `txrm2tiff-2.0.4/src/txrm2tiff/txrm_functions/images.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/utils/file_handler.py` & `txrm2tiff-2.0.4/src/txrm2tiff/utils/file_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import tifffile as tf
 import numpy as np
 from numpy.typing import DTypeLike
-from os import access, R_OK, remove, PathLike
+from os import access, R_OK, PathLike
 from pathlib import Path
 from typing import Optional, Union, List
 from olefile import OleFileIO, isOleFile
 from oxdls import OMEXML
 
 from .metadata import dtype_dict
 from .image_processing import cast_to_dtype
```

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/utils/image_processing.py` & `txrm2tiff-2.0.4/src/txrm2tiff/utils/image_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,42 +83,56 @@
                 dtype_info = np.iinfo(dtype)
             elif np.issubdtype(dtype, np.floating):
                 dtype_info = np.finfo(dtype)
             else:
                 raise TypeError(f"Cannot cast to invalid data type {data_type}")
             # Round min/max to avoid this warning when the issue is just going to be rounded away.
             img_min, img_max = image.min(), image.max()
-            if dtype_info.min > img_min:
+            dtype_min, dtype_max = dtype_info.min, dtype_info.max
+            if dtype_min > img_min:
                 logging.warning(
                     "Image min %f below %s minimum of %i, values below this will be cut off",
                     img_min,
                     dtype,
-                    dtype_info.min,
+                    dtype_min,
                 )
-            if dtype_info.max < img_max:
+            else:
+                dtype_min = None
+            if dtype_max < img_max:
                 logging.warning(
                     "Image max %f above %s maximum of %i, values above this will be cut off",
                     img_max,
                     dtype,
-                    dtype_info.max,
+                    dtype_max,
                 )
-            np.clip(image, dtype_info.min, dtype_info.max, out=image)
+            else:
+                dtype_max = None
+            
+            if dtype_min is not None or dtype_max is not None:
+                np.clip(image, dtype_min, dtype_max, out=image)
+
             if np.issubdtype(dtype, np.integer) and np.issubdtype(
                 image.dtype, np.floating
             ):
                 image = np.around(image, decimals=0)
-            image = image.astype(dtype)
+
+            image = image.astype(dtype, copy=False)
             logging.info("Image has been cast to %s", data_type)
-    except Exception as e:
+    except TypeError:
         logging.warning(
             "Invalid data type given: %s aka %s. Image will remain as %s.",
             data_type,
             dtype,
             image.dtype,
         )
+    except Exception:
+        logging.error(
+            "An error occurred casting image from %s to %s", image.dtype, data_type
+        )
+        raise
     return image
 
 
 def tile_image_data_to_mosaic(
     refdata: np.ndarray,
     image_rows: int,
     image_columns: int,
```

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/utils/logging.py` & `txrm2tiff-2.0.4/src/txrm2tiff/utils/logging.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/utils/metadata.py` & `txrm2tiff-2.0.4/src/txrm2tiff/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/utils/shortcut_creation.py` & `txrm2tiff-2.0.4/src/txrm2tiff/utils/shortcut_creation.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/xradia_properties/enums.py` & `txrm2tiff-2.0.4/src/txrm2tiff/xradia_properties/enums.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff/xradia_properties/stream_dtypes.py` & `txrm2tiff-2.0.4/src/txrm2tiff/xradia_properties/stream_dtypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     "ImageInfo/CamPixelSize": XrmDataTypes.XRM_FLOAT,
     "ImageInfo/Current": XrmDataTypes.XRM_FLOAT,
     "ImageInfo/Date": XrmDataTypes.XRM_STRING,
     "ImageInfo/Energy": XrmDataTypes.XRM_FLOAT,
     "ImageInfo/ExpTime": XrmDataTypes.XRM_FLOAT,
     "ImageInfo/ExpTimes": XrmDataTypes.XRM_FLOAT,
     "ImageInfo/HorizontalBin": XrmDataTypes.XRM_INT,
+    "ImageInfo/VerticalalBin": XrmDataTypes.XRM_INT,
     "ImageInfo/ImageHeight": XrmDataTypes.XRM_INT,
     "ImageInfo/ImageWidth": XrmDataTypes.XRM_INT,
     "ImageInfo/ImagesPerProjection": XrmDataTypes.XRM_INT,
     "ImageInfo/ImagesTaken": XrmDataTypes.XRM_UNSIGNED_INT,
     "ImageInfo/IonChamberCurrent": XrmDataTypes.XRM_FLOAT,
     "ImageInfo/MosaicFastAxis": XrmDataTypes.XRM_INT,
     "ImageInfo/MosaicSlowAxis": XrmDataTypes.XRM_INT,
```

### Comparing `txrm2tiff-2.0.2/src/txrm2tiff.egg-info/PKG-INFO` & `txrm2tiff-2.0.4/src/txrm2tiff.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: txrm2tiff
-Version: 2.0.2
-Summary: A converter for Zeiss txrm and xrm files, created from B24 of Diamond Light Source
-Home-page: https://github.com/DiamondLightSource/txrm2tiff
-Author: Thomas Fish
-Author-email: thomas.fish@diamond.ac.uk
-License: BSD 3-Clause
-Platform: UNKNOWN
+Version: 2.0.4
+Summary: A converter for Zeiss txrm and xrm files, created by & for B24 of Diamond Light Source
+Author-email: Thomas Fish <thomas.fish@diamond.ac.uk>
+License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >3.6
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # txrm2tiff
 
 Converts TXRM/XRM files to OME-TIFF files.
 
 Txrm2tiff was created for users of beamline B24 of Diamond Light Source by Thomas Fish. This has been adapted from, and is used by, B24's the automatic processing pipeline. Parts of this code were originally written by Kevin Savage, with further additions and amendments by Peter Chang, Victoria Beilsten-Edmands.
@@ -118,9 +116,7 @@
 * Any annotations from XRM/TXRM v5.0 files can be exported and saved (along with a scale bar).
 * Data type of the output image can be specified (warnings will be given if the data type limits off the dynamic range of the image, also values are rounded before casting float -> integer).
 * Metadata will be added in OME XML format to the header.
 * Batch convert options.
 * Inspector (can extract any information from XRM/TXRM files).
 * Within Python, XRM/TXRM files can be opened and interacted with using the function `open_txrm` (`from txrm2tiff import open_txrm`), which returns a `Txrm` object of the correct version. Recomended usage: `with open_txrm(...) as txrm:`.
 * Within Python, XRM/TXRM files can quickly be converted and saved using `convert_and_save` (`from txrm2tiff import convert_and_save`).
-
-
```

