# Comparing `tmp/musif-1.1.2.tar.gz` & `tmp/musif-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musif-1.1.2.tar", last modified: Mon May 29 09:38:51 2023, max compression
+gzip compressed data, was "musif-1.1.3.tar", last modified: Tue May 30 16:03:00 2023, max compression
```

## Comparing `musif-1.1.2.tar` & `musif-1.1.3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0     2143 2023-05-29 09:31:41.363076 musif-1.1.2/README.md
--rw-r--r--   0        0        0      258 2023-04-19 09:15:49.949723 musif-1.1.2/musif/__init__.py
--rw-r--r--   0        0        0     7344 2023-04-26 14:35:45.753205 musif-1.1.2/musif/__main__.py
--rw-r--r--   0        0        0      232 2023-04-19 09:14:37.169723 musif-1.1.2/musif/cache/__init__.py
--rw-r--r--   0        0        0    17854 2023-04-26 14:35:45.753205 musif-1.1.2/musif/cache/cache.py
--rw-r--r--   0        0        0     7606 2023-04-26 14:35:45.753205 musif-1.1.2/musif/cache/utils.py
--rw-r--r--   0        0        0        1 2023-04-19 09:14:37.169723 musif-1.1.2/musif/common/__init__.py
--rw-r--r--   0        0        0      202 2023-04-19 09:14:37.169723 musif-1.1.2/musif/common/_constants.py
--rw-r--r--   0        0        0     2402 2023-04-19 09:14:37.169723 musif-1.1.2/musif/common/_logs.py
--rw-r--r--   0        0        0     3067 2023-04-19 09:14:37.169723 musif-1.1.2/musif/common/_utils.py
--rw-r--r--   0        0        0      826 2023-04-19 09:14:37.169723 musif-1.1.2/musif/common/constants.py
--rw-r--r--   0        0        0     1700 2023-04-19 09:14:37.169723 musif-1.1.2/musif/common/didone_utils.py
--rw-r--r--   0        0        0     1175 2023-04-19 09:14:37.169723 musif-1.1.2/musif/common/exceptions.py
--rw-r--r--   0        0        0     4102 2023-04-19 09:14:37.169723 musif-1.1.2/musif/common/sort.py
--rw-r--r--   0        0        0     2103 2023-04-19 09:14:37.169723 musif-1.1.2/musif/common/translate.py
--rw-r--r--   0        0        0     7287 2023-04-26 14:35:45.753205 musif-1.1.2/musif/config.py
--rw-r--r--   0        0        0       52 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/basic_modules/file_name_generic/__init__.py
--rw-r--r--   0        0        0       34 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/basic_modules/file_name_generic/constants.py
--rw-r--r--   0        0        0      999 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/basic_modules/file_name_generic/handler.py
--rw-r--r--   0        0        0        0 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/basic_modules/scoring/__init__.py
--rw-r--r--   0        0        0      646 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/basic_modules/scoring/constants.py
--rw-r--r--   0        0        0     5686 2023-05-29 08:41:47.409829 musif-1.1.2/musif/extract/basic_modules/scoring/handler.py
--rw-r--r--   0        0        0     1600 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/common.py
--rw-r--r--   0        0        0     1178 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/constants.py
--rw-r--r--   0        0        0    28678 2023-05-29 08:47:17.936486 musif-1.1.2/musif/extract/extract.py
--rw-r--r--   0        0        0    28677 2023-04-19 11:27:49.216307 musif-1.1.2/musif/extract/extract.py~
--rw-r--r--   0        0        0        0 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/features/__init__.py
--rw-r--r--   0        0        0       25 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/features/ambitus/__init__.py
--rw-r--r--   0        0        0      270 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/features/ambitus/constants.py
--rw-r--r--   0        0        0     2705 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/features/ambitus/handler.py
--rw-r--r--   0        0        0        0 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/features/core/__init__.py
--rw-r--r--   0        0        0      465 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/features/core/constants.py
--rw-r--r--   0        0        0     7246 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/core/handler.py
--rw-r--r--   0        0        0       55 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/features/density/__init__.py
--rw-r--r--   0        0        0       57 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/features/density/constants.py
--rw-r--r--   0        0        0     7668 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/density/handler.py
--rw-r--r--   0        0        0       25 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/features/dynamics/__init__.py
--rw-r--r--   0        0        0      821 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/dynamics/constants.py
--rw-r--r--   0        0        0     9029 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/features/dynamics/handler.py
--rw-r--r--   0        0        0        0 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/features/harmony/__init__.py
--rw-r--r--   0        0        0      815 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/features/harmony/constants.py
--rw-r--r--   0        0        0     2741 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/features/harmony/handler.py
--rw-r--r--   0        0        0    26047 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/features/harmony/utils.py
--rw-r--r--   0        0        0       29 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/jsymbolic/__init__.py
--rw-r--r--   0        0        0      282 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/jsymbolic/__main__.py
--rw-r--r--   0        0        0      234 2023-04-19 11:25:57.299641 musif-1.1.2/musif/extract/features/jsymbolic/__main__.py~
--rw-r--r--   0        0        0     2827 2023-05-29 08:39:41.526500 musif-1.1.2/musif/extract/features/jsymbolic/handler.py
--rw-r--r--   0        0        0     1809 2023-04-19 11:32:59.902970 musif-1.1.2/musif/extract/features/jsymbolic/handler.py~
--rw-r--r--   0        0        0     3381 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/jsymbolic/utils.py
--rw-r--r--   0        0        0     2315 2023-04-19 11:25:00.146309 musif-1.1.2/musif/extract/features/jsymbolic/utils.py~
--rw-r--r--   0        0        0        0 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/key/__init__.py
--rw-r--r--   0        0        0      165 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/key/constants.py
--rw-r--r--   0        0        0     1044 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/features/key/handler.py
--rw-r--r--   0        0        0       25 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/lyrics/__init__.py
--rw-r--r--   0        0        0      113 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/lyrics/constants.py
--rw-r--r--   0        0        0     3669 2023-04-19 09:15:49.953056 musif-1.1.2/musif/extract/features/lyrics/handler.py
--rw-r--r--   0        0        0       25 2023-04-19 09:15:49.953056 musif-1.1.2/musif/extract/features/melody/__init__.py
--rw-r--r--   0        0        0    10534 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/melody/constants.py
--rw-r--r--   0        0        0    30504 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/melody/handler.py
--rw-r--r--   0        0        0       80 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/music21/__init__.py
--rw-r--r--   0        0        0      173 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/music21/constants.py
--rw-r--r--   0        0        0     2182 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/music21/handler.py
--rw-r--r--   0        0        0     1919 2023-04-19 11:30:50.492972 musif-1.1.2/musif/extract/features/music21/handler.py~
--rw-r--r--   0        0        0     3554 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/prefix.py
--rw-r--r--   0        0        0        0 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/rhythm/__init__.py
--rw-r--r--   0        0        0      273 2023-04-19 09:15:49.953056 musif-1.1.2/musif/extract/features/rhythm/constants.py
--rw-r--r--   0        0        0     5925 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/rhythm/handler.py
--rw-r--r--   0        0        0        0 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/scale/__init__.py
--rw-r--r--   0        0        0      269 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/scale/constants.py
--rw-r--r--   0        0        0     3627 2023-04-19 09:15:49.953056 musif-1.1.2/musif/extract/features/scale/handler.py
--rw-r--r--   0        0        0        0 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/scale_relative/__init__.py
--rw-r--r--   0        0        0      102 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/scale_relative/constants.py
--rw-r--r--   0        0        0     2842 2023-04-19 09:15:49.953056 musif-1.1.2/musif/extract/features/scale_relative/handler.py
--rw-r--r--   0        0        0     7321 2023-04-19 09:15:49.953056 musif-1.1.2/musif/extract/features/scale_relative/utils.py
--rw-r--r--   0        0        0        0 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/tempo/__init__.py
--rw-r--r--   0        0        0      306 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/tempo/constants.py
--rw-r--r--   0        0        0     5145 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/tempo/handler.py
--rw-r--r--   0        0        0        0 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/texture/__init__.py
--rw-r--r--   0        0        0       45 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/texture/constants.py
--rw-r--r--   0        0        0     3077 2023-04-19 09:15:49.953056 musif-1.1.2/musif/extract/features/texture/handler.py
--rw-r--r--   0        0        0    21081 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/utils.py
--rw-r--r--   0        0        0     2011 2023-04-19 09:14:37.176390 musif-1.1.2/musif/logs.py
--rw-r--r--   0        0        0       61 2023-04-19 09:15:49.953056 musif-1.1.2/musif/musescore/__init__.py
--rw-r--r--   0        0        0      948 2023-04-19 09:14:37.176390 musif-1.1.2/musif/musescore/common.py
--rw-r--r--   0        0        0       95 2023-04-19 09:15:49.953056 musif-1.1.2/musif/musescore/constants.py
--rw-r--r--   0        0        0       91 2023-04-19 09:15:49.953056 musif-1.1.2/musif/musicxml/__init__.py
--rw-r--r--   0        0        0     7670 2023-05-29 09:27:28.939750 musif-1.1.2/musif/musicxml/common.py
--rw-r--r--   0        0        0    15310 2023-04-26 14:35:45.753205 musif-1.1.2/musif/musicxml/constants.py
--rw-r--r--   0        0        0     2092 2023-04-19 09:15:49.953056 musif-1.1.2/musif/musicxml/key.py
--rw-r--r--   0        0        0    17541 2023-04-19 09:14:37.179723 musif-1.1.2/musif/musicxml/repeat.py
--rw-r--r--   0        0        0     4513 2023-04-26 14:35:45.753205 musif-1.1.2/musif/musicxml/scoring.py
--rw-r--r--   0        0        0     8151 2023-04-26 14:35:45.753205 musif-1.1.2/musif/musicxml/tempo.py
--rw-r--r--   0        0        0        0 2023-04-19 09:14:37.179723 musif-1.1.2/musif/process/__init__.py
--rw-r--r--   0        0        0      410 2023-04-19 09:15:49.953056 musif-1.1.2/musif/process/constants.py
--rw-r--r--   0        0        0    11327 2023-04-26 14:35:45.756538 musif-1.1.2/musif/process/processor.py
--rw-r--r--   0        0        0     7824 2023-04-26 14:35:45.756538 musif-1.1.2/musif/process/utils.py
--rw-r--r--   0        0        0      650 2023-05-29 09:27:28.939750 musif-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2384 1970-01-01 00:00:00.000000 musif-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2215 2023-05-30 15:50:33.123269 musif-1.1.3/README.md
+-rw-r--r--   0        0        0      258 2023-04-19 09:15:49.949723 musif-1.1.3/musif/__init__.py
+-rw-r--r--   0        0        0     7344 2023-04-26 14:35:45.753205 musif-1.1.3/musif/__main__.py
+-rw-r--r--   0        0        0      232 2023-04-19 09:14:37.169723 musif-1.1.3/musif/cache/__init__.py
+-rw-r--r--   0        0        0    17854 2023-04-26 14:35:45.753205 musif-1.1.3/musif/cache/cache.py
+-rw-r--r--   0        0        0     7606 2023-04-26 14:35:45.753205 musif-1.1.3/musif/cache/utils.py
+-rw-r--r--   0        0        0        1 2023-04-19 09:14:37.169723 musif-1.1.3/musif/common/__init__.py
+-rw-r--r--   0        0        0      202 2023-04-19 09:14:37.169723 musif-1.1.3/musif/common/_constants.py
+-rw-r--r--   0        0        0     2402 2023-04-19 09:14:37.169723 musif-1.1.3/musif/common/_logs.py
+-rw-r--r--   0        0        0     3067 2023-04-19 09:14:37.169723 musif-1.1.3/musif/common/_utils.py
+-rw-r--r--   0        0        0      826 2023-04-19 09:14:37.169723 musif-1.1.3/musif/common/constants.py
+-rw-r--r--   0        0        0     1700 2023-04-19 09:14:37.169723 musif-1.1.3/musif/common/didone_utils.py
+-rw-r--r--   0        0        0     1175 2023-04-19 09:14:37.169723 musif-1.1.3/musif/common/exceptions.py
+-rw-r--r--   0        0        0     4102 2023-04-19 09:14:37.169723 musif-1.1.3/musif/common/sort.py
+-rw-r--r--   0        0        0     2103 2023-04-19 09:14:37.169723 musif-1.1.3/musif/common/translate.py
+-rw-r--r--   0        0        0     7393 2023-05-30 15:24:16.943315 musif-1.1.3/musif/config.py
+-rw-r--r--   0        0        0       52 2023-04-19 09:14:37.173057 musif-1.1.3/musif/extract/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:15:49.949723 musif-1.1.3/musif/extract/basic_modules/file_name_generic/__init__.py
+-rw-r--r--   0        0        0       34 2023-04-19 09:15:49.949723 musif-1.1.3/musif/extract/basic_modules/file_name_generic/constants.py
+-rw-r--r--   0        0        0      999 2023-04-19 09:15:49.949723 musif-1.1.3/musif/extract/basic_modules/file_name_generic/handler.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.173057 musif-1.1.3/musif/extract/basic_modules/scoring/__init__.py
+-rw-r--r--   0        0        0      646 2023-04-19 09:14:37.173057 musif-1.1.3/musif/extract/basic_modules/scoring/constants.py
+-rw-r--r--   0        0        0     5686 2023-05-29 08:41:47.409829 musif-1.1.3/musif/extract/basic_modules/scoring/handler.py
+-rw-r--r--   0        0        0     1600 2023-04-19 09:15:49.949723 musif-1.1.3/musif/extract/common.py
+-rw-r--r--   0        0        0     1178 2023-04-19 09:15:49.949723 musif-1.1.3/musif/extract/constants.py
+-rw-r--r--   0        0        0    28730 2023-05-30 15:24:16.943315 musif-1.1.3/musif/extract/extract.py
+-rw-r--r--   0        0        0    28677 2023-04-19 11:27:49.216307 musif-1.1.3/musif/extract/extract.py~
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.173057 musif-1.1.3/musif/extract/features/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-19 09:14:37.173057 musif-1.1.3/musif/extract/features/ambitus/__init__.py
+-rw-r--r--   0        0        0      270 2023-04-19 09:14:37.173057 musif-1.1.3/musif/extract/features/ambitus/constants.py
+-rw-r--r--   0        0        0     2705 2023-04-19 09:15:49.949723 musif-1.1.3/musif/extract/features/ambitus/handler.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.173057 musif-1.1.3/musif/extract/features/core/__init__.py
+-rw-r--r--   0        0        0      465 2023-04-19 09:15:49.949723 musif-1.1.3/musif/extract/features/core/constants.py
+-rw-r--r--   0        0        0     7246 2023-04-26 14:35:45.753205 musif-1.1.3/musif/extract/features/core/handler.py
+-rw-r--r--   0        0        0       55 2023-04-19 09:14:37.173057 musif-1.1.3/musif/extract/features/density/__init__.py
+-rw-r--r--   0        0        0       57 2023-04-19 09:14:37.173057 musif-1.1.3/musif/extract/features/density/constants.py
+-rw-r--r--   0        0        0     7668 2023-04-26 14:35:45.753205 musif-1.1.3/musif/extract/features/density/handler.py
+-rw-r--r--   0        0        0       25 2023-04-19 09:14:37.173057 musif-1.1.3/musif/extract/features/dynamics/__init__.py
+-rw-r--r--   0        0        0      821 2023-04-26 14:35:45.753205 musif-1.1.3/musif/extract/features/dynamics/constants.py
+-rw-r--r--   0        0        0     9029 2023-04-19 09:15:49.949723 musif-1.1.3/musif/extract/features/dynamics/handler.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.173057 musif-1.1.3/musif/extract/features/harmony/__init__.py
+-rw-r--r--   0        0        0      815 2023-04-19 09:14:37.173057 musif-1.1.3/musif/extract/features/harmony/constants.py
+-rw-r--r--   0        0        0     2741 2023-04-19 09:15:49.949723 musif-1.1.3/musif/extract/features/harmony/handler.py
+-rw-r--r--   0        0        0    26047 2023-04-19 09:15:49.949723 musif-1.1.3/musif/extract/features/harmony/utils.py
+-rw-r--r--   0        0        0       29 2023-04-26 14:35:45.753205 musif-1.1.3/musif/extract/features/jsymbolic/__init__.py
+-rw-r--r--   0        0        0      282 2023-04-26 14:35:45.753205 musif-1.1.3/musif/extract/features/jsymbolic/__main__.py
+-rw-r--r--   0        0        0      234 2023-04-19 11:25:57.299641 musif-1.1.3/musif/extract/features/jsymbolic/__main__.py~
+-rw-r--r--   0        0        0     3565 2023-05-30 15:24:16.943315 musif-1.1.3/musif/extract/features/jsymbolic/handler.py
+-rw-r--r--   0        0        0     1809 2023-04-19 11:32:59.902970 musif-1.1.3/musif/extract/features/jsymbolic/handler.py~
+-rw-r--r--   0        0        0     3381 2023-04-26 14:35:45.753205 musif-1.1.3/musif/extract/features/jsymbolic/utils.py
+-rw-r--r--   0        0        0     2315 2023-04-19 11:25:00.146309 musif-1.1.3/musif/extract/features/jsymbolic/utils.py~
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.176390 musif-1.1.3/musif/extract/features/key/__init__.py
+-rw-r--r--   0        0        0      165 2023-04-19 09:14:37.176390 musif-1.1.3/musif/extract/features/key/constants.py
+-rw-r--r--   0        0        0     1044 2023-04-19 09:15:49.949723 musif-1.1.3/musif/extract/features/key/handler.py
+-rw-r--r--   0        0        0       25 2023-04-19 09:14:37.176390 musif-1.1.3/musif/extract/features/lyrics/__init__.py
+-rw-r--r--   0        0        0      113 2023-04-19 09:14:37.176390 musif-1.1.3/musif/extract/features/lyrics/constants.py
+-rw-r--r--   0        0        0     3669 2023-04-19 09:15:49.953056 musif-1.1.3/musif/extract/features/lyrics/handler.py
+-rw-r--r--   0        0        0       25 2023-04-19 09:15:49.953056 musif-1.1.3/musif/extract/features/melody/__init__.py
+-rw-r--r--   0        0        0    10534 2023-04-26 14:35:45.753205 musif-1.1.3/musif/extract/features/melody/constants.py
+-rw-r--r--   0        0        0    30504 2023-04-26 14:35:45.753205 musif-1.1.3/musif/extract/features/melody/handler.py
+-rw-r--r--   0        0        0       80 2023-04-26 14:35:45.753205 musif-1.1.3/musif/extract/features/music21/__init__.py
+-rw-r--r--   0        0        0      173 2023-04-26 14:35:45.753205 musif-1.1.3/musif/extract/features/music21/constants.py
+-rw-r--r--   0        0        0     2182 2023-04-26 14:35:45.753205 musif-1.1.3/musif/extract/features/music21/handler.py
+-rw-r--r--   0        0        0     1919 2023-04-19 11:30:50.492972 musif-1.1.3/musif/extract/features/music21/handler.py~
+-rw-r--r--   0        0        0     3554 2023-04-19 09:14:37.176390 musif-1.1.3/musif/extract/features/prefix.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.176390 musif-1.1.3/musif/extract/features/rhythm/__init__.py
+-rw-r--r--   0        0        0      273 2023-04-19 09:15:49.953056 musif-1.1.3/musif/extract/features/rhythm/constants.py
+-rw-r--r--   0        0        0     5925 2023-04-26 14:35:45.753205 musif-1.1.3/musif/extract/features/rhythm/handler.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.176390 musif-1.1.3/musif/extract/features/scale/__init__.py
+-rw-r--r--   0        0        0      269 2023-04-26 14:35:45.753205 musif-1.1.3/musif/extract/features/scale/constants.py
+-rw-r--r--   0        0        0     3627 2023-04-19 09:15:49.953056 musif-1.1.3/musif/extract/features/scale/handler.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.176390 musif-1.1.3/musif/extract/features/scale_relative/__init__.py
+-rw-r--r--   0        0        0      102 2023-04-19 09:14:37.176390 musif-1.1.3/musif/extract/features/scale_relative/constants.py
+-rw-r--r--   0        0        0     2842 2023-04-19 09:15:49.953056 musif-1.1.3/musif/extract/features/scale_relative/handler.py
+-rw-r--r--   0        0        0     7321 2023-04-19 09:15:49.953056 musif-1.1.3/musif/extract/features/scale_relative/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.176390 musif-1.1.3/musif/extract/features/tempo/__init__.py
+-rw-r--r--   0        0        0      306 2023-04-19 09:14:37.176390 musif-1.1.3/musif/extract/features/tempo/constants.py
+-rw-r--r--   0        0        0     5145 2023-04-26 14:35:45.753205 musif-1.1.3/musif/extract/features/tempo/handler.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.176390 musif-1.1.3/musif/extract/features/texture/__init__.py
+-rw-r--r--   0        0        0       45 2023-04-19 09:14:37.176390 musif-1.1.3/musif/extract/features/texture/constants.py
+-rw-r--r--   0        0        0     3077 2023-04-19 09:15:49.953056 musif-1.1.3/musif/extract/features/texture/handler.py
+-rw-r--r--   0        0        0    21081 2023-04-26 14:35:45.753205 musif-1.1.3/musif/extract/utils.py
+-rw-r--r--   0        0        0     2011 2023-04-19 09:14:37.176390 musif-1.1.3/musif/logs.py
+-rw-r--r--   0        0        0       61 2023-04-19 09:15:49.953056 musif-1.1.3/musif/musescore/__init__.py
+-rw-r--r--   0        0        0      948 2023-04-19 09:14:37.176390 musif-1.1.3/musif/musescore/common.py
+-rw-r--r--   0        0        0       95 2023-04-19 09:15:49.953056 musif-1.1.3/musif/musescore/constants.py
+-rw-r--r--   0        0        0       91 2023-04-19 09:15:49.953056 musif-1.1.3/musif/musicxml/__init__.py
+-rw-r--r--   0        0        0     8391 2023-05-30 15:24:16.943315 musif-1.1.3/musif/musicxml/common.py
+-rw-r--r--   0        0        0    15310 2023-04-26 14:35:45.753205 musif-1.1.3/musif/musicxml/constants.py
+-rw-r--r--   0        0        0     2092 2023-04-19 09:15:49.953056 musif-1.1.3/musif/musicxml/key.py
+-rw-r--r--   0        0        0    17541 2023-04-19 09:14:37.179723 musif-1.1.3/musif/musicxml/repeat.py
+-rw-r--r--   0        0        0     4513 2023-04-26 14:35:45.753205 musif-1.1.3/musif/musicxml/scoring.py
+-rw-r--r--   0        0        0     8151 2023-04-26 14:35:45.753205 musif-1.1.3/musif/musicxml/tempo.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.179723 musif-1.1.3/musif/process/__init__.py
+-rw-r--r--   0        0        0      410 2023-04-19 09:15:49.953056 musif-1.1.3/musif/process/constants.py
+-rw-r--r--   0        0        0    11327 2023-04-26 14:35:45.756538 musif-1.1.3/musif/process/processor.py
+-rw-r--r--   0        0        0     7824 2023-04-26 14:35:45.756538 musif-1.1.3/musif/process/utils.py
+-rw-r--r--   0        0        0      650 2023-05-30 15:50:33.123269 musif-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2456 1970-01-01 00:00:00.000000 musif-1.1.3/PKG-INFO
```

### Comparing `musif-1.1.2/README.md` & `musif-1.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -16,19 +16,19 @@
  
 In case of problems when installing Java or getting it to work as a command, these sites might be helpful:
 https://www.theserverside.com/blog/Coffee-Talk-Java-News-Stories-and-Opinions/How-do-I-install-Java-on-Ubuntu
 https://www.wikihow.com/Set-Java-Home
 
 ## Changelog
 
