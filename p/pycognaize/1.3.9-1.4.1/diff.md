# Comparing `tmp/pycognaize-1.3.9.tar.gz` & `tmp/pycognaize-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycognaize-1.3.9.tar", last modified: Thu Mar 30 15:40:49 2023, max compression
+gzip compressed data, was "pycognaize-1.4.1.tar", last modified: Tue May 30 10:48:20 2023, max compression
```

## Comparing `pycognaize-1.3.9.tar` & `pycognaize-1.4.1.tar`

### file list

```diff
@@ -1,58 +1,68 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-30 15:40:49.360445 pycognaize-1.3.9/
--rw-rw-r--   0 david     (1000) david     (1000)    30728 2023-03-30 15:40:15.000000 pycognaize-1.3.9/CHANGELOG.md
--rw-rw-r--   0 david     (1000) david     (1000)    35137 2023-01-20 10:59:34.000000 pycognaize-1.3.9/LICENSE.txt
--rw-rw-r--   0 david     (1000) david     (1000)    32496 2023-03-30 15:40:49.360445 pycognaize-1.3.9/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     1310 2023-02-10 17:58:58.000000 pycognaize-1.3.9/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-30 15:40:49.360445 pycognaize-1.3.9/pycognaize/
--rw-rw-r--   0 david     (1000) david     (1000)      361 2023-03-30 15:40:15.000000 pycognaize-1.3.9/pycognaize/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2168 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/clidriver.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-30 15:40:49.360445 pycognaize-1.3.9/pycognaize/common/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/common/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2359 2023-03-09 16:00:53.000000 pycognaize-1.3.9/pycognaize/common/confidence.py
--rw-rw-r--   0 david     (1000) david     (1000)     1650 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/common/decorators.py
--rw-rw-r--   0 david     (1000) david     (1000)     4893 2023-03-11 19:46:36.000000 pycognaize-1.3.9/pycognaize/common/enums.py
--rw-rw-r--   0 david     (1000) david     (1000)      394 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/common/exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)     1750 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/common/field_collection.py
--rw-rw-r--   0 david     (1000) david     (1000)     2352 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/common/lazy_dict.py
--rw-rw-r--   0 david     (1000) david     (1000)     2096 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/common/lazy_group_dict.py
--rw-rw-r--   0 david     (1000) david     (1000)     6826 2023-02-10 17:58:58.000000 pycognaize-1.3.9/pycognaize/common/numeric_parser.py
--rw-rw-r--   0 david     (1000) david     (1000)     3899 2023-02-21 11:37:37.000000 pycognaize-1.3.9/pycognaize/common/table_utils.py
--rw-rw-r--   0 david     (1000) david     (1000)    21720 2023-02-21 11:37:37.000000 pycognaize-1.3.9/pycognaize/common/utils.py
--rw-rw-r--   0 david     (1000) david     (1000)      285 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/common/white_pixel.jpeg
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-30 15:40:49.360445 pycognaize-1.3.9/pycognaize/document/
--rw-rw-r--   0 david     (1000) david     (1000)      129 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/document/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    22604 2023-02-21 11:37:37.000000 pycognaize-1.3.9/pycognaize/document/document.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-30 15:40:49.360445 pycognaize-1.3.9/pycognaize/document/field/
--rw-rw-r--   0 david     (1000) david     (1000)      606 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/document/field/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3049 2023-02-21 11:37:37.000000 pycognaize-1.3.9/pycognaize/document/field/area_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     2793 2023-02-10 17:58:58.000000 pycognaize-1.3.9/pycognaize/document/field/date_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     2718 2023-02-10 17:58:58.000000 pycognaize-1.3.9/pycognaize/document/field/field.py
--rw-rw-r--   0 david     (1000) david     (1000)     3520 2023-02-21 11:37:37.000000 pycognaize-1.3.9/pycognaize/document/field/numeric_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     2928 2023-02-10 17:58:58.000000 pycognaize-1.3.9/pycognaize/document/field/section_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     2486 2023-02-10 17:58:58.000000 pycognaize-1.3.9/pycognaize/document/field/span_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     5201 2023-02-21 11:37:37.000000 pycognaize-1.3.9/pycognaize/document/field/table_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     3728 2023-02-21 11:37:37.000000 pycognaize-1.3.9/pycognaize/document/field/text_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     2882 2023-03-30 15:40:15.000000 pycognaize-1.3.9/pycognaize/document/html_info.py
--rw-rw-r--   0 david     (1000) david     (1000)    21421 2023-02-10 17:58:58.000000 pycognaize-1.3.9/pycognaize/document/page.py
--rw-rw-r--   0 david     (1000) david     (1000)     3098 2023-02-21 09:10:53.000000 pycognaize-1.3.9/pycognaize/document/snapshot.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-30 15:40:49.360445 pycognaize-1.3.9/pycognaize/document/tag/
--rw-rw-r--   0 david     (1000) david     (1000)      116 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/document/tag/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3449 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/document/tag/cell.py
--rw-rw-r--   0 david     (1000) david     (1000)     6090 2023-02-10 17:58:58.000000 pycognaize-1.3.9/pycognaize/document/tag/extraction_tag.py
--rw-rw-r--   0 david     (1000) david     (1000)    13097 2023-02-21 11:37:37.000000 pycognaize-1.3.9/pycognaize/document/tag/html_tag.py
--rw-rw-r--   0 david     (1000) david     (1000)     2091 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/document/tag/section_tag.py
--rw-rw-r--   0 david     (1000) david     (1000)     1794 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/document/tag/span_tag.py
--rw-rw-r--   0 david     (1000) david     (1000)     8858 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/document/tag/table_tag.py
--rw-rw-r--   0 david     (1000) david     (1000)    14977 2023-02-21 11:37:51.000000 pycognaize-1.3.9/pycognaize/document/tag/tag.py
--rw-rw-r--   0 david     (1000) david     (1000)     2863 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/index.py
--rw-rw-r--   0 david     (1000) david     (1000)     3866 2023-02-21 09:10:53.000000 pycognaize-1.3.9/pycognaize/login.py
--rw-rw-r--   0 david     (1000) david     (1000)    21976 2023-03-28 12:10:24.000000 pycognaize-1.3.9/pycognaize/model.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-30 15:40:49.360445 pycognaize-1.3.9/pycognaize.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)    32496 2023-03-30 15:40:49.000000 pycognaize-1.3.9/pycognaize.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     1562 2023-03-30 15:40:49.000000 pycognaize-1.3.9/pycognaize.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-03-30 15:40:49.000000 pycognaize-1.3.9/pycognaize.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       47 2023-03-30 15:40:49.000000 pycognaize-1.3.9/pycognaize.egg-info/entry_points.txt
--rw-rw-r--   0 david     (1000) david     (1000)      147 2023-03-30 15:40:49.000000 pycognaize-1.3.9/pycognaize.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       11 2023-03-30 15:40:49.000000 pycognaize-1.3.9/pycognaize.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)      881 2023-03-30 15:40:49.360445 pycognaize-1.3.9/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)      999 2023-01-20 10:59:34.000000 pycognaize-1.3.9/setup.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-30 10:48:20.812630 pycognaize-1.4.1/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    31498 2023-05-30 10:47:37.000000 pycognaize-1.4.1/CHANGELOG.md
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    35137 2022-11-15 12:53:10.000000 pycognaize-1.4.1/LICENSE.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    33266 2023-05-30 10:48:20.812630 pycognaize-1.4.1/PKG-INFO
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1310 2023-02-20 13:34:43.000000 pycognaize-1.4.1/README.md
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-30 10:48:20.808629 pycognaize-1.4.1/pycognaize/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      361 2023-05-30 10:47:37.000000 pycognaize-1.4.1/pycognaize/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      210 2023-04-28 11:57:35.000000 pycognaize-1.4.1/pycognaize/cli.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2168 2023-01-11 08:15:39.000000 pycognaize-1.4.1/pycognaize/clidriver.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-30 10:48:20.808629 pycognaize-1.4.1/pycognaize/common/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-11-15 12:53:10.000000 pycognaize-1.4.1/pycognaize/common/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      968 2023-05-30 10:47:37.000000 pycognaize-1.4.1/pycognaize/common/classification_labels.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2359 2023-03-07 12:26:57.000000 pycognaize-1.4.1/pycognaize/common/confidence.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1650 2022-11-15 12:53:10.000000 pycognaize-1.4.1/pycognaize/common/decorators.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5138 2023-05-30 10:47:37.000000 pycognaize-1.4.1/pycognaize/common/enums.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      394 2022-12-06 11:01:27.000000 pycognaize-1.4.1/pycognaize/common/exceptions.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1750 2022-12-06 11:01:27.000000 pycognaize-1.4.1/pycognaize/common/field_collection.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2352 2022-12-06 11:01:27.000000 pycognaize-1.4.1/pycognaize/common/lazy_dict.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2096 2022-12-06 11:01:27.000000 pycognaize-1.4.1/pycognaize/common/lazy_group_dict.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     6826 2023-01-26 10:20:57.000000 pycognaize-1.4.1/pycognaize/common/numeric_parser.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3903 2023-05-04 16:18:45.000000 pycognaize-1.4.1/pycognaize/common/table_utils.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    22777 2023-04-28 14:56:56.000000 pycognaize-1.4.1/pycognaize/common/utils.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      285 2022-11-15 12:53:10.000000 pycognaize-1.4.1/pycognaize/common/white_pixel.jpeg
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-30 10:48:20.812630 pycognaize-1.4.1/pycognaize/document/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      129 2022-11-15 12:53:10.000000 pycognaize-1.4.1/pycognaize/document/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    23603 2023-05-30 10:47:37.000000 pycognaize-1.4.1/pycognaize/document/document.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-30 10:48:20.812630 pycognaize-1.4.1/pycognaize/document/field/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      674 2023-05-30 10:47:37.000000 pycognaize-1.4.1/pycognaize/document/field/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3367 2023-05-30 10:47:37.000000 pycognaize-1.4.1/pycognaize/document/field/area_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2818 2023-05-30 10:47:37.000000 pycognaize-1.4.1/pycognaize/document/field/date_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3200 2023-05-30 10:47:37.000000 pycognaize-1.4.1/pycognaize/document/field/field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3988 2023-05-30 10:47:37.000000 pycognaize-1.4.1/pycognaize/document/field/link_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3566 2023-05-30 10:47:37.000000 pycognaize-1.4.1/pycognaize/document/field/numeric_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     4202 2023-05-30 10:47:37.000000 pycognaize-1.4.1/pycognaize/document/field/section_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2825 2023-05-30 10:47:37.000000 pycognaize-1.4.1/pycognaize/document/field/span_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5242 2023-05-30 10:47:37.000000 pycognaize-1.4.1/pycognaize/document/field/table_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     4051 2023-05-30 10:47:37.000000 pycognaize-1.4.1/pycognaize/document/field/text_field.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2904 2023-05-30 10:47:37.000000 pycognaize-1.4.1/pycognaize/document/html_info.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    21421 2023-02-20 13:34:43.000000 pycognaize-1.4.1/pycognaize/document/page.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3349 2023-04-28 14:56:56.000000 pycognaize-1.4.1/pycognaize/document/snapshot.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-30 10:48:20.812630 pycognaize-1.4.1/pycognaize/document/tag/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      116 2022-11-15 12:53:10.000000 pycognaize-1.4.1/pycognaize/document/tag/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3449 2022-11-15 12:53:10.000000 pycognaize-1.4.1/pycognaize/document/tag/cell.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     6090 2023-05-29 14:26:12.000000 pycognaize-1.4.1/pycognaize/document/tag/extraction_tag.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    14209 2023-05-04 16:18:45.000000 pycognaize-1.4.1/pycognaize/document/tag/html_tag.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2657 2023-05-30 10:47:37.000000 pycognaize-1.4.1/pycognaize/document/tag/section_tag.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1794 2022-12-06 11:01:27.000000 pycognaize-1.4.1/pycognaize/document/tag/span_tag.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     8858 2023-01-27 15:01:05.000000 pycognaize-1.4.1/pycognaize/document/tag/table_tag.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    14977 2023-05-29 14:03:01.000000 pycognaize-1.4.1/pycognaize/document/tag/tag.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2863 2022-11-15 12:53:10.000000 pycognaize-1.4.1/pycognaize/index.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3866 2023-05-29 08:03:29.000000 pycognaize-1.4.1/pycognaize/login.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    21992 2023-05-04 16:18:45.000000 pycognaize-1.4.1/pycognaize/model.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-30 10:48:20.812630 pycognaize-1.4.1/pycognaize/model_registry/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      133 2023-04-28 11:57:35.000000 pycognaize-1.4.1/pycognaize/model_registry/__init__.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-30 10:48:20.812630 pycognaize-1.4.1/pycognaize/model_registry/db/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2023-04-28 11:57:35.000000 pycognaize-1.4.1/pycognaize/model_registry/db/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      787 2023-04-28 11:57:35.000000 pycognaize-1.4.1/pycognaize/model_registry/db/models.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      598 2023-04-28 11:57:35.000000 pycognaize-1.4.1/pycognaize/model_registry/login.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     4687 2023-04-28 11:57:35.000000 pycognaize-1.4.1/pycognaize/model_registry/submit.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-30 10:48:20.808629 pycognaize-1.4.1/pycognaize.egg-info/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    33266 2023-05-30 10:48:20.000000 pycognaize-1.4.1/pycognaize.egg-info/PKG-INFO
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1852 2023-05-30 10:48:20.000000 pycognaize-1.4.1/pycognaize.egg-info/SOURCES.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        1 2023-05-30 10:48:20.000000 pycognaize-1.4.1/pycognaize.egg-info/dependency_links.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       53 2023-05-30 10:48:20.000000 pycognaize-1.4.1/pycognaize.egg-info/entry_points.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      160 2023-05-30 10:48:20.000000 pycognaize-1.4.1/pycognaize.egg-info/requires.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       11 2023-05-30 10:48:20.000000 pycognaize-1.4.1/pycognaize.egg-info/top_level.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      896 2023-05-30 10:48:20.816630 pycognaize-1.4.1/setup.cfg
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1005 2023-04-28 11:57:35.000000 pycognaize-1.4.1/setup.py
```

### Comparing `pycognaize-1.3.9/CHANGELOG.md` & `pycognaize-1.4.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,39 @@
 # Changelog
 
