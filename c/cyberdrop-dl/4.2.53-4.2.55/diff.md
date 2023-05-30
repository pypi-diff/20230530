# Comparing `tmp/cyberdrop-dl-4.2.53.tar.gz` & `tmp/cyberdrop-dl-4.2.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.53.tar", last modified: Mon May 29 15:28:13 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.55.tar", last modified: Tue May 30 19:12:55 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.53.tar` & `cyberdrop-dl-4.2.55.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:13.454269 cyberdrop-dl-4.2.53/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-29 15:28:13.454269 cyberdrop-dl-4.2.53/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17777 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:13.446268 cyberdrop-dl-4.2.53/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:13.450269 cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:13.450269 cyberdrop-dl-4.2.53/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:13.450269 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:13.454269 cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18292 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17678 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20640 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:13.454269 cyberdrop-dl-4.2.53/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:13.446268 cyberdrop-dl-4.2.53/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-29 15:28:13.000000 cyberdrop-dl-4.2.53/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-29 15:28:13.000000 cyberdrop-dl-4.2.53/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 15:28:13.000000 cyberdrop-dl-4.2.53/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 15:28:13.000000 cyberdrop-dl-4.2.53/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-29 15:28:13.000000 cyberdrop-dl-4.2.53/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 15:28:13.000000 cyberdrop-dl-4.2.53/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-29 15:28:13.454269 cyberdrop-dl-4.2.53/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:55.917214 cyberdrop-dl-4.2.55/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-05-30 19:12:55.917214 cyberdrop-dl-4.2.55/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:55.909214 cyberdrop-dl-4.2.55/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:55.909214 cyberdrop-dl-4.2.55/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:55.913214 cyberdrop-dl-4.2.55/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:55.917214 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:55.917214 cyberdrop-dl-4.2.55/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18292 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17678 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20640 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:55.917214 cyberdrop-dl-4.2.55/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20796 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:55.909214 cyberdrop-dl-4.2.55/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-05-30 19:12:55.000000 cyberdrop-dl-4.2.55/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-30 19:12:55.000000 cyberdrop-dl-4.2.55/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:12:55.000000 cyberdrop-dl-4.2.55/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-30 19:12:55.000000 cyberdrop-dl-4.2.55/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-30 19:12:55.000000 cyberdrop-dl-4.2.55/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 19:12:55.000000 cyberdrop-dl-4.2.55/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-30 19:12:55.917214 cyberdrop-dl-4.2.55/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:12:42.000000 cyberdrop-dl-4.2.55/setup.py
```

### Comparing `cyberdrop-dl-4.2.53/LICENSE` & `cyberdrop-dl-4.2.55/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/PKG-INFO` & `cyberdrop-dl-4.2.55/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.53
+Version: 4.2.55
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -56,15 +56,15 @@
 | Fapello                                 | Models: fapello.com/...                                                                                                                                                                                                                |
 | Gallery.DeltaPorno.com                  | Albums: Gallery.DeltaPorno.com/album/... <br> Direct Images: Gallery.DeltaPorno.com/image/... <br> User Profile: Gallery.DeltaPorno.com/#USER# <br> All User Albums: Gallery.DeltaPorno.com/#USER#/albums                              |
 | GoFile                                  | Albums: gofile.io/d/...                                                                                                                                                                                                                |
 | Gfycat                                  | Gif: gfycat.com/...                                                                                                                                                                                                                    |
 | HGameCG                                 | Albums: hgamecg.com/.../index.html                                                                                                                                                                                                     |
 | ImgBox                                  | Albums: imgbox.com/g/... <br> Direct Images: images#.imgbox.com/... <br> Single Files: imgbox.com/...                                                                                                                                  |
 | IMG.Kiwi                                | Albums: img.kiwi/album/... <br> Direct Images: img.kiwi/image/... <br> User Profile: img.kiwi/#USER# <br> All User Albums: img.kiwi/#USER#/albums                                                                                      |