-#### v1.1.2
+#### v1.1.1 - v1.1.3
 * fixed major bug with music21 automatic onversion to MIDI for jSymbolic features
-
-#### v1.1.1
 * added exception handling for jSymbolic
+* fixed repeats for MIDI conversion for jSymbolic
+* fixed initial anacrusis
 
 #### v1.1.0
 * bug fixing
 * improved musif parsing abilities for non-well formatted files
 * added option `ignore_errors` for ignoring errors while parsing large datasets
 * better file naming for cache
 * automatically removing unpitched objects (e.g. percussion symbols)
```

### Comparing `musif-1.1.2/musif/__main__.py` & `musif-1.1.3/musif/__main__.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/cache/cache.py` & `musif-1.1.3/musif/cache/cache.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/cache/utils.py` & `musif-1.1.3/musif/cache/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/common/_logs.py` & `musif-1.1.3/musif/common/_logs.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/common/_utils.py` & `musif-1.1.3/musif/common/_utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/common/constants.py` & `musif-1.1.3/musif/common/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/common/didone_utils.py` & `musif-1.1.3/musif/common/didone_utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/common/exceptions.py` & `musif-1.1.3/musif/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/common/sort.py` & `musif-1.1.3/musif/common/sort.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/common/translate.py` & `musif-1.1.3/musif/common/translate.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/config.py` & `musif-1.1.3/musif/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 WINDOW_SIZE = "window_size"
 OVERLAP = "overlap"
 PRECACHE_HOOKS = "precache_hooks"
 REMOVE_UNPITCHED_OBJECTS = "remove_unpitched_objects"
 MSCORE_EXEC = "mscore_exec"
 JSYMBOLIC_CONFIG_FILE = "jsymbolic_config_file"
 JSYMBOLIC_MAX_RAM = "jsymbolic_max_ram"