+## [1.4]
+
+### [1.4.1] - 2023-05-29
+- Add section field and section tag functionality
+
+
+### [1.4.0] - 2023-05-25
+- Add classification labels functionality to ``Field`` objects
+
 ## [1.3]
 
+### [1.3.14] - 2023-05-10
+- Add LinkField object
+- Add returning group name in to_dict functionality of Field object 
+
+### [1.3.13] - 2023-05-01
+- Add exclude folders option for ``lisdir`` in ``html_info``
+- Update version cloudstorageio >= 1.2.8
+### [1.3.12] - 2023-05-01
+- Rename HTMLTag to HTMLTagABC
+- Rename TDTag to HTMLTag
+- Handle out of table tags in XBRL
+
+### [1.3.11] - 2023-04-28
+- Add interface to create directory summary hashes
+- Add automatic snapshot hash creation for ``snapshot.download``
+
+### [1.3.10] - 2023-03-31
+- Add login command and code for submit to model registry
+
 ### [1.3.9] - 2023-03-30
 - Refactor HTML._validate_path() to include try-except block
 
 ### [1.3.8] - 2023-03-28
 - Improve html file path validation by adding a new check
 in HTML._validate_path()
```

### Comparing `pycognaize-1.3.9/LICENSE.txt` & `pycognaize-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.9/PKG-INFO` & `pycognaize-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycognaize
-Version: 1.3.9
+Version: 1.4.1
 Home-page: https://github.com/cognaize/pycognaize
 Author: Cognaize
 License: Apache License 2.0
 Project-URL: Source, https://github.com/cognaize/pycognaize
 Project-URL: Reference, https://pycognaize.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/cognaize/pycognaize/blob/master/CHANGELOG.md
 Requires-Python: >= 3.7
@@ -43,16 +43,44 @@
 ```
 
 Have a look at the [quick tutorial](http://pycognaize-docs.com.s3-website.us-east-2.amazonaws.com/tutorials/quick_tutorial.html) 
 for understanding main concepts of the SDK.
 
 # Changelog
 
+## [1.4]
+
+### [1.4.1] - 2023-05-29
+- Add section field and section tag functionality
+
+
+### [1.4.0] - 2023-05-25
+- Add classification labels functionality to ``Field`` objects
+
 ## [1.3]
 
+### [1.3.14] - 2023-05-10
+- Add LinkField object
+- Add returning group name in to_dict functionality of Field object 
+
+### [1.3.13] - 2023-05-01
+- Add exclude folders option for ``lisdir`` in ``html_info``
+- Update version cloudstorageio >= 1.2.8
+### [1.3.12] - 2023-05-01
+- Rename HTMLTag to HTMLTagABC
+- Rename TDTag to HTMLTag
+- Handle out of table tags in XBRL
+
+### [1.3.11] - 2023-04-28
+- Add interface to create directory summary hashes
+- Add automatic snapshot hash creation for ``snapshot.download``
+
+### [1.3.10] - 2023-03-31
+- Add login command and code for submit to model registry
+
 ### [1.3.9] - 2023-03-30
 - Refactor HTML._validate_path() to include try-except block
 
 ### [1.3.8] - 2023-03-28
 - Improve html file path validation by adding a new check
 in HTML._validate_path()
```

### Comparing `pycognaize-1.3.9/README.md` & `pycognaize-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.9/pycognaize/clidriver.py` & `pycognaize-1.4.1/pycognaize/clidriver.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.9/pycognaize/common/confidence.py` & `pycognaize-1.4.1/pycognaize/common/confidence.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.9/pycognaize/common/decorators.py` & `pycognaize-1.4.1/pycognaize/common/decorators.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.9/pycognaize/common/enums.py` & `pycognaize-1.4.1/pycognaize/common/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import enum
 
 ID = "_id"
+START = 'start'
+END = 'end'
+HASH_FILE = "document_summary_hash.md5"
 
 IMG_EXTENSION = 'jpeg'
 OCR_DATA_EXTENSION = 'json'
 SNAPSHOT_EXTENSION = 'pickle'
 
 
 class FieldDataTypeEnum(enum.Enum):
@@ -60,14 +63,15 @@
     template = 'template'
     fields = 'fields'
     tags = 'tags'
     pages = 'pages'
     name = 'name'
     section = 'section'
     field_type = 'fieldType'
+    field_category = 'fieldCategories'
     field_id = '_id'
     src_field_id = "srcFieldId"
     page = 'page'
     src = 'src'
     page_src = 'src'
 
 
@@ -83,15 +87,17 @@
     order = 'order'
     repeatable = 'repeatable'
     required = 'required'
     src_field_id = 'srcFieldId'
     tags = 'tags'
     template_id = 'templateId'
     value = 'value'
+    ocr_value = 'ocrValue'
     repeat_parent = 'repeatParent'
+    section = 'section'
 
 
 class IqTagKeyEnum(enum.Enum):
     value = 'value'
     has_valid_value = 'hasValidValue'
     top = 'top'
     left = 'left'
@@ -108,17 +114,19 @@
     page = 'page'
     src = 'src'
 
 
 class IqDataTypesEnum(enum.Enum):
     table = 'table'
     text = 'text'
+    section = 'section'
     date = 'date'
     number = 'number'
     area = 'area'
+    link = 'link'
 
 
 class IqRecipeEnum(enum.Enum):
     id = '_id'
     field_id = 'fieldId'
     name = 'name'
     templates = 'templates'
@@ -180,14 +188,16 @@
     ids = 'ids'
     row_index = 'rowIndex'
     col_index = 'colIndex'
     tag_id = 'tagId'
     ocr_value = 'ocrValue'
     value = 'value'
     is_table = 'isTable'
+    html = 'html'
+    parent_id = 'parentId'
 
 
 class XBRLCellEnum(enum.Enum):
     id = 'id'
     source = 'source'
     ids = 'ids'
     html_id = 'id'
