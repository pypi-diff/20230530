# Comparing `tmp/satellighte-0.2.4.tar.gz` & `tmp/satellighte-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satellighte-0.2.4.tar", last modified: Fri Sep 16 12:48:15 2022, max compression
+gzip compressed data, was "satellighte-0.2.5.tar", last modified: Tue May 30 07:26:35 2023, max compression
```

## Comparing `satellighte-0.2.4.tar` & `satellighte-0.2.5.tar`

### file list

```diff
@@ -1,67 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 12:48:15.937957 satellighte-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-09-16 12:47:06.000000 satellighte-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-16 12:47:06.000000 satellighte-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    15082 2022-09-16 12:48:15.937957 satellighte-0.2.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)    14300 2022-09-16 12:47:06.000000 satellighte-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-09-16 12:47:06.000000 satellighte-0.2.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 12:48:15.933956 satellighte-0.2.4/satellighte/
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/.config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 12:48:15.933956 satellighte-0.2.4/satellighte/api/
--rw-r--r--   0 runner    (1001) docker     (121)     2893 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 12:48:15.933956 satellighte-0.2.4/satellighte/archs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/archs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 12:48:15.933956 satellighte-0.2.4/satellighte/archs/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/archs/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 12:48:15.937957 satellighte-0.2.4/satellighte/archs/efficientnet/blocks/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/archs/efficientnet/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8051 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/archs/efficientnet/blocks/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (121)    13586 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/archs/efficientnet/blocks/layers.py
--rw-r--r--   0 runner    (1001) docker     (121)    12417 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/archs/efficientnet/module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 12:48:15.937957 satellighte-0.2.4/satellighte/archs/mobilenetv2/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/archs/mobilenetv2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 12:48:15.937957 satellighte-0.2.4/satellighte/archs/mobilenetv2/blocks/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/archs/mobilenetv2/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5630 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/archs/mobilenetv2/blocks/layers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4708 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/archs/mobilenetv2/blocks/mobilenetv2.py
--rw-r--r--   0 runner    (1001) docker     (121)     6542 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/archs/mobilenetv2/module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 12:48:15.937957 satellighte-0.2.4/satellighte/archs/resnet/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/archs/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 12:48:15.937957 satellighte-0.2.4/satellighte/archs/resnet/blocks/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/archs/resnet/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3965 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/archs/resnet/blocks/layers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3756 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/archs/resnet/blocks/resnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     8082 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/archs/resnet/module.py
--rw-r--r--   0 runner    (1001) docker     (121)     6431 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 12:48:15.937957 satellighte-0.2.4/satellighte/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4105 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/datasets/eurosat.py
--rw-r--r--   0 runner    (1001) docker     (121)     4047 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/datasets/resisc45.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 12:48:15.937957 satellighte-0.2.4/satellighte/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/models/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 12:48:15.937957 satellighte-0.2.4/satellighte/models/efficientnet_b0_eurosat/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/models/efficientnet_b0_eurosat/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 12:48:15.937957 satellighte-0.2.4/satellighte/models/efficientnet_b0_eurosat/v0/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/models/efficientnet_b0_eurosat/v0/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 12:48:15.937957 satellighte-0.2.4/satellighte/models/mobilenetv2_default_eurosat/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/models/mobilenetv2_default_eurosat/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 12:48:15.937957 satellighte-0.2.4/satellighte/models/mobilenetv2_default_eurosat/v0/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/models/mobilenetv2_default_eurosat/v0/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 12:48:15.937957 satellighte-0.2.4/satellighte/models/mobilenetv2_default_eurosat/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/models/mobilenetv2_default_eurosat/v1/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)    13467 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/module.py
--rw-r--r--   0 runner    (1001) docker     (121)     3639 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-09-16 12:47:06.000000 satellighte-0.2.4/satellighte/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 12:48:15.933956 satellighte-0.2.4/satellighte.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15082 2022-09-16 12:48:15.000000 satellighte-0.2.4/satellighte.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-09-16 12:48:15.000000 satellighte-0.2.4/satellighte.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-16 12:48:15.000000 satellighte-0.2.4/satellighte.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-09-16 12:48:15.000000 satellighte-0.2.4/satellighte.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-16 12:48:15.000000 satellighte-0.2.4/satellighte.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 12:48:15.937957 satellighte-0.2.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 12:47:06.000000 satellighte-0.2.4/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-09-16 12:47:06.000000 satellighte-0.2.4/scripts/release.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-16 12:48:15.937957 satellighte-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3922 2022-09-16 12:47:06.000000 satellighte-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.196066 satellighte-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-05-30 07:24:54.000000 satellighte-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-05-30 07:24:54.000000 satellighte-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    15374 2023-05-30 07:26:35.196066 satellighte-0.2.5/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (122)    14612 2023-05-30 07:24:54.000000 satellighte-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2023-05-30 07:24:54.000000 satellighte-0.2.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.184066 satellighte-0.2.5/satellighte/
+-rw-r--r--   0 runner    (1001) docker     (122)     1277 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.184066 satellighte-0.2.5/satellighte/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     2893 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.184066 satellighte-0.2.5/satellighte/archs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.184066 satellighte-0.2.5/satellighte/archs/coatnet/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/coatnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.184066 satellighte-0.2.5/satellighte/archs/coatnet/blocks/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/coatnet/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2511 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/coatnet/blocks/coatnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6587 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/coatnet/blocks/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8127 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/coatnet/module.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.188066 satellighte-0.2.5/satellighte/archs/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.188066 satellighte-0.2.5/satellighte/archs/efficientnet/blocks/
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/efficientnet/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8051 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/efficientnet/blocks/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13586 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/efficientnet/blocks/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12417 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/efficientnet/module.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.188066 satellighte-0.2.5/satellighte/archs/mobilenetv2/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/mobilenetv2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.192066 satellighte-0.2.5/satellighte/archs/mobilenetv2/blocks/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/mobilenetv2/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5630 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/mobilenetv2/blocks/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4708 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/mobilenetv2/blocks/mobilenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6542 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/mobilenetv2/module.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.192066 satellighte-0.2.5/satellighte/archs/resnet/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.192066 satellighte-0.2.5/satellighte/archs/resnet/blocks/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/resnet/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/resnet/blocks/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3756 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/resnet/blocks/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8082 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/archs/resnet/module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6431 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.192066 satellighte-0.2.5/satellighte/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4105 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/datasets/eurosat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4047 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/datasets/resisc45.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.192066 satellighte-0.2.5/satellighte/models/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/models/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.192066 satellighte-0.2.5/satellighte/models/efficientnet_b0_eurosat/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/models/efficientnet_b0_eurosat/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.192066 satellighte-0.2.5/satellighte/models/efficientnet_b0_eurosat/v0/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/models/efficientnet_b0_eurosat/v0/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.192066 satellighte-0.2.5/satellighte/models/mobilenetv2_default_eurosat/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/models/mobilenetv2_default_eurosat/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.192066 satellighte-0.2.5/satellighte/models/mobilenetv2_default_eurosat/v0/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/models/mobilenetv2_default_eurosat/v0/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.196066 satellighte-0.2.5/satellighte/models/mobilenetv2_default_eurosat/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/models/mobilenetv2_default_eurosat/v1/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (122)    13467 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3639 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-30 07:24:54.000000 satellighte-0.2.5/satellighte/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.184066 satellighte-0.2.5/satellighte.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    15374 2023-05-30 07:26:35.000000 satellighte-0.2.5/satellighte.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-05-30 07:26:35.000000 satellighte-0.2.5/satellighte.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 07:26:35.000000 satellighte-0.2.5/satellighte.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      919 2023-05-30 07:26:35.000000 satellighte-0.2.5/satellighte.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-30 07:26:35.000000 satellighte-0.2.5/satellighte.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:26:35.196066 satellighte-0.2.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 07:24:54.000000 satellighte-0.2.5/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1244 2023-05-30 07:24:54.000000 satellighte-0.2.5/scripts/release.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-30 07:26:35.196066 satellighte-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3922 2023-05-30 07:24:54.000000 satellighte-0.2.5/setup.py
```

### Comparing `satellighte-0.2.4/LICENSE` & `satellighte-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/PKG-INFO` & `satellighte-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: satellighte
-Version: 0.2.4
+Version: 0.2.5
 Summary: PyTorch Lightning Implementations of Recent Satellite Image Classification !
 Home-page: https://github.com/canturan10/satellighte
 Author: Oguzcan Turan
 Author-email: can.turan.10@gmail.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