-| jpg.church<br/>jpg.fish<br/>jpg.fishing | Albums: jpg.church/album/... <br> Direct Images: jpg.church/image/... <br> User Profile: jpg.church/#USER# <br> All User Albums: jpg.church/#USER#/albums                                                                              |
+| jpg.church<br/>jpg.fish<br/>jpg.fishing<br/>jpg.pet | Albums: jpg.church/album/... <br> Direct Images: jpg.church/image/... <br> User Profile: jpg.church/#USER# <br> All User Albums: jpg.church/#USER#/albums                                                                              |
 | LoveFap                                 | Albums: lovefap.com/a/... <br> Direct Images: s*.lovefap.com/content/photos/... <br> Videos: lovefap.com/video/...                                                                                                                     |
 | NSFW.XXX                                | Profile: nsfw.xxx/user/... <br> Post: nsfw.xxx/post/...                                                                                                                                                                                |
 | PimpAndHost                             | Albums: pimpandhost.com/album/... <br> Single Files: pimpandhost.com/image/...                                                                                                                                                         |
 | PixelDrain                              | Albums: Pixeldrain.com/l/... <br> Single Files: Pixeldrain.com/u/...                                                                                                                                                                   |
 | Pixl                                    | Albums: pixl.li/album/... <br> Direct Images: pixl.li/image/...  <br> User Profile: pixl.li/#USER# <br> All User Albums: pixl.li/#USER#/albums                                                                                         |
 | Postimg.cc                              | Albums: postimg.cc/gallery/... <br> Direct Images: postimg.cc/...                                                                                                                                                                      |
 | NudoStar                                | Thread: nudostar.com/forum/threads/...  <br> Continue from (will download this post and after): nudostar.com/forum/threads/...post-NUMBER                                                                                              |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.53 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.55 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
@@ -56,15 +56,16 @@
 hgamecg.com/.../index.html | | ImgBox | Albums: imgbox.com/g/...
 Direct Images: images#.imgbox.com/...
 Single Files: imgbox.com/... | | IMG.Kiwi | Albums: img.kiwi/album/...
 Direct Images: img.kiwi/image/...
 User Profile: img.kiwi/#USER#
 All User Albums: img.kiwi/#USER#/albums | | jpg.church
 jpg.fish
-jpg.fishing | Albums: jpg.church/album/...
+jpg.fishing
+jpg.pet | Albums: jpg.church/album/...
 Direct Images: jpg.church/image/...
 User Profile: jpg.church/#USER#
 All User Albums: jpg.church/#USER#/albums | | LoveFap | Albums: lovefap.com/
 a/...
 Direct Images: s*.lovefap.com/content/photos/...
 Videos: lovefap.com/video/... | | NSFW.XXX | Profile: nsfw.xxx/user/...
 Post: nsfw.xxx/post/... | | PimpAndHost | Albums: pimpandhost.com/album/...
```

### Comparing `cyberdrop-dl-4.2.53/README.md` & `cyberdrop-dl-4.2.55/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 | Fapello                                 | Models: fapello.com/...                                                                                                                                                                                                                |
 | Gallery.DeltaPorno.com                  | Albums: Gallery.DeltaPorno.com/album/... <br> Direct Images: Gallery.DeltaPorno.com/image/... <br> User Profile: Gallery.DeltaPorno.com/#USER# <br> All User Albums: Gallery.DeltaPorno.com/#USER#/albums                              |
 | GoFile                                  | Albums: gofile.io/d/...                                                                                                                                                                                                                |
 | Gfycat                                  | Gif: gfycat.com/...                                                                                                                                                                                                                    |
 | HGameCG                                 | Albums: hgamecg.com/.../index.html                                                                                                                                                                                                     |
 | ImgBox                                  | Albums: imgbox.com/g/... <br> Direct Images: images#.imgbox.com/... <br> Single Files: imgbox.com/...                                                                                                                                  |
 | IMG.Kiwi                                | Albums: img.kiwi/album/... <br> Direct Images: img.kiwi/image/... <br> User Profile: img.kiwi/#USER# <br> All User Albums: img.kiwi/#USER#/albums                                                                                      |
-| jpg.church<br/>jpg.fish<br/>jpg.fishing | Albums: jpg.church/album/... <br> Direct Images: jpg.church/image/... <br> User Profile: jpg.church/#USER# <br> All User Albums: jpg.church/#USER#/albums                                                                              |
+| jpg.church<br/>jpg.fish<br/>jpg.fishing<br/>jpg.pet | Albums: jpg.church/album/... <br> Direct Images: jpg.church/image/... <br> User Profile: jpg.church/#USER# <br> All User Albums: jpg.church/#USER#/albums                                                                              |
 | LoveFap                                 | Albums: lovefap.com/a/... <br> Direct Images: s*.lovefap.com/content/photos/... <br> Videos: lovefap.com/video/...                                                                                                                     |
 | NSFW.XXX                                | Profile: nsfw.xxx/user/... <br> Post: nsfw.xxx/post/...                                                                                                                                                                                |
 | PimpAndHost                             | Albums: pimpandhost.com/album/... <br> Single Files: pimpandhost.com/image/...                                                                                                                                                         |
 | PixelDrain                              | Albums: Pixeldrain.com/l/... <br> Single Files: Pixeldrain.com/u/...                                                                                                                                                                   |
 | Pixl                                    | Albums: pixl.li/album/... <br> Direct Images: pixl.li/image/...  <br> User Profile: pixl.li/#USER# <br> All User Albums: pixl.li/#USER#/albums                                                                                         |
 | Postimg.cc                              | Albums: postimg.cc/gallery/... <br> Direct Images: postimg.cc/...                                                                                                                                                                      |
 | NudoStar                                | Thread: nudostar.com/forum/threads/...  <br> Continue from (will download this post and after): nudostar.com/forum/threads/...post-NUMBER                                                                                              |