```

### Comparing `pycognaize-1.3.9/pycognaize/common/field_collection.py` & `pycognaize-1.4.1/pycognaize/common/field_collection.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.9/pycognaize/common/lazy_dict.py` & `pycognaize-1.4.1/pycognaize/common/lazy_dict.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.9/pycognaize/common/lazy_group_dict.py` & `pycognaize-1.4.1/pycognaize/common/lazy_group_dict.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.9/pycognaize/common/numeric_parser.py` & `pycognaize-1.4.1/pycognaize/common/numeric_parser.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.9/pycognaize/common/table_utils.py` & `pycognaize-1.4.1/pycognaize/common/table_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from itertools import groupby
 from typing import Optional
 
-from pycognaize.document.tag.html_tag import HTMLTableTag, TDTag
+from pycognaize.document.tag.html_tag import HTMLTableTag, HTMLTag
 
 
 def filter_out_invalid_tables(tables):
     """
     Filters tables that have tag.
     """
     valid_tables = []
@@ -67,15 +67,15 @@
     :param threshold: intersection threshold
     """
     tables_dict = {}
     valid_tables = filter_out_invalid_tables(tables)
     if not valid_tables:
         return tables_dict
     if all(isinstance(table.tags[0], HTMLTableTag) or
-           isinstance(table.tags[0], TDTag) for table in valid_tables):
+           isinstance(table.tags[0], HTMLTag) for table in valid_tables):
         if not all_tables:
             logging.error('Missing argument: list of all table fields')
             return tables_dict
         all_valid_tables = filter_out_invalid_tables(all_tables)
         tables_html_id_idx_mapping = {
             table.tags[0].html_id: (idx, 0)
             for idx, table in enumerate(all_valid_tables, start=1)}
```

### Comparing `pycognaize-1.3.9/pycognaize/common/utils.py` & `pycognaize-1.4.1/pycognaize/common/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import io
 import os
+import pathlib
 import re
+
+import hashlib
 import numpy as np
 import bson
 import logging
 
 from PIL import Image
 from itertools import groupby
 from typing import Union, List, Optional, Iterable, Dict
@@ -624,7 +627,42 @@
         ci_instance = CloudInterface(
             aws_access_key_id=login_instance.aws_access_key,
             aws_secret_access_key=login_instance.aws_secret_access_key,
             aws_session_token=login_instance.aws_session_token)
     else:
         ci_instance = CloudInterface()
     return ci_instance
+
+
+def directory_summary_hash(dirname: str):
+    """ Computes hash of directory summary"""
+    hash_func = hashlib.md5
+
+    if not os.path.isdir(dirname):
+        raise TypeError("{} is not a directory.".format(dirname))
+
+    hash_values = []
+    path = pathlib.Path(dirname)
+    directories = sorted([str(i) for i in path.iterdir() if i.is_dir()])
+    for dir_name in directories:
+        hash_values.append(_dirhash(os.path.join(dirname, dir_name),
+                                    hash_func))
+    return _reduce_hash(hash_values, hash_func)
+
+
+def _dirhash(filepath, hash_function):
+    """ Computes hash of dir"""
+    hasher = hash_function()
+
+    if not os.path.exists(filepath):
+        return hasher.hexdigest()
+    hasher.update(filepath.encode("utf-8"))
+
+    return hasher.hexdigest()
+
+
+def _reduce_hash(hashlist, hash_function):
+    """ Computes hash of hashlist"""
+    hasher = hash_function()
+    for hash_value in sorted(hashlist):
+        hasher.update(hash_value.encode("utf-8"))
+    return hasher.hexdigest()
```

### Comparing `pycognaize-1.3.9/pycognaize/document/document.py` & `pycognaize-1.4.1/pycognaize/document/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from collections import OrderedDict
 from typing import Dict, List, Tuple, Any, Optional, Callable, Union
 
 import fitz
 import pandas as pd
 from fitz.utils import getColor, getColorList
 
+from pycognaize.common.classification_labels import ClassificationLabels
 from pycognaize.document.html_info import HTML
 from pycognaize.login import Login
 from pycognaize.common.enums import IqDocumentKeysEnum, FieldTypeEnum
 from pycognaize.common.field_collection import FieldCollection
 from pycognaize.common.utils import cloud_interface_login
 from pycognaize.document.field import FieldMapping, TableField
 from pycognaize.document.field.field import Field
@@ -29,20 +30,21 @@
     """Definition of input and output for a single document,
      depending on a given model"""
 
     def __init__(self,
                  input_fields: 'FieldCollection[str, List[Field]]',
                  output_fields: 'FieldCollection[str, List[Field]]',
                  pages: Dict[int, Page],
+                 classification_labels: Dict[str, ClassificationLabels],
                  html_info: HTML,
                  metadata: Dict[str, Any]):
         self._login_instance = Login()
         self._metadata = metadata
         self._pages: Dict[int, Page] = pages if pages else None
-
+        self._classification_labels = classification_labels
         self._is_xbrl: bool = False
         self._html_info: HTML = html_info
         self._x: FieldCollection[str, List[Field]] = input_fields
         self._y: FieldCollection[str, List[Field]] = output_fields
 
     @property
     def x(self) -> 'FieldCollection[str, List[Field]]':
@@ -406,14 +408,15 @@
         """
         if not isinstance(raw, dict):
             raise TypeError(
                 f"Expected dict for 'raw' argument got {type(raw)} instead")
         metadata = raw['metadata']
         pages = OrderedDict()
         html_info = HTML(path=data_path, document_id=metadata['document_id'])
+        classification_labels = ClassificationLabels(raw)
         for page_n in range(1, metadata['numberOfPages'] + 1):
             if (
                     'pages' in raw
                     and str(page_n) in raw['pages']
                     and 'width' in raw['pages'][str(page_n)]
                     and 'height' in raw['pages'][str(page_n)]
             ):