+JSYMBOLIC_TRY_WITHOUT_REPEATS = "jsymbolic_try_without_repeats"
 # Didone specific?
 SPLIT_KEYWORDS = "split_keywords"
 
 DELETE_FILES = "delete_failed_files"
 DELETE_HARMONY = "delete_files_without_harmony"
 UNBUNDLE_INSTRUMENTATION = "separate_intrumentation_column"
 INSTRUMENTS_TO_KEEP = "instruments_to_keep"
@@ -69,15 +70,16 @@
     EXPAND_REPEATS: False,
     WINDOW_SIZE: None,
     OVERLAP: 2,
     MSCORE_EXEC: None,
     DFS_DIR: None,
     REMOVE_UNPITCHED_OBJECTS: True,
     JSYMBOLIC_MAX_RAM: "4g",
-    JSYMBOLIC_CONFIG_FILE: None
+    JSYMBOLIC_CONFIG_FILE: None,
+    JSYMBOLIC_TRY_WITHOUT_REPEATS: False
 }
 
 _CONFIG_POST_FALLBACK = {
     DELETE_FILES: False,
     GROUPED: False,
     DELETE_FILES: False,
     DELETE_HARMONY: False,
```

### Comparing `musif-1.1.2/musif/extract/basic_modules/file_name_generic/handler.py` & `musif-1.1.3/musif/extract/basic_modules/file_name_generic/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/basic_modules/scoring/constants.py` & `musif-1.1.3/musif/extract/basic_modules/scoring/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/basic_modules/scoring/handler.py` & `musif-1.1.3/musif/extract/basic_modules/scoring/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/common.py` & `musif-1.1.3/musif/extract/common.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/constants.py` & `musif-1.1.3/musif/extract/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/extract.py` & `musif-1.1.3/musif/extract/extract.py~`

 * *Files 1% similar despite different names*

```diff
@@ -250,20 +250,20 @@
         )
         # self.regex = re.compile("from {FEATURES_MODULES}.([\w\.]+) import")
         # creates the directory for the cache
         if self._cfg.cache_dir is not None:
             pinfo("Cache activated!")
             Path(self._cfg.cache_dir).mkdir(exist_ok=True)
 