@@ -167,18 +166,18 @@
 - [Arch Model with Random Weight Initialization](https://github.com/canturan10/satellighte/blob/master/satellighte/api/README.md#arch-model-with-random-weight-initialization)
 
 _For more information, please refer to the [APIs](https://github.com/canturan10/satellighte/blob/master/satellighte/api)_
 
 <!-- ARCHITECTURES -->
 ## Architectures
 
-- [x] [MobileNetV2](https://github.com/canturan10/satellighte/blob/master/satellighte/archs/README.md#mobilenetv2)
+- [x] [CoAtNet](https://github.com/canturan10/satellighte/blob/master/satellighte/archs/README.md#coatnet)
 - [x] [EfficientNet](https://github.com/canturan10/satellighte/blob/master/satellighte/archs/README.md#efficientnet)
+- [x] [MobileNetV2](https://github.com/canturan10/satellighte/blob/master/satellighte/archs/README.md#mobilenetv2)
 - [x] [ResNet](https://github.com/canturan10/satellighte/blob/master/satellighte/archs/README.md#resnet)
-- [ ] [CoAtNet](https://github.com/canturan10/satellighte/blob/master/satellighte/archs/README.md)
 
 _For more information, please refer to the [Architectures](https://github.com/canturan10/satellighte/blob/master/satellighte/archs)_
 
 <!-- DATASETS -->
 ## Datasets
 
 - [x] [EuroSAT](https://github.com/canturan10/satellighte/blob/master/satellighte/datasets/README.md#EuroSAT)
@@ -279,15 +278,15 @@
             </a>
         </td>
         <td align="center">
             <a href="https://github.com/canturan10">
                 <h3>
                     You ?
                 </h3>
-                <img src="https://raw.githubusercontent.com/canturan10/readme-template/master/src/you.png"
+                <img src="https://raw.githubusercontent.com/canturan10/satellighte/master/src/you_satellighte.png"
                     width="200px;" alt="Oğuzcan Turan" /><br>
                 <a href="#">
                     <img src="https://img.shields.io/badge/-Reserved%20Place-red?style=flat&logoColor=white"
                         width="110px;" alt="Reserved" />
                 </a>
             </a>
         </td>
@@ -317,14 +316,25 @@
 
 <!-- CITATIONS -->
 ## Citations
 
 <details>
   <summary>Click to expand!</summary>
 
+  ```BibTeX
+@misc{dai2021coatnet,
+      title={CoAtNet: Marrying Convolution and Attention for All Data Sizes},
+      author={Zihang Dai and Hanxiao Liu and Quoc V. Le and Mingxing Tan},
+      year={2021},
+      eprint={2106.04803},
+      archivePrefix={arXiv},
+      primaryClass={cs.CV}
+}
+```
+
   ```bibtex
 @article{DBLP:journals/corr/ChengHL17,
   author    = {Gong Cheng and
                Junwei Han and
                Xiaoqiang Lu},
   title     = {Remote Sensing Image Scene Classification: Benchmark and State of
                the Art},
@@ -421,9 +431,7 @@
 </details>
 
 ![-----------------------------------------------------](https://raw.githubusercontent.com/canturan10/readme-template/master/src/colored_4b.png)
 
 Give a ⭐️ if this project helped you!
 
 _This readme file is made using the [readme-template](https://github.com/canturan10/readme-template)_
-
-
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: satellighte Version: 0.2.4 Summary: PyTorch
+Metadata-Version: 2.1 Name: satellighte Version: 0.2.5 Summary: PyTorch
 Lightning Implementations of Recent Satellite Image Classification ! Home-page:
 https://github.com/canturan10/satellighte Author: Oguzcan Turan Author-email:
-can.turan.10@gmail.com License: MIT License Platform: UNKNOWN Classifier: Topic
-:: Scientific/Engineering :: Artificial Intelligence Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-test Provides-Extra: docs Provides-Extra: deploy Provides-Extra: all License-
-File: LICENSE
+can.turan.10@gmail.com License: MIT License Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: License :: OSI Approved ::
+MIT License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Requires-Python: >=3.8
+Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
+docs Provides-Extra: deploy Provides-Extra: all License-File: LICENSE
                 [https://img.buymeacoffee.com/button-api/?text=You_can_buy_me_a
 coffee&emoji=&slug=canturan10&button_colour=5F7FFF&font_colour=ffffff&font_family=Comic&outline_colour=000000&coffee_colour=FFDD00]
                                  [Satellighte]
                             ***** Satellighte *****
                     *** Satellite Image Classification ***
                            Website â¢ Docs â¢ Pypi
                                    Demo_Page
@@ -69,97 +68,100 @@
 blob/master/satellighte/api/README.md#model-with-random-weight-initialization)
    - [Pretrained Arch Model](https://github.com/canturan10/satellighte/blob/
   master/satellighte/api/README.md#pretrained-arch-model) - [Arch Model with
  Random Weight Initialization](https://github.com/canturan10/satellighte/blob/
 master/satellighte/api/README.md#arch-model-with-random-weight-initialization)
      _For more information, please refer to the [APIs](https://github.com/
  canturan10/satellighte/blob/master/satellighte/api)_  ## Architectures - [x]
+ [CoAtNet](https://github.com/canturan10/satellighte/blob/master/satellighte/
+ archs/README.md#coatnet) - [x] [EfficientNet](https://github.com/canturan10/
+   satellighte/blob/master/satellighte/archs/README.md#efficientnet) - [x]
      [MobileNetV2](https://github.com/canturan10/satellighte/blob/master/
-    satellighte/archs/README.md#mobilenetv2) - [x] [EfficientNet](https://
-       github.com/canturan10/satellighte/blob/master/satellighte/archs/
-     README.md#efficientnet) - [x] [ResNet](https://github.com/canturan10/
-  satellighte/blob/master/satellighte/archs/README.md#resnet) - [ ] [CoAtNet]
-   (https://github.com/canturan10/satellighte/blob/master/satellighte/archs/
-README.md) _For more information, please refer to the [Architectures](https://
-github.com/canturan10/satellighte/blob/master/satellighte/archs)_  ## Datasets
-    - [x] [EuroSAT](https://github.com/canturan10/satellighte/blob/master/
- satellighte/datasets/README.md#EuroSAT) - [x] [RESISC45](https://github.com/
- canturan10/satellighte/blob/master/satellighte/datasets/README.md) _For more
-  information, please refer to the [Datasets](https://github.com/canturan10/
-satellighte/blob/master/satellighte/datasets)_  ## Deployments - [x] [FastAPI]
-      (https://github.com/canturan10/satellighte/blob/master/deployment/
-README.md#fastapi) - [x] [ONNX](https://github.com/canturan10/satellighte/blob/
-   master/deployment/README.md#onnx) - [x] [DeepSparse](https://github.com/
-  canturan10/satellighte/blob/master/deployment/README.md#deepsparse) - [x]
-[TensorFlow](https://github.com/canturan10/satellighte/blob/master/deployment/
- README.md#tensorflow) - [x] [TensorFlow Lite](https://github.com/canturan10/
-    satellighte/blob/master/deployment/README.md#tensorflow-lite) _For more
- information, please refer to the [Deployment](https://github.com/canturan10/
-  satellighte/blob/master/deployment)_  ## Training To training, follow these
-     steps: For installing Satellighte, please refer to the [Installation]
- (#installation). ```bash python training/eurosat_training.py ``` For optional
-  arguments, ```bash python training/eurosat_training.py --help ```  ## Tests
-  During development, you might like to have tests run. Install dependencies
-     ```bash pip install -e ".[test]" ``` ### Linting Tests ```bash pytest
-  satellighte --pylint --pylint-error-types=EF ``` ### Document Tests ```bash
- pytest satellighte --doctest-modules ``` ### Coverage Tests ```bash pytest --
-  doctest-modules --cov satellighte --cov-report term ```  ## Contributing To
- contribute to `Satellighte`, follow these steps: 1. Fork this repository. 2.
-Create a branch: `git checkout -b `. 3. Make your changes and commit them: `git
- commit -m ''` 4. Push to the original branch: `git push origin` 5. Create the
-pull request. Alternatively see the `GitHub` documentation on [creating a pull
-request](https://help.github.com/en/github/collaborating-with-issues-and-pull-
-              requests/creating-a-pull-request).  ## Contributors
+  satellighte/archs/README.md#mobilenetv2) - [x] [ResNet](https://github.com/
+  canturan10/satellighte/blob/master/satellighte/archs/README.md#resnet) _For
+   more information, please refer to the [Architectures](https://github.com/
+  canturan10/satellighte/blob/master/satellighte/archs)_  ## Datasets - [x]
+ [EuroSAT](https://github.com/canturan10/satellighte/blob/master/satellighte/
+  datasets/README.md#EuroSAT) - [x] [RESISC45](https://github.com/canturan10/
+satellighte/blob/master/satellighte/datasets/README.md) _For more information,
+please refer to the [Datasets](https://github.com/canturan10/satellighte/blob/
+    master/satellighte/datasets)_  ## Deployments - [x] [FastAPI](https://
+github.com/canturan10/satellighte/blob/master/deployment/README.md#fastapi) -
+ [x] [ONNX](https://github.com/canturan10/satellighte/blob/master/deployment/
+ README.md#onnx) - [x] [DeepSparse](https://github.com/canturan10/satellighte/
+   blob/master/deployment/README.md#deepsparse) - [x] [TensorFlow](https://
+github.com/canturan10/satellighte/blob/master/deployment/README.md#tensorflow)
+- [x] [TensorFlow Lite](https://github.com/canturan10/satellighte/blob/master/
+ deployment/README.md#tensorflow-lite) _For more information, please refer to
+    the [Deployment](https://github.com/canturan10/satellighte/blob/master/
+   deployment)_  ## Training To training, follow these steps: For installing
+Satellighte, please refer to the [Installation](#installation). ```bash python
+    training/eurosat_training.py ``` For optional arguments, ```bash python
+training/eurosat_training.py --help ```  ## Tests During development, you might
+ like to have tests run. Install dependencies ```bash pip install -e ".[test]"
+   ``` ### Linting Tests ```bash pytest satellighte --pylint --pylint-error-
+ types=EF ``` ### Document Tests ```bash pytest satellighte --doctest-modules
+ ``` ### Coverage Tests ```bash pytest --doctest-modules --cov satellighte --
+  cov-report term ```  ## Contributing To contribute to `Satellighte`, follow
+ these steps: 1. Fork this repository. 2. Create a branch: `git checkout -b `.
+    3. Make your changes and commit them: `git commit -m ''` 4. Push to the
+ original branch: `git push origin` 5. Create the pull request. Alternatively
+     see the `GitHub` documentation on [creating a pull request](https://
+help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-
+                       a-pull-request).  ## Contributors
                   ****_OÄuzcan_Turan_**** ****_You_?_****
                       [OÄuzcan_Turan]     [OÄuzcan_Turan]
                    [Linkedin]_[Portfolio]       [Reserved]
            ## Contact If you want to contact me you can reach me at
    [can.turan.10@gmail.com](mailto:can.turan.10@gmail.com).  ## License This
   project is licensed under `MIT` license. See [`LICENSE`](LICENSE) for more
    information.  ## References The references used in the development of the
  project are as follows. - [Img Shields](https://shields.io) - [GitHub Pages]
    (https://pages.github.com) - [FastFace](https://github.com/borhanMorphy/
  fastface) - [PyTorch Lightning](https://github.com/PyTorchLightning/pytorch-
   lightning) - [Torchvision](https://github.com/pytorch/vision)  ## Citations
-  Click to expand! ```bibtex @article{DBLP:journals/corr/ChengHL17, author =
-  {Gong Cheng and Junwei Han and Xiaoqiang Lu}, title = {Remote Sensing Image
-Scene Classification: Benchmark and State of the Art}, journal = {CoRR}, volume
-  = {abs/1703.00121}, year = {2017}, url = {http://arxiv.org/abs/1703.00121},
-eprinttype = {arXiv}, eprint = {1703.00121}, timestamp = {Mon, 02 Dec 2019 09:
-  32:19 +0100}, biburl = {https://dblp.org/rec/journals/corr/ChengHL17.bib},
-   bibsource = {dblp computer science bibliography, https://dblp.org} } ```
-```bibtex @article{helber2019eurosat, title={Eurosat: A novel dataset and deep
-learning benchmark for land use and land cover classification}, author={Helber,
-Patrick and Bischke, Benjamin and Dengel, Andreas and Borth, Damian}, journal=
-   {IEEE Journal of Selected Topics in Applied Earth Observations and Remote
-    Sensing}, year={2019}, publisher={IEEE} } ``` ```bibtex @inproceedings
- {helber2018introducing, title={Introducing EuroSAT: A Novel Dataset and Deep
-Learning Benchmark for Land Use and Land Cover Classification}, author={Helber,
-     Patrick and Bischke, Benjamin and Dengel, Andreas and Borth, Damian},
- booktitle={IGARSS 2018-2018 IEEE International Geoscience and Remote Sensing
-Symposium}, pages={204--207}, year={2018}, organization={IEEE} } ``` ```bibtex
- @article{DBLP:journals/corr/abs-1801-04381, author = {Mark Sandler and Andrew
-G. Howard and Menglong Zhu and Andrey Zhmoginov and Liang{-}Chieh Chen}, title
-       = {Inverted Residuals and Linear Bottlenecks: Mobile Networks for
- Classification, Detection and Segmentation}, journal = {CoRR}, volume = {abs/
-     1801.04381}, year = {2018}, url = {http://arxiv.org/abs/1801.04381},
- archivePrefix = {arXiv}, eprint = {1801.04381}, timestamp = {Tue, 12 Jan 2021
-    15:30:06 +0100}, biburl = {https://dblp.org/rec/journals/corr/abs-1801-
-04381.bib}, bibsource = {dblp computer science bibliography, https://dblp.org}
-} ``` ```BibTeX @article{DBLP:journals/corr/abs-1905-11946, author = {Mingxing
-   Tan and Quoc V. Le}, title = {EfficientNet: Rethinking Model Scaling for
- Convolutional Neural Networks}, journal = {CoRR}, volume = {abs/1905.11946},
- year = {2019}, url = {http://arxiv.org/abs/1905.11946}, eprinttype = {arXiv},
-eprint = {1905.11946}, timestamp = {Mon, 03 Jun 2019 13:42:33 +0200}, biburl =
-  {https://dblp.org/rec/journals/corr/abs-1905-11946.bib}, bibsource = {dblp
-computer science bibliography, https://dblp.org} } ``` ```BibTeX @article{DBLP:
-journals/corr/HeZRS15, author = {Kaiming He and Xiangyu Zhang and Shaoqing Ren
-and Jian Sun}, title = {Deep Residual Learning for Image Recognition}, journal
- = {CoRR}, volume = {abs/1512.03385}, year = {2015}, url = {http://arxiv.org/
-abs/1512.03385}, eprinttype = {arXiv}, eprint = {1512.03385}, timestamp = {Wed,
-  17 Apr 2019 17:23:45 +0200}, biburl = {https://dblp.org/rec/journals/corr/
-    HeZRS15.bib}, bibsource = {dblp computer science bibliography, https://
-   dblp.org} } ```  ![-----------------------------------------------------]
-   (https://raw.githubusercontent.com/canturan10/readme-template/master/src/
-colored_4b.png) Give a â­ï¸ if this project helped you! _This readme file is
-    made using the [readme-template](https://github.com/canturan10/readme-
-                                  template)_
+   Click to expand! ```BibTeX @misc{dai2021coatnet, title={CoAtNet: Marrying
+ Convolution and Attention for All Data Sizes}, author={Zihang Dai and Hanxiao
+    Liu and Quoc V. Le and Mingxing Tan}, year={2021}, eprint={2106.04803},
+  archivePrefix={arXiv}, primaryClass={cs.CV} } ``` ```bibtex @article{DBLP:
+journals/corr/ChengHL17, author = {Gong Cheng and Junwei Han and Xiaoqiang Lu},
+title = {Remote Sensing Image Scene Classification: Benchmark and State of the
+Art}, journal = {CoRR}, volume = {abs/1703.00121}, year = {2017}, url = {http:/
+   /arxiv.org/abs/1703.00121}, eprinttype = {arXiv}, eprint = {1703.00121},
+timestamp = {Mon, 02 Dec 2019 09:32:19 +0100}, biburl = {https://dblp.org/rec/
+journals/corr/ChengHL17.bib}, bibsource = {dblp computer science bibliography,
+https://dblp.org} } ``` ```bibtex @article{helber2019eurosat, title={Eurosat: A
+     novel dataset and deep learning benchmark for land use and land cover
+  classification}, author={Helber, Patrick and Bischke, Benjamin and Dengel,
+Andreas and Borth, Damian}, journal={IEEE Journal of Selected Topics in Applied
+  Earth Observations and Remote Sensing}, year={2019}, publisher={IEEE} } ```
+ ```bibtex @inproceedings{helber2018introducing, title={Introducing EuroSAT: A
+     Novel Dataset and Deep Learning Benchmark for Land Use and Land Cover
+  Classification}, author={Helber, Patrick and Bischke, Benjamin and Dengel,
+  Andreas and Borth, Damian}, booktitle={IGARSS 2018-2018 IEEE International
+   Geoscience and Remote Sensing Symposium}, pages={204--207}, year={2018},
+organization={IEEE} } ``` ```bibtex @article{DBLP:journals/corr/abs-1801-04381,
+    author = {Mark Sandler and Andrew G. Howard and Menglong Zhu and Andrey
+   Zhmoginov and Liang{-}Chieh Chen}, title = {Inverted Residuals and Linear
+ Bottlenecks: Mobile Networks for Classification, Detection and Segmentation},
+  journal = {CoRR}, volume = {abs/1801.04381}, year = {2018}, url = {http://
+  arxiv.org/abs/1801.04381}, archivePrefix = {arXiv}, eprint = {1801.04381},
+timestamp = {Tue, 12 Jan 2021 15:30:06 +0100}, biburl = {https://dblp.org/rec/
+     journals/corr/abs-1801-04381.bib}, bibsource = {dblp computer science
+ bibliography, https://dblp.org} } ``` ```BibTeX @article{DBLP:journals/corr/
+abs-1905-11946, author = {Mingxing Tan and Quoc V. Le}, title = {EfficientNet:
+Rethinking Model Scaling for Convolutional Neural Networks}, journal = {CoRR},
+    volume = {abs/1905.11946}, year = {2019}, url = {http://arxiv.org/abs/
+1905.11946}, eprinttype = {arXiv}, eprint = {1905.11946}, timestamp = {Mon, 03
+  Jun 2019 13:42:33 +0200}, biburl = {https://dblp.org/rec/journals/corr/abs-
+  1905-11946.bib}, bibsource = {dblp computer science bibliography, https://
+   dblp.org} } ``` ```BibTeX @article{DBLP:journals/corr/HeZRS15, author =
+  {Kaiming He and Xiangyu Zhang and Shaoqing Ren and Jian Sun}, title = {Deep
+  Residual Learning for Image Recognition}, journal = {CoRR}, volume = {abs/
+1512.03385}, year = {2015}, url = {http://arxiv.org/abs/1512.03385}, eprinttype
+   = {arXiv}, eprint = {1512.03385}, timestamp = {Wed, 17 Apr 2019 17:23:45
++0200}, biburl = {https://dblp.org/rec/journals/corr/HeZRS15.bib}, bibsource =
+{dblp computer science bibliography, https://dblp.org} } ```  ![---------------
+  --------------------------------------](https://raw.githubusercontent.com/
+  canturan10/readme-template/master/src/colored_4b.png) Give a â­ï¸ if this
+   project helped you! _This readme file is made using the [readme-template]
+               (https://github.com/canturan10/readme-template)_
```

### Comparing `satellighte-0.2.4/README.md` & `satellighte-0.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -144,18 +144,18 @@
 - [Arch Model with Random Weight Initialization](https://github.com/canturan10/satellighte/blob/master/satellighte/api/README.md#arch-model-with-random-weight-initialization)
 
 _For more information, please refer to the [APIs](https://github.com/canturan10/satellighte/blob/master/satellighte/api)_
 
 <!-- ARCHITECTURES -->
 ## Architectures
 
-- [x] [MobileNetV2](https://github.com/canturan10/satellighte/blob/master/satellighte/archs/README.md#mobilenetv2)
+- [x] [CoAtNet](https://github.com/canturan10/satellighte/blob/master/satellighte/archs/README.md#coatnet)
 - [x] [EfficientNet](https://github.com/canturan10/satellighte/blob/master/satellighte/archs/README.md#efficientnet)
+- [x] [MobileNetV2](https://github.com/canturan10/satellighte/blob/master/satellighte/archs/README.md#mobilenetv2)
 - [x] [ResNet](https://github.com/canturan10/satellighte/blob/master/satellighte/archs/README.md#resnet)
-- [ ] [CoAtNet](https://github.com/canturan10/satellighte/blob/master/satellighte/archs/README.md)
 
 _For more information, please refer to the [Architectures](https://github.com/canturan10/satellighte/blob/master/satellighte/archs)_
 
 <!-- DATASETS -->
 ## Datasets
 
 - [x] [EuroSAT](https://github.com/canturan10/satellighte/blob/master/satellighte/datasets/README.md#EuroSAT)
@@ -256,15 +256,15 @@
             </a>
         </td>
         <td align="center">
             <a href="https://github.com/canturan10">
                 <h3>
                     You ?
                 </h3>
-                <img src="https://raw.githubusercontent.com/canturan10/readme-template/master/src/you.png"
+                <img src="https://raw.githubusercontent.com/canturan10/satellighte/master/src/you_satellighte.png"
                     width="200px;" alt="Oğuzcan Turan" /><br>
                 <a href="#">
                     <img src="https://img.shields.io/badge/-Reserved%20Place-red?style=flat&logoColor=white"
                         width="110px;" alt="Reserved" />
                 </a>
             </a>
         </td>
@@ -294,14 +294,25 @@
 
 <!-- CITATIONS -->
 ## Citations
 
 <details>
   <summary>Click to expand!</summary>
 
+  ```BibTeX
+@misc{dai2021coatnet,
+      title={CoAtNet: Marrying Convolution and Attention for All Data Sizes},
+      author={Zihang Dai and Hanxiao Liu and Quoc V. Le and Mingxing Tan},
+      year={2021},
+      eprint={2106.04803},
+      archivePrefix={arXiv},
+      primaryClass={cs.CV}
+}
+```
+
   ```bibtex
 @article{DBLP:journals/corr/ChengHL17,
   author    = {Gong Cheng and
                Junwei Han and
                Xiaoqiang Lu},
   title     = {Remote Sensing Image Scene Classification: Benchmark and State of
                the Art},
```

#### html2text {}

```diff
@@ -58,97 +58,100 @@
 blob/master/satellighte/api/README.md#model-with-random-weight-initialization)
    - [Pretrained Arch Model](https://github.com/canturan10/satellighte/blob/
   master/satellighte/api/README.md#pretrained-arch-model) - [Arch Model with
  Random Weight Initialization](https://github.com/canturan10/satellighte/blob/
 master/satellighte/api/README.md#arch-model-with-random-weight-initialization)
      _For more information, please refer to the [APIs](https://github.com/
  canturan10/satellighte/blob/master/satellighte/api)_  ## Architectures - [x]
+ [CoAtNet](https://github.com/canturan10/satellighte/blob/master/satellighte/
+ archs/README.md#coatnet) - [x] [EfficientNet](https://github.com/canturan10/
+   satellighte/blob/master/satellighte/archs/README.md#efficientnet) - [x]
      [MobileNetV2](https://github.com/canturan10/satellighte/blob/master/
-    satellighte/archs/README.md#mobilenetv2) - [x] [EfficientNet](https://
-       github.com/canturan10/satellighte/blob/master/satellighte/archs/
-     README.md#efficientnet) - [x] [ResNet](https://github.com/canturan10/
-  satellighte/blob/master/satellighte/archs/README.md#resnet) - [ ] [CoAtNet]
-   (https://github.com/canturan10/satellighte/blob/master/satellighte/archs/
-README.md) _For more information, please refer to the [Architectures](https://
-github.com/canturan10/satellighte/blob/master/satellighte/archs)_  ## Datasets
-    - [x] [EuroSAT](https://github.com/canturan10/satellighte/blob/master/
- satellighte/datasets/README.md#EuroSAT) - [x] [RESISC45](https://github.com/
- canturan10/satellighte/blob/master/satellighte/datasets/README.md) _For more
-  information, please refer to the [Datasets](https://github.com/canturan10/
-satellighte/blob/master/satellighte/datasets)_  ## Deployments - [x] [FastAPI]
-      (https://github.com/canturan10/satellighte/blob/master/deployment/
-README.md#fastapi) - [x] [ONNX](https://github.com/canturan10/satellighte/blob/
-   master/deployment/README.md#onnx) - [x] [DeepSparse](https://github.com/
-  canturan10/satellighte/blob/master/deployment/README.md#deepsparse) - [x]
-[TensorFlow](https://github.com/canturan10/satellighte/blob/master/deployment/
- README.md#tensorflow) - [x] [TensorFlow Lite](https://github.com/canturan10/
-    satellighte/blob/master/deployment/README.md#tensorflow-lite) _For more
- information, please refer to the [Deployment](https://github.com/canturan10/
-  satellighte/blob/master/deployment)_  ## Training To training, follow these
-     steps: For installing Satellighte, please refer to the [Installation]
- (#installation). ```bash python training/eurosat_training.py ``` For optional
-  arguments, ```bash python training/eurosat_training.py --help ```  ## Tests
-  During development, you might like to have tests run. Install dependencies
-     ```bash pip install -e ".[test]" ``` ### Linting Tests ```bash pytest
-  satellighte --pylint --pylint-error-types=EF ``` ### Document Tests ```bash
- pytest satellighte --doctest-modules ``` ### Coverage Tests ```bash pytest --
-  doctest-modules --cov satellighte --cov-report term ```  ## Contributing To
- contribute to `Satellighte`, follow these steps: 1. Fork this repository. 2.
-Create a branch: `git checkout -b `. 3. Make your changes and commit them: `git
- commit -m ''` 4. Push to the original branch: `git push origin` 5. Create the
-pull request. Alternatively see the `GitHub` documentation on [creating a pull
-request](https://help.github.com/en/github/collaborating-with-issues-and-pull-
-              requests/creating-a-pull-request).  ## Contributors
+  satellighte/archs/README.md#mobilenetv2) - [x] [ResNet](https://github.com/
+  canturan10/satellighte/blob/master/satellighte/archs/README.md#resnet) _For
+   more information, please refer to the [Architectures](https://github.com/
+  canturan10/satellighte/blob/master/satellighte/archs)_  ## Datasets - [x]
+ [EuroSAT](https://github.com/canturan10/satellighte/blob/master/satellighte/
+  datasets/README.md#EuroSAT) - [x] [RESISC45](https://github.com/canturan10/
+satellighte/blob/master/satellighte/datasets/README.md) _For more information,
+please refer to the [Datasets](https://github.com/canturan10/satellighte/blob/
+    master/satellighte/datasets)_  ## Deployments - [x] [FastAPI](https://
+github.com/canturan10/satellighte/blob/master/deployment/README.md#fastapi) -
+ [x] [ONNX](https://github.com/canturan10/satellighte/blob/master/deployment/
+ README.md#onnx) - [x] [DeepSparse](https://github.com/canturan10/satellighte/
+   blob/master/deployment/README.md#deepsparse) - [x] [TensorFlow](https://
+github.com/canturan10/satellighte/blob/master/deployment/README.md#tensorflow)
+- [x] [TensorFlow Lite](https://github.com/canturan10/satellighte/blob/master/
+ deployment/README.md#tensorflow-lite) _For more information, please refer to
+    the [Deployment](https://github.com/canturan10/satellighte/blob/master/
+   deployment)_  ## Training To training, follow these steps: For installing
+Satellighte, please refer to the [Installation](#installation). ```bash python
+    training/eurosat_training.py ``` For optional arguments, ```bash python
+training/eurosat_training.py --help ```  ## Tests During development, you might
+ like to have tests run. Install dependencies ```bash pip install -e ".[test]"
+   ``` ### Linting Tests ```bash pytest satellighte --pylint --pylint-error-
+ types=EF ``` ### Document Tests ```bash pytest satellighte --doctest-modules
+ ``` ### Coverage Tests ```bash pytest --doctest-modules --cov satellighte --
+  cov-report term ```  ## Contributing To contribute to `Satellighte`, follow
+ these steps: 1. Fork this repository. 2. Create a branch: `git checkout -b `.
+    3. Make your changes and commit them: `git commit -m ''` 4. Push to the
+ original branch: `git push origin` 5. Create the pull request. Alternatively
+     see the `GitHub` documentation on [creating a pull request](https://
+help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-
+                       a-pull-request).  ## Contributors
                   ****_OÄuzcan_Turan_**** ****_You_?_****
                       [OÄuzcan_Turan]     [OÄuzcan_Turan]
                    [Linkedin]_[Portfolio]       [Reserved]
            ## Contact If you want to contact me you can reach me at
    [can.turan.10@gmail.com](mailto:can.turan.10@gmail.com).  ## License This
   project is licensed under `MIT` license. See [`LICENSE`](LICENSE) for more
    information.  ## References The references used in the development of the
  project are as follows. - [Img Shields](https://shields.io) - [GitHub Pages]
    (https://pages.github.com) - [FastFace](https://github.com/borhanMorphy/
  fastface) - [PyTorch Lightning](https://github.com/PyTorchLightning/pytorch-
   lightning) - [Torchvision](https://github.com/pytorch/vision)  ## Citations
-  Click to expand! ```bibtex @article{DBLP:journals/corr/ChengHL17, author =
-  {Gong Cheng and Junwei Han and Xiaoqiang Lu}, title = {Remote Sensing Image
-Scene Classification: Benchmark and State of the Art}, journal = {CoRR}, volume
-  = {abs/1703.00121}, year = {2017}, url = {http://arxiv.org/abs/1703.00121},
-eprinttype = {arXiv}, eprint = {1703.00121}, timestamp = {Mon, 02 Dec 2019 09:
-  32:19 +0100}, biburl = {https://dblp.org/rec/journals/corr/ChengHL17.bib},
-   bibsource = {dblp computer science bibliography, https://dblp.org} } ```
-```bibtex @article{helber2019eurosat, title={Eurosat: A novel dataset and deep
-learning benchmark for land use and land cover classification}, author={Helber,
-Patrick and Bischke, Benjamin and Dengel, Andreas and Borth, Damian}, journal=
-   {IEEE Journal of Selected Topics in Applied Earth Observations and Remote
-    Sensing}, year={2019}, publisher={IEEE} } ``` ```bibtex @inproceedings
- {helber2018introducing, title={Introducing EuroSAT: A Novel Dataset and Deep
-Learning Benchmark for Land Use and Land Cover Classification}, author={Helber,
-     Patrick and Bischke, Benjamin and Dengel, Andreas and Borth, Damian},
- booktitle={IGARSS 2018-2018 IEEE International Geoscience and Remote Sensing
-Symposium}, pages={204--207}, year={2018}, organization={IEEE} } ``` ```bibtex
- @article{DBLP:journals/corr/abs-1801-04381, author = {Mark Sandler and Andrew
-G. Howard and Menglong Zhu and Andrey Zhmoginov and Liang{-}Chieh Chen}, title
-       = {Inverted Residuals and Linear Bottlenecks: Mobile Networks for
- Classification, Detection and Segmentation}, journal = {CoRR}, volume = {abs/
-     1801.04381}, year = {2018}, url = {http://arxiv.org/abs/1801.04381},
- archivePrefix = {arXiv}, eprint = {1801.04381}, timestamp = {Tue, 12 Jan 2021
-    15:30:06 +0100}, biburl = {https://dblp.org/rec/journals/corr/abs-1801-
-04381.bib}, bibsource = {dblp computer science bibliography, https://dblp.org}
-} ``` ```BibTeX @article{DBLP:journals/corr/abs-1905-11946, author = {Mingxing
-   Tan and Quoc V. Le}, title = {EfficientNet: Rethinking Model Scaling for
- Convolutional Neural Networks}, journal = {CoRR}, volume = {abs/1905.11946},
- year = {2019}, url = {http://arxiv.org/abs/1905.11946}, eprinttype = {arXiv},
-eprint = {1905.11946}, timestamp = {Mon, 03 Jun 2019 13:42:33 +0200}, biburl =
-  {https://dblp.org/rec/journals/corr/abs-1905-11946.bib}, bibsource = {dblp
-computer science bibliography, https://dblp.org} } ``` ```BibTeX @article{DBLP:
-journals/corr/HeZRS15, author = {Kaiming He and Xiangyu Zhang and Shaoqing Ren
-and Jian Sun}, title = {Deep Residual Learning for Image Recognition}, journal
- = {CoRR}, volume = {abs/1512.03385}, year = {2015}, url = {http://arxiv.org/
-abs/1512.03385}, eprinttype = {arXiv}, eprint = {1512.03385}, timestamp = {Wed,
-  17 Apr 2019 17:23:45 +0200}, biburl = {https://dblp.org/rec/journals/corr/
-    HeZRS15.bib}, bibsource = {dblp computer science bibliography, https://
-   dblp.org} } ```  ![-----------------------------------------------------]
-   (https://raw.githubusercontent.com/canturan10/readme-template/master/src/
-colored_4b.png) Give a â­ï¸ if this project helped you! _This readme file is
-    made using the [readme-template](https://github.com/canturan10/readme-
-                                  template)_
+   Click to expand! ```BibTeX @misc{dai2021coatnet, title={CoAtNet: Marrying
+ Convolution and Attention for All Data Sizes}, author={Zihang Dai and Hanxiao
+    Liu and Quoc V. Le and Mingxing Tan}, year={2021}, eprint={2106.04803},
+  archivePrefix={arXiv}, primaryClass={cs.CV} } ``` ```bibtex @article{DBLP:
+journals/corr/ChengHL17, author = {Gong Cheng and Junwei Han and Xiaoqiang Lu},
+title = {Remote Sensing Image Scene Classification: Benchmark and State of the
+Art}, journal = {CoRR}, volume = {abs/1703.00121}, year = {2017}, url = {http:/
+   /arxiv.org/abs/1703.00121}, eprinttype = {arXiv}, eprint = {1703.00121},
+timestamp = {Mon, 02 Dec 2019 09:32:19 +0100}, biburl = {https://dblp.org/rec/
+journals/corr/ChengHL17.bib}, bibsource = {dblp computer science bibliography,
+https://dblp.org} } ``` ```bibtex @article{helber2019eurosat, title={Eurosat: A
+     novel dataset and deep learning benchmark for land use and land cover
+  classification}, author={Helber, Patrick and Bischke, Benjamin and Dengel,
+Andreas and Borth, Damian}, journal={IEEE Journal of Selected Topics in Applied
+  Earth Observations and Remote Sensing}, year={2019}, publisher={IEEE} } ```
+ ```bibtex @inproceedings{helber2018introducing, title={Introducing EuroSAT: A
+     Novel Dataset and Deep Learning Benchmark for Land Use and Land Cover
+  Classification}, author={Helber, Patrick and Bischke, Benjamin and Dengel,
+  Andreas and Borth, Damian}, booktitle={IGARSS 2018-2018 IEEE International
+   Geoscience and Remote Sensing Symposium}, pages={204--207}, year={2018},
+organization={IEEE} } ``` ```bibtex @article{DBLP:journals/corr/abs-1801-04381,
+    author = {Mark Sandler and Andrew G. Howard and Menglong Zhu and Andrey
+   Zhmoginov and Liang{-}Chieh Chen}, title = {Inverted Residuals and Linear
+ Bottlenecks: Mobile Networks for Classification, Detection and Segmentation},
+  journal = {CoRR}, volume = {abs/1801.04381}, year = {2018}, url = {http://
+  arxiv.org/abs/1801.04381}, archivePrefix = {arXiv}, eprint = {1801.04381},
+timestamp = {Tue, 12 Jan 2021 15:30:06 +0100}, biburl = {https://dblp.org/rec/
+     journals/corr/abs-1801-04381.bib}, bibsource = {dblp computer science
+ bibliography, https://dblp.org} } ``` ```BibTeX @article{DBLP:journals/corr/
+abs-1905-11946, author = {Mingxing Tan and Quoc V. Le}, title = {EfficientNet:
+Rethinking Model Scaling for Convolutional Neural Networks}, journal = {CoRR},
+    volume = {abs/1905.11946}, year = {2019}, url = {http://arxiv.org/abs/
+1905.11946}, eprinttype = {arXiv}, eprint = {1905.11946}, timestamp = {Mon, 03
+  Jun 2019 13:42:33 +0200}, biburl = {https://dblp.org/rec/journals/corr/abs-
+  1905-11946.bib}, bibsource = {dblp computer science bibliography, https://
+   dblp.org} } ``` ```BibTeX @article{DBLP:journals/corr/HeZRS15, author =
+  {Kaiming He and Xiangyu Zhang and Shaoqing Ren and Jian Sun}, title = {Deep
+  Residual Learning for Image Recognition}, journal = {CoRR}, volume = {abs/
+1512.03385}, year = {2015}, url = {http://arxiv.org/abs/1512.03385}, eprinttype
+   = {arXiv}, eprint = {1512.03385}, timestamp = {Wed, 17 Apr 2019 17:23:45
++0200}, biburl = {https://dblp.org/rec/journals/corr/HeZRS15.bib}, bibsource =
+{dblp computer science bibliography, https://dblp.org} } ```  ![---------------
+  --------------------------------------](https://raw.githubusercontent.com/
+  canturan10/readme-template/master/src/colored_4b.png) Give a â­ï¸ if this
+   project helped you! _This readme file is made using the [readme-template]
+               (https://github.com/canturan10/readme-template)_
```

### Comparing `satellighte-0.2.4/satellighte/.config.yaml` & `satellighte-0.2.5/satellighte/.config.yaml`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/satellighte/__about__.py` & `satellighte-0.2.5/satellighte/__about__.py`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/satellighte/api/__init__.py` & `satellighte-0.2.5/satellighte/api/__init__.py`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/satellighte/archs/efficientnet/blocks/efficientnet.py` & `satellighte-0.2.5/satellighte/archs/efficientnet/blocks/efficientnet.py`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/satellighte/archs/efficientnet/blocks/layers.py` & `satellighte-0.2.5/satellighte/archs/efficientnet/blocks/layers.py`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/satellighte/archs/efficientnet/module.py` & `satellighte-0.2.5/satellighte/archs/efficientnet/module.py`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/satellighte/archs/mobilenetv2/blocks/layers.py` & `satellighte-0.2.5/satellighte/archs/mobilenetv2/blocks/layers.py`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/satellighte/archs/mobilenetv2/blocks/mobilenetv2.py` & `satellighte-0.2.5/satellighte/archs/mobilenetv2/blocks/mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/satellighte/archs/mobilenetv2/module.py` & `satellighte-0.2.5/satellighte/archs/mobilenetv2/module.py`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/satellighte/archs/resnet/blocks/layers.py` & `satellighte-0.2.5/satellighte/archs/resnet/blocks/layers.py`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/satellighte/archs/resnet/blocks/resnet.py` & `satellighte-0.2.5/satellighte/archs/resnet/blocks/resnet.py`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/satellighte/archs/resnet/module.py` & `satellighte-0.2.5/satellighte/archs/resnet/module.py`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/satellighte/core.py` & `satellighte-0.2.5/satellighte/core.py`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/satellighte/datasets/base.py` & `satellighte-0.2.5/satellighte/datasets/base.py`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/satellighte/datasets/eurosat.py` & `satellighte-0.2.5/satellighte/datasets/eurosat.py`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/satellighte/datasets/resisc45.py` & `satellighte-0.2.5/satellighte/datasets/resisc45.py`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/satellighte/module.py` & `satellighte-0.2.5/satellighte/module.py`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/satellighte/utils.py` & `satellighte-0.2.5/satellighte/utils.py`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/satellighte.egg-info/PKG-INFO` & `satellighte-0.2.5/satellighte.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: satellighte
-Version: 0.2.4
+Version: 0.2.5
 Summary: PyTorch Lightning Implementations of Recent Satellite Image Classification !
 Home-page: https://github.com/canturan10/satellighte
 Author: Oguzcan Turan
 Author-email: can.turan.10@gmail.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
@@ -167,18 +166,18 @@
 - [Arch Model with Random Weight Initialization](https://github.com/canturan10/satellighte/blob/master/satellighte/api/README.md#arch-model-with-random-weight-initialization)
 
 _For more information, please refer to the [APIs](https://github.com/canturan10/satellighte/blob/master/satellighte/api)_
 
 <!-- ARCHITECTURES -->
 ## Architectures
 
-- [x] [MobileNetV2](https://github.com/canturan10/satellighte/blob/master/satellighte/archs/README.md#mobilenetv2)
+- [x] [CoAtNet](https://github.com/canturan10/satellighte/blob/master/satellighte/archs/README.md#coatnet)
 - [x] [EfficientNet](https://github.com/canturan10/satellighte/blob/master/satellighte/archs/README.md#efficientnet)
+- [x] [MobileNetV2](https://github.com/canturan10/satellighte/blob/master/satellighte/archs/README.md#mobilenetv2)
 - [x] [ResNet](https://github.com/canturan10/satellighte/blob/master/satellighte/archs/README.md#resnet)
-- [ ] [CoAtNet](https://github.com/canturan10/satellighte/blob/master/satellighte/archs/README.md)
 
 _For more information, please refer to the [Architectures](https://github.com/canturan10/satellighte/blob/master/satellighte/archs)_
 
 <!-- DATASETS -->
 ## Datasets
 
 - [x] [EuroSAT](https://github.com/canturan10/satellighte/blob/master/satellighte/datasets/README.md#EuroSAT)
@@ -279,15 +278,15 @@
             </a>
         </td>
         <td align="center">
             <a href="https://github.com/canturan10">
                 <h3>
                     You ?
                 </h3>
-                <img src="https://raw.githubusercontent.com/canturan10/readme-template/master/src/you.png"
+                <img src="https://raw.githubusercontent.com/canturan10/satellighte/master/src/you_satellighte.png"
                     width="200px;" alt="Oğuzcan Turan" /><br>
                 <a href="#">
                     <img src="https://img.shields.io/badge/-Reserved%20Place-red?style=flat&logoColor=white"
                         width="110px;" alt="Reserved" />
                 </a>
             </a>
         </td>
@@ -317,14 +316,25 @@
 
 <!-- CITATIONS -->
 ## Citations
 
 <details>
   <summary>Click to expand!</summary>
 
+  ```BibTeX
+@misc{dai2021coatnet,
+      title={CoAtNet: Marrying Convolution and Attention for All Data Sizes},
+      author={Zihang Dai and Hanxiao Liu and Quoc V. Le and Mingxing Tan},
+      year={2021},
+      eprint={2106.04803},
+      archivePrefix={arXiv},
+      primaryClass={cs.CV}
+}
+```
+
   ```bibtex
 @article{DBLP:journals/corr/ChengHL17,
   author    = {Gong Cheng and
                Junwei Han and
                Xiaoqiang Lu},
   title     = {Remote Sensing Image Scene Classification: Benchmark and State of
                the Art},
@@ -421,9 +431,7 @@
 </details>
 
 ![-----------------------------------------------------](https://raw.githubusercontent.com/canturan10/readme-template/master/src/colored_4b.png)
 
 Give a ⭐️ if this project helped you!
 
 _This readme file is made using the [readme-template](https://github.com/canturan10/readme-template)_
-
-
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: satellighte Version: 0.2.4 Summary: PyTorch
+Metadata-Version: 2.1 Name: satellighte Version: 0.2.5 Summary: PyTorch
 Lightning Implementations of Recent Satellite Image Classification ! Home-page:
 https://github.com/canturan10/satellighte Author: Oguzcan Turan Author-email:
-can.turan.10@gmail.com License: MIT License Platform: UNKNOWN Classifier: Topic
-:: Scientific/Engineering :: Artificial Intelligence Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-test Provides-Extra: docs Provides-Extra: deploy Provides-Extra: all License-
-File: LICENSE
+can.turan.10@gmail.com License: MIT License Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: License :: OSI Approved ::
+MIT License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Requires-Python: >=3.8
+Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
+docs Provides-Extra: deploy Provides-Extra: all License-File: LICENSE
                 [https://img.buymeacoffee.com/button-api/?text=You_can_buy_me_a
 coffee&emoji=&slug=canturan10&button_colour=5F7FFF&font_colour=ffffff&font_family=Comic&outline_colour=000000&coffee_colour=FFDD00]
                                  [Satellighte]
                             ***** Satellighte *****
                     *** Satellite Image Classification ***
                            Website â¢ Docs â¢ Pypi
                                    Demo_Page
@@ -69,97 +68,100 @@
 blob/master/satellighte/api/README.md#model-with-random-weight-initialization)
    - [Pretrained Arch Model](https://github.com/canturan10/satellighte/blob/
   master/satellighte/api/README.md#pretrained-arch-model) - [Arch Model with
  Random Weight Initialization](https://github.com/canturan10/satellighte/blob/
 master/satellighte/api/README.md#arch-model-with-random-weight-initialization)
      _For more information, please refer to the [APIs](https://github.com/
  canturan10/satellighte/blob/master/satellighte/api)_  ## Architectures - [x]
+ [CoAtNet](https://github.com/canturan10/satellighte/blob/master/satellighte/
+ archs/README.md#coatnet) - [x] [EfficientNet](https://github.com/canturan10/
+   satellighte/blob/master/satellighte/archs/README.md#efficientnet) - [x]
      [MobileNetV2](https://github.com/canturan10/satellighte/blob/master/
-    satellighte/archs/README.md#mobilenetv2) - [x] [EfficientNet](https://
-       github.com/canturan10/satellighte/blob/master/satellighte/archs/
-     README.md#efficientnet) - [x] [ResNet](https://github.com/canturan10/
-  satellighte/blob/master/satellighte/archs/README.md#resnet) - [ ] [CoAtNet]
-   (https://github.com/canturan10/satellighte/blob/master/satellighte/archs/
-README.md) _For more information, please refer to the [Architectures](https://
-github.com/canturan10/satellighte/blob/master/satellighte/archs)_  ## Datasets
-    - [x] [EuroSAT](https://github.com/canturan10/satellighte/blob/master/
- satellighte/datasets/README.md#EuroSAT) - [x] [RESISC45](https://github.com/
- canturan10/satellighte/blob/master/satellighte/datasets/README.md) _For more
-  information, please refer to the [Datasets](https://github.com/canturan10/
-satellighte/blob/master/satellighte/datasets)_  ## Deployments - [x] [FastAPI]
-      (https://github.com/canturan10/satellighte/blob/master/deployment/
-README.md#fastapi) - [x] [ONNX](https://github.com/canturan10/satellighte/blob/
-   master/deployment/README.md#onnx) - [x] [DeepSparse](https://github.com/
-  canturan10/satellighte/blob/master/deployment/README.md#deepsparse) - [x]
-[TensorFlow](https://github.com/canturan10/satellighte/blob/master/deployment/
- README.md#tensorflow) - [x] [TensorFlow Lite](https://github.com/canturan10/
-    satellighte/blob/master/deployment/README.md#tensorflow-lite) _For more
- information, please refer to the [Deployment](https://github.com/canturan10/
-  satellighte/blob/master/deployment)_  ## Training To training, follow these
-     steps: For installing Satellighte, please refer to the [Installation]
- (#installation). ```bash python training/eurosat_training.py ``` For optional
-  arguments, ```bash python training/eurosat_training.py --help ```  ## Tests
-  During development, you might like to have tests run. Install dependencies
-     ```bash pip install -e ".[test]" ``` ### Linting Tests ```bash pytest
-  satellighte --pylint --pylint-error-types=EF ``` ### Document Tests ```bash
- pytest satellighte --doctest-modules ``` ### Coverage Tests ```bash pytest --
-  doctest-modules --cov satellighte --cov-report term ```  ## Contributing To
- contribute to `Satellighte`, follow these steps: 1. Fork this repository. 2.
-Create a branch: `git checkout -b `. 3. Make your changes and commit them: `git
- commit -m ''` 4. Push to the original branch: `git push origin` 5. Create the
-pull request. Alternatively see the `GitHub` documentation on [creating a pull
-request](https://help.github.com/en/github/collaborating-with-issues-and-pull-
-              requests/creating-a-pull-request).  ## Contributors
+  satellighte/archs/README.md#mobilenetv2) - [x] [ResNet](https://github.com/
+  canturan10/satellighte/blob/master/satellighte/archs/README.md#resnet) _For
+   more information, please refer to the [Architectures](https://github.com/
+  canturan10/satellighte/blob/master/satellighte/archs)_  ## Datasets - [x]
+ [EuroSAT](https://github.com/canturan10/satellighte/blob/master/satellighte/
+  datasets/README.md#EuroSAT) - [x] [RESISC45](https://github.com/canturan10/
+satellighte/blob/master/satellighte/datasets/README.md) _For more information,
+please refer to the [Datasets](https://github.com/canturan10/satellighte/blob/
+    master/satellighte/datasets)_  ## Deployments - [x] [FastAPI](https://
+github.com/canturan10/satellighte/blob/master/deployment/README.md#fastapi) -
+ [x] [ONNX](https://github.com/canturan10/satellighte/blob/master/deployment/
+ README.md#onnx) - [x] [DeepSparse](https://github.com/canturan10/satellighte/
+   blob/master/deployment/README.md#deepsparse) - [x] [TensorFlow](https://
+github.com/canturan10/satellighte/blob/master/deployment/README.md#tensorflow)
+- [x] [TensorFlow Lite](https://github.com/canturan10/satellighte/blob/master/
+ deployment/README.md#tensorflow-lite) _For more information, please refer to
+    the [Deployment](https://github.com/canturan10/satellighte/blob/master/
+   deployment)_  ## Training To training, follow these steps: For installing
+Satellighte, please refer to the [Installation](#installation). ```bash python
+    training/eurosat_training.py ``` For optional arguments, ```bash python
+training/eurosat_training.py --help ```  ## Tests During development, you might
+ like to have tests run. Install dependencies ```bash pip install -e ".[test]"
+   ``` ### Linting Tests ```bash pytest satellighte --pylint --pylint-error-
+ types=EF ``` ### Document Tests ```bash pytest satellighte --doctest-modules
+ ``` ### Coverage Tests ```bash pytest --doctest-modules --cov satellighte --
+  cov-report term ```  ## Contributing To contribute to `Satellighte`, follow
+ these steps: 1. Fork this repository. 2. Create a branch: `git checkout -b `.
+    3. Make your changes and commit them: `git commit -m ''` 4. Push to the
+ original branch: `git push origin` 5. Create the pull request. Alternatively
+     see the `GitHub` documentation on [creating a pull request](https://
+help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-
+                       a-pull-request).  ## Contributors
                   ****_OÄuzcan_Turan_**** ****_You_?_****
                       [OÄuzcan_Turan]     [OÄuzcan_Turan]
                    [Linkedin]_[Portfolio]       [Reserved]
            ## Contact If you want to contact me you can reach me at
    [can.turan.10@gmail.com](mailto:can.turan.10@gmail.com).  ## License This
   project is licensed under `MIT` license. See [`LICENSE`](LICENSE) for more
    information.  ## References The references used in the development of the
  project are as follows. - [Img Shields](https://shields.io) - [GitHub Pages]
    (https://pages.github.com) - [FastFace](https://github.com/borhanMorphy/
  fastface) - [PyTorch Lightning](https://github.com/PyTorchLightning/pytorch-
   lightning) - [Torchvision](https://github.com/pytorch/vision)  ## Citations
-  Click to expand! ```bibtex @article{DBLP:journals/corr/ChengHL17, author =
-  {Gong Cheng and Junwei Han and Xiaoqiang Lu}, title = {Remote Sensing Image
-Scene Classification: Benchmark and State of the Art}, journal = {CoRR}, volume
-  = {abs/1703.00121}, year = {2017}, url = {http://arxiv.org/abs/1703.00121},
-eprinttype = {arXiv}, eprint = {1703.00121}, timestamp = {Mon, 02 Dec 2019 09:
-  32:19 +0100}, biburl = {https://dblp.org/rec/journals/corr/ChengHL17.bib},
-   bibsource = {dblp computer science bibliography, https://dblp.org} } ```
-```bibtex @article{helber2019eurosat, title={Eurosat: A novel dataset and deep
-learning benchmark for land use and land cover classification}, author={Helber,
-Patrick and Bischke, Benjamin and Dengel, Andreas and Borth, Damian}, journal=
-   {IEEE Journal of Selected Topics in Applied Earth Observations and Remote
-    Sensing}, year={2019}, publisher={IEEE} } ``` ```bibtex @inproceedings
- {helber2018introducing, title={Introducing EuroSAT: A Novel Dataset and Deep
-Learning Benchmark for Land Use and Land Cover Classification}, author={Helber,
-     Patrick and Bischke, Benjamin and Dengel, Andreas and Borth, Damian},
- booktitle={IGARSS 2018-2018 IEEE International Geoscience and Remote Sensing
-Symposium}, pages={204--207}, year={2018}, organization={IEEE} } ``` ```bibtex
- @article{DBLP:journals/corr/abs-1801-04381, author = {Mark Sandler and Andrew
-G. Howard and Menglong Zhu and Andrey Zhmoginov and Liang{-}Chieh Chen}, title
-       = {Inverted Residuals and Linear Bottlenecks: Mobile Networks for
- Classification, Detection and Segmentation}, journal = {CoRR}, volume = {abs/
-     1801.04381}, year = {2018}, url = {http://arxiv.org/abs/1801.04381},
- archivePrefix = {arXiv}, eprint = {1801.04381}, timestamp = {Tue, 12 Jan 2021
-    15:30:06 +0100}, biburl = {https://dblp.org/rec/journals/corr/abs-1801-
-04381.bib}, bibsource = {dblp computer science bibliography, https://dblp.org}
-} ``` ```BibTeX @article{DBLP:journals/corr/abs-1905-11946, author = {Mingxing
-   Tan and Quoc V. Le}, title = {EfficientNet: Rethinking Model Scaling for
- Convolutional Neural Networks}, journal = {CoRR}, volume = {abs/1905.11946},
- year = {2019}, url = {http://arxiv.org/abs/1905.11946}, eprinttype = {arXiv},
-eprint = {1905.11946}, timestamp = {Mon, 03 Jun 2019 13:42:33 +0200}, biburl =
-  {https://dblp.org/rec/journals/corr/abs-1905-11946.bib}, bibsource = {dblp
-computer science bibliography, https://dblp.org} } ``` ```BibTeX @article{DBLP:
-journals/corr/HeZRS15, author = {Kaiming He and Xiangyu Zhang and Shaoqing Ren
-and Jian Sun}, title = {Deep Residual Learning for Image Recognition}, journal
- = {CoRR}, volume = {abs/1512.03385}, year = {2015}, url = {http://arxiv.org/
-abs/1512.03385}, eprinttype = {arXiv}, eprint = {1512.03385}, timestamp = {Wed,
-  17 Apr 2019 17:23:45 +0200}, biburl = {https://dblp.org/rec/journals/corr/
-    HeZRS15.bib}, bibsource = {dblp computer science bibliography, https://
-   dblp.org} } ```  ![-----------------------------------------------------]
-   (https://raw.githubusercontent.com/canturan10/readme-template/master/src/
-colored_4b.png) Give a â­ï¸ if this project helped you! _This readme file is
-    made using the [readme-template](https://github.com/canturan10/readme-
-                                  template)_
+   Click to expand! ```BibTeX @misc{dai2021coatnet, title={CoAtNet: Marrying
+ Convolution and Attention for All Data Sizes}, author={Zihang Dai and Hanxiao
+    Liu and Quoc V. Le and Mingxing Tan}, year={2021}, eprint={2106.04803},
+  archivePrefix={arXiv}, primaryClass={cs.CV} } ``` ```bibtex @article{DBLP:
+journals/corr/ChengHL17, author = {Gong Cheng and Junwei Han and Xiaoqiang Lu},
+title = {Remote Sensing Image Scene Classification: Benchmark and State of the
+Art}, journal = {CoRR}, volume = {abs/1703.00121}, year = {2017}, url = {http:/
+   /arxiv.org/abs/1703.00121}, eprinttype = {arXiv}, eprint = {1703.00121},
+timestamp = {Mon, 02 Dec 2019 09:32:19 +0100}, biburl = {https://dblp.org/rec/
+journals/corr/ChengHL17.bib}, bibsource = {dblp computer science bibliography,
+https://dblp.org} } ``` ```bibtex @article{helber2019eurosat, title={Eurosat: A
+     novel dataset and deep learning benchmark for land use and land cover
+  classification}, author={Helber, Patrick and Bischke, Benjamin and Dengel,
+Andreas and Borth, Damian}, journal={IEEE Journal of Selected Topics in Applied
+  Earth Observations and Remote Sensing}, year={2019}, publisher={IEEE} } ```
+ ```bibtex @inproceedings{helber2018introducing, title={Introducing EuroSAT: A
+     Novel Dataset and Deep Learning Benchmark for Land Use and Land Cover
+  Classification}, author={Helber, Patrick and Bischke, Benjamin and Dengel,
+  Andreas and Borth, Damian}, booktitle={IGARSS 2018-2018 IEEE International
+   Geoscience and Remote Sensing Symposium}, pages={204--207}, year={2018},
+organization={IEEE} } ``` ```bibtex @article{DBLP:journals/corr/abs-1801-04381,
+    author = {Mark Sandler and Andrew G. Howard and Menglong Zhu and Andrey
+   Zhmoginov and Liang{-}Chieh Chen}, title = {Inverted Residuals and Linear
+ Bottlenecks: Mobile Networks for Classification, Detection and Segmentation},
+  journal = {CoRR}, volume = {abs/1801.04381}, year = {2018}, url = {http://
+  arxiv.org/abs/1801.04381}, archivePrefix = {arXiv}, eprint = {1801.04381},
+timestamp = {Tue, 12 Jan 2021 15:30:06 +0100}, biburl = {https://dblp.org/rec/
+     journals/corr/abs-1801-04381.bib}, bibsource = {dblp computer science
+ bibliography, https://dblp.org} } ``` ```BibTeX @article{DBLP:journals/corr/
+abs-1905-11946, author = {Mingxing Tan and Quoc V. Le}, title = {EfficientNet:
+Rethinking Model Scaling for Convolutional Neural Networks}, journal = {CoRR},
+    volume = {abs/1905.11946}, year = {2019}, url = {http://arxiv.org/abs/
+1905.11946}, eprinttype = {arXiv}, eprint = {1905.11946}, timestamp = {Mon, 03
+  Jun 2019 13:42:33 +0200}, biburl = {https://dblp.org/rec/journals/corr/abs-
+  1905-11946.bib}, bibsource = {dblp computer science bibliography, https://
+   dblp.org} } ``` ```BibTeX @article{DBLP:journals/corr/HeZRS15, author =
+  {Kaiming He and Xiangyu Zhang and Shaoqing Ren and Jian Sun}, title = {Deep
+  Residual Learning for Image Recognition}, journal = {CoRR}, volume = {abs/
+1512.03385}, year = {2015}, url = {http://arxiv.org/abs/1512.03385}, eprinttype
+   = {arXiv}, eprint = {1512.03385}, timestamp = {Wed, 17 Apr 2019 17:23:45
++0200}, biburl = {https://dblp.org/rec/journals/corr/HeZRS15.bib}, bibsource =
+{dblp computer science bibliography, https://dblp.org} } ```  ![---------------
+  --------------------------------------](https://raw.githubusercontent.com/
+  canturan10/readme-template/master/src/colored_4b.png) Give a â­ï¸ if this
+   project helped you! _This readme file is made using the [readme-template]
+               (https://github.com/canturan10/readme-template)_
```

### Comparing `satellighte-0.2.4/satellighte.egg-info/SOURCES.txt` & `satellighte-0.2.5/satellighte.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 satellighte.egg-info/PKG-INFO
 satellighte.egg-info/SOURCES.txt
 satellighte.egg-info/dependency_links.txt
 satellighte.egg-info/requires.txt
 satellighte.egg-info/top_level.txt
 satellighte/api/__init__.py
 satellighte/archs/__init__.py
+satellighte/archs/coatnet/__init__.py
+satellighte/archs/coatnet/module.py
+satellighte/archs/coatnet/blocks/__init__.py
+satellighte/archs/coatnet/blocks/coatnet.py
+satellighte/archs/coatnet/blocks/layers.py
 satellighte/archs/efficientnet/__init__.py
 satellighte/archs/efficientnet/module.py
 satellighte/archs/efficientnet/blocks/__init__.py
 satellighte/archs/efficientnet/blocks/efficientnet.py
 satellighte/archs/efficientnet/blocks/layers.py
 satellighte/archs/mobilenetv2/__init__.py
 satellighte/archs/mobilenetv2/module.py
```

### Comparing `satellighte-0.2.4/scripts/release.py` & `satellighte-0.2.5/scripts/release.py`

 * *Files identical despite different names*

### Comparing `satellighte-0.2.4/setup.py` & `satellighte-0.2.5/setup.py`

 * *Files identical despite different names*