@@ -428,29 +431,40 @@
                                  image_width=image_width,
                                  image_height=image_height)
         input_fields = FieldCollection(
             {name: [
                 FieldMapping[
                     field[IqDocumentKeysEnum.data_type.value]
                 ].value.construct_from_raw(raw=field, pages=pages,
-                                           html=html_info)
+                                           html=html_info,
+                                           labels=classification_labels.get(
+                                               field.get(
+                                                   IqDocumentKeysEnum.
+                                                   src_field_id.value, ''),
+                                               None))
                 for field in fields]
              for name, fields in raw['input_fields'].items()})
         output_fields = FieldCollection(
             {name: [
                 FieldMapping[
                     field[IqDocumentKeysEnum.data_type.value]
                 ].value.construct_from_raw(raw=field, pages=pages,
-                                           html=html_info)
+                                           html=html_info,
+                                           labels=classification_labels.get(
+                                               field.get(
+                                                   IqDocumentKeysEnum.
+                                                   src_field_id.value, ''),
+                                               None))
                 for field in fields]
              for name, fields in raw['output_fields'].items()})
         return cls(input_fields=input_fields,
                    output_fields=output_fields,
                    pages=pages, html_info=html_info,
-                   metadata=metadata)
+                   metadata=metadata,
+                   classification_labels=classification_labels)
 
     def _collect_all_tags_for_fields(self,
                                      field_names: List[str],
                                      is_input_field: bool = True)\
             -> List[Union[BoxTag, LineTag]]:
         """Collect all tags of given field names from either input or output
             fields
```

### Comparing `pycognaize-1.3.9/pycognaize/document/field/__init__.py` & `pycognaize-1.4.1/pycognaize/document/field/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 from .field import Field
 from .date_field import DateField
 from .numeric_field import NumericField
 from .section_field import SectionField
 from .table_field import TableField
 from .text_field import TextField
 from .area_field import AreaField
+from .link_field import LinkField
 
 
 __all__ = ['Field', 'DateField', 'NumericField',
-           'TableField', 'TextField', 'AreaField', 'FieldMapping']
+           'TableField', 'TextField', 'AreaField', 'FieldMapping', 'LinkField']
 
 
 class FieldMapping(enum.Enum):
     """Mapping of IQ field type names and python classes"""
     number = NumericField
     date = DateField
     text = TextField
     table = TableField
     area = AreaField
     section = SectionField
+    link = LinkField
```

### Comparing `pycognaize-1.3.9/pycognaize/document/field/area_field.py` & `pycognaize-1.4.1/pycognaize/document/field/date_field.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,81 +1,79 @@
 import logging
-from typing import List, Optional, Dict, Type, Union
+from typing import List, Optional, Dict, Type
+
 
 from pycognaize.common.enums import (
     IqDocumentKeysEnum,
-    IqTagKeyEnum,
     ID,
     IqFieldKeyEnum,
     IqDataTypesEnum
 )
 from pycognaize.document.field import Field
 from pycognaize.document.html_info import HTML
 from pycognaize.document.tag import ExtractionTag
 from pycognaize.document.page import Page
-from pycognaize.document.tag.html_tag import HTMLTag
 
 
-class AreaField(Field):
-    """Base class for all pycognaize area fields"""
+class DateField(Field):
+    """Base class for all pycognaize date fields"""
     tag_class: Type[ExtractionTag] = ExtractionTag
 
     def __init__(self,
                  name: str,
                  value: str = '',
-                 tags: Optional[List[Union[ExtractionTag, HTMLTag]]] = None,
+                 tags: Optional[List[ExtractionTag]] = None,
                  field_id: Optional[str] = None,
                  group_key: str = None,
                  confidence: Optional[float] = -1.0,
                  group_name: str = None
                  ):
         super().__init__(name=name, value=value, tags=tags,
                          group_key=group_key, confidence=confidence,
                          group_name=group_name)
         self._field_id = field_id
-        if self.tags:
-            self._value = '; '.join([i.raw_value for i in self.tags])
-        elif isinstance(value, str):
-            self._value = value
-        else:
-            logging.warning(
-                f"Expected value of type str, received {type(value)},"
-                f" setting value to empty string")
-            self._value = ''
+        self._value = '; '.join([i.raw_value
+                                 for i in self.tags]) if self.tags else value
+
+    @property
+    def field_id(self):
+        return self._field_id
 
     @property
     def value(self):
         return self._value
 
     @classmethod
-    def construct_from_raw(cls, raw: dict, pages: Dict[int, Page],
-                           html: Optional[HTML] = None) -> 'AreaField':
-        """Create AreaField object from dictionary"""
+    def construct_from_raw(
+            cls, raw: dict, pages: Dict[int, Page],
+            html: Optional[HTML] = None,
+            labels=None) -> 'DateField':
+        """Create DateField object from dictionary"""
         tag_dicts: List[dict] = raw[IqDocumentKeysEnum.tags.value]
         tags = []
         for i in tag_dicts:
             try:
                 tags.append(cls.tag_class.construct_from_raw(
                     raw=i, page=pages[i['page']]))
             except Exception as e:
                 logging.debug(f"Failed creating tag for field {raw[ID]}: {e}")
         return cls(name=raw[IqDocumentKeysEnum.name.value],
-                   value=raw[IqTagKeyEnum.value.value],
+                   value=raw[IqFieldKeyEnum.value.value],
                    tags=tags,
                    field_id=str(raw[ID]),
                    group_key=raw.get(IqFieldKeyEnum.group_key.value, ''),
                    group_name=raw.get(IqFieldKeyEnum.group.value, '')
                    )
 
     def to_dict(self) -> dict:
-        """Converts AreaField object to dictionary"""
+        """Converts DateField object to dictionary"""
         field_dict = super().to_dict()
         field_dict[IqFieldKeyEnum.value.value] = self.value
         field_dict[ID] = self._field_id
-        field_dict[IqFieldKeyEnum.data_type.value] = IqDataTypesEnum.area.value
+        field_dict[IqFieldKeyEnum.data_type.value] = IqDataTypesEnum.date.value
         return field_dict
 
     def __repr__(self):
         return (f"<{self.__class__.__name__}: {self.name}:"
                 f" {'|'.join([i.raw_value for i in self.tags])}>")
 
     def __str__(self):
```

### Comparing `pycognaize-1.3.9/pycognaize/document/field/date_field.py` & `pycognaize-1.4.1/pycognaize/document/field/span_field.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,77 @@
+from typing import Optional, Dict, List, Type
 import logging
-from typing import List, Optional, Dict, Type
-
 
+from pycognaize.common.classification_labels import ClassificationLabels
 from pycognaize.common.enums import (
     IqDocumentKeysEnum,
     ID,
-    IqFieldKeyEnum,
-    IqDataTypesEnum
+    IqDataTypesEnum,
+    IqFieldKeyEnum
 )
+
 from pycognaize.document.field import Field
 from pycognaize.document.html_info import HTML
-from pycognaize.document.tag import ExtractionTag
+from pycognaize.document.tag.span_tag import SpanTag
 from pycognaize.document.page import Page
 
 
-class DateField(Field):
-    """Base class for all pycognaize date fields"""
-    tag_class: Type[ExtractionTag] = ExtractionTag
+class SpanField(Field):
+    """Base class for all pycognaize table fields"""
+    tag_class: Type[SpanTag] = SpanTag
 
     def __init__(self,
                  name: str,
-                 value: str = '',
-                 tags: Optional[List[ExtractionTag]] = None,
+                 tags: Optional[SpanTag] = None,
                  field_id: Optional[str] = None,
                  group_key: str = None,
                  confidence: Optional[float] = -1.0,
-                 group_name: str = None
+                 group_name: str = None,
+                 classification_labels: Optional[ClassificationLabels] = None
                  ):
-        super().__init__(name=name, value=value, tags=tags,
+        self._classification_labels = classification_labels
+        tags = [] if tags is None else tags
+        super().__init__(name=name, tags=tags,
                          group_key=group_key, confidence=confidence,
-                         group_name=group_name)
+                         group_name=group_name,)
         self._field_id = field_id
-        self._value = '; '.join([i.raw_value
-                                 for i in self.tags]) if self.tags else value
-
-    @property
-    def field_id(self):
-        return self._field_id
-
-    @property
-    def value(self):
-        return self._value
 
     @classmethod
-    def construct_from_raw(
-            cls, raw: dict, pages: Dict[int, Page],
-            html: Optional[HTML] = None) -> 'DateField':
-        """Create DateField object from dictionary"""
+    def construct_from_raw(cls, raw: dict, pages: Dict[int, Page],
+                           html: Optional[HTML] = None,
+                           labels: ClassificationLabels = None)\
+            -> 'SpanField':
+        """Create SnapField object from dictionary"""
         tag_dicts: List[dict] = raw[IqDocumentKeysEnum.tags.value]
         tags = []
         for i in tag_dicts:
             try:
                 tags.append(cls.tag_class.construct_from_raw(
                     raw=i, page=pages[i['page']]))
             except Exception as e:
                 logging.debug(f"Failed creating tag for field {raw[ID]}: {e}")
         return cls(name=raw[IqDocumentKeysEnum.name.value],
-                   value=raw[IqFieldKeyEnum.value.value],
-                   tags=tags,
+                   tags=tags[0] if tags else None,
                    field_id=str(raw[ID]),
                    group_key=raw.get(IqFieldKeyEnum.group_key.value, ''),
-                   group_name=raw.get(IqFieldKeyEnum.group.value, '')
+                   group_name=raw.get(IqFieldKeyEnum.group.value, ''),
+                   classification_labels=labels,
                    )
 
     def to_dict(self) -> dict:
-        """Converts DateField object to dictionary"""
+        """Converts TableField object to dictionary"""
         field_dict = super().to_dict()
-        field_dict[IqFieldKeyEnum.value.value] = self.value
         field_dict[ID] = self._field_id
-        field_dict[IqFieldKeyEnum.data_type.value] = IqDataTypesEnum.date.value
+        field_dict[
+            IqFieldKeyEnum.data_type.value] = IqDataTypesEnum.table.value
+        field_dict[IqFieldKeyEnum.value.value] = ''
         return field_dict
 
+    def order_tags(self):
+        """Order tags by pdf data"""
+        raise NotImplementedError
+
     def __repr__(self):
-        return (f"<{self.__class__.__name__}: {self.name}:"
-                f" {'|'.join([i.raw_value for i in self.tags])}>")
+        return f"<{self.__class__.__name__}: {self.name}>"
 
     def __str__(self):
-        return f"{'|'.join([i.raw_value for i in self.tags])}"
+        return self.__repr__()
```

### Comparing `pycognaize-1.3.9/pycognaize/document/field/field.py` & `pycognaize-1.4.1/pycognaize/document/field/field.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import abc
 
 from typing import List, Optional, Dict, Type
 
+from pycognaize.common.classification_labels import ClassificationLabels
 from pycognaize.common.enums import IqFieldKeyEnum
 from pycognaize.document.html_info import HTML
 from pycognaize.document.page import Page
 from pycognaize.document.tag.tag import BoxTag
 
 
 class Field(metaclass=abc.ABCMeta):
@@ -15,14 +16,15 @@
     def __init__(self, name: str,
                  value: str = '',
                  tags: Optional[List[BoxTag]] = None,
                  field_id: Optional[str] = None,
                  group_key: Optional[str] = None,
                  confidence: Optional[float] = -1.0,
                  group_name: Optional[str] = None,
+                 classification_labels: Optional[ClassificationLabels] = None
                  ):
         self._raw_value = value
         self._confidence = confidence
         if group_key is None:
             group_key = ''
         self._group_key = group_key
         if group_name is None:
@@ -31,14 +33,15 @@
         self._name = name
         if tags is None:
             self._tags = []
         else:
             self._tags = tags
         self._value = value
         self._field_id = field_id
+        self._classification_labels = classification_labels
 
     @property
     def raw_value(self):
         return self._raw_value
 
     @property
     def name(self):
@@ -60,14 +63,18 @@
     def value(self):
         return self._value
 
     @property
     def field_id(self):
         return self._field_id
 
+    @property
+    def classification_labels(self):
+        return self._classification_labels
+
     @group_key.setter
     def group_key(self, value):
         if not isinstance(value, str):
             raise TypeError(f"expected str, got {type(value)}")
         self._group_key = value
 
     @property
@@ -79,21 +86,25 @@
 
     def __str__(self):
         return f"{self.tags}"
 
     @classmethod
     @abc.abstractmethod
     def construct_from_raw(cls, raw: dict, pages: Dict[int, Page],
-                           html: Optional[HTML] = None) -> 'Field':
+                           html: Optional[HTML] = None,
+                           labels: ClassificationLabels = None)\
+            -> 'Field':
         """Use raw dictionary in order to recreate the Field python object"""
         pass
 
     @abc.abstractmethod
     def to_dict(self) -> dict:
         """Return a dictionary representing the field object"""
         field_dict = dict()
         field_dict[IqFieldKeyEnum.name.value] = self.name
         if self._group_key:
             field_dict[IqFieldKeyEnum.group_key.value] = self._group_key
+        if self._group_name:
+            field_dict[IqFieldKeyEnum.group.value] = self._group_name
         field_dict[IqFieldKeyEnum.tags.value] = [
             i.to_dict() for i in self.tags]
         return field_dict
```

### Comparing `pycognaize-1.3.9/pycognaize/document/field/numeric_field.py` & `pycognaize-1.4.1/pycognaize/document/field/numeric_field.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,21 +9,21 @@
     IqFieldKeyEnum,
     IqDataTypesEnum
 )
 from pycognaize.document.html_info import HTML
 from pycognaize.document.page import Page
 from pycognaize.document.field import Field
 from pycognaize.document.tag import ExtractionTag
-from pycognaize.document.tag.html_tag import TDTag
+from pycognaize.document.tag.html_tag import HTMLTag
 
 
 class NumericField(Field):
     """Base class for all pycognaize number fields"""
     tag_class: Type[ExtractionTag] = ExtractionTag
-    html_tag_class: Type[TDTag] = TDTag
+    html_tag_class: Type[HTMLTag] = HTMLTag
 
     def __init__(self,
                  name: str,
                  value: str = '',
                  tags: Optional[List[ExtractionTag]] = None,
                  field_id: Optional[str] = None,
                  group_key: str = None,
@@ -45,15 +45,16 @@
 
     @property
     def value(self):
         return self._value
 
     @classmethod
     def construct_from_raw(cls, raw: dict, pages: Dict[int, Page],
-                           html: Optional[HTML] = None) -> 'NumericField':
+                           html: Optional[HTML] = None,
+                           labels=None) -> 'NumericField':
         """Create NumericField object from dictionary"""
         tag_dicts: List[dict] = raw[IqDocumentKeysEnum.tags.value]
         tags = []
         for i in tag_dicts:
             try:
                 if pages:
                     tags.append(cls.tag_class.construct_from_raw(
```

### Comparing `pycognaize-1.3.9/pycognaize/document/field/section_field.py` & `pycognaize-1.4.1/pycognaize/document/field/area_field.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,87 @@
 import logging
-from typing import List, Optional, Dict, Type
-
+from typing import List, Optional, Dict, Type, Union
 
+from pycognaize.common.classification_labels import ClassificationLabels
 from pycognaize.common.enums import (
     IqDocumentKeysEnum,
+    IqTagKeyEnum,
     ID,
     IqFieldKeyEnum,
     IqDataTypesEnum
 )
+from pycognaize.document.field import Field
 from pycognaize.document.html_info import HTML
+from pycognaize.document.tag import ExtractionTag
 from pycognaize.document.page import Page
-from pycognaize.document.field import Field
-from pycognaize.document.tag.section_tag import SectionTag
+from pycognaize.document.tag.html_tag import HTMLTag
 
 
-class SectionField(Field):
-    """Base class for all pycognaize Section fields"""
-    tag_class: Type[SectionTag] = SectionTag
+class AreaField(Field):
+    """Base class for all pycognaize area fields"""
+    tag_class: Type[ExtractionTag] = ExtractionTag
 
     def __init__(self,
                  name: str,
-                 tags: Optional[List[SectionTag]] = None,
+                 value: str = '',
+                 tags: Optional[List[Union[ExtractionTag, HTMLTag]]] = None,
                  field_id: Optional[str] = None,
                  group_key: str = None,
                  confidence: Optional[float] = -1.0,
-                 group_name: str = None
+                 group_name: str = None,
+                 classification_labels: Optional[ClassificationLabels] = None
                  ):
-        """ Create a SectionField object
-
-        :param name: Name of the field
-        :param value: Value of the field
-            (left empty if values provided through tags)
-        :param tags: List of tag objects
-        :param field_id: The id of the field
-        """
-        super().__init__(name=name, tags=tags,
+        super().__init__(name=name, value=value, tags=tags,
                          group_key=group_key, confidence=confidence,
                          group_name=group_name)
         self._field_id = field_id
+        self._classification_labels = classification_labels
+        if self.tags:
+            self._value = '; '.join([i.raw_value for i in self.tags])
+        elif isinstance(value, str):
+            self._value = value
+        else:
+            logging.warning(
+                f"Expected value of type str, received {type(value)},"
+                f" setting value to empty string")
+            self._value = ''
+
+    @property
+    def value(self):
+        return self._value
 
     @classmethod
     def construct_from_raw(cls, raw: dict, pages: Dict[int, Page],
-                           html: Optional[HTML] = None) -> 'SectionField':
-        """Create SectionField object from dictionary"""
-        section_dict: List[dict] = raw[IqDocumentKeysEnum.tags.value]
+                           html: Optional[HTML] = None,
+                           labels: ClassificationLabels = None)\
+            -> 'AreaField':
+        """Create AreaField object from dictionary"""
+        tag_dicts: List[dict] = raw[IqDocumentKeysEnum.tags.value]
         tags = []
-        for i in section_dict:
-            for tag_type, tag_data in i[IqDocumentKeysEnum.
-                                        section.value].items():
-                try:
-                    tags.append(cls.tag_class.construct_from_raw(
-                                raw=tag_data,
-                                pages=pages,
-                                tag_type=tag_type))
-                except Exception as e:
-                    logging.debug(f"Failed creating tag"
-                                  f" for field {raw[ID]}: {e}")
+        for i in tag_dicts:
+            try:
+                tags.append(cls.tag_class.construct_from_raw(
+                    raw=i, page=pages[i['page']]))
+            except Exception as e:
+                logging.debug(f"Failed creating tag for field {raw[ID]}: {e}")
         return cls(name=raw[IqDocumentKeysEnum.name.value],
+                   value=raw[IqTagKeyEnum.value.value],
                    tags=tags,
                    field_id=str(raw[ID]),
                    group_key=raw.get(IqFieldKeyEnum.group_key.value, ''),
-                   group_name=raw.get(IqFieldKeyEnum.group.value, '')
-                   )
+                   group_name=raw.get(IqFieldKeyEnum.group.value, ''),
+                   classification_labels=labels)
 
     def to_dict(self) -> dict:
-        """Converts TextField object to dictionary"""
+        """Converts AreaField object to dictionary"""
         field_dict = super().to_dict()
-        field_dict[ID] = self._field_id
         field_dict[IqFieldKeyEnum.value.value] = self.value
-        field_dict[IqFieldKeyEnum.data_type.value] = IqDataTypesEnum.text.value
+        field_dict[ID] = self._field_id
+        field_dict[IqFieldKeyEnum.data_type.value] = IqDataTypesEnum.area.value
         return field_dict
 
     def __repr__(self):
-        return f"<{self.__class__.__name__}: {self.name}>"
+        return (f"<{self.__class__.__name__}: {self.name}:"
+                f" {'|'.join([i.raw_value for i in self.tags])}>")
 
     def __str__(self):
-        return f"<{self.__class__.__name__}: {self.name}>"
+        return f"{'|'.join([i.raw_value for i in self.tags])}"
```

### Comparing `pycognaize-1.3.9/pycognaize/document/field/span_field.py` & `pycognaize-1.4.1/pycognaize/document/field/link_field.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,108 @@
-from typing import Optional, Dict, List, Type
+"""
+| LinkField objects represent a single labeled pycognaize field.
+| The latter can have no tags, a single tag or multiple tags.
+
+>>> from pycognaize.document.field.link_field import LinkField
+>>> link_field = LinkField(name='URL', value='https://LinkField')
+>>> link_field.name
+'URL'
+>>> link_field.value
+'LinkField'
+>>> link_field.tags
+[]
+"""
 import logging
+from typing import List, Optional, Dict, Type
 
+from pycognaize.common.classification_labels import ClassificationLabels
 from pycognaize.common.enums import (
     IqDocumentKeysEnum,
+    IqTagKeyEnum,
     ID,
-    IqDataTypesEnum,
-    IqFieldKeyEnum
+    IqFieldKeyEnum,
+    IqDataTypesEnum
 )
-
-from pycognaize.document.field import Field
 from pycognaize.document.html_info import HTML
-from pycognaize.document.tag.span_tag import SpanTag
 from pycognaize.document.page import Page
+from pycognaize.document.field import Field
+from pycognaize.document.tag import ExtractionTag
+from pycognaize.document.tag.html_tag import HTMLTag
 
 
-class SpanField(Field):
-    """Base class for all pycognaize table fields"""
-    tag_class: Type[SpanTag] = SpanTag
+class LinkField(Field):
+    """Base class for all pycognaize link fields"""
+    tag_class: Type[ExtractionTag] = ExtractionTag
+    html_tag_class: Type[HTMLTag] = HTMLTag
 
     def __init__(self,
                  name: str,
-                 tags: Optional[SpanTag] = None,
+                 value: str = '',
+                 tags: Optional[List[ExtractionTag]] = None,
                  field_id: Optional[str] = None,
                  group_key: str = None,
                  confidence: Optional[float] = -1.0,
-                 group_name: str = None,
+                 group_name: str = None
                  ):
-        tags = [] if tags is None else tags
-        super().__init__(name=name, tags=tags,
+        """ Create a LinkField object
+
+        :param name: Name of the field
+        :param value: Value of the field
+            (left empty if values provided through tags)
+        :param tags: List of tag objects
+        :param field_id: The id of the field
+        """
+        super().__init__(name=name, tags=tags, value=value,
                          group_key=group_key, confidence=confidence,
                          group_name=group_name)
         self._field_id = field_id
+        self._value = '; '.join([i.raw_value
+                                 for i in self.tags]) if self.tags else value
+
+    @property
+    def value(self):
+        return self._value
 
     @classmethod
     def construct_from_raw(cls, raw: dict, pages: Dict[int, Page],
-                           html: Optional[HTML] = None) -> 'SpanField':
-        """Create SnapField object from dictionary"""
+                           html: Optional[HTML] = None,
+                           labels: ClassificationLabels = None) -> 'LinkField':
+        """Create LinkField object from dictionary"""
         tag_dicts: List[dict] = raw[IqDocumentKeysEnum.tags.value]
         tags = []
         for i in tag_dicts:
             try:
-                tags.append(cls.tag_class.construct_from_raw(
-                    raw=i, page=pages[i['page']]))
+                if pages:
+                    tags.append(cls.tag_class.construct_from_raw(
+                        raw=i, page=pages[i['page']]))
+                else:
+                    tags.append(cls.html_tag_class.construct_from_raw(
+                        raw=i, html=html))
             except Exception as e:
                 logging.debug(f"Failed creating tag for field {raw[ID]}: {e}")
+        value = (tags[0].raw_value if (html.path and tags)
+                 else raw[IqTagKeyEnum.value.value])
         return cls(name=raw[IqDocumentKeysEnum.name.value],
-                   tags=tags[0] if tags else None,
+                   value=value,
+                   tags=tags,
                    field_id=str(raw[ID]),
                    group_key=raw.get(IqFieldKeyEnum.group_key.value, ''),
                    group_name=raw.get(IqFieldKeyEnum.group.value, '')
                    )
 
     def to_dict(self) -> dict:
-        """Converts TableField object to dictionary"""
+        """Converts LinkField object to dictionary"""
         field_dict = super().to_dict()
         field_dict[ID] = self._field_id
-        field_dict[
-            IqFieldKeyEnum.data_type.value] = IqDataTypesEnum.table.value
-        field_dict[IqFieldKeyEnum.value.value] = ''
+        field_dict[IqFieldKeyEnum.value.value] = self.value
+        field_dict[IqFieldKeyEnum.data_type.value] = IqDataTypesEnum.link.value
         return field_dict
 
-    def order_tags(self):
-        """Order tags by pdf data"""
-        raise NotImplementedError
-
     def __repr__(self):
-        return f"<{self.__class__.__name__}: {self.name}>"
+        repr_values = ('|'.join([i.raw_value for i in self.tags])
+                       if self.tags else self.value)
+        return f"<{self.__class__.__name__}: {self.name}: {repr_values}>"
 
     def __str__(self):
-        return self.__repr__()
+        str_value = '|'.join([i.raw_value for i in self.tags]) \
+            if self.tags else self.value
+        return str_value
```

### Comparing `pycognaize-1.3.9/pycognaize/document/field/table_field.py` & `pycognaize-1.4.1/pycognaize/document/field/table_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     def __init__(self,
                  name: str,
                  tag: Optional[Union[TableTag, HTMLTableTag]] = None,
                  field_id: Optional[str] = None,
                  group_key: str = None,
                  confidence: Optional[float] = -1.0,
-                 group_name: str = None
+                 group_name: str = None,
                  ):
         tags = [] if tag is None else [tag]
         super().__init__(name=name, tags=tags, group_key=group_key,
                          confidence=confidence, group_name=group_name)
         self._field_id = field_id
 
     def get_table_title(self, n_lines_above=8, margin=10) -> str:
@@ -87,15 +87,16 @@
         all_rows_above = all_rows_above[:index_of_first_non_empty_line + 1]
         title = ' '.join(
             itertools.chain.from_iterable(all_rows_above[-n_lines_above:]))
         return title
 
     @classmethod
     def construct_from_raw(cls, raw: dict, pages: Dict[int, Page],
-                           html: Optional[HTML] = None) -> 'TableField':
+                           html: Optional[HTML] = None,
+                           labels=None) -> 'TableField':
         """Create TableField object from dictionary"""
         tag_dicts: List[dict] = raw[IqDocumentKeysEnum.tags.value]
         tags = []
         for i in tag_dicts:
             try:
                 if not pages:
                     tags.append(cls.html_tag_class.construct_from_raw(
```

### Comparing `pycognaize-1.3.9/pycognaize/document/field/text_field.py` & `pycognaize-1.4.1/pycognaize/document/field/text_field.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,65 +10,69 @@
 'gooloogooloo'
 >>> text_field.tags
 []
 """
 import logging
 from typing import List, Optional, Dict, Type
 
