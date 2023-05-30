# Comparing `tmp/bcos-0.0.4.tar.gz` & `tmp/bcos-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcos-0.0.4.tar", last modified: Mon Apr 17 11:13:56 2023, max compression
+gzip compressed data, was "bcos-0.1.0.tar", last modified: Tue May 30 17:29:47 2023, max compression
```

## Comparing `bcos-0.0.4.tar` & `bcos-0.1.0.tar`

### file list

```diff
@@ -1,96 +1,100 @@
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.610777 bcos-0.0.4/
--rw-r--r--   0 singh     (1000) singh     (1000)    11368 2023-03-27 17:57:32.000000 bcos-0.0.4/LICENSE
--rw-r--r--   0 singh     (1000) singh     (1000)    10720 2023-04-17 11:13:56.610777 bcos-0.0.4/PKG-INFO
--rw-r--r--   0 singh     (1000) singh     (1000)    10403 2023-04-02 15:27:36.000000 bcos-0.0.4/README.md
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.604110 bcos-0.0.4/bcos/
--rw-r--r--   0 singh     (1000) singh     (1000)     1308 2023-04-01 21:28:12.000000 bcos-0.0.4/bcos/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)    18686 2023-04-01 21:28:12.000000 bcos-0.0.4/bcos/common.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.607444 bcos-0.0.4/bcos/data/
--rw-r--r--   0 singh     (1000) singh     (1000)        0 2023-01-30 11:46:04.000000 bcos-0.0.4/bcos/data/__init__.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.607444 bcos-0.0.4/bcos/data/caching/
--rw-r--r--   0 singh     (1000) singh     (1000)      154 2023-03-06 17:39:07.000000 bcos-0.0.4/bcos/data/caching/__init__.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.607444 bcos-0.0.4/bcos/data/caching/cached_imagefolder/
--rw-r--r--   0 singh     (1000) singh     (1000)       50 2023-02-14 11:37:10.000000 bcos-0.0.4/bcos/data/caching/cached_imagefolder/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)     1395 2023-03-27 18:57:21.000000 bcos-0.0.4/bcos/data/caching/cached_imagefolder/cached_imagefolder.py
--rw-r--r--   0 singh     (1000) singh     (1000)     4771 2023-03-27 18:57:30.000000 bcos-0.0.4/bcos/data/caching/cached_imagefolder/cached_loader.py
--rw-r--r--   0 singh     (1000) singh     (1000)     2156 2023-03-27 18:57:36.000000 bcos-0.0.4/bcos/data/caching/cached_imagefolder/env.py
--rw-r--r--   0 singh     (1000) singh     (1000)     7776 2023-03-27 18:57:41.000000 bcos-0.0.4/bcos/data/caching/cached_imagefolder/redis_store.py
--rw-r--r--   0 singh     (1000) singh     (1000)     4179 2023-03-27 18:57:46.000000 bcos-0.0.4/bcos/data/caching/cached_imagefolder/store.py
--rw-r--r--   0 singh     (1000) singh     (1000)     1269 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/data/caching/shm_caching.py
--rw-r--r--   0 singh     (1000) singh     (1000)    18020 2023-01-30 11:46:04.000000 bcos-0.0.4/bcos/data/categories.py
--rw-r--r--   0 singh     (1000) singh     (1000)     9296 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/data/datamodules.py
--rw-r--r--   0 singh     (1000) singh     (1000)     6767 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/data/presets.py
--rw-r--r--   0 singh     (1000) singh     (1000)     3048 2023-02-14 11:37:10.000000 bcos-0.0.4/bcos/data/sampler.py
--rw-r--r--   0 singh     (1000) singh     (1000)     8868 2023-03-23 14:26:09.000000 bcos-0.0.4/bcos/data/transforms.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.604110 bcos-0.0.4/bcos/experiments/
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.604110 bcos-0.0.4/bcos/experiments/CIFAR10/
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.607444 bcos-0.0.4/bcos/experiments/CIFAR10/norm_ablations_final/
--rw-r--r--   0 singh     (1000) singh     (1000)     3830 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/experiments/CIFAR10/norm_ablations_final/experiment_parameters.py
--rw-r--r--   0 singh     (1000) singh     (1000)      755 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/experiments/CIFAR10/norm_ablations_final/model.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.604110 bcos-0.0.4/bcos/experiments/ImageNet/
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.607444 bcos-0.0.4/bcos/experiments/ImageNet/baseline/
--rw-r--r--   0 singh     (1000) singh     (1000)     2666 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/experiments/ImageNet/baseline/experiment_parameters.py
--rw-r--r--   0 singh     (1000) singh     (1000)      331 2023-02-14 11:37:10.000000 bcos-0.0.4/bcos/experiments/ImageNet/baseline/model.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.607444 bcos-0.0.4/bcos/experiments/ImageNet/bcos_final/
--rw-r--r--   0 singh     (1000) singh     (1000)     3547 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/experiments/ImageNet/bcos_final/experiment_parameters.py
--rw-r--r--   0 singh     (1000) singh     (1000)     1275 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/experiments/ImageNet/bcos_final/model.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.607444 bcos-0.0.4/bcos/experiments/ImageNet/bcos_final_long/
--rw-r--r--   0 singh     (1000) singh     (1000)     4249 2023-03-27 15:19:32.000000 bcos-0.0.4/bcos/experiments/ImageNet/bcos_final_long/experiment_parameters.py
--rw-r--r--   0 singh     (1000) singh     (1000)     1275 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/experiments/ImageNet/bcos_final_long/model.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.607444 bcos-0.0.4/bcos/experiments/utils/
--rw-r--r--   0 singh     (1000) singh     (1000)      121 2023-03-17 12:11:07.000000 bcos-0.0.4/bcos/experiments/utils/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)     7487 2023-04-02 14:57:16.000000 bcos-0.0.4/bcos/experiments/utils/config_utils.py
--rw-r--r--   0 singh     (1000) singh     (1000)      338 2023-03-17 12:11:07.000000 bcos-0.0.4/bcos/experiments/utils/exceptions.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.607444 bcos-0.0.4/bcos/experiments/utils/experiment_utils/
--rw-r--r--   0 singh     (1000) singh     (1000)       89 2023-03-17 12:11:07.000000 bcos-0.0.4/bcos/experiments/utils/experiment_utils/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)    12167 2023-03-27 18:16:53.000000 bcos-0.0.4/bcos/experiments/utils/experiment_utils/experiment_utils.py
--rw-r--r--   0 singh     (1000) singh     (1000)    13331 2023-04-17 11:11:28.000000 bcos-0.0.4/bcos/experiments/utils/experiment_utils/loading_utils.py
--rw-r--r--   0 singh     (1000) singh     (1000)     4213 2023-03-17 12:11:07.000000 bcos-0.0.4/bcos/experiments/utils/experiment_utils/metric_utils.py
--rw-r--r--   0 singh     (1000) singh     (1000)      419 2023-03-17 12:11:07.000000 bcos-0.0.4/bcos/experiments/utils/structure_constants.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.610777 bcos-0.0.4/bcos/models/
--rw-r--r--   0 singh     (1000) singh     (1000)      128 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/models/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)    10339 2023-04-01 15:05:25.000000 bcos-0.0.4/bcos/models/convnext.py
--rw-r--r--   0 singh     (1000) singh     (1000)    15823 2023-04-01 21:28:12.000000 bcos-0.0.4/bcos/models/densenet.py
--rw-r--r--   0 singh     (1000) singh     (1000)    26244 2023-03-27 16:33:18.000000 bcos-0.0.4/bcos/models/pretrained.py
--rw-r--r--   0 singh     (1000) singh     (1000)    24106 2023-04-01 21:28:12.000000 bcos-0.0.4/bcos/models/resnet.py
--rw-r--r--   0 singh     (1000) singh     (1000)     7068 2023-03-27 16:23:30.000000 bcos-0.0.4/bcos/models/vgg.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.610777 bcos-0.0.4/bcos/modules/
--rw-r--r--   0 singh     (1000) singh     (1000)      242 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/modules/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)     9520 2023-03-27 16:28:20.000000 bcos-0.0.4/bcos/modules/bcosconv2d.py
--rw-r--r--   0 singh     (1000) singh     (1000)     4089 2023-03-27 16:30:21.000000 bcos-0.0.4/bcos/modules/bcoslinear.py
--rw-r--r--   0 singh     (1000) singh     (1000)     1060 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/modules/common.py
--rw-r--r--   0 singh     (1000) singh     (1000)     1013 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/modules/logitlayer.py
--rw-r--r--   0 singh     (1000) singh     (1000)     4189 2023-03-27 16:23:13.000000 bcos-0.0.4/bcos/modules/losses.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.610777 bcos-0.0.4/bcos/modules/norms/
--rw-r--r--   0 singh     (1000) singh     (1000)      130 2023-02-14 11:37:10.000000 bcos-0.0.4/bcos/modules/norms/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)     6654 2023-03-27 16:23:30.000000 bcos-0.0.4/bcos/modules/norms/centered_norms.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.610777 bcos-0.0.4/bcos/modules/norms/uncentered_norms/
--rw-r--r--   0 singh     (1000) singh     (1000)      140 2023-03-17 12:11:07.000000 bcos-0.0.4/bcos/modules/norms/uncentered_norms/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)     4018 2023-03-24 13:32:00.000000 bcos-0.0.4/bcos/modules/norms/uncentered_norms/allnorm_uncentered.py
--rw-r--r--   0 singh     (1000) singh     (1000)     3895 2023-03-24 13:32:00.000000 bcos-0.0.4/bcos/modules/norms/uncentered_norms/batchnorm_uncentered.py
--rw-r--r--   0 singh     (1000) singh     (1000)     2518 2023-03-27 16:23:30.000000 bcos-0.0.4/bcos/modules/norms/uncentered_norms/groupnorm_uncentered.py
--rw-r--r--   0 singh     (1000) singh     (1000)     1492 2023-03-27 16:23:30.000000 bcos-0.0.4/bcos/modules/norms/uncentered_norms/posnorm_uncentered.py
--rw-r--r--   0 singh     (1000) singh     (1000)     2005 2023-02-14 11:37:10.000000 bcos-0.0.4/bcos/modules/norms/utils.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.610777 bcos-0.0.4/bcos/optim/
--rw-r--r--   0 singh     (1000) singh     (1000)       69 2023-03-23 14:26:09.000000 bcos-0.0.4/bcos/optim/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)     7725 2023-03-27 16:25:26.000000 bcos-0.0.4/bcos/optim/lr_scheduler_factory.py
--rw-r--r--   0 singh     (1000) singh     (1000)     6451 2023-03-27 16:26:11.000000 bcos-0.0.4/bcos/optim/optimizer_factory.py
--rw-r--r--   0 singh     (1000) singh     (1000)      686 2023-04-01 21:28:12.000000 bcos-0.0.4/bcos/settings.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.610777 bcos-0.0.4/bcos/training/
--rw-r--r--   0 singh     (1000) singh     (1000)       33 2023-02-14 11:37:10.000000 bcos-0.0.4/bcos/training/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)     1465 2023-03-08 10:36:14.000000 bcos-0.0.4/bcos/training/agc.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.610777 bcos-0.0.4/bcos/training/callbacks/
--rw-r--r--   0 singh     (1000) singh     (1000)       94 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/training/callbacks/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)     8850 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/training/callbacks/explanation_logger.py
--rw-r--r--   0 singh     (1000) singh     (1000)     1858 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/training/callbacks/metricstracker.py
--rw-r--r--   0 singh     (1000) singh     (1000)      766 2023-01-30 11:46:04.000000 bcos-0.0.4/bcos/training/ema.py
--rw-r--r--   0 singh     (1000) singh     (1000)    13515 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/training/trainer.py
--rw-r--r--   0 singh     (1000) singh     (1000)      146 2023-04-17 11:12:34.000000 bcos-0.0.4/bcos/version.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.604110 bcos-0.0.4/bcos.egg-info/
--rw-r--r--   0 singh     (1000) singh     (1000)    10720 2023-04-17 11:13:56.000000 bcos-0.0.4/bcos.egg-info/PKG-INFO
--rw-r--r--   0 singh     (1000) singh     (1000)     2538 2023-04-17 11:13:56.000000 bcos-0.0.4/bcos.egg-info/SOURCES.txt
--rw-r--r--   0 singh     (1000) singh     (1000)        1 2023-04-17 11:13:56.000000 bcos-0.0.4/bcos.egg-info/dependency_links.txt
--rw-r--r--   0 singh     (1000) singh     (1000)        5 2023-04-17 11:13:56.000000 bcos-0.0.4/bcos.egg-info/top_level.txt
--rw-r--r--   0 singh     (1000) singh     (1000)      842 2023-04-17 11:12:34.000000 bcos-0.0.4/pyproject.toml
--rw-r--r--   0 singh     (1000) singh     (1000)       38 2023-04-17 11:13:56.610777 bcos-0.0.4/setup.cfg
--rw-r--r--   0 singh     (1000) singh     (1000)       85 2023-03-27 13:43:57.000000 bcos-0.0.4/setup.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.452402 bcos-0.1.0/
+-rw-r--r--   0 singh     (1000) singh     (1000)    11368 2023-03-27 17:57:32.000000 bcos-0.1.0/LICENSE
+-rw-r--r--   0 singh     (1000) singh     (1000)    15467 2023-05-30 17:29:47.452402 bcos-0.1.0/PKG-INFO
+-rw-r--r--   0 singh     (1000) singh     (1000)    15150 2023-05-30 17:18:39.000000 bcos-0.1.0/README.md
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.445736 bcos-0.1.0/bcos/
+-rw-r--r--   0 singh     (1000) singh     (1000)     1308 2023-04-01 21:28:12.000000 bcos-0.1.0/bcos/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)    18686 2023-04-01 21:28:12.000000 bcos-0.1.0/bcos/common.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.445736 bcos-0.1.0/bcos/data/
+-rw-r--r--   0 singh     (1000) singh     (1000)        0 2023-01-30 11:46:04.000000 bcos-0.1.0/bcos/data/__init__.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.445736 bcos-0.1.0/bcos/data/caching/
+-rw-r--r--   0 singh     (1000) singh     (1000)      154 2023-03-06 17:39:07.000000 bcos-0.1.0/bcos/data/caching/__init__.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.449069 bcos-0.1.0/bcos/data/caching/cached_imagefolder/
+-rw-r--r--   0 singh     (1000) singh     (1000)       50 2023-02-14 11:37:10.000000 bcos-0.1.0/bcos/data/caching/cached_imagefolder/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     1395 2023-03-27 18:57:21.000000 bcos-0.1.0/bcos/data/caching/cached_imagefolder/cached_imagefolder.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     4771 2023-03-27 18:57:30.000000 bcos-0.1.0/bcos/data/caching/cached_imagefolder/cached_loader.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     2156 2023-03-27 18:57:36.000000 bcos-0.1.0/bcos/data/caching/cached_imagefolder/env.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     7776 2023-03-27 18:57:41.000000 bcos-0.1.0/bcos/data/caching/cached_imagefolder/redis_store.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     4179 2023-03-27 18:57:46.000000 bcos-0.1.0/bcos/data/caching/cached_imagefolder/store.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     1269 2023-03-27 13:43:57.000000 bcos-0.1.0/bcos/data/caching/shm_caching.py
+-rw-r--r--   0 singh     (1000) singh     (1000)    18020 2023-01-30 11:46:04.000000 bcos-0.1.0/bcos/data/categories.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     9296 2023-03-27 13:43:57.000000 bcos-0.1.0/bcos/data/datamodules.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     6767 2023-03-27 13:43:57.000000 bcos-0.1.0/bcos/data/presets.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     3048 2023-02-14 11:37:10.000000 bcos-0.1.0/bcos/data/sampler.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     8868 2023-03-23 14:26:09.000000 bcos-0.1.0/bcos/data/transforms.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.445736 bcos-0.1.0/bcos/experiments/
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.442402 bcos-0.1.0/bcos/experiments/CIFAR10/
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.449069 bcos-0.1.0/bcos/experiments/CIFAR10/norm_ablations_final/
+-rw-r--r--   0 singh     (1000) singh     (1000)     3830 2023-03-27 13:43:57.000000 bcos-0.1.0/bcos/experiments/CIFAR10/norm_ablations_final/experiment_parameters.py
+-rw-r--r--   0 singh     (1000) singh     (1000)      755 2023-03-27 13:43:57.000000 bcos-0.1.0/bcos/experiments/CIFAR10/norm_ablations_final/model.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.445736 bcos-0.1.0/bcos/experiments/ImageNet/
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.449069 bcos-0.1.0/bcos/experiments/ImageNet/baseline/
+-rw-r--r--   0 singh     (1000) singh     (1000)     2666 2023-03-27 13:43:57.000000 bcos-0.1.0/bcos/experiments/ImageNet/baseline/experiment_parameters.py
+-rw-r--r--   0 singh     (1000) singh     (1000)      331 2023-02-14 11:37:10.000000 bcos-0.1.0/bcos/experiments/ImageNet/baseline/model.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.449069 bcos-0.1.0/bcos/experiments/ImageNet/bcos_final/
+-rw-r--r--   0 singh     (1000) singh     (1000)     3547 2023-03-27 13:43:57.000000 bcos-0.1.0/bcos/experiments/ImageNet/bcos_final/experiment_parameters.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     1275 2023-03-27 13:43:57.000000 bcos-0.1.0/bcos/experiments/ImageNet/bcos_final/model.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.449069 bcos-0.1.0/bcos/experiments/ImageNet/bcos_final_long/
+-rw-r--r--   0 singh     (1000) singh     (1000)     4249 2023-03-27 15:19:32.000000 bcos-0.1.0/bcos/experiments/ImageNet/bcos_final_long/experiment_parameters.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     1275 2023-03-27 13:43:57.000000 bcos-0.1.0/bcos/experiments/ImageNet/bcos_final_long/model.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.449069 bcos-0.1.0/bcos/experiments/ImageNet/vit_final/
+-rw-r--r--   0 singh     (1000) singh     (1000)     5362 2023-05-30 17:18:39.000000 bcos-0.1.0/bcos/experiments/ImageNet/vit_final/experiment_parameters.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     1374 2023-05-30 17:18:39.000000 bcos-0.1.0/bcos/experiments/ImageNet/vit_final/model.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.449069 bcos-0.1.0/bcos/experiments/utils/
+-rw-r--r--   0 singh     (1000) singh     (1000)      121 2023-03-17 12:11:07.000000 bcos-0.1.0/bcos/experiments/utils/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     7487 2023-04-02 14:57:16.000000 bcos-0.1.0/bcos/experiments/utils/config_utils.py
+-rw-r--r--   0 singh     (1000) singh     (1000)      338 2023-03-17 12:11:07.000000 bcos-0.1.0/bcos/experiments/utils/exceptions.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.449069 bcos-0.1.0/bcos/experiments/utils/experiment_utils/
+-rw-r--r--   0 singh     (1000) singh     (1000)       89 2023-03-17 12:11:07.000000 bcos-0.1.0/bcos/experiments/utils/experiment_utils/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)    12167 2023-03-27 18:16:53.000000 bcos-0.1.0/bcos/experiments/utils/experiment_utils/experiment_utils.py
+-rw-r--r--   0 singh     (1000) singh     (1000)    13331 2023-04-17 11:11:28.000000 bcos-0.1.0/bcos/experiments/utils/experiment_utils/loading_utils.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     4213 2023-03-17 12:11:07.000000 bcos-0.1.0/bcos/experiments/utils/experiment_utils/metric_utils.py
+-rw-r--r--   0 singh     (1000) singh     (1000)      419 2023-03-17 12:11:07.000000 bcos-0.1.0/bcos/experiments/utils/structure_constants.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.449069 bcos-0.1.0/bcos/models/
+-rw-r--r--   0 singh     (1000) singh     (1000)      128 2023-03-27 13:43:57.000000 bcos-0.1.0/bcos/models/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)    10339 2023-04-01 15:05:25.000000 bcos-0.1.0/bcos/models/convnext.py
+-rw-r--r--   0 singh     (1000) singh     (1000)    15823 2023-04-01 21:28:12.000000 bcos-0.1.0/bcos/models/densenet.py
+-rw-r--r--   0 singh     (1000) singh     (1000)    48769 2023-05-30 17:18:39.000000 bcos-0.1.0/bcos/models/pretrained.py
+-rw-r--r--   0 singh     (1000) singh     (1000)    24106 2023-04-01 21:28:12.000000 bcos-0.1.0/bcos/models/resnet.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     7068 2023-03-27 16:23:30.000000 bcos-0.1.0/bcos/models/vgg.py
+-rw-r--r--   0 singh     (1000) singh     (1000)    14403 2023-05-30 17:18:39.000000 bcos-0.1.0/bcos/models/vit.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.449069 bcos-0.1.0/bcos/modules/
+-rw-r--r--   0 singh     (1000) singh     (1000)      242 2023-03-27 13:43:57.000000 bcos-0.1.0/bcos/modules/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     9520 2023-03-27 16:28:20.000000 bcos-0.1.0/bcos/modules/bcosconv2d.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     4089 2023-03-27 16:30:21.000000 bcos-0.1.0/bcos/modules/bcoslinear.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     1060 2023-03-27 13:43:57.000000 bcos-0.1.0/bcos/modules/common.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     1013 2023-03-27 13:43:57.000000 bcos-0.1.0/bcos/modules/logitlayer.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     4189 2023-03-27 16:23:13.000000 bcos-0.1.0/bcos/modules/losses.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.449069 bcos-0.1.0/bcos/modules/norms/
+-rw-r--r--   0 singh     (1000) singh     (1000)      130 2023-02-14 11:37:10.000000 bcos-0.1.0/bcos/modules/norms/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     6654 2023-03-27 16:23:30.000000 bcos-0.1.0/bcos/modules/norms/centered_norms.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.452402 bcos-0.1.0/bcos/modules/norms/uncentered_norms/
+-rw-r--r--   0 singh     (1000) singh     (1000)      140 2023-03-17 12:11:07.000000 bcos-0.1.0/bcos/modules/norms/uncentered_norms/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     4018 2023-03-24 13:32:00.000000 bcos-0.1.0/bcos/modules/norms/uncentered_norms/allnorm_uncentered.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     3895 2023-03-24 13:32:00.000000 bcos-0.1.0/bcos/modules/norms/uncentered_norms/batchnorm_uncentered.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     2518 2023-03-27 16:23:30.000000 bcos-0.1.0/bcos/modules/norms/uncentered_norms/groupnorm_uncentered.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     1492 2023-03-27 16:23:30.000000 bcos-0.1.0/bcos/modules/norms/uncentered_norms/posnorm_uncentered.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     2005 2023-02-14 11:37:10.000000 bcos-0.1.0/bcos/modules/norms/utils.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.452402 bcos-0.1.0/bcos/optim/
+-rw-r--r--   0 singh     (1000) singh     (1000)       69 2023-03-23 14:26:09.000000 bcos-0.1.0/bcos/optim/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     7725 2023-03-27 16:25:26.000000 bcos-0.1.0/bcos/optim/lr_scheduler_factory.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     6451 2023-03-27 16:26:11.000000 bcos-0.1.0/bcos/optim/optimizer_factory.py
+-rw-r--r--   0 singh     (1000) singh     (1000)      686 2023-04-01 21:28:12.000000 bcos-0.1.0/bcos/settings.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.452402 bcos-0.1.0/bcos/training/
+-rw-r--r--   0 singh     (1000) singh     (1000)       33 2023-02-14 11:37:10.000000 bcos-0.1.0/bcos/training/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     1465 2023-03-08 10:36:14.000000 bcos-0.1.0/bcos/training/agc.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.452402 bcos-0.1.0/bcos/training/callbacks/
+-rw-r--r--   0 singh     (1000) singh     (1000)       94 2023-03-27 13:43:57.000000 bcos-0.1.0/bcos/training/callbacks/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     8850 2023-03-27 13:43:57.000000 bcos-0.1.0/bcos/training/callbacks/explanation_logger.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     1858 2023-03-27 13:43:57.000000 bcos-0.1.0/bcos/training/callbacks/metricstracker.py
+-rw-r--r--   0 singh     (1000) singh     (1000)      766 2023-01-30 11:46:04.000000 bcos-0.1.0/bcos/training/ema.py
+-rw-r--r--   0 singh     (1000) singh     (1000)    13515 2023-03-27 13:43:57.000000 bcos-0.1.0/bcos/training/trainer.py
+-rw-r--r--   0 singh     (1000) singh     (1000)      146 2023-05-30 17:18:58.000000 bcos-0.1.0/bcos/version.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-05-30 17:29:47.445736 bcos-0.1.0/bcos.egg-info/
+-rw-r--r--   0 singh     (1000) singh     (1000)    15467 2023-05-30 17:29:47.000000 bcos-0.1.0/bcos.egg-info/PKG-INFO
+-rw-r--r--   0 singh     (1000) singh     (1000)     2663 2023-05-30 17:29:47.000000 bcos-0.1.0/bcos.egg-info/SOURCES.txt
+-rw-r--r--   0 singh     (1000) singh     (1000)        1 2023-05-30 17:29:47.000000 bcos-0.1.0/bcos.egg-info/dependency_links.txt
+-rw-r--r--   0 singh     (1000) singh     (1000)        5 2023-05-30 17:29:47.000000 bcos-0.1.0/bcos.egg-info/top_level.txt
+-rw-r--r--   0 singh     (1000) singh     (1000)      842 2023-05-30 17:18:58.000000 bcos-0.1.0/pyproject.toml
+-rw-r--r--   0 singh     (1000) singh     (1000)       38 2023-05-30 17:29:47.452402 bcos-0.1.0/setup.cfg
+-rw-r--r--   0 singh     (1000) singh     (1000)       85 2023-03-27 13:43:57.000000 bcos-0.1.0/setup.py
```

### Comparing `bcos-0.0.4/LICENSE` & `bcos-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/__init__.py` & `bcos-0.1.0/bcos/__init__.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/common.py` & `bcos-0.1.0/bcos/common.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/data/caching/cached_imagefolder/cached_imagefolder.py` & `bcos-0.1.0/bcos/data/caching/cached_imagefolder/cached_imagefolder.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/data/caching/cached_imagefolder/cached_loader.py` & `bcos-0.1.0/bcos/data/caching/cached_imagefolder/cached_loader.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/data/caching/cached_imagefolder/env.py` & `bcos-0.1.0/bcos/data/caching/cached_imagefolder/env.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/data/caching/cached_imagefolder/redis_store.py` & `bcos-0.1.0/bcos/data/caching/cached_imagefolder/redis_store.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/data/caching/cached_imagefolder/store.py` & `bcos-0.1.0/bcos/data/caching/cached_imagefolder/store.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/data/caching/shm_caching.py` & `bcos-0.1.0/bcos/data/caching/shm_caching.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/data/categories.py` & `bcos-0.1.0/bcos/data/categories.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/data/datamodules.py` & `bcos-0.1.0/bcos/data/datamodules.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/data/presets.py` & `bcos-0.1.0/bcos/data/presets.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/data/sampler.py` & `bcos-0.1.0/bcos/data/sampler.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/data/transforms.py` & `bcos-0.1.0/bcos/data/transforms.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/experiments/CIFAR10/norm_ablations_final/experiment_parameters.py` & `bcos-0.1.0/bcos/experiments/CIFAR10/norm_ablations_final/experiment_parameters.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/experiments/CIFAR10/norm_ablations_final/model.py` & `bcos-0.1.0/bcos/experiments/CIFAR10/norm_ablations_final/model.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/experiments/ImageNet/baseline/experiment_parameters.py` & `bcos-0.1.0/bcos/experiments/ImageNet/baseline/experiment_parameters.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/experiments/ImageNet/bcos_final/experiment_parameters.py` & `bcos-0.1.0/bcos/experiments/ImageNet/bcos_final/experiment_parameters.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/experiments/ImageNet/bcos_final/model.py` & `bcos-0.1.0/bcos/experiments/ImageNet/bcos_final/model.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/experiments/ImageNet/bcos_final_long/experiment_parameters.py` & `bcos-0.1.0/bcos/experiments/ImageNet/bcos_final_long/experiment_parameters.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/experiments/ImageNet/bcos_final_long/model.py` & `bcos-0.1.0/bcos/experiments/ImageNet/bcos_final_long/model.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/experiments/utils/config_utils.py` & `bcos-0.1.0/bcos/experiments/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/experiments/utils/experiment_utils/experiment_utils.py` & `bcos-0.1.0/bcos/experiments/utils/experiment_utils/experiment_utils.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/experiments/utils/experiment_utils/loading_utils.py` & `bcos-0.1.0/bcos/experiments/utils/experiment_utils/loading_utils.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/experiments/utils/experiment_utils/metric_utils.py` & `bcos-0.1.0/bcos/experiments/utils/experiment_utils/metric_utils.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/models/convnext.py` & `bcos-0.1.0/bcos/models/convnext.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/models/densenet.py` & `bcos-0.1.0/bcos/models/densenet.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/models/pretrained.py` & `bcos-0.1.0/bcos/models/pretrained.py`

 * *Files 24% similar despite different names*

```diff
@@ -63,14 +63,33 @@
         "convnext_base_pn": f"{BASE}/convnext_base_pn-b0495852c6.pth",
         "convnext_tiny_bnu": f"{BASE}/convnext_tiny_bnu-dbd7f5ef9d.pth",
         "convnext_base_bnu": f"{BASE}/convnext_base_bnu-7c32a704b3.pth",
         "densenet_121": f"{BASE}/densenet_121_long-5175461597.pth",
         "resnet_50": f"{BASE}/resnet_50_long-ef38a88533.pth",
         "resnet_152": f"{BASE}/resnet_152_long-0b4b434939.pth",
     },