-        if "jsymbolic" in self._cfg.features:
+        if 'jsymbolic' in self._cfg.features:
             from musif.extract.features import jsymbolic
-
             jsymbolic.utils.download_jsymbolic()
             jsymbolic.utils.get_java_path()
 
+
     def extract(self) -> DataFrame:
         """
         Extracts features given in the configuration data getting a file, directory or several file paths,
         returning a DataFrame containing musical features.
 
         Returns
         ------
@@ -350,15 +350,15 @@
                 df_score = df_score.reindex(sorted(df_score.columns), axis=1)
                 df_score.replace("NA", pd.NA, inplace=True)
                 all_dfs.append(df_score)
             all_dfs = pd.concat(all_dfs, axis=0, keys=range(len(all_dfs)))
         else:
             all_dfs = DataFrame(scores_features)
             all_dfs = all_dfs.reindex(sorted(all_dfs.columns), axis=1)
-            all_dfs = all_dfs.replace("NA", pd.NA)
+            all_dfs = all_dfs.replace(pd.NA, "NA").replace("NA", pd.NA)
         return all_dfs
 
     def _init_score_processing(self, idx: int, filename: PurePath):
         if self._cfg.cache_dir is not None:
             cache_name = (
                 Path(self._cfg.cache_dir)
                 / filename.parent
@@ -450,18 +450,16 @@
 
     def _select_window_data(
         self, score_data: dict, parts_data: list, first_measure: int, last_measure: int
     ):
         window_score = score_data[C.DATA_SCORE].measures(
             first_measure, last_measure, indicesNotNumbers=True
         )
-        filtered_partNames = [i.partName for i in score_data["parts"]]
-        window_parts = [
-            i for i in window_score.parts if i.partName in filtered_partNames
-        ]
+        filtered_partNames = [i.partName for i in score_data['parts']]
+        window_parts = [i for i in window_score.parts if i.partName in filtered_partNames]
         if (
             self._cfg.is_requested_musescore_file()
             and score_data[C.DATA_MUSESCORE_SCORE] is not None
         ):
             window_mscore = score_data[C.DATA_MUSESCORE_SCORE].loc[
                 (score_data[C.DATA_MUSESCORE_SCORE]["mn"] <= last_measure)
                 & (score_data[C.DATA_MUSESCORE_SCORE]["mn"] >= first_measure)
```

### Comparing `musif-1.1.2/musif/extract/extract.py~` & `musif-1.1.3/musif/extract/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     cast_mixed_dtypes,
     extract_global_time_signature,
     process_musescore_file,
 )
 from musif.logs import ldebug, lerr, linfo, lwarn, pdebug, perr, pinfo
 from musif.musescore import constants as mscore_c
 from musif.musicxml import constants as musicxml_c
-from musif.musicxml import extract_numeric_tempo, name_parts, split_layers
+from musif.musicxml import extract_numeric_tempo, name_parts, split_layers, fix_repeats
 from musif.musicxml.scoring import (
     _extract_abbreviated_part,
     extract_sound,
     to_abbreviation,
 )
 
 _cache = FileCacheIntoRAM(10000)  # To cache scanned scores
@@ -76,27 +76,28 @@
      ParseFileError
        If the xml file can't be parsed for any reason.
     """
     score = _cache.get(file_path)
     if score is not None:
         return score
     try:
-        score = parse(file_path)
+        score = parse(file_path).makeRests()
         if export_dfs_to is not None:
             dest_path = Path(export_dfs_to)
             dest_path /= Path(file_path).with_suffix(".pkl").name
             store_score_df(score, dest_path)
         # give a name to all parts in the score
         name_parts(score)
         if remove_unpitched_objects:
             unpitched_objs = list(
                 score.flatten().getElementsByClass(["PercussionChord", "Unpitched"])
             )
             score.remove(unpitched_objs, recurse=True)
         split_layers(score, split_keywords)
+        fix_repeats(score)
         if expand_repeats:
             score = score.expandRepeats()
         _cache.put(file_path, score)
     except Exception as e:
         print(file_path)
         raise ParseFileError(file_path) from e
     return score
@@ -250,20 +251,20 @@
         )
         # self.regex = re.compile("from {FEATURES_MODULES}.([\w\.]+) import")
         # creates the directory for the cache
         if self._cfg.cache_dir is not None:
             pinfo("Cache activated!")
             Path(self._cfg.cache_dir).mkdir(exist_ok=True)
 
-        if 'jsymbolic' in self._cfg.features:
+        if "jsymbolic" in self._cfg.features:
             from musif.extract.features import jsymbolic
+
             jsymbolic.utils.download_jsymbolic()
             jsymbolic.utils.get_java_path()
 