-
+from pycognaize.common.classification_labels import ClassificationLabels
 from pycognaize.common.enums import (
     IqDocumentKeysEnum,
     IqTagKeyEnum,
     ID,
     IqFieldKeyEnum,
     IqDataTypesEnum
 )
 from pycognaize.document.html_info import HTML
 from pycognaize.document.page import Page
 from pycognaize.document.field import Field
 from pycognaize.document.tag import ExtractionTag
-from pycognaize.document.tag.html_tag import TDTag
+from pycognaize.document.tag.html_tag import HTMLTag
 
 
 class TextField(Field):
     """Base class for all pycognaize text fields"""
     tag_class: Type[ExtractionTag] = ExtractionTag
-    html_tag_class: Type[TDTag] = TDTag
+    html_tag_class: Type[HTMLTag] = HTMLTag
 
     def __init__(self,
                  name: str,
                  value: str = '',
                  tags: Optional[List[ExtractionTag]] = None,
                  field_id: Optional[str] = None,
                  group_key: str = None,
                  confidence: Optional[float] = -1.0,
-                 group_name: str = None
+                 group_name: str = None,
+                 classification_labels: Optional[ClassificationLabels] = None
                  ):
         """ Create a TextField object
 
         :param name: Name of the field
         :param value: Value of the field
             (left empty if values provided through tags)
         :param tags: List of tag objects
         :param field_id: The id of the field
         """
         super().__init__(name=name, tags=tags, value=value,
                          group_key=group_key, confidence=confidence,
                          group_name=group_name)