+    "vit_final": {
+        "bcos_simple_vit_ti_patch16_224": f"{BASE}/bcos_simple_vit_ti_patch16_224-4b0824b1c1.pth",
+        "bcos_simple_vit_s_patch16_224": f"{BASE}/bcos_simple_vit_s_patch16_224-75e99d1f73.pth",
+        "bcos_simple_vit_b_patch16_224": f"{BASE}/bcos_simple_vit_b_patch16_224-1fc4750806.pth",
+        "bcos_simple_vit_l_patch16_224": f"{BASE}/bcos_simple_vit_l_patch16_224-9613b2ad0a.pth",
+        "bcos_vitc_ti_patch1_14": f"{BASE}/bcos_vitc_ti_patch1_14-ddd6193a77.pth",
+        "bcos_vitc_s_patch1_14": f"{BASE}/bcos_vitc_s_patch1_14-cf55c88f0c.pth",
+        "bcos_vitc_b_patch1_14": f"{BASE}/bcos_vitc_b_patch1_14-a13c46397b.pth",
+        "bcos_vitc_l_patch1_14": f"{BASE}/bcos_vitc_l_patch1_14-8739e18b8d.pth",
+        # standard! ie non-B-cos
+        "simple_vit_ti_patch16_224": f"{BASE}/standard_simple_vit_ti_patch16_224-2ae8c65a39.pth",
+        "simple_vit_s_patch16_224": f"{BASE}/standard_simple_vit_s_patch16_224-f2934fcdcf.pth",
+        "simple_vit_b_patch16_224": f"{BASE}/standard_simple_vit_b_patch16_224-87074200ed.pth",
+        "simple_vit_l_patch16_224": f"{BASE}/standard_simple_vit_l_patch16_224-62dc536e03.pth",
+        "vitc_ti_patch1_14": f"{BASE}/standard_vitc_ti_patch1_14-a5d6bded37.pth",
+        "vitc_s_patch1_14": f"{BASE}/standard_vitc_s_patch1_14-34ecd7288e.pth",
+        "vitc_b_patch1_14": f"{BASE}/standard_vitc_b_patch1_14-4d374b0220.pth",
+        "vitc_l_patch1_14": f"{BASE}/standard_vitc_l_patch1_14-560e48f246.pth",
+    },
 }
 
 
 def _get_model(
     experiment_name: str,
     pretrained: bool,
     progress: bool,
@@ -809,7 +828,686 @@
     **kwargs : Any, optional
         Additional arguments passed to the model constructor
         Please see source code for details.
     """
     return _get_model(
         "resnet_152", pretrained, progress, base_network="bcos_final_long", **kwargs
     )
+
+
+# ----------------------------------------------------------------------------------------------------------------------
+# ViT models (both B-cos and non-B-cos)
+# non-B-cos i.e. standard models are prefixed with "standard_"
+# ----------------------------------------------------------------------------------------------------------------------
+def _requires_einops():
+    """Checks if einops is installed."""
+    try:
+        import einops  # noqa: F401
+    except ImportError:
+        raise RuntimeError(
+            "This model requires einops to be installed. "
+            "To fix this, run `pip install einops`."
+        )
+
+
+def _get_vit_model(*args, **kwargs):
+    """Gets a ViT model, which requires einops. Hence, it checks for it."""
+    _requires_einops()
+    return _get_model(*args, **kwargs)
+
+
+@register
+def simple_vit_ti_patch16_224(
+    pretrained: bool = False, progress: bool = True, **kwargs
+):
+    """B-cos Simple ViT-Ti with 16x16 patch size and 224x224 image size.
+
+    +---------+-------------------+
+    | Name    | Value             |
+    +=========+===================+
+    | Acc@1   |  59.960%          |
+    +---------+-------------------+
+    | Acc@5   |  81.838%          |
+    +---------+-------------------+
+    | #Params |  5.80M            |
+    +---------+-------------------+
+
+    References
+    ----------
+    `B-cos Networks: Alignment is All We Need for Interpretability <https://arxiv.org/abs/2205.10268>`_
+
+    `Better plain ViT baselines for ImageNet-1k <https://arxiv.org/abs/2205.01580>`_
+
+    Parameters
+    ----------
+    pretrained : bool
+        If True, returns a model pre-trained on ImageNet
+    progress : bool
+        If True, displays a progress bar of the download to stderr
+    **kwargs : Any, optional
+        Additional arguments passed to the model constructor
+        Please see source code for details.
+    """
+    return _get_vit_model(
+        "bcos_simple_vit_ti_patch16_224",
+        pretrained,
+        progress,
+        base_network="vit_final",
+        **kwargs,
+    )
+
+
+@register
+def simple_vit_s_patch16_224(pretrained: bool = False, progress: bool = True, **kwargs):
+    """B-cos Simple ViT-S with 16x16 patch size and 224x224 image size.
+
+    +---------+-------------------+
+    | Name    | Value             |
+    +=========+===================+
+    | Acc@1   |  69.246%          |
+    +---------+-------------------+
+    | Acc@5   |  88.096%          |
+    +---------+-------------------+
+    | #Params |  22.28M           |
+    +---------+-------------------+
+
+    References
+    ----------
+    `B-cos Networks: Alignment is All We Need for Interpretability <https://arxiv.org/abs/2205.10268>`_
+
+    `Better plain ViT baselines for ImageNet-1k <https://arxiv.org/abs/2205.01580>`_
+
+    Parameters
+    ----------
+    pretrained : bool
+        If True, returns a model pre-trained on ImageNet
+    progress : bool
+        If True, displays a progress bar of the download to stderr
+    **kwargs : Any, optional
+        Additional arguments passed to the model constructor
+        Please see source code for details.
+    """
+    return _get_vit_model(
+        "bcos_simple_vit_s_patch16_224",
+        pretrained,
+        progress,
+        base_network="vit_final",
+        **kwargs,
+    )
+
+
+@register
+def simple_vit_b_patch16_224(pretrained: bool = False, progress: bool = True, **kwargs):
+    """B-cos Simple ViT-B with 16x16 patch size and 224x224 image size.
+
+    +---------+-------------------+
+    | Name    | Value             |
+    +=========+===================+
+    | Acc@1   |  74.408%          |
+    +---------+-------------------+
+    | Acc@5   |  91.156%          |
+    +---------+-------------------+
+    | #Params |  86.90M           |
+    +---------+-------------------+
+
+    References
+    ----------
+    `B-cos Networks: Alignment is All We Need for Interpretability <https://arxiv.org/abs/2205.10268>`_
+
+    `Better plain ViT baselines for ImageNet-1k <https://arxiv.org/abs/2205.01580>`_
+
+    Parameters
+    ----------
+    pretrained : bool
+        If True, returns a model pre-trained on ImageNet
+    progress : bool
+        If True, displays a progress bar of the download to stderr
+    **kwargs : Any, optional
+        Additional arguments passed to the model constructor
+        Please see source code for details.
+    """
+    return _get_vit_model(
+        "bcos_simple_vit_b_patch16_224",
+        pretrained,
+        progress,
+        base_network="vit_final",
+        **kwargs,
+    )
+
+
+@register
+def simple_vit_l_patch16_224(pretrained: bool = False, progress: bool = True, **kwargs):
+    """B-cos Simple ViT-L with 16x16 patch size and 224x224 image size.
+
+    +---------+-------------------+
+    | Name    | Value             |
+    +=========+===================+
+    | Acc@1   |  75.060%          |
+    +---------+-------------------+
+    | Acc@5   |  91.378%          |
+    +---------+-------------------+
+    | #Params |  178.79M          |
+    +---------+-------------------+
+
+    References
+    ----------
+    `B-cos Networks: Alignment is All We Need for Interpretability <https://arxiv.org/abs/2205.10268>`_
+
+    `Better plain ViT baselines for ImageNet-1k <https://arxiv.org/abs/2205.01580>`_
+
+    Parameters
+    ----------
+    pretrained : bool
+        If True, returns a model pre-trained on ImageNet
+    progress : bool
+        If True, displays a progress bar of the download to stderr
+    **kwargs : Any, optional
+        Additional arguments passed to the model constructor
+        Please see source code for details.
+    """
+    return _get_vit_model(
+        "bcos_simple_vit_l_patch16_224",
+        pretrained,
+        progress,
+        base_network="vit_final",
+        **kwargs,
+    )
+
+
+@register
+def vitc_ti_patch1_14(pretrained: bool = False, progress: bool = True, **kwargs):
+    """B-cos Simple ViT-Ti with a convolutional stem.
+    The ViT, after the convolution stem, accepts a 1x1 patch size and 14x14 image size.
+
+    +---------+-------------------+
+    | Name    | Value             |
+    +=========+===================+
+    | Acc@1   |  67.260%          |
+    +---------+-------------------+
+    | Acc@5   |  86.774%          |
+    +---------+-------------------+
+    | #Params |  5.32M            |
+    +---------+-------------------+
+
+    References
+    ----------
+    `B-cos Networks: Alignment is All We Need for Interpretability <https://arxiv.org/abs/2205.10268>`_
+
+    `Better plain ViT baselines for ImageNet-1k <https://arxiv.org/abs/2205.01580>`_
+
+    `Early Convolutions Help Transformers See Better <https://arxiv.org/abs/2106.14881>`_
+
+    Parameters
+    ----------
+    pretrained : bool
+        If True, returns a model pre-trained on ImageNet
+    progress : bool
+        If True, displays a progress bar of the download to stderr
+    **kwargs : Any, optional
+        Additional arguments passed to the model constructor
+        Please see source code for details.
+    """
+    return _get_vit_model(
+        "bcos_vitc_ti_patch1_14",
+        pretrained,
+        progress,
+        base_network="vit_final",
+        **kwargs,
+    )
+
+
+@register
+def vitc_s_patch1_14(pretrained: bool = False, progress: bool = True, **kwargs):
+    """B-cos Simple ViT-S with a convolutional stem.
+    The ViT, after the convolution stem, accepts a 1x1 patch size and 14x14 image size.
+
+    +---------+-------------------+
+    | Name    | Value             |
+    +=========+===================+
+    | Acc@1   |  74.504%          |
+    +---------+-------------------+
+    | Acc@5   |  91.288%          |
+    +---------+-------------------+
+    | #Params |  20.88M           |
+    +---------+-------------------+
+
+    References
+    ----------
+    `B-cos Networks: Alignment is All We Need for Interpretability <https://arxiv.org/abs/2205.10268>`_
+
+    `Better plain ViT baselines for ImageNet-1k <https://arxiv.org/abs/2205.01580>`_
+
+    `Early Convolutions Help Transformers See Better <https://arxiv.org/abs/2106.14881>`_
+
+    Parameters
+    ----------
+    pretrained : bool
+        If True, returns a model pre-trained on ImageNet
+    progress : bool
+        If True, displays a progress bar of the download to stderr
+    **kwargs : Any, optional
+        Additional arguments passed to the model constructor
+        Please see source code for details.
+    """
+    return _get_vit_model(
+        "bcos_vitc_s_patch1_14",
+        pretrained,
+        progress,
+        base_network="vit_final",
+        **kwargs,
+    )
+
+
+@register
+def vitc_b_patch1_14(pretrained: bool = False, progress: bool = True, **kwargs):
+    """B-cos Simple ViT-B with a convolutional stem.
+    The ViT, after the convolution stem, accepts a 1x1 patch size and 14x14 image size.
+
+    +---------+-------------------+
+    | Name    | Value             |
+    +=========+===================+
+    | Acc@1   |  77.152%          |
+    +---------+-------------------+
+    | Acc@5   |  92.926%          |
+    +---------+-------------------+
+    | #Params |  81.37M           |
+    +---------+-------------------+
+
+    References
+    ----------
+    `B-cos Networks: Alignment is All We Need for Interpretability <https://arxiv.org/abs/2205.10268>`_
+
+    `Better plain ViT baselines for ImageNet-1k <https://arxiv.org/abs/2205.01580>`_
+
+    `Early Convolutions Help Transformers See Better <https://arxiv.org/abs/2106.14881>`_
+
+    Parameters
+    ----------
+    pretrained : bool
+        If True, returns a model pre-trained on ImageNet
+    progress : bool
+        If True, displays a progress bar of the download to stderr
+    **kwargs : Any, optional
+        Additional arguments passed to the model constructor
+        Please see source code for details.
+    """
+    return _get_vit_model(
+        "bcos_vitc_b_patch1_14",
+        pretrained,
+        progress,
+        base_network="vit_final",
+        **kwargs,
+    )
+
+
+@register
+def vitc_l_patch1_14(pretrained: bool = False, progress: bool = True, **kwargs):
+    """B-cos Simple ViT-L with a convolutional stem.
+    The ViT, after the convolution stem, accepts a 1x1 patch size and 14x14 image size.
+
+    +---------+-------------------+
+    | Name    | Value             |
+    +=========+===================+
+    | Acc@1   |  77.782%          |
+    +---------+-------------------+
+    | Acc@5   |  92.966%          |
+    +---------+-------------------+
+    | #Params |  167.44M          |
+    +---------+-------------------+
+
+    References
+    ----------
+    `B-cos Networks: Alignment is All We Need for Interpretability <https://arxiv.org/abs/2205.10268>`_
+
+    `Better plain ViT baselines for ImageNet-1k <https://arxiv.org/abs/2205.01580>`_
+
+    `Early Convolutions Help Transformers See Better <https://arxiv.org/abs/2106.14881>`_
+
+    Parameters
+    ----------
+    pretrained : bool
+        If True, returns a model pre-trained on ImageNet
+    progress : bool
+        If True, displays a progress bar of the download to stderr
+    **kwargs : Any, optional
+        Additional arguments passed to the model constructor
+        Please see source code for details.
+    """
+    return _get_vit_model(
+        "bcos_vitc_l_patch1_14",
+        pretrained,
+        progress,
+        base_network="vit_final",
+        **kwargs,
+    )
+
+
+@register
+def standard_simple_vit_ti_patch16_224(
+    pretrained: bool = False, progress: bool = True, **kwargs
+):
+    """Standard Simple ViT-Ti with 16x16 patch size and 224x224 image size.
+    This is NOT a B-cos model.
+
+    +---------+-------------------+
+    | Name    | Value             |
+    +=========+===================+
+    | Acc@1   |  70.230%          |
+    +---------+-------------------+
+    | Acc@5   |  89.380%          |
+    +---------+-------------------+
+    | #Params |  5.67M            |
+    +---------+-------------------+
+
+    References
+    ----------
+    `Better plain ViT baselines for ImageNet-1k <https://arxiv.org/abs/2205.01580>`_
+
+    Parameters
+    ----------
+    pretrained : bool
+        If True, returns a model pre-trained on ImageNet
+    progress : bool
+        If True, displays a progress bar of the download to stderr
+    **kwargs : Any, optional
+        Additional arguments passed to the model constructor
+        Please see source code for details.
+    """
+    return _get_vit_model(
+        "simple_vit_ti_patch16_224",
+        pretrained,
+        progress,
+        base_network="vit_final",
+        **kwargs,
+    )
+
+
+@register
+def standard_simple_vit_s_patch16_224(
+    pretrained: bool = False, progress: bool = True, **kwargs
+):
+    """Standard Simple ViT-S with 16x16 patch size and 224x224 image size.
+    This is NOT a B-cos model.
+
+    +---------+-------------------+
+    | Name    | Value             |
+    +=========+===================+
+    | Acc@1   |  74.470%          |
+    +---------+-------------------+
+    | Acc@5   |  91.226%          |
+    +---------+-------------------+
+    | #Params |  21.96M           |
+    +---------+-------------------+
+
+    References
+    ----------
+    `Better plain ViT baselines for ImageNet-1k <https://arxiv.org/abs/2205.01580>`_
+
+    Parameters
+    ----------
+    pretrained : bool
+        If True, returns a model pre-trained on ImageNet
+    progress : bool
+        If True, displays a progress bar of the download to stderr
+    **kwargs : Any, optional
+        Additional arguments passed to the model constructor
+        Please see source code for details.
+    """
+    return _get_vit_model(
+        "simple_vit_s_patch16_224",
+        pretrained,
+        progress,
+        base_network="vit_final",
+        **kwargs,
+    )
+
+
+@register
+def standard_simple_vit_b_patch16_224(
+    pretrained: bool = False, progress: bool = True, **kwargs
+):
+    """Standard Simple ViT-B with 16x16 patch size and 224x224 image size.
+    This is NOT a B-cos model.
+
+    +---------+-------------------+
+    | Name    | Value             |
+    +=========+===================+
+    | Acc@1   |  75.300%          |
+    +---------+-------------------+
+    | Acc@5   |  91.026%          |
+    +---------+-------------------+
+    | #Params |  86.38M           |
+    +---------+-------------------+
+
+    References
+    ----------
+    `Better plain ViT baselines for ImageNet-1k <https://arxiv.org/abs/2205.01580>`_
+
+    Parameters
+    ----------
+    pretrained : bool
+        If True, returns a model pre-trained on ImageNet
+    progress : bool
+        If True, displays a progress bar of the download to stderr
+    **kwargs : Any, optional
+        Additional arguments passed to the model constructor
+        Please see source code for details.
+    """
+    return _get_vit_model(
+        "simple_vit_b_patch16_224",
+        pretrained,
+        progress,
+        base_network="vit_final",
+        **kwargs,
+    )
+
+
+@register
+def standard_simple_vit_l_patch16_224(
+    pretrained: bool = False, progress: bool = True, **kwargs
+):
+    """Standard Simple ViT-L with 16x16 patch size and 224x224 image size.
+    This is NOT a B-cos model.
+
+    +---------+-------------------+
+    | Name    | Value             |
+    +=========+===================+
+    | Acc@1   |  75.710%          |
+    +---------+-------------------+
+    | Acc@5   |  90.050%          |
+    +---------+-------------------+
+    | #Params |  178.10M          |
+    +---------+-------------------+
+
+    References
+    ----------
+    `Better plain ViT baselines for ImageNet-1k <https://arxiv.org/abs/2205.01580>`_
+
+    Parameters
+    ----------
+    pretrained : bool
+        If True, returns a model pre-trained on ImageNet
+    progress : bool
+        If True, displays a progress bar of the download to stderr
+    **kwargs : Any, optional
+        Additional arguments passed to the model constructor
+        Please see source code for details.
+    """
+    return _get_vit_model(
+        "simple_vit_l_patch16_224",
+        pretrained,
+        progress,
+        base_network="vit_final",
+        **kwargs,
+    )
+
+
+@register
+def standard_vitc_ti_patch1_14(
+    pretrained: bool = False, progress: bool = True, **kwargs
+):
+    """Standard Simple ViT-Ti with a convolutional stem.
+    The ViT, after the convolution stem, accepts a 1x1 patch size and 14x14 image size.
+    This is NOT a B-cos model.
+
+    +---------+-------------------+
+    | Name    | Value             |
+    +=========+===================+
+    | Acc@1   |  72.590%          |
+    +---------+-------------------+
+    | Acc@5   |  90.788%          |
+    +---------+-------------------+
+    | #Params |  5.33M            |
+    +---------+-------------------+
+
+    References
+    ----------
+    `Better plain ViT baselines for ImageNet-1k <https://arxiv.org/abs/2205.01580>`_
+
+    `Early Convolutions Help Transformers See Better <https://arxiv.org/abs/2106.14881>`_
+
+    Parameters
+    ----------
+    pretrained : bool
+        If True, returns a model pre-trained on ImageNet
+    progress : bool
+        If True, displays a progress bar of the download to stderr
+    **kwargs : Any, optional
+        Additional arguments passed to the model constructor
+        Please see source code for details.
+    """
+    return _get_vit_model(
+        "vitc_ti_patch1_14",
+        pretrained,
+        progress,
+        base_network="vit_final",
+        **kwargs,
+    )
+
+
+@register
+def standard_vitc_s_patch1_14(
+    pretrained: bool = False, progress: bool = True, **kwargs
+):
+    """Standard Simple ViT-S with a convolutional stem.
+    The ViT, after the convolution stem, accepts a 1x1 patch size and 14x14 image size.
+    This is NOT a B-cos model.
+
+    +---------+-------------------+
+    | Name    | Value             |
+    +=========+===================+
+    | Acc@1   |  75.756%          |
+    +---------+-------------------+
+    | Acc@5   |  91.994%          |
+    +---------+-------------------+
+    | #Params |  20.91M           |
+    +---------+-------------------+
+
+    References
+    ----------
+    `Better plain ViT baselines for ImageNet-1k <https://arxiv.org/abs/2205.01580>`_
+
+    `Early Convolutions Help Transformers See Better <https://arxiv.org/abs/2106.14881>`_
+
+    Parameters
+    ----------
+    pretrained : bool
+        If True, returns a model pre-trained on ImageNet
+    progress : bool
+        If True, displays a progress bar of the download to stderr
+    **kwargs : Any, optional
+        Additional arguments passed to the model constructor
+        Please see source code for details.
+    """
+    return _get_vit_model(
+        "vitc_s_patch1_14",
+        pretrained,
+        progress,
+        base_network="vit_final",
+        **kwargs,
+    )
+
+
+@register
+def standard_vitc_b_patch1_14(
+    pretrained: bool = False, progress: bool = True, **kwargs
+):
+    """Standard Simple ViT-B with a convolutional stem.
+    The ViT, after the convolution stem, accepts a 1x1 patch size and 14x14 image size.
+    This is NOT a B-cos model.
+
+    +---------+-------------------+
+    | Name    | Value             |
+    +=========+===================+
+    | Acc@1   |  76.790%          |
+    +---------+-------------------+
+    | Acc@5   |  92.024%          |
+    +---------+-------------------+
+    | #Params |  81.39M           |
+    +---------+-------------------+
+
+    References
+    ----------
+    `Better plain ViT baselines for ImageNet-1k <https://arxiv.org/abs/2205.01580>`_
+
+    `Early Convolutions Help Transformers See Better <https://arxiv.org/abs/2106.14881>`_
+
+    Parameters
+    ----------
+    pretrained : bool
+        If True, returns a model pre-trained on ImageNet
+    progress : bool
+        If True, displays a progress bar of the download to stderr
+    **kwargs : Any, optional
+        Additional arguments passed to the model constructor
+        Please see source code for details.
+    """
+    return _get_vit_model(
+        "vitc_b_patch1_14",
+        pretrained,
+        progress,
+        base_network="vit_final",
+        **kwargs,
+    )
+
+
+@register
+def standard_vitc_l_patch1_14(
+    pretrained: bool = False, progress: bool = True, **kwargs
+):
+    """Standard Simple ViT-L with a convolutional stem.
+    The ViT, after the convolution stem, accepts a 1x1 patch size and 14x14 image size.
+    This is NOT a B-cos model.
+
+    +---------+-------------------+
+    | Name    | Value             |
+    +=========+===================+
+    | Acc@1   |  77.866%          |
+    +---------+-------------------+
+    | Acc@5   |  92.298%          |
+    +---------+-------------------+
+    | #Params |  167.54M          |
+    +---------+-------------------+
+
+    References
+    ----------
+    `Better plain ViT baselines for ImageNet-1k <https://arxiv.org/abs/2205.01580>`_
+
+    `Early Convolutions Help Transformers See Better <https://arxiv.org/abs/2106.14881>`_
+
+    Parameters
+    ----------
+    pretrained : bool
+        If True, returns a model pre-trained on ImageNet
+    progress : bool
+        If True, displays a progress bar of the download to stderr
+    **kwargs : Any, optional
+        Additional arguments passed to the model constructor
+        Please see source code for details.
+    """
+    return _get_vit_model(
+        "vitc_l_patch1_14",
+        pretrained,
+        progress,
+        base_network="vit_final",
+        **kwargs,
+    )
```

### Comparing `bcos-0.0.4/bcos/models/resnet.py` & `bcos-0.1.0/bcos/models/resnet.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/models/vgg.py` & `bcos-0.1.0/bcos/models/vgg.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/modules/bcosconv2d.py` & `bcos-0.1.0/bcos/modules/bcosconv2d.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/modules/bcoslinear.py` & `bcos-0.1.0/bcos/modules/bcoslinear.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/modules/common.py` & `bcos-0.1.0/bcos/modules/common.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/modules/logitlayer.py` & `bcos-0.1.0/bcos/modules/logitlayer.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/modules/losses.py` & `bcos-0.1.0/bcos/modules/losses.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/modules/norms/centered_norms.py` & `bcos-0.1.0/bcos/modules/norms/centered_norms.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/modules/norms/uncentered_norms/allnorm_uncentered.py` & `bcos-0.1.0/bcos/modules/norms/uncentered_norms/allnorm_uncentered.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/modules/norms/uncentered_norms/batchnorm_uncentered.py` & `bcos-0.1.0/bcos/modules/norms/uncentered_norms/batchnorm_uncentered.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/modules/norms/uncentered_norms/groupnorm_uncentered.py` & `bcos-0.1.0/bcos/modules/norms/uncentered_norms/groupnorm_uncentered.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/modules/norms/uncentered_norms/posnorm_uncentered.py` & `bcos-0.1.0/bcos/modules/norms/uncentered_norms/posnorm_uncentered.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/modules/norms/utils.py` & `bcos-0.1.0/bcos/modules/norms/utils.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/optim/lr_scheduler_factory.py` & `bcos-0.1.0/bcos/optim/lr_scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/optim/optimizer_factory.py` & `bcos-0.1.0/bcos/optim/optimizer_factory.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/settings.py` & `bcos-0.1.0/bcos/settings.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/training/agc.py` & `bcos-0.1.0/bcos/training/agc.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/training/callbacks/explanation_logger.py` & `bcos-0.1.0/bcos/training/callbacks/explanation_logger.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/training/callbacks/metricstracker.py` & `bcos-0.1.0/bcos/training/callbacks/metricstracker.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/training/ema.py` & `bcos-0.1.0/bcos/training/ema.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos/training/trainer.py` & `bcos-0.1.0/bcos/training/trainer.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.4/bcos.egg-info/SOURCES.txt` & `bcos-0.1.0/bcos.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -28,28 +28,31 @@
 bcos/experiments/CIFAR10/norm_ablations_final/model.py
 bcos/experiments/ImageNet/baseline/experiment_parameters.py
 bcos/experiments/ImageNet/baseline/model.py
 bcos/experiments/ImageNet/bcos_final/experiment_parameters.py
 bcos/experiments/ImageNet/bcos_final/model.py
 bcos/experiments/ImageNet/bcos_final_long/experiment_parameters.py
 bcos/experiments/ImageNet/bcos_final_long/model.py
+bcos/experiments/ImageNet/vit_final/experiment_parameters.py
+bcos/experiments/ImageNet/vit_final/model.py
 bcos/experiments/utils/__init__.py
 bcos/experiments/utils/config_utils.py
 bcos/experiments/utils/exceptions.py
 bcos/experiments/utils/structure_constants.py
 bcos/experiments/utils/experiment_utils/__init__.py
 bcos/experiments/utils/experiment_utils/experiment_utils.py
 bcos/experiments/utils/experiment_utils/loading_utils.py
 bcos/experiments/utils/experiment_utils/metric_utils.py
 bcos/models/__init__.py
 bcos/models/convnext.py
 bcos/models/densenet.py
 bcos/models/pretrained.py
 bcos/models/resnet.py
 bcos/models/vgg.py
+bcos/models/vit.py
 bcos/modules/__init__.py
 bcos/modules/bcosconv2d.py
 bcos/modules/bcoslinear.py
 bcos/modules/common.py
 bcos/modules/logitlayer.py
 bcos/modules/losses.py
 bcos/modules/norms/__init__.py
```

### Comparing `bcos-0.0.4/pyproject.toml` & `bcos-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "bcos"
 authors = [
     {name = "Moritz Böhle", email = "mboehle@mpi-inf.mpg.de"},
     {name = "Navdeeppal Singh", email = "npsingh0181@gmail.com"},
 ]
-version = "0.0.4"
+version = "0.1.0"
 description = "B-cos models."
 readme = "README.md"
 license = {text = "Apache License 2.0"}
 
 [project.urls]
 repository = "https://github.com/B-cos/B-cos-v2/"
```