-
     def extract(self) -> DataFrame:
         """
         Extracts features given in the configuration data getting a file, directory or several file paths,
         returning a DataFrame containing musical features.
 
         Returns
         ------
@@ -350,15 +351,15 @@
                 df_score = df_score.reindex(sorted(df_score.columns), axis=1)
                 df_score.replace("NA", pd.NA, inplace=True)
                 all_dfs.append(df_score)
             all_dfs = pd.concat(all_dfs, axis=0, keys=range(len(all_dfs)))
         else:
             all_dfs = DataFrame(scores_features)
             all_dfs = all_dfs.reindex(sorted(all_dfs.columns), axis=1)
-            all_dfs = all_dfs.replace(pd.NA, "NA").replace("NA", pd.NA)
+            all_dfs = all_dfs.replace("NA", pd.NA)
         return all_dfs
 
     def _init_score_processing(self, idx: int, filename: PurePath):
         if self._cfg.cache_dir is not None:
             cache_name = (
                 Path(self._cfg.cache_dir)
                 / filename.parent
@@ -450,16 +451,18 @@
 
     def _select_window_data(
         self, score_data: dict, parts_data: list, first_measure: int, last_measure: int
     ):
         window_score = score_data[C.DATA_SCORE].measures(
             first_measure, last_measure, indicesNotNumbers=True
         )
-        filtered_partNames = [i.partName for i in score_data['parts']]
-        window_parts = [i for i in window_score.parts if i.partName in filtered_partNames]
+        filtered_partNames = [i.partName for i in score_data["parts"]]
+        window_parts = [
+            i for i in window_score.parts if i.partName in filtered_partNames
+        ]
         if (
             self._cfg.is_requested_musescore_file()
             and score_data[C.DATA_MUSESCORE_SCORE] is not None
         ):
             window_mscore = score_data[C.DATA_MUSESCORE_SCORE].loc[
                 (score_data[C.DATA_MUSESCORE_SCORE]["mn"] <= last_measure)
                 & (score_data[C.DATA_MUSESCORE_SCORE]["mn"] >= first_measure)
```

### Comparing `musif-1.1.2/musif/extract/features/ambitus/handler.py` & `musif-1.1.3/musif/extract/features/ambitus/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/core/handler.py` & `musif-1.1.3/musif/extract/features/core/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/density/handler.py` & `musif-1.1.3/musif/extract/features/density/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/dynamics/constants.py` & `musif-1.1.3/musif/extract/features/dynamics/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/dynamics/handler.py` & `musif-1.1.3/musif/extract/features/dynamics/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/harmony/constants.py` & `musif-1.1.3/musif/extract/features/harmony/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/harmony/handler.py` & `musif-1.1.3/musif/extract/features/harmony/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/harmony/utils.py` & `musif-1.1.3/musif/extract/features/harmony/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/jsymbolic/handler.py` & `musif-1.1.3/musif/extract/features/jsymbolic/handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,49 +18,69 @@
 def get_tmpdir():
     if os.path.exists("/dev/shm"):
         return tempfile.TemporaryDirectory(dir="/dev/shm")
     else:
         return tempfile.TemporaryDirectory()
 
 
+def write_midi(score, midi_path):
+    with open(os.devnull, "w") as devnull:
+        with contextlib.redirect_stdout(devnull):
+            score.write("MIDI", midi_path)
+
+
 def update_score_objects(
     score_data: dict,
     parts_data: List[dict],
     cfg: ExtractConfiguration,
     parts_features: List[dict],
     score_features: dict,
 ):
+    score = score_data["score"]
     # 1. create a temporary directory (if Linux, force RAM usig /dev/shm)
     with get_tmpdir() as tmpdirname:
         # 2. convert the score to MEI usiing music21
         # TODO: if music21 implements export to MEI, use it
         midi_path = os.path.abspath(os.path.join(tmpdirname, "score.midi"))
         try:
-            with open(os.devnull, 'w') as devnull:
-                with contextlib.redirect_stdout(devnull):
-                    score_data['score'].write("MIDI", midi_path)
+            write_midi(score, midi_path)
         except Exception as e:
             filename = score_data[C.DATA_FILE]
-            pwarn(f"jSymbolic: could not convert {filename} to MIDI: {e}")
-            return
+            if cfg.jsymbolic_try_without_repeats:
+                found = False
+                for el in score.recurse().getElementsByClass("RepeatMark"):
+                    found = True
+                    # WARNING! this is not campatible with the cache system!
+                    score.remove(el, recurse=True)
+                if found:
+                    try:
+                        write_midi(score, midi_path)
+                    except Exception as e:
+                        pwarn(f"jsymbolic: could not convert {filename} to midi: {e}")
+                        return
+            if not cfg.jsymbolic_try_without_repeats or not found:
+                pwarn(f"jSymbolic: could not convert {filename} to MIDI: {e}")
+                return
 
-        # 3. run the MEI file through the jSymbolic jar savign csv into the temporary
+        # 3. run the MEI file through the jSymbolic jar saving csv into the temporary
         # directory in RAM
         out_path = os.path.abspath(os.path.join(tmpdirname, "features"))
-        cmd = [JAVA_PATH,
-               f"-Xmx{cfg.jsymbolic_max_ram}",
-               "-jar",
-               JSYMBOLIC_JAR,
-               "-csv",
-               ]
+        cmd = [
+            JAVA_PATH,
+            f"-Xmx{cfg.jsymbolic_max_ram}",
+            "-jar",
+            JSYMBOLIC_JAR,
+            "-csv",
+        ]
         if cfg.jsymbolic_config_file is not None:
             cmd += ["-configrun", cfg.jsymbolic_config_file]
         try:
             subprocess.run(
-                cmd + [
+                cmd
+                + [
                     midi_path,
                     out_path + ".xml",
                     out_path + "_def.xml",
                 ],
                 check=True,
                 stdout=subprocess.DEVNULL,
             )
@@ -70,14 +90,14 @@
             return
         # 4. read the csv file into a pandas dataframe
         df = pd.read_csv(out_path + ".csv", na_values=["NaN", " NaN", "NaN ", " NaN "])
         df = df.drop(columns=df.columns[0])
         # 5. add `js_` prefix to the column names
         df.columns = ["js_" + c for c in df.columns]
         # 6. load the features into the score_features dictionary
-        score_features.update(df.to_dict(orient='records')[0])
+        score_features.update(df.to_dict(orient="records")[0])
 
 
 def update_part_objects(
     score_data: dict, part_data: dict, cfg: ExtractConfiguration, part_features: dict
 ):
     pass
```

### Comparing `musif-1.1.2/musif/extract/features/jsymbolic/handler.py~` & `musif-1.1.3/musif/extract/features/jsymbolic/handler.py~`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/jsymbolic/utils.py` & `musif-1.1.3/musif/extract/features/jsymbolic/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/jsymbolic/utils.py~` & `musif-1.1.3/musif/extract/features/jsymbolic/utils.py~`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/key/handler.py` & `musif-1.1.3/musif/extract/features/key/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/lyrics/handler.py` & `musif-1.1.3/musif/extract/features/lyrics/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/melody/constants.py` & `musif-1.1.3/musif/extract/features/melody/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/melody/handler.py` & `musif-1.1.3/musif/extract/features/melody/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/music21/handler.py` & `musif-1.1.3/musif/extract/features/music21/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/music21/handler.py~` & `musif-1.1.3/musif/extract/features/music21/handler.py~`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/prefix.py` & `musif-1.1.3/musif/extract/features/prefix.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/rhythm/handler.py` & `musif-1.1.3/musif/extract/features/rhythm/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/scale/handler.py` & `musif-1.1.3/musif/extract/features/scale/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/scale_relative/handler.py` & `musif-1.1.3/musif/extract/features/scale_relative/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/scale_relative/utils.py` & `musif-1.1.3/musif/extract/features/scale_relative/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/tempo/handler.py` & `musif-1.1.3/musif/extract/features/tempo/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/features/texture/handler.py` & `musif-1.1.3/musif/extract/features/texture/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/extract/utils.py` & `musif-1.1.3/musif/extract/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/logs.py` & `musif-1.1.3/musif/logs.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/musescore/common.py` & `musif-1.1.3/musif/musescore/common.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/musicxml/common.py` & `musif-1.1.3/musif/musicxml/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from copy import deepcopy
 from typing import List, Tuple
+import itertools
 
 from music21.interval import Interval
 from music21.note import Note
 from music21.repeat import RepeatMark
 from music21.scale import MajorScale, MinorScale
 from music21.stream.base import Measure, Part, Score, Voice
 from music21.text import assembleLyrics
@@ -89,15 +90,15 @@
             else:
                 final_parts.append(part)  # without any change
                 score.remove(part)
         else:
             final_parts.append(part)  # without any change
             score.remove(part)
 
-    for part in final_parts:
+    for idx, part in enumerate(final_parts):
         try:
             score.insert(0, part)
         except Exception:
             pass
 
 
 def get_notes_and_measures(
@@ -132,17 +133,15 @@
     for measure in part.elements:
         # add missing information to both parts (dynamics, text annotations, etc are
         # missing)
         if isinstance(measure, Measure):
             num_measure += 1
             if any(not isinstance(e, Voice) for e in measure.elements):
                 not_voices_elements = [
-                    e
-                    for e in measure.elements
-                    if not isinstance(e, (RepeatMark, Voice))
+                    e for e in measure.elements if not isinstance(e, Voice)
                 ]  # elements such as clefs, dynamics, text annotations...
                 for p in parts_splitted:
                     if measure.measureNumber == 0 and isinstance(measure, Measure):
                         # number = measure.measureNumber+1
                         # only add elements if we are in am measure
                         if isinstance(p.elements[num_measure], Measure):
                             p.elements[num_measure].elements += tuple(
@@ -160,19 +159,14 @@
                         )
     for num, p in enumerate(parts_splitted, 1):
         p.id = part.id + " " + toRoman(num)  # only I or II
         p.partName = part.partName + " " + toRoman(num)  # only I or II
         # p.elements = p.elements
         final_parts.append(p)
 
-        # p_copy = copy.deepcopy(part)
-        # p_copy.id = p_copy.id + " " + toRoman(num)  # only I or II
-        # p_copy.partName = p_copy.partName + " " + toRoman(num)  # only I or II
-        # p_copy.elements = p.elements
-        # final_parts.append(p_copy)
     score.remove(part)
 
 
 def _get_part_clef(part):
     """
     Extracts the clef in the score by checking the first measure of the part
 