+        self._classification_labels = classification_labels
         self._field_id = field_id
         self._value = '; '.join([i.raw_value
                                  for i in self.tags]) if self.tags else value
 
     @property
     def value(self):
         return self._value
 
     @classmethod
     def construct_from_raw(cls, raw: dict, pages: Dict[int, Page],
-                           html: Optional[HTML] = None) -> 'TextField':
+                           html: Optional[HTML] = None,
+                           labels: ClassificationLabels = None)\
+            -> 'TextField':
         """Create TextField object from dictionary"""
         tag_dicts: List[dict] = raw[IqDocumentKeysEnum.tags.value]
         tags = []
         for i in tag_dicts:
             try:
                 if pages:
                     tags.append(cls.tag_class.construct_from_raw(
@@ -81,16 +85,16 @@
         value = (tags[0].raw_value if (html.path and tags)
                  else raw[IqTagKeyEnum.value.value])
         return cls(name=raw[IqDocumentKeysEnum.name.value],
                    value=value,
                    tags=tags,
                    field_id=str(raw[ID]),
                    group_key=raw.get(IqFieldKeyEnum.group_key.value, ''),
-                   group_name=raw.get(IqFieldKeyEnum.group.value, '')
-                   )
+                   group_name=raw.get(IqFieldKeyEnum.group.value, ''),
+                   classification_labels=labels)
 
     def to_dict(self) -> dict:
         """Converts TextField object to dictionary"""
         field_dict = super().to_dict()
         field_dict[ID] = self._field_id
         field_dict[IqFieldKeyEnum.value.value] = self.value
         field_dict[IqFieldKeyEnum.data_type.value] = IqDataTypesEnum.text.value
```

### Comparing `pycognaize-1.3.9/pycognaize/document/html_info.py` & `pycognaize-1.4.1/pycognaize/document/html_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         """
         valid_path = ''
         try:
             joined_path = os.path.join(path, document_id)
             if (
                     self.ci.isdir(joined_path)
                     and StorageEnum.html_file.value
-                    in self.ci.listdir(joined_path)
+                    in self.ci.listdir(joined_path, exclude_folders=True)
             ):
                 valid_path = joined_path
             elif StorageEnum.html_file.value in self.ci.listdir(path):
                 valid_path = path
         except Exception as e:
             logging.debug(f"An error occurred while validating the path: {e}")
         return valid_path
```

### Comparing `pycognaize-1.3.9/pycognaize/document/page.py` & `pycognaize-1.4.1/pycognaize/document/page.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.9/pycognaize/document/snapshot.py` & `pycognaize-1.4.1/pycognaize/document/snapshot.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import logging
 from typing import Mapping, Tuple
 
+from pycognaize.common.utils import directory_summary_hash
 from pycognaize.login import Login
 from pycognaize.common import utils
-from pycognaize.common.enums import EnvConfigEnum
+from pycognaize.common.enums import EnvConfigEnum, HASH_FILE
 from pycognaize.common.exceptions import AuthenthicationError
 from pycognaize.common.lazy_dict import LazyDocumentDict
 
 
 class Snapshot:
     """A snapshot of annotated documents from one or more collections"""
 
@@ -45,14 +46,18 @@
 
         if login_instance.logged_in:
             snapshot_path = os.path.join(login_instance.snapshot_root,
                                          snapshot_id)
             ci = utils.cloud_interface_login(login_instance)
             ci.copy_dir(snapshot_path, destination_dir)
 
+            summary_hash = directory_summary_hash(destination_dir)
+            with open(os.path.join(destination_dir, HASH_FILE), 'w') as f:
+                f.write(summary_hash)
+
             logging.info(f"Snapshot {snapshot_id} downloaded to "
                          f"{destination_dir}. To use the snapshot, check our "
                          f"documentation at: ",
                          "http://pycognaize-docs.com."
                          "s3-website.us-east-2.amazonaws.com")
 
             return cls(path=snapshot_path), \
```

### Comparing `pycognaize-1.3.9/pycognaize/document/tag/cell.py` & `pycognaize-1.4.1/pycognaize/document/tag/cell.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.9/pycognaize/document/tag/extraction_tag.py` & `pycognaize-1.4.1/pycognaize/document/tag/extraction_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.9/pycognaize/document/tag/html_tag.py` & `pycognaize-1.4.1/pycognaize/document/tag/html_tag.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import abc
-from typing import Optional, List
+from typing import Optional, List, Union
 
 import bson
 import pandas as pd
 
 from pycognaize.common.enums import (IqRecipeEnum, XBRLCellEnum,
                                      XBRLTableTagEnum, XBRLTagEnum, ID)
 from pycognaize.document.html_info import HTML
 from pycognaize.document.tag.tag import Tag
 
 
-class HTMLTag(Tag, metaclass=abc.ABCMeta):
+class HTMLTagABC(Tag, metaclass=abc.ABCMeta):
     """Base class for XBRL document tags"""
-    def __init__(self, html_id: List[str], xpath: str,
+    def __init__(self, html_id: Union[str, List[str]], xpath: str,
                  tag_id: Optional[str] = None):
         self._html_id = html_id
         self._xpath = xpath
         self._tag_id = tag_id
 
     @property
     def html_id(self):
@@ -27,24 +27,25 @@
         return self._xpath
 
     @property
     def tag_id(self):
         return self._tag_id
 
     @classmethod
-    def construct_from_raw(cls, raw: dict, html: HTML) -> 'HTMLTag':
+    def construct_from_raw(cls, raw: dict, html: HTML) -> 'HTMLTagABC':
         ...
 
 
-class HTMLTableTag(HTMLTag):
+class HTMLTableTag(HTMLTagABC):
     """Represents table's coordinate data in XBRL document"""
 
     def __init__(self, tag_id: str,  value: str, ocr_value: str,
-                 xpath: str, title: str, html_id: List[str], cell_data: dict,
-                 html: HTML, source_ids, is_table: bool = True):
+                 xpath: str, title: str, html_id: Union[str, List[str]],
+                 cell_data: dict, html: HTML, source_ids,
+                 is_table: bool = True):
         super().__init__(html_id=html_id, xpath=xpath, tag_id=tag_id)
         self._value = value
         self._ocr_value = ocr_value
         self._is_table = is_table
         self._title = title
         self._cell_data = cell_data
         self._cells = {}