```

#### html2text {}

```diff
@@ -50,15 +50,16 @@
 hgamecg.com/.../index.html | | ImgBox | Albums: imgbox.com/g/...
 Direct Images: images#.imgbox.com/...
 Single Files: imgbox.com/... | | IMG.Kiwi | Albums: img.kiwi/album/...
 Direct Images: img.kiwi/image/...
 User Profile: img.kiwi/#USER#
 All User Albums: img.kiwi/#USER#/albums | | jpg.church
 jpg.fish
-jpg.fishing | Albums: jpg.church/album/...
+jpg.fishing
+jpg.pet | Albums: jpg.church/album/...
 Direct Images: jpg.church/image/...
 User Profile: jpg.church/#USER#
 All User Albums: jpg.church/#USER#/albums | | LoveFap | Albums: lovefap.com/
 a/...
 Direct Images: s*.lovefap.com/content/photos/...
 Videos: lovefap.com/video/... | | NSFW.XXX | Profile: nsfw.xxx/user/...
 Post: nsfw.xxx/post/... | | PimpAndHost | Albums: pimpandhost.com/album/...
```

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/base_functions/data_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,12 +232,12 @@
 
 @dataclass
 class SkipData:
     """The allows optoins for domains to skip when scraping"""
     supported_hosts: ClassVar[Tuple[str, ...]] = ("anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop",
                                                   "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gofile",
                                                   "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish",
-                                                  "jpg.fishing", "gallery.deltaporno.com", "kemono.party",
+                                                  "jpg.fishing", "jpg.pet", "gallery.deltaporno.com", "kemono.party",
                                                   "lovefap", "nsfw.xxx", "pimpandhost", "pixeldrain", "pixl.li",
                                                   "postimg", "saint", "nudostar", "simpcity", "socialmediagirls",
                                                   "xbunker", "xbunkr")
     sites: List[str]
```

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.55/cyberdrop_dl/scraper/Scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,19 +85,20 @@
         self.xbunker_semaphore = asyncio.Semaphore(1)
 
         self.mapping = {"anonfiles": self.Anonfiles, "bayfiles": self.Anonfiles, "xbunkr": self.XBunkr,
                         "bunkr": self.Bunkr, "cyberdrop": self.Cyberdrop, "cyberfile": self.CyberFile,
                         "erome": self.Erome, "fapello": self.Fapello, "gfycat": self.Gfycat, "gofile": self.GoFile,
                         "hgamecg": self.HGameCG, "imgbox": self.ImgBox, "pixeldrain": self.PixelDrain,
                         "postimg": self.PostImg, "saint": self.Saint, "img.kiwi": self.ShareX,
-                        "jpg.church": self.ShareX, "jpg.fish": self.ShareX, "pixl.li": self.ShareX,
-                        "nsfw.xxx": self.NSFW_XXX, "pimpandhost": self.PimpAndHost, "lovefap": self.LoveFap,
-                        "e-hentai": self.EHentai, "gallery.deltaporno": self.ShareX, "vk.com": self.vk_redirect,
-                        "coomer.party": self.Coomeno, "kemono.party": self.Coomeno, "nudostar": self.Xenforo,
-                        "simpcity": self.Xenforo, "socialmediagirls": self.Xenforo, "xbunker": self.Xenforo}
+                        "jpg.church": self.ShareX, "jpg.fish": self.ShareX, "jpg.pet": self.ShareX,
+                        "pixl.li": self.ShareX, "nsfw.xxx": self.NSFW_XXX, "pimpandhost": self.PimpAndHost,
+                        "lovefap": self.LoveFap, "e-hentai": self.EHentai, "gallery.deltaporno": self.ShareX,
+                        "vk.com": self.vk_redirect, "coomer.party": self.Coomeno, "kemono.party": self.Coomeno,
+                        "nudostar": self.Xenforo, "simpcity": self.Xenforo, "socialmediagirls": self.Xenforo,
+                        "xbunker": self.Xenforo}
 
     async def _handle_album_additions(self, domain: str, album_obj: AlbumItem, title=None) -> None:
         if title:
             await album_obj.append_title(title)
             await self.Forums.add_album_to_thread(title, domain, album_obj)
         else:
             await self.Cascade.add_album(domain, album_obj.title, album_obj)