@@ -220,7 +214,31 @@
         if note.lyrics is None or len(note.lyrics) == 0:
             continue
         note_lyrics = [
             syllable.text for syllable in note.lyrics if syllable.text is not None
         ]
         lyrics.extend(note_lyrics)
     return lyrics
+
+
+def fix_repeats(score: Score):
+    """Fix the repeat sign in the score by ensuring that all the parts have
+    the same signs"""
+    signs = score.recurse().getElementsByClass("RepeatMark")
+    # measure_parts is an iterator, but successive loops won't restart from index
+    # 0 but from where the previous one was left
+    # for this, we use itertools.chain to force the creation of a proper
+    # iterator
+    measure_parts = [
+        itertools.chain(p.getElementsByClass("Measure")) for p in score.parts
+    ]
+    for sign in signs:
+        measure_sign = sign.activeSite
+        measure_sign_offset = measure_sign.offset
+        offset_sign = sign.offset
+        for measures in measure_parts:
+            for m in measures:
+                if m.offset == measure_sign_offset:
+                    marks = m.getElementsByClass("RepeatMark")
+                    if sign.__class__ not in [mark.__class__ for mark in marks]:
+                        m.insert(offset_sign, sign)
+                    break
```

### Comparing `musif-1.1.2/musif/musicxml/constants.py` & `musif-1.1.3/musif/musicxml/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/musicxml/key.py` & `musif-1.1.3/musif/musicxml/key.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/musicxml/repeat.py` & `musif-1.1.3/musif/musicxml/repeat.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/musicxml/scoring.py` & `musif-1.1.3/musif/musicxml/scoring.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/musicxml/tempo.py` & `musif-1.1.3/musif/musicxml/tempo.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/process/processor.py` & `musif-1.1.3/musif/process/processor.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/musif/process/utils.py` & `musif-1.1.3/musif/process/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.2/pyproject.toml` & `musif-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "roman>=3.3",
     "joblib>=1.0.0",
     "scipy>=1.6.0",
     "music21>=8,<9",
     "deepdiff>=6.2.1",
 ]
 name = "musif"