@@ -100,15 +101,15 @@
         if self._df is None:
             self._df = self.raw_df.applymap(
                 lambda x: self._extract_value(x))
         return self._df
 
     @staticmethod
     def _extract_value(x):
-        """Returns text value from `TDTag` object"""
+        """Returns text value from `HTMLTag` object"""
         try:
             return x.raw_value
         except AttributeError:
             return ''
 
     def _populate_cells(self):
         for row_col_index, cell_dict in self.cell_data.items():
@@ -118,15 +119,15 @@
             if XBRLTableTagEnum.left_indentation.value not in cell_dict:
                 cell_dict[XBRLTableTagEnum.left_indentation.value] = None
             self._cells[keys] = (
                 self._populate_cell(keys=keys, cell_dict=cell_dict))
 
     @staticmethod
     def _populate_cell(keys: tuple, cell_dict: dict) -> 'HTMLCell':
-        """ Creates `TDTag` object for each item in Table"""
+        """ Creates `HTMLCell` object for each item in Table"""
         return HTMLCell(
             html_id=cell_dict[XBRLCellEnum.id.value],
             xpath=cell_dict[XBRLCellEnum.xpath.value],
             row_index=keys[1],
             col_index=keys[0],
             col_span=cell_dict[XBRLCellEnum.col_span.value],
             row_span=cell_dict[XBRLCellEnum.row_span.value],
@@ -172,17 +173,17 @@
         source_ids = raw[XBRLTableTagEnum.source.value]
         return cls(tag_id=tag_id, ocr_value=ocr_value, value=value,
                    is_table=True, xpath=xpath, title=title,
                    html_id=html_id, cell_data=cell_data,
                    html=html, source_ids=source_ids)
 
     def _build_df(self) -> pd.DataFrame:
-        """Build pandas data frame using `TDTag` Cells
+        """Build pandas data frame using `HTMLTag` Cells
 
-        :return: DataFrame object,where each cell contains an TDTag
+        :return: DataFrame object,where each cell contains an HTMLTag
             object with the html_id and values from the annotated
             document
         """
         cols = set()
         rows = set()
         for cell_ in self.cells.values():
             cols.add(cell_.col_index - 1)
@@ -193,31 +194,31 @@
         rows.sort()
         df = pd.DataFrame(columns=cols, index=rows)
         for cell_ in self.cells.values():
             row_index = cell_.row_index - 1
             col_index = cell_.col_index - 1
             for col_n in range(col_index, col_index + cell_.col_span):
                 for row_n in range(row_index, row_index + cell_.row_span):
-                    df[col_n][row_n] = TDTag(is_table=False,
-                                             html_id=cell_.html_id,
-                                             xpath=cell_.xpath,
-                                             raw_value=cell_.raw_value,
-                                             raw_ocr_value=cell_.raw_value,
-                                             field_id='',
-                                             tag_id=self.tag_id,
-                                             row_index=row_index,
-                                             col_index=col_index)
+                    df[col_n][row_n] = HTMLTag(is_table=False,
+                                               html_id=cell_.html_id,
+                                               xpath=cell_.xpath,
+                                               raw_value=cell_.raw_value,
+                                               raw_ocr_value=cell_.raw_value,
+                                               field_id='',
+                                               tag_id=self.tag_id,
+                                               row_index=row_index,
+                                               col_index=col_index)
         return df
 
 
 class HTMLCell:
     """Represents cell tag for XBRL tables"""
     def __init__(self, row_index: int, col_index: int,
                  col_span: int, row_span: int,
-                 html_id: List[str], xpath: str,
+                 html_id: Union[str, List[str]], xpath: str,
                  raw_value: str, is_bold: False,
                  left_indentation: None):
         self._row_index = row_index
         self._col_index = col_index
         self._col_span = col_span
         self._row_span = row_span
         self._html_id = html_id
@@ -260,15 +261,15 @@
 
     @property
     def left_indentation(self) -> str:
         return self._left_indentation
 
     @classmethod
     def construct_from_raw(cls, raw: dict) -> 'HTMLCell':
-        """Build TDTag from pycognaize raw data
+        """Build HTMLTAG from pycognaize raw data
 
         :param raw: pycognaize field's tag info
         :return:
         """
         source_data = raw[XBRLCellEnum.source.value]
         row_index = source_data[XBRLCellEnum.row_index.value]
         col_index = source_data[XBRLCellEnum.col_index.value]
@@ -295,26 +296,28 @@
             XBRLCellEnum.xpath.value: self.xpath,
             XBRLCellEnum.raw_value.value: self.raw_value,
             XBRLCellEnum.left_indentation.value: self.left_indentation,
             XBRLCellEnum.is_bold.value: self.is_bold}
         return {f"{self.col_index}:{self.row_index}": cell_dict}
 
 
-class TDTag(HTMLTag):
+class HTMLTag(HTMLTagABC):
     def __init__(self, raw_value: str, raw_ocr_value: str,
-                 is_table: bool, html_id: List[str],
+                 is_table: bool, html_id: Union[str, List[str]],
                  field_id: Optional[str], tag_id: Optional[str],
-                 row_index: int, col_index: int, xpath: str):
+                 row_index: int, col_index: int, xpath: str,
+                 is_td: bool = True):
         super().__init__(html_id=html_id, xpath=xpath, tag_id=tag_id)
         self._raw_value = raw_value
         self._raw_ocr_value = raw_ocr_value
         self._is_table = is_table
         self._field_id = field_id
         self._row_index = row_index
         self._col_index = col_index
+        self._is_td = is_td
 
     @property
     def raw_value(self):
         """returns adjusted value"""
         return self._raw_value
 
     @property
@@ -333,47 +336,71 @@
     def row_index(self):
         return self._row_index
 
     @property
     def col_index(self):
         return self._col_index
 
+    @property
+    def is_td(self):
+        return self._is_td
+
     @classmethod
-    def construct_from_raw(cls, raw: dict, html: HTML) -> 'TDTag':
-        """Build TDTag from pycognaize raw data
+    def construct_from_raw(cls, raw: dict, html: HTML) -> 'HTMLTag':
+        """Build HTMLTag from pycognaize raw data
         :param html: HTML
         :param raw: pycognaize field's tag info
         :return:
         """
         source_data = raw[XBRLTagEnum.source.value]
+        if XBRLTagEnum.html.value in source_data:
+            is_td = False
+            html_id = source_data[XBRLTagEnum.html.value][
+                XBRLTagEnum.parent_id.value]
+        else:
+            is_td = True
+            html_id = source_data[XBRLTagEnum.ids.value]
         raw_value = raw[XBRLTagEnum.value.value]
         raw_ocr_value = raw[XBRLTagEnum.ocr_value.value]
         is_table = raw[XBRLTagEnum.is_table.value]
-        html_id = source_data[XBRLTagEnum.ids.value]
         field_id = source_data[IqRecipeEnum.field_id.value]
         tag_id = source_data[XBRLTagEnum.tag_id.value]
         row_index = source_data[XBRLTagEnum.row_index.value]
         col_index = source_data[XBRLTagEnum.col_index.value] - 1
         xpath = source_data[XBRLTagEnum.xpath.value]
         return cls(html_id=html_id,  raw_value=raw_value,
                    raw_ocr_value=raw_ocr_value, is_table=is_table,
                    field_id=field_id, tag_id=tag_id,
                    row_index=row_index, col_index=col_index,
-                   xpath=xpath)
+                   xpath=xpath, is_td=is_td)
 
     def to_dict(self) -> dict:
         """Converts tag to dict"""
-        tag_info = {
-            XBRLTagEnum.ids.value: self.html_id,
-            IqRecipeEnum.field_id.value: self.field_id,
-            XBRLTagEnum.tag_id.value: self.tag_id,
-            XBRLTagEnum.row_index.value: self.row_index,
-            XBRLTagEnum.col_index.value: self.col_index + 1,
-            XBRLTagEnum.xpath.value: self.xpath,
-        }
+        if self.is_td:
+            tag_info = {
+                XBRLTagEnum.ids.value: self.html_id,
+                IqRecipeEnum.field_id.value: self.field_id,
+                XBRLTagEnum.tag_id.value: self.tag_id,
+                XBRLTagEnum.row_index.value: self.row_index,
+                XBRLTagEnum.col_index.value: self.col_index + 1,
+                XBRLTagEnum.xpath.value: self.xpath,
+            }
+        else:
+            tag_info = {
+                XBRLTagEnum.html.value: {
+                    XBRLTagEnum.parent_id.value: self.html_id,
+                    XBRLTagEnum.value.value: self.raw_value
+                },
+                XBRLTagEnum.ids.value: [],
+                IqRecipeEnum.field_id.value: self.field_id,
+                XBRLTagEnum.tag_id.value: self.tag_id,
+                XBRLTagEnum.row_index.value: self.row_index,
+                XBRLTagEnum.col_index.value: self.col_index + 1,
+                XBRLTagEnum.xpath.value: self.xpath,
+            }
         output_dict = {
             ID: str(bson.ObjectId()),
             XBRLTagEnum.value.value: self.raw_value,
             XBRLTagEnum.ocr_value.value: self.raw_ocr_value,
             XBRLTagEnum.is_table.value: self.is_table,
             XBRLTagEnum.source.value: tag_info,
          }
```

### Comparing `pycognaize-1.3.9/pycognaize/document/tag/section_tag.py` & `pycognaize-1.4.1/pycognaize/document/tag/section_tag.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,18 +9,22 @@
 if TYPE_CHECKING:
     from pycognaize.document.page import Page
 
 
 class SectionTag(LineTag):
     """Represents field's coordinate data on document"""
 
-    def __init__(self, top, page, tag_type):
-        super().__init__(top=top, page=page, tag_type=tag_type)
+    def __init__(self, top, left, height, width, page, tag_type):
+        super().__init__(top=top,
+                         page=page, tag_type=tag_type)
         self._type = tag_type
         self._top = top