```

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.55/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.53
+Version: 4.2.55
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -56,15 +56,15 @@
 | Fapello                                 | Models: fapello.com/...                                                                                                                                                                                                                |
 | Gallery.DeltaPorno.com                  | Albums: Gallery.DeltaPorno.com/album/... <br> Direct Images: Gallery.DeltaPorno.com/image/... <br> User Profile: Gallery.DeltaPorno.com/#USER# <br> All User Albums: Gallery.DeltaPorno.com/#USER#/albums                              |
 | GoFile                                  | Albums: gofile.io/d/...                                                                                                                                                                                                                |
 | Gfycat                                  | Gif: gfycat.com/...                                                                                                                                                                                                                    |
 | HGameCG                                 | Albums: hgamecg.com/.../index.html                                                                                                                                                                                                     |
 | ImgBox                                  | Albums: imgbox.com/g/... <br> Direct Images: images#.imgbox.com/... <br> Single Files: imgbox.com/...                                                                                                                                  |
 | IMG.Kiwi                                | Albums: img.kiwi/album/... <br> Direct Images: img.kiwi/image/... <br> User Profile: img.kiwi/#USER# <br> All User Albums: img.kiwi/#USER#/albums                                                                                      |
-| jpg.church<br/>jpg.fish<br/>jpg.fishing | Albums: jpg.church/album/... <br> Direct Images: jpg.church/image/... <br> User Profile: jpg.church/#USER# <br> All User Albums: jpg.church/#USER#/albums                                                                              |
+| jpg.church<br/>jpg.fish<br/>jpg.fishing<br/>jpg.pet | Albums: jpg.church/album/... <br> Direct Images: jpg.church/image/... <br> User Profile: jpg.church/#USER# <br> All User Albums: jpg.church/#USER#/albums                                                                              |
 | LoveFap                                 | Albums: lovefap.com/a/... <br> Direct Images: s*.lovefap.com/content/photos/... <br> Videos: lovefap.com/video/...                                                                                                                     |
 | NSFW.XXX                                | Profile: nsfw.xxx/user/... <br> Post: nsfw.xxx/post/...                                                                                                                                                                                |
 | PimpAndHost                             | Albums: pimpandhost.com/album/... <br> Single Files: pimpandhost.com/image/...                                                                                                                                                         |
 | PixelDrain                              | Albums: Pixeldrain.com/l/... <br> Single Files: Pixeldrain.com/u/...                                                                                                                                                                   |
 | Pixl                                    | Albums: pixl.li/album/... <br> Direct Images: pixl.li/image/...  <br> User Profile: pixl.li/#USER# <br> All User Albums: pixl.li/#USER#/albums                                                                                         |
 | Postimg.cc                              | Albums: postimg.cc/gallery/... <br> Direct Images: postimg.cc/...                                                                                                                                                                      |
 | NudoStar                                | Thread: nudostar.com/forum/threads/...  <br> Continue from (will download this post and after): nudostar.com/forum/threads/...post-NUMBER                                                                                              |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.53 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.55 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
@@ -56,15 +56,16 @@
 hgamecg.com/.../index.html | | ImgBox | Albums: imgbox.com/g/...
 Direct Images: images#.imgbox.com/...
 Single Files: imgbox.com/... | | IMG.Kiwi | Albums: img.kiwi/album/...
 Direct Images: img.kiwi/image/...
 User Profile: img.kiwi/#USER#
 All User Albums: img.kiwi/#USER#/albums | | jpg.church
 jpg.fish
-jpg.fishing | Albums: jpg.church/album/...
+jpg.fishing
+jpg.pet | Albums: jpg.church/album/...
 Direct Images: jpg.church/image/...
 User Profile: jpg.church/#USER#
 All User Albums: jpg.church/#USER#/albums | | LoveFap | Albums: lovefap.com/
 a/...
 Direct Images: s*.lovefap.com/content/photos/...
 Videos: lovefap.com/video/... | | NSFW.XXX | Profile: nsfw.xxx/user/...
 Post: nsfw.xxx/post/... | | PimpAndHost | Albums: pimpandhost.com/album/...
```

### Comparing `cyberdrop-dl-4.2.53/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.55/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.53/setup.cfg` & `cyberdrop-dl-4.2.55/setup.cfg`

 * *Files identical despite different names*