-version = "1.1.2"
+version = "1.1.3"
 description = "Music feature extraction library from the DIDONE project"
 authors = [
     { name = "Didone Project", email = "didone@iccmu.es" },
 ]
 requires-python = ">=3.10"
 readme = "README.md"
```

### Comparing `musif-1.1.2/PKG-INFO` & `musif-1.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musif
-Version: 1.1.2
+Version: 1.1.3
 Summary: Music feature extraction library from the DIDONE project
 License: MIT
 Author-email: Didone Project <didone@iccmu.es>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # musif
@@ -25,19 +25,19 @@
  
 In case of problems when installing Java or getting it to work as a command, these sites might be helpful:
 https://www.theserverside.com/blog/Coffee-Talk-Java-News-Stories-and-Opinions/How-do-I-install-Java-on-Ubuntu
 https://www.wikihow.com/Set-Java-Home
 
 ## Changelog
 
-#### v1.1.2
+#### v1.1.1 - v1.1.3
 * fixed major bug with music21 automatic onversion to MIDI for jSymbolic features
-
-#### v1.1.1
 * added exception handling for jSymbolic
+* fixed repeats for MIDI conversion for jSymbolic
+* fixed initial anacrusis
 
 #### v1.1.0
 * bug fixing
 * improved musif parsing abilities for non-well formatted files
 * added option `ignore_errors` for ignoring errors while parsing large datasets
 * better file naming for cache
 * automatically removing unpitched objects (e.g. percussion symbols)
```