+        self._left = left
+        self._height = height
+        self._width = width
         self._page = page
 
     @classmethod
     def construct_from_raw(cls, raw: dict,
                            pages: Dict[int, 'Page'],
                            tag_type: str) -> 'SectionTag':
         """Builds Tag object from pycognaize raw data
@@ -28,15 +32,23 @@
         :param raw: pycognaize field's tag info
         :param pages: `Page` to which the tag belongs
         :param tag_type: `Page` to which the tag belongs
         :return:
         """
         page_number = raw['page']
         top = convert_coord_to_num(raw['top'])
-        tag = cls(top=top, page=pages[page_number],
+        left = convert_coord_to_num(raw['left'])
+        height = convert_coord_to_num(raw['height'])
+        width = convert_coord_to_num(raw['width'])
+
+        tag = cls(top=top,
+                  left=left,
+                  height=height,
+                  width=width,
+                  page=pages[page_number],
                   tag_type=tag_type)
         return tag
 
     def vshift(self, by) -> 'SectionTag':
         """Shifts line vertically
 
         :param by: the amount by which the tag should be vertically shifted
@@ -55,8 +67,11 @@
         return SectionTag(top=top, page=self.page, tag_type=self.type)
 
     def to_dict(self) -> dict:
         """Converts extraction tag to dict"""
         return {
             ID: str(bson.ObjectId()),
             IqTagKeyEnum.top.value: f"{self.top}%",
+            IqTagKeyEnum.left.value: f"{self._left}%",
+            IqTagKeyEnum.height.value: f"{self._height}%",
+            IqTagKeyEnum.width.value: f"{self._width}%",
             IqTagKeyEnum.page.value: self.page.page_number}
```

### Comparing `pycognaize-1.3.9/pycognaize/document/tag/span_tag.py` & `pycognaize-1.4.1/pycognaize/document/tag/span_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.9/pycognaize/document/tag/table_tag.py` & `pycognaize-1.4.1/pycognaize/document/tag/table_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.9/pycognaize/document/tag/tag.py` & `pycognaize-1.4.1/pycognaize/document/tag/tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.9/pycognaize/index.py` & `pycognaize-1.4.1/pycognaize/index.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.9/pycognaize/login.py` & `pycognaize-1.4.1/pycognaize/login.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.9/pycognaize/model.py` & `pycognaize-1.4.1/pycognaize/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from pycognaize.common.utils import (
     replace_object_ids_with_string,
     ConfusionMatrix
 )
 from pycognaize.document.document import Document
 from pycognaize.document.tag import ExtractionTag
-from pycognaize.document.tag.html_tag import TDTag, HTMLTableTag
+from pycognaize.document.tag.html_tag import HTMLTag, HTMLTableTag
 
 
 def join_url(*parts):
     """Join parts into a single url string"""
     return '/'.join(s.strip('/') for s in parts)
 
 
@@ -367,32 +367,32 @@
             for field_name in document.y.keys():
                 for item in document.y[field_name]:
                     if item.group_key == key:
                         groups[key][field_name] = item
         return groups
 
     @staticmethod
-    def matches(act_tag: Union['ExtractionTag', 'TDTag', 'HTMLTableTag'],
-                pred_tag: Union['ExtractionTag', 'TDTag', 'HTMLTableTag'],
+    def matches(act_tag: Union['ExtractionTag', 'HTMLTag', 'HTMLTableTag'],
+                pred_tag: Union['ExtractionTag', 'HTMLTag', 'HTMLTableTag'],
                 threshold: float = 0.6) -> bool:
-        """ If tags are TDTag checks that two tags have the same html_id,
+        """ If tags are HTMLTag checks that two tags have the same html_id,
             otherwise detects if there is a match between two extraction tags
             having the same page number. Returns true if
         intersection is greater than the threshold"""
         is_match = False
-        if isinstance(act_tag, TDTag) and isinstance(pred_tag, TDTag):
+        if isinstance(act_tag, HTMLTag) and isinstance(pred_tag, HTMLTag):
             cell_xpath = max(act_tag.xpath, pred_tag.xpath, key=len)
             field_xpath = min(act_tag.xpath, pred_tag.xpath, key=len)
             is_match = field_xpath in cell_xpath \
                 and act_tag.col_index == pred_tag.col_index\
                 and act_tag.row_index == pred_tag.row_index
-        elif ((isinstance(act_tag, TDTag)
+        elif ((isinstance(act_tag, HTMLTag)
               and isinstance(pred_tag, HTMLTableTag)) or
               (isinstance(act_tag, HTMLTableTag)
-               and isinstance(pred_tag, TDTag))):
+               and isinstance(pred_tag, HTMLTag))):
             is_match = act_tag.tag_id == pred_tag.tag_id
         else:
             is_match = (
                     act_tag.page.page_number == pred_tag.page.page_number
                     and ((act_tag & pred_tag) / min(act_tag, pred_tag,
                          key=lambda x: x.area).area >= threshold)
             )
```

### Comparing `pycognaize-1.3.9/pycognaize.egg-info/PKG-INFO` & `pycognaize-1.4.1/pycognaize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycognaize
-Version: 1.3.9
+Version: 1.4.1
 Home-page: https://github.com/cognaize/pycognaize
 Author: Cognaize
 License: Apache License 2.0
 Project-URL: Source, https://github.com/cognaize/pycognaize
 Project-URL: Reference, https://pycognaize.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/cognaize/pycognaize/blob/master/CHANGELOG.md
 Requires-Python: >= 3.7
@@ -43,16 +43,44 @@
 ```
 
 Have a look at the [quick tutorial](http://pycognaize-docs.com.s3-website.us-east-2.amazonaws.com/tutorials/quick_tutorial.html) 
 for understanding main concepts of the SDK.
 
 # Changelog
 
+## [1.4]
+
+### [1.4.1] - 2023-05-29
+- Add section field and section tag functionality
+
+
+### [1.4.0] - 2023-05-25
+- Add classification labels functionality to ``Field`` objects
+
 ## [1.3]
 
+### [1.3.14] - 2023-05-10
+- Add LinkField object
+- Add returning group name in to_dict functionality of Field object 
+
+### [1.3.13] - 2023-05-01
+- Add exclude folders option for ``lisdir`` in ``html_info``
+- Update version cloudstorageio >= 1.2.8
+### [1.3.12] - 2023-05-01
+- Rename HTMLTag to HTMLTagABC
+- Rename TDTag to HTMLTag
+- Handle out of table tags in XBRL
+
+### [1.3.11] - 2023-04-28
+- Add interface to create directory summary hashes
+- Add automatic snapshot hash creation for ``snapshot.download``
+
+### [1.3.10] - 2023-03-31
+- Add login command and code for submit to model registry
+
 ### [1.3.9] - 2023-03-30
 - Refactor HTML._validate_path() to include try-except block
 
 ### [1.3.8] - 2023-03-28
 - Improve html file path validation by adding a new check
 in HTML._validate_path()
```

### Comparing `pycognaize-1.3.9/pycognaize.egg-info/SOURCES.txt` & `pycognaize-1.4.1/pycognaize.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 CHANGELOG.md
 LICENSE.txt
 README.md
 setup.cfg
 setup.py
 pycognaize/__init__.py
+pycognaize/cli.py
 pycognaize/clidriver.py
 pycognaize/index.py
 pycognaize/login.py
 pycognaize/model.py
 pycognaize.egg-info/PKG-INFO
 pycognaize.egg-info/SOURCES.txt
 pycognaize.egg-info/dependency_links.txt
 pycognaize.egg-info/entry_points.txt
 pycognaize.egg-info/requires.txt
 pycognaize.egg-info/top_level.txt
 pycognaize/common/__init__.py
+pycognaize/common/classification_labels.py
 pycognaize/common/confidence.py
 pycognaize/common/decorators.py
 pycognaize/common/enums.py
 pycognaize/common/exceptions.py
 pycognaize/common/field_collection.py
 pycognaize/common/lazy_dict.py
 pycognaize/common/lazy_group_dict.py
@@ -31,20 +33,26 @@
 pycognaize/document/html_info.py
 pycognaize/document/page.py
 pycognaize/document/snapshot.py
 pycognaize/document/field/__init__.py
 pycognaize/document/field/area_field.py
 pycognaize/document/field/date_field.py
 pycognaize/document/field/field.py
+pycognaize/document/field/link_field.py
 pycognaize/document/field/numeric_field.py
 pycognaize/document/field/section_field.py
 pycognaize/document/field/span_field.py
 pycognaize/document/field/table_field.py
 pycognaize/document/field/text_field.py
 pycognaize/document/tag/__init__.py
 pycognaize/document/tag/cell.py
 pycognaize/document/tag/extraction_tag.py
 pycognaize/document/tag/html_tag.py
 pycognaize/document/tag/section_tag.py
 pycognaize/document/tag/span_tag.py
 pycognaize/document/tag/table_tag.py
-pycognaize/document/tag/tag.py
+pycognaize/document/tag/tag.py
+pycognaize/model_registry/__init__.py
+pycognaize/model_registry/login.py
+pycognaize/model_registry/submit.py
+pycognaize/model_registry/db/__init__.py
+pycognaize/model_registry/db/models.py
```

### Comparing `pycognaize-1.3.9/setup.cfg` & `pycognaize-1.4.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 	simplejson
 	pillow
 	pymupdf==1.21.1
 	urllib3
 	lxml
 	beautifulsoup4
 	dataclasses; python_version <= '3.6'
+	PyYAML
+	click
 
 [options.packages.find]
 exclude = 
 	pycognaize.temp.*
 	pycognaize.temp
 	pycognaize.tests.*
 	pycognaize.tests
```

### Comparing `pycognaize-1.3.9/setup.py` & `pycognaize-1.4.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 setup_options = dict(
     license="Apache License 2.0",
     python_requires=">= 3.7",
     entry_points='''
         [console_scripts]
-        cognaize=bin.cognaize:main''',
+        cognaize=pycognaize.cli:cognaize''',
     project_urls={
         'Source': 'https://github.com/cognaize/pycognaize',
         'Reference': 'https://pycognaize.readthedocs.io/en/latest/',
         'Changelog': 'https://github.com/cognaize/pycognaize/blob/master/CHANGELOG.md',
     },
 )
```

