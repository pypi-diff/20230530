# Comparing `tmp/innerverz-0.0.20.tar.gz` & `tmp/innerverz-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innerverz-0.0.20.tar", last modified: Sun May 28 05:17:53 2023, max compression
+gzip compressed data, was "innerverz-0.0.21.tar", last modified: Tue May 30 02:39:15 2023, max compression
```

## Comparing `innerverz-0.0.20.tar` & `innerverz-0.0.21.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.425320 innerverz-0.0.20/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1073 2023-05-26 05:00:26.000000 innerverz-0.0.20/LICENSE.txt
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      194 2023-05-28 05:17:53.425320 innerverz-0.0.20/PKG-INFO
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       10 2023-05-26 05:00:26.000000 innerverz-0.0.20/README.md
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.417321 innerverz-0.0.20/innerverz/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1417 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/__init__.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.417321 innerverz-0.0.20/innerverz/data_process/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       30 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/data_process/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3493 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/data_process/main.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.417321 innerverz-0.0.20/innerverz/deblurrer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deblurrer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2171 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deblurrer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3609 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deblurrer/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      867 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deblurrer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.417321 innerverz-0.0.20/innerverz/deca/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       23 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deca/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    16976 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deca/main.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.417321 innerverz-0.0.20/innerverz/deca/models/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12616 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deca/models/FLAME.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deca/models/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2464 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deca/models/decoders.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1983 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deca/models/detectors.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1427 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deca/models/encoders.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1983 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deca/models/face_detectors.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    13786 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deca/models/lbs.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8386 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deca/models/resnet.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1126 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deca/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.417321 innerverz-0.0.20/innerverz/deca/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deca/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5036 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deca/utils/cfg.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.417321 innerverz-0.0.20/innerverz/deca/utils/rasterizer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deca/utils/rasterizer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      706 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deca/utils/rasterizer/setup.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    22281 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deca/utils/renderer.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12710 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deca/utils/rotation_converter.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5574 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deca/utils/tensor_cropper.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    26962 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deca/utils/util.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.417321 innerverz-0.0.20/innerverz/deep3dmm/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deep3dmm/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3414 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deep3dmm/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    25860 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deep3dmm/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      651 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/deep3dmm/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.417321 innerverz-0.0.20/innerverz/face_alignment/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      125 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_alignment/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6646 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_alignment/graphic_utils.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5089 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_alignment/landmark.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9474 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_alignment/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12774 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_alignment/retina_face.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      656 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_alignment/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.417321 innerverz-0.0.20/innerverz/face_alignment/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       24 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_alignment/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3354 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_alignment/utils/face_align.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4933 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_alignment/utils/transform.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.417321 innerverz-0.0.20/innerverz/face_color_transfer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       22 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_color_transfer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5238 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_color_transfer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8503 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_color_transfer/nets.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.417321 innerverz-0.0.20/innerverz/face_color_transfer/sub_nets/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      100 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_color_transfer/sub_nets/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     7018 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_color_transfer/sub_nets/blend_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3642 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_color_transfer/sub_nets/discriminator.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3788 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_color_transfer/sub_nets/vgg19_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9366 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_color_transfer/sub_nets/warp_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2047 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_color_transfer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.417321 innerverz-0.0.20/innerverz/face_enhancer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       30 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_enhancer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3745 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_enhancer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4079 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_enhancer/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      792 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_enhancer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.421321 innerverz-0.0.20/innerverz/face_parser/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       28 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_parser/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2682 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_parser/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    11822 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_parser/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      713 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/face_parser/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.421321 innerverz-0.0.20/innerverz/head_color_transfer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       22 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/head_color_transfer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5409 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/head_color_transfer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8742 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/head_color_transfer/nets.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.421321 innerverz-0.0.20/innerverz/head_color_transfer/sub_nets/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      100 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/head_color_transfer/sub_nets/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     7018 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/head_color_transfer/sub_nets/blend_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3642 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/head_color_transfer/sub_nets/discriminator.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3788 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/head_color_transfer/sub_nets/vgg19_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9366 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/head_color_transfer/sub_nets/warp_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1997 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/head_color_transfer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.421321 innerverz-0.0.20/innerverz/id_extractor/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       29 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/id_extractor/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2253 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/id_extractor/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5192 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/id_extractor/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      717 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/id_extractor/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.421321 innerverz-0.0.20/innerverz/relighter/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/relighter/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2912 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/relighter/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4546 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/relighter/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3078 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/relighter/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.421321 innerverz-0.0.20/innerverz/upsampler/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       28 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/upsampler/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2250 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/upsampler/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    36818 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/upsampler/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      854 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/upsampler/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.421321 innerverz-0.0.20/innerverz/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      109 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1438 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/utils/download.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1009 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/utils/input.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    15896 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/utils/utils.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.421321 innerverz-0.0.20/innerverz/video_faceparser/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       34 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/video_faceparser/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6039 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/video_faceparser/main.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.421321 innerverz-0.0.20/innerverz/video_faceparser/model/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       79 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/video_faceparser/model/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4009 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/video_faceparser/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      217 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/video_faceparser/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.421321 innerverz-0.0.20/innerverz/video_faceparser/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       94 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/video_faceparser/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3079 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/video_faceparser/utils/corr.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8847 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/video_faceparser/utils/extractor.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3984 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/video_faceparser/utils/update.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6502 2023-05-28 05:15:07.000000 innerverz-0.0.20/innerverz/video_faceparser/utils/util.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.417321 innerverz-0.0.20/innerverz.egg-info/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      194 2023-05-28 05:17:53.000000 innerverz-0.0.20/innerverz.egg-info/PKG-INFO
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6840 2023-05-28 05:17:53.000000 innerverz-0.0.20/innerverz.egg-info/SOURCES.txt
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        1 2023-05-28 05:17:53.000000 innerverz-0.0.20/innerverz.egg-info/dependency_links.txt
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       74 2023-05-28 05:17:53.000000 innerverz-0.0.20/innerverz.egg-info/requires.txt
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       21 2023-05-28 05:17:53.000000 innerverz-0.0.20/innerverz.egg-info/top_level.txt
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.421321 innerverz-0.0.20/innerverz_/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1417 2023-05-26 07:19:35.000000 innerverz-0.0.20/innerverz_/__init__.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.421321 innerverz-0.0.20/innerverz_/data_process/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       30 2023-05-26 07:19:35.000000 innerverz-0.0.20/innerverz_/data_process/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3459 2023-05-26 07:19:35.000000 innerverz-0.0.20/innerverz_/data_process/main.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.421321 innerverz-0.0.20/innerverz_/deblurrer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-26 07:19:35.000000 innerverz-0.0.20/innerverz_/deblurrer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2171 2023-05-26 07:19:35.000000 innerverz-0.0.20/innerverz_/deblurrer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3609 2023-05-26 07:19:35.000000 innerverz-0.0.20/innerverz_/deblurrer/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      867 2023-05-26 07:19:35.000000 innerverz-0.0.20/innerverz_/deblurrer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.421321 innerverz-0.0.20/innerverz_/deca/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       23 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deca/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    16976 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deca/main.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.421321 innerverz-0.0.20/innerverz_/deca/models/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12616 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deca/models/FLAME.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deca/models/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2464 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deca/models/decoders.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1983 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deca/models/detectors.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1427 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deca/models/encoders.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1983 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deca/models/face_detectors.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    13786 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deca/models/lbs.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8386 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deca/models/resnet.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1126 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deca/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.421321 innerverz-0.0.20/innerverz_/deca/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deca/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5036 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deca/utils/cfg.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.421321 innerverz-0.0.20/innerverz_/deca/utils/rasterizer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deca/utils/rasterizer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      706 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deca/utils/rasterizer/setup.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    22281 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deca/utils/renderer.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12710 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deca/utils/rotation_converter.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5574 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deca/utils/tensor_cropper.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    26962 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deca/utils/util.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.425320 innerverz-0.0.20/innerverz_/deep3dmm/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deep3dmm/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3414 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deep3dmm/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    25860 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deep3dmm/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      651 2023-05-26 07:19:36.000000 innerverz-0.0.20/innerverz_/deep3dmm/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.425320 innerverz-0.0.20/innerverz_/face_alignment/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      125 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_alignment/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6646 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_alignment/graphic_utils.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5089 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_alignment/landmark.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9535 2023-05-26 08:27:23.000000 innerverz-0.0.20/innerverz_/face_alignment/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12774 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_alignment/retina_face.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      656 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_alignment/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.425320 innerverz-0.0.20/innerverz_/face_alignment/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       24 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_alignment/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3354 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_alignment/utils/face_align.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4933 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_alignment/utils/transform.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.425320 innerverz-0.0.20/innerverz_/face_color_transfer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       22 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_color_transfer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5238 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_color_transfer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8503 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_color_transfer/nets.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.425320 innerverz-0.0.20/innerverz_/face_color_transfer/sub_nets/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      100 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_color_transfer/sub_nets/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     7018 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_color_transfer/sub_nets/blend_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3642 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_color_transfer/sub_nets/discriminator.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3788 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_color_transfer/sub_nets/vgg19_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9366 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_color_transfer/sub_nets/warp_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2047 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_color_transfer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.425320 innerverz-0.0.20/innerverz_/face_enhancer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       30 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_enhancer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3745 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_enhancer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4079 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_enhancer/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      792 2023-05-26 07:19:37.000000 innerverz-0.0.20/innerverz_/face_enhancer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.425320 innerverz-0.0.20/innerverz_/face_parser/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       28 2023-05-26 07:19:38.000000 innerverz-0.0.20/innerverz_/face_parser/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2682 2023-05-26 07:19:38.000000 innerverz-0.0.20/innerverz_/face_parser/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    11822 2023-05-26 07:19:38.000000 innerverz-0.0.20/innerverz_/face_parser/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      713 2023-05-26 07:19:38.000000 innerverz-0.0.20/innerverz_/face_parser/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.425320 innerverz-0.0.20/innerverz_/head_color_transfer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       22 2023-05-26 07:19:38.000000 innerverz-0.0.20/innerverz_/head_color_transfer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5409 2023-05-26 07:19:38.000000 innerverz-0.0.20/innerverz_/head_color_transfer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8742 2023-05-26 07:19:38.000000 innerverz-0.0.20/innerverz_/head_color_transfer/nets.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.425320 innerverz-0.0.20/innerverz_/head_color_transfer/sub_nets/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      100 2023-05-26 07:19:38.000000 innerverz-0.0.20/innerverz_/head_color_transfer/sub_nets/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     7018 2023-05-26 07:19:38.000000 innerverz-0.0.20/innerverz_/head_color_transfer/sub_nets/blend_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3642 2023-05-26 07:19:38.000000 innerverz-0.0.20/innerverz_/head_color_transfer/sub_nets/discriminator.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3788 2023-05-26 07:19:38.000000 innerverz-0.0.20/innerverz_/head_color_transfer/sub_nets/vgg19_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9366 2023-05-26 07:19:38.000000 innerverz-0.0.20/innerverz_/head_color_transfer/sub_nets/warp_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1997 2023-05-26 07:19:38.000000 innerverz-0.0.20/innerverz_/head_color_transfer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.425320 innerverz-0.0.20/innerverz_/id_extractor/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       29 2023-05-26 07:19:39.000000 innerverz-0.0.20/innerverz_/id_extractor/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2253 2023-05-26 07:19:39.000000 innerverz-0.0.20/innerverz_/id_extractor/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5192 2023-05-26 07:19:39.000000 innerverz-0.0.20/innerverz_/id_extractor/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      717 2023-05-26 07:19:39.000000 innerverz-0.0.20/innerverz_/id_extractor/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.425320 innerverz-0.0.20/innerverz_/relighter/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-26 07:19:39.000000 innerverz-0.0.20/innerverz_/relighter/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2912 2023-05-26 07:19:39.000000 innerverz-0.0.20/innerverz_/relighter/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4546 2023-05-26 07:19:39.000000 innerverz-0.0.20/innerverz_/relighter/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3078 2023-05-26 07:19:39.000000 innerverz-0.0.20/innerverz_/relighter/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.425320 innerverz-0.0.20/innerverz_/upsampler/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       28 2023-05-26 07:19:39.000000 innerverz-0.0.20/innerverz_/upsampler/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2250 2023-05-26 07:19:39.000000 innerverz-0.0.20/innerverz_/upsampler/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    36818 2023-05-26 07:19:39.000000 innerverz-0.0.20/innerverz_/upsampler/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      854 2023-05-26 07:19:39.000000 innerverz-0.0.20/innerverz_/upsampler/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.425320 innerverz-0.0.20/innerverz_/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      109 2023-05-26 07:19:39.000000 innerverz-0.0.20/innerverz_/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1438 2023-05-26 07:19:39.000000 innerverz-0.0.20/innerverz_/utils/download.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1009 2023-05-26 07:19:39.000000 innerverz-0.0.20/innerverz_/utils/input.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    15902 2023-05-26 07:19:39.000000 innerverz-0.0.20/innerverz_/utils/utils.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.425320 innerverz-0.0.20/innerverz_/video_faceparser/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       34 2023-05-26 07:19:40.000000 innerverz-0.0.20/innerverz_/video_faceparser/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6039 2023-05-26 07:19:40.000000 innerverz-0.0.20/innerverz_/video_faceparser/main.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.425320 innerverz-0.0.20/innerverz_/video_faceparser/model/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       79 2023-05-26 07:19:40.000000 innerverz-0.0.20/innerverz_/video_faceparser/model/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4009 2023-05-26 07:19:40.000000 innerverz-0.0.20/innerverz_/video_faceparser/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      217 2023-05-26 07:19:40.000000 innerverz-0.0.20/innerverz_/video_faceparser/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:17:53.425320 innerverz-0.0.20/innerverz_/video_faceparser/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       94 2023-05-26 07:19:40.000000 innerverz-0.0.20/innerverz_/video_faceparser/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3079 2023-05-26 07:19:40.000000 innerverz-0.0.20/innerverz_/video_faceparser/utils/corr.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8847 2023-05-26 07:19:40.000000 innerverz-0.0.20/innerverz_/video_faceparser/utils/extractor.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3984 2023-05-26 07:19:40.000000 innerverz-0.0.20/innerverz_/video_faceparser/utils/update.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6502 2023-05-26 07:19:40.000000 innerverz-0.0.20/innerverz_/video_faceparser/utils/util.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       89 2023-05-26 05:00:26.000000 innerverz-0.0.20/pyproject.toml
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       38 2023-05-28 05:17:53.429320 innerverz-0.0.20/setup.cfg
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      809 2023-05-28 05:14:55.000000 innerverz-0.0.20/setup.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.716017 innerverz-0.0.21/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1073 2023-05-26 05:00:26.000000 innerverz-0.0.21/LICENSE.txt
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      194 2023-05-30 02:39:15.716017 innerverz-0.0.21/PKG-INFO
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       10 2023-05-26 05:00:26.000000 innerverz-0.0.21/README.md
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.704017 innerverz-0.0.21/innerverz/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1417 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/__init__.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.704017 innerverz-0.0.21/innerverz/data_process/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       30 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/data_process/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3493 2023-05-30 02:35:02.000000 innerverz-0.0.21/innerverz/data_process/main.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.704017 innerverz-0.0.21/innerverz/deblurrer/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deblurrer/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2171 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deblurrer/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3609 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deblurrer/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      867 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deblurrer/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.704017 innerverz-0.0.21/innerverz/deca/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       23 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deca/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    16976 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deca/main.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.704017 innerverz-0.0.21/innerverz/deca/models/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12616 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deca/models/FLAME.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deca/models/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2464 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deca/models/decoders.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1983 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deca/models/detectors.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1427 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deca/models/encoders.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1983 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deca/models/face_detectors.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    13786 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deca/models/lbs.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8386 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deca/models/resnet.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1126 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deca/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.704017 innerverz-0.0.21/innerverz/deca/utils/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deca/utils/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5036 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deca/utils/cfg.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.704017 innerverz-0.0.21/innerverz/deca/utils/rasterizer/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deca/utils/rasterizer/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      706 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deca/utils/rasterizer/setup.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    22281 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deca/utils/renderer.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12710 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deca/utils/rotation_converter.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5574 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deca/utils/tensor_cropper.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    26962 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deca/utils/util.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.704017 innerverz-0.0.21/innerverz/deep3dmm/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deep3dmm/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3414 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deep3dmm/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    25860 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deep3dmm/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      651 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/deep3dmm/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.708017 innerverz-0.0.21/innerverz/face_alignment/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      125 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_alignment/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6646 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_alignment/graphic_utils.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5089 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_alignment/landmark.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9719 2023-05-30 02:24:53.000000 innerverz-0.0.21/innerverz/face_alignment/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12774 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_alignment/retina_face.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      656 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_alignment/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.708017 innerverz-0.0.21/innerverz/face_alignment/utils/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       24 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_alignment/utils/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3354 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_alignment/utils/face_align.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4933 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_alignment/utils/transform.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.708017 innerverz-0.0.21/innerverz/face_color_transfer/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       22 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_color_transfer/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5238 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_color_transfer/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8503 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_color_transfer/nets.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.708017 innerverz-0.0.21/innerverz/face_color_transfer/sub_nets/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      100 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_color_transfer/sub_nets/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     7018 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_color_transfer/sub_nets/blend_net.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3642 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_color_transfer/sub_nets/discriminator.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3788 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_color_transfer/sub_nets/vgg19_net.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9366 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_color_transfer/sub_nets/warp_net.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2047 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_color_transfer/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.708017 innerverz-0.0.21/innerverz/face_enhancer/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       30 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_enhancer/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3745 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_enhancer/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4079 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_enhancer/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      792 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_enhancer/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.708017 innerverz-0.0.21/innerverz/face_parser/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       28 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_parser/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2682 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_parser/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    11822 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_parser/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      713 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/face_parser/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.708017 innerverz-0.0.21/innerverz/head_color_transfer/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       22 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/head_color_transfer/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5409 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/head_color_transfer/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8742 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/head_color_transfer/nets.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.708017 innerverz-0.0.21/innerverz/head_color_transfer/sub_nets/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      100 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/head_color_transfer/sub_nets/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     7018 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/head_color_transfer/sub_nets/blend_net.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3642 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/head_color_transfer/sub_nets/discriminator.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3788 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/head_color_transfer/sub_nets/vgg19_net.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9366 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/head_color_transfer/sub_nets/warp_net.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1997 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/head_color_transfer/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.708017 innerverz-0.0.21/innerverz/id_extractor/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       29 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/id_extractor/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2253 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/id_extractor/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5192 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/id_extractor/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      717 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/id_extractor/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.708017 innerverz-0.0.21/innerverz/relighter/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/relighter/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2912 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/relighter/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4546 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/relighter/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3078 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/relighter/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.708017 innerverz-0.0.21/innerverz/upsampler/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       28 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/upsampler/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2250 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/upsampler/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    36818 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/upsampler/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      854 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/upsampler/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.708017 innerverz-0.0.21/innerverz/utils/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      109 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/utils/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1438 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/utils/download.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1135 2023-05-30 02:34:43.000000 innerverz-0.0.21/innerverz/utils/input.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    15896 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/utils/utils.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.708017 innerverz-0.0.21/innerverz/video_faceparser/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       34 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/video_faceparser/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6039 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/video_faceparser/main.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.708017 innerverz-0.0.21/innerverz/video_faceparser/model/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       79 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/video_faceparser/model/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4009 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/video_faceparser/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      217 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/video_faceparser/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.712017 innerverz-0.0.21/innerverz/video_faceparser/utils/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       94 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/video_faceparser/utils/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3079 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/video_faceparser/utils/corr.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8847 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/video_faceparser/utils/extractor.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3984 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/video_faceparser/utils/update.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6502 2023-05-28 05:15:07.000000 innerverz-0.0.21/innerverz/video_faceparser/utils/util.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.704017 innerverz-0.0.21/innerverz.egg-info/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      194 2023-05-30 02:39:15.000000 innerverz-0.0.21/innerverz.egg-info/PKG-INFO
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6840 2023-05-30 02:39:15.000000 innerverz-0.0.21/innerverz.egg-info/SOURCES.txt
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        1 2023-05-30 02:39:15.000000 innerverz-0.0.21/innerverz.egg-info/dependency_links.txt
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       74 2023-05-30 02:39:15.000000 innerverz-0.0.21/innerverz.egg-info/requires.txt
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       21 2023-05-30 02:39:15.000000 innerverz-0.0.21/innerverz.egg-info/top_level.txt
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.712017 innerverz-0.0.21/innerverz_/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1417 2023-05-26 07:19:35.000000 innerverz-0.0.21/innerverz_/__init__.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.712017 innerverz-0.0.21/innerverz_/data_process/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       30 2023-05-26 07:19:35.000000 innerverz-0.0.21/innerverz_/data_process/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3459 2023-05-26 07:19:35.000000 innerverz-0.0.21/innerverz_/data_process/main.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.712017 innerverz-0.0.21/innerverz_/deblurrer/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-26 07:19:35.000000 innerverz-0.0.21/innerverz_/deblurrer/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2171 2023-05-26 07:19:35.000000 innerverz-0.0.21/innerverz_/deblurrer/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3609 2023-05-26 07:19:35.000000 innerverz-0.0.21/innerverz_/deblurrer/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      867 2023-05-26 07:19:35.000000 innerverz-0.0.21/innerverz_/deblurrer/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.712017 innerverz-0.0.21/innerverz_/deca/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       23 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deca/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    16976 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deca/main.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.712017 innerverz-0.0.21/innerverz_/deca/models/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12616 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deca/models/FLAME.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deca/models/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2464 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deca/models/decoders.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1983 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deca/models/detectors.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1427 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deca/models/encoders.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1983 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deca/models/face_detectors.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    13786 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deca/models/lbs.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8386 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deca/models/resnet.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1126 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deca/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.712017 innerverz-0.0.21/innerverz_/deca/utils/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deca/utils/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5036 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deca/utils/cfg.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.712017 innerverz-0.0.21/innerverz_/deca/utils/rasterizer/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deca/utils/rasterizer/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      706 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deca/utils/rasterizer/setup.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    22281 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deca/utils/renderer.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12710 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deca/utils/rotation_converter.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5574 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deca/utils/tensor_cropper.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    26962 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deca/utils/util.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.712017 innerverz-0.0.21/innerverz_/deep3dmm/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deep3dmm/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3414 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deep3dmm/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    25860 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deep3dmm/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      651 2023-05-26 07:19:36.000000 innerverz-0.0.21/innerverz_/deep3dmm/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.712017 innerverz-0.0.21/innerverz_/face_alignment/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      125 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_alignment/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6646 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_alignment/graphic_utils.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5089 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_alignment/landmark.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9535 2023-05-26 08:27:23.000000 innerverz-0.0.21/innerverz_/face_alignment/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12774 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_alignment/retina_face.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      656 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_alignment/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.712017 innerverz-0.0.21/innerverz_/face_alignment/utils/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       24 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_alignment/utils/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3354 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_alignment/utils/face_align.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4933 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_alignment/utils/transform.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.712017 innerverz-0.0.21/innerverz_/face_color_transfer/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       22 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_color_transfer/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5238 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_color_transfer/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8503 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_color_transfer/nets.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.712017 innerverz-0.0.21/innerverz_/face_color_transfer/sub_nets/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      100 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_color_transfer/sub_nets/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     7018 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_color_transfer/sub_nets/blend_net.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3642 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_color_transfer/sub_nets/discriminator.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3788 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_color_transfer/sub_nets/vgg19_net.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9366 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_color_transfer/sub_nets/warp_net.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2047 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_color_transfer/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.712017 innerverz-0.0.21/innerverz_/face_enhancer/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       30 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_enhancer/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3745 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_enhancer/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4079 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_enhancer/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      792 2023-05-26 07:19:37.000000 innerverz-0.0.21/innerverz_/face_enhancer/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.716017 innerverz-0.0.21/innerverz_/face_parser/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       28 2023-05-26 07:19:38.000000 innerverz-0.0.21/innerverz_/face_parser/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2682 2023-05-26 07:19:38.000000 innerverz-0.0.21/innerverz_/face_parser/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    11822 2023-05-26 07:19:38.000000 innerverz-0.0.21/innerverz_/face_parser/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      713 2023-05-26 07:19:38.000000 innerverz-0.0.21/innerverz_/face_parser/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.716017 innerverz-0.0.21/innerverz_/head_color_transfer/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       22 2023-05-26 07:19:38.000000 innerverz-0.0.21/innerverz_/head_color_transfer/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5409 2023-05-26 07:19:38.000000 innerverz-0.0.21/innerverz_/head_color_transfer/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8742 2023-05-26 07:19:38.000000 innerverz-0.0.21/innerverz_/head_color_transfer/nets.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.716017 innerverz-0.0.21/innerverz_/head_color_transfer/sub_nets/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      100 2023-05-26 07:19:38.000000 innerverz-0.0.21/innerverz_/head_color_transfer/sub_nets/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     7018 2023-05-26 07:19:38.000000 innerverz-0.0.21/innerverz_/head_color_transfer/sub_nets/blend_net.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3642 2023-05-26 07:19:38.000000 innerverz-0.0.21/innerverz_/head_color_transfer/sub_nets/discriminator.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3788 2023-05-26 07:19:38.000000 innerverz-0.0.21/innerverz_/head_color_transfer/sub_nets/vgg19_net.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9366 2023-05-26 07:19:38.000000 innerverz-0.0.21/innerverz_/head_color_transfer/sub_nets/warp_net.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1997 2023-05-26 07:19:38.000000 innerverz-0.0.21/innerverz_/head_color_transfer/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.716017 innerverz-0.0.21/innerverz_/id_extractor/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       29 2023-05-26 07:19:39.000000 innerverz-0.0.21/innerverz_/id_extractor/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2253 2023-05-26 07:19:39.000000 innerverz-0.0.21/innerverz_/id_extractor/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5192 2023-05-26 07:19:39.000000 innerverz-0.0.21/innerverz_/id_extractor/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      717 2023-05-26 07:19:39.000000 innerverz-0.0.21/innerverz_/id_extractor/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.716017 innerverz-0.0.21/innerverz_/relighter/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-26 07:19:39.000000 innerverz-0.0.21/innerverz_/relighter/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2912 2023-05-26 07:19:39.000000 innerverz-0.0.21/innerverz_/relighter/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4546 2023-05-26 07:19:39.000000 innerverz-0.0.21/innerverz_/relighter/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3078 2023-05-26 07:19:39.000000 innerverz-0.0.21/innerverz_/relighter/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.716017 innerverz-0.0.21/innerverz_/upsampler/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       28 2023-05-26 07:19:39.000000 innerverz-0.0.21/innerverz_/upsampler/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2250 2023-05-26 07:19:39.000000 innerverz-0.0.21/innerverz_/upsampler/main.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    36818 2023-05-26 07:19:39.000000 innerverz-0.0.21/innerverz_/upsampler/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      854 2023-05-26 07:19:39.000000 innerverz-0.0.21/innerverz_/upsampler/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.716017 innerverz-0.0.21/innerverz_/utils/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      109 2023-05-26 07:19:39.000000 innerverz-0.0.21/innerverz_/utils/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1438 2023-05-26 07:19:39.000000 innerverz-0.0.21/innerverz_/utils/download.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1009 2023-05-26 07:19:39.000000 innerverz-0.0.21/innerverz_/utils/input.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    15902 2023-05-26 07:19:39.000000 innerverz-0.0.21/innerverz_/utils/utils.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.716017 innerverz-0.0.21/innerverz_/video_faceparser/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       34 2023-05-26 07:19:40.000000 innerverz-0.0.21/innerverz_/video_faceparser/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6039 2023-05-26 07:19:40.000000 innerverz-0.0.21/innerverz_/video_faceparser/main.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.716017 innerverz-0.0.21/innerverz_/video_faceparser/model/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       79 2023-05-26 07:19:40.000000 innerverz-0.0.21/innerverz_/video_faceparser/model/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4009 2023-05-26 07:19:40.000000 innerverz-0.0.21/innerverz_/video_faceparser/nets.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      217 2023-05-26 07:19:40.000000 innerverz-0.0.21/innerverz_/video_faceparser/test.py
+drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 02:39:15.716017 innerverz-0.0.21/innerverz_/video_faceparser/utils/
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       94 2023-05-26 07:19:40.000000 innerverz-0.0.21/innerverz_/video_faceparser/utils/__init__.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3079 2023-05-26 07:19:40.000000 innerverz-0.0.21/innerverz_/video_faceparser/utils/corr.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8847 2023-05-26 07:19:40.000000 innerverz-0.0.21/innerverz_/video_faceparser/utils/extractor.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3984 2023-05-26 07:19:40.000000 innerverz-0.0.21/innerverz_/video_faceparser/utils/update.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6502 2023-05-26 07:19:40.000000 innerverz-0.0.21/innerverz_/video_faceparser/utils/util.py
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       89 2023-05-26 05:00:26.000000 innerverz-0.0.21/pyproject.toml
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       38 2023-05-30 02:39:15.716017 innerverz-0.0.21/setup.cfg
+-rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      809 2023-05-30 02:14:31.000000 innerverz-0.0.21/setup.py
```

### Comparing `innerverz-0.0.20/LICENSE.txt` & `innerverz-0.0.21/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/__init__.py` & `innerverz-0.0.21/innerverz/__init__.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/data_process/main.py` & `innerverz-0.0.21/innerverz/data_process/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deblurrer/main.py` & `innerverz-0.0.21/innerverz/deblurrer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deblurrer/nets.py` & `innerverz-0.0.21/innerverz/deblurrer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deblurrer/test.py` & `innerverz-0.0.21/innerverz/deblurrer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deca/main.py` & `innerverz-0.0.21/innerverz/deca/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deca/models/FLAME.py` & `innerverz-0.0.21/innerverz/deca/models/FLAME.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deca/models/decoders.py` & `innerverz-0.0.21/innerverz/deca/models/decoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deca/models/detectors.py` & `innerverz-0.0.21/innerverz/deca/models/detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deca/models/encoders.py` & `innerverz-0.0.21/innerverz/deca/models/encoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deca/models/face_detectors.py` & `innerverz-0.0.21/innerverz/deca/models/face_detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deca/models/lbs.py` & `innerverz-0.0.21/innerverz/deca/models/lbs.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deca/models/resnet.py` & `innerverz-0.0.21/innerverz/deca/models/resnet.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deca/test.py` & `innerverz-0.0.21/innerverz/deca/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deca/utils/cfg.py` & `innerverz-0.0.21/innerverz/deca/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deca/utils/rasterizer/setup.py` & `innerverz-0.0.21/innerverz/deca/utils/rasterizer/setup.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deca/utils/renderer.py` & `innerverz-0.0.21/innerverz/deca/utils/renderer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deca/utils/rotation_converter.py` & `innerverz-0.0.21/innerverz/deca/utils/rotation_converter.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deca/utils/tensor_cropper.py` & `innerverz-0.0.21/innerverz/deca/utils/tensor_cropper.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deca/utils/util.py` & `innerverz-0.0.21/innerverz/deca/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deep3dmm/main.py` & `innerverz-0.0.21/innerverz/deep3dmm/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deep3dmm/nets.py` & `innerverz-0.0.21/innerverz/deep3dmm/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/deep3dmm/test.py` & `innerverz-0.0.21/innerverz/deep3dmm/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/face_alignment/graphic_utils.py` & `innerverz-0.0.21/innerverz/face_alignment/graphic_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/face_alignment/landmark.py` & `innerverz-0.0.21/innerverz/face_alignment/landmark.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/face_alignment/main.py` & `innerverz-0.0.21/innerverz_/face_alignment/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .retina_face import RetinaFace
 from .landmark import Landmark
 from .graphic_utils import *
 
 class FaceAligner():
     def __init__(self, size = 1024, align_style = 'invz'):
         '''
-        algin_style has 2 options  
+        align_style has 2 options  
         
         "ffhq" : algorithm used in FFHQ dataset  
         
         "invz" : algorithm costumed by Innerverz.co    
         
         Methods
         --------
@@ -22,16 +22,16 @@
         - align_face_from_106
         - affine_transform
         '''
         
         self.backbone = RetinaFace()
         self.lmk_detector = Landmark()
         self.size = size
-        self.algin_style = align_style
-        if self.algin_style == 'ffhq':
+        self.align_style = align_style
+        if self.align_style == 'ffhq':
             self.index_5 = [38,88,86,52,61]
         else:
             self.index_5 = None
         
     
     def get_face(self, img):
         """
@@ -70,15 +70,15 @@
         temp, _ = self.backbone.detect(img)
 
         if len(temp):
             FaceBool = True
             bbox = temp[0][0:4]
             lms_106 = self.lmk_detector.get(img, bbox)
             if self.align_style == 'ffhq': lms_5 = np.array([lms_106[self.index_5[0]], lms_106[self.index_5[1]], lms_106[self.index_5[2]], lms_106[self.index_5[3]], lms_106[self.index_5[4]]])
-
+            else: lms_5 = None
 
             aligned_face, tfm, tfm_inv = self.align_face_from_5(img, lms_5)
             return aligned_face, tfm, tfm_inv, lms_5, FaceBool, lms_106
     
         else :
             return None, None, None, None, False, None, 
     
@@ -107,14 +107,15 @@
         assert target_face_num < len(temp), 'index is larger than detected face' 
         
         if len(temp):
             FaceBool = True
             bbox = temp[0][0:4]
             lms_106 = self.lmk_detector.get(img, bbox)
             if self.align_style == 'ffhq': lms_5 = np.array([lms_106[self.index_5[0]], lms_106[self.index_5[1]], lms_106[self.index_5[2]], lms_106[self.index_5[3]], lms_106[self.index_5[4]]])
+            else: lms_5 = None
 
         if FaceBool:
             return FaceBool, lms_106, lms_5
 
         else:
             return FaceBool, None, None
     
@@ -140,15 +141,15 @@
                 - shape : (2, 3)
             - tfm_inv
                 - dtype : numpy array
                 - shape : (2, 3)
         """
         if size == None: size = self.size 
         
-        if self.algin_style == 'ffhq':
+        if self.align_style == 'ffhq':
             eye_left     = lms_5p[0]
             eye_right    = lms_5p[1]
             eye_avg      = (eye_left + eye_right) * 0.5
             eye_to_eye   = eye_right - eye_left
             mouth_left   = lms_5p[3]
             mouth_right  = lms_5p[4]
             mouth_avg    = (mouth_left + mouth_right) * 0.5
```

### Comparing `innerverz-0.0.20/innerverz/face_alignment/retina_face.py` & `innerverz-0.0.21/innerverz/face_alignment/retina_face.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/face_alignment/test.py` & `innerverz-0.0.21/innerverz/face_alignment/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/face_alignment/utils/face_align.py` & `innerverz-0.0.21/innerverz/face_alignment/utils/face_align.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/face_alignment/utils/transform.py` & `innerverz-0.0.21/innerverz/face_alignment/utils/transform.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/face_color_transfer/main.py` & `innerverz-0.0.21/innerverz/face_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/face_color_transfer/nets.py` & `innerverz-0.0.21/innerverz/face_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/face_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.21/innerverz/face_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/face_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.21/innerverz/face_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/face_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.21/innerverz/face_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/face_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.21/innerverz/face_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/face_color_transfer/test.py` & `innerverz-0.0.21/innerverz/face_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/face_enhancer/main.py` & `innerverz-0.0.21/innerverz/face_enhancer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/face_enhancer/nets.py` & `innerverz-0.0.21/innerverz/face_enhancer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/face_enhancer/test.py` & `innerverz-0.0.21/innerverz/face_enhancer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/face_parser/main.py` & `innerverz-0.0.21/innerverz/face_parser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/face_parser/nets.py` & `innerverz-0.0.21/innerverz/face_parser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/face_parser/test.py` & `innerverz-0.0.21/innerverz/face_parser/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/head_color_transfer/main.py` & `innerverz-0.0.21/innerverz/head_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/head_color_transfer/nets.py` & `innerverz-0.0.21/innerverz/head_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/head_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.21/innerverz/head_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/head_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.21/innerverz/head_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/head_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.21/innerverz/head_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/head_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.21/innerverz/head_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/head_color_transfer/test.py` & `innerverz-0.0.21/innerverz/head_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/id_extractor/main.py` & `innerverz-0.0.21/innerverz/id_extractor/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/id_extractor/nets.py` & `innerverz-0.0.21/innerverz/id_extractor/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/id_extractor/test.py` & `innerverz-0.0.21/innerverz/id_extractor/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/relighter/main.py` & `innerverz-0.0.21/innerverz/relighter/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/relighter/nets.py` & `innerverz-0.0.21/innerverz/relighter/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/relighter/test.py` & `innerverz-0.0.21/innerverz/relighter/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/upsampler/main.py` & `innerverz-0.0.21/innerverz/upsampler/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/upsampler/nets.py` & `innerverz-0.0.21/innerverz/upsampler/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/upsampler/test.py` & `innerverz-0.0.21/innerverz/upsampler/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/utils/download.py` & `innerverz-0.0.21/innerverz/utils/download.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/utils/input.py` & `innerverz-0.0.21/innerverz_/utils/input.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/utils/utils.py` & `innerverz-0.0.21/innerverz/utils/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/video_faceparser/main.py` & `innerverz-0.0.21/innerverz/video_faceparser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/video_faceparser/nets.py` & `innerverz-0.0.21/innerverz/video_faceparser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/video_faceparser/utils/corr.py` & `innerverz-0.0.21/innerverz/video_faceparser/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/video_faceparser/utils/extractor.py` & `innerverz-0.0.21/innerverz/video_faceparser/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/video_faceparser/utils/update.py` & `innerverz-0.0.21/innerverz/video_faceparser/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz/video_faceparser/utils/util.py` & `innerverz-0.0.21/innerverz/video_faceparser/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz.egg-info/SOURCES.txt` & `innerverz-0.0.21/innerverz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/__init__.py` & `innerverz-0.0.21/innerverz_/__init__.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/data_process/main.py` & `innerverz-0.0.21/innerverz_/data_process/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deblurrer/main.py` & `innerverz-0.0.21/innerverz_/deblurrer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deblurrer/nets.py` & `innerverz-0.0.21/innerverz_/deblurrer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deblurrer/test.py` & `innerverz-0.0.21/innerverz_/deblurrer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deca/main.py` & `innerverz-0.0.21/innerverz_/deca/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deca/models/FLAME.py` & `innerverz-0.0.21/innerverz_/deca/models/FLAME.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deca/models/decoders.py` & `innerverz-0.0.21/innerverz_/deca/models/decoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deca/models/detectors.py` & `innerverz-0.0.21/innerverz_/deca/models/detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deca/models/encoders.py` & `innerverz-0.0.21/innerverz_/deca/models/encoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deca/models/face_detectors.py` & `innerverz-0.0.21/innerverz_/deca/models/face_detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deca/models/lbs.py` & `innerverz-0.0.21/innerverz_/deca/models/lbs.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deca/models/resnet.py` & `innerverz-0.0.21/innerverz_/deca/models/resnet.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deca/test.py` & `innerverz-0.0.21/innerverz_/deca/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deca/utils/cfg.py` & `innerverz-0.0.21/innerverz_/deca/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deca/utils/rasterizer/setup.py` & `innerverz-0.0.21/innerverz_/deca/utils/rasterizer/setup.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deca/utils/renderer.py` & `innerverz-0.0.21/innerverz_/deca/utils/renderer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deca/utils/rotation_converter.py` & `innerverz-0.0.21/innerverz_/deca/utils/rotation_converter.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deca/utils/tensor_cropper.py` & `innerverz-0.0.21/innerverz_/deca/utils/tensor_cropper.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deca/utils/util.py` & `innerverz-0.0.21/innerverz_/deca/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deep3dmm/main.py` & `innerverz-0.0.21/innerverz_/deep3dmm/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deep3dmm/nets.py` & `innerverz-0.0.21/innerverz_/deep3dmm/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/deep3dmm/test.py` & `innerverz-0.0.21/innerverz_/deep3dmm/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/face_alignment/graphic_utils.py` & `innerverz-0.0.21/innerverz_/face_alignment/graphic_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/face_alignment/landmark.py` & `innerverz-0.0.21/innerverz_/face_alignment/landmark.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/face_alignment/main.py` & `innerverz-0.0.21/innerverz/face_alignment/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,54 +70,57 @@
         temp, _ = self.backbone.detect(img)
 
         if len(temp):
             FaceBool = True
             bbox = temp[0][0:4]
             lms_106 = self.lmk_detector.get(img, bbox)
             if self.align_style == 'ffhq': lms_5 = np.array([lms_106[self.index_5[0]], lms_106[self.index_5[1]], lms_106[self.index_5[2]], lms_106[self.index_5[3]], lms_106[self.index_5[4]]])
-            else: lms_5 = None
+
 
             aligned_face, tfm, tfm_inv = self.align_face_from_5(img, lms_5)
             return aligned_face, tfm, tfm_inv, lms_5, FaceBool, lms_106
     
         else :
             return None, None, None, None, False, None, 
     
-    def detect_lmk(self, img, target_face_num=0):
+    def detect_lmk(self, img, target_face_num=0, pad=256):
         """
         Input
         ---------
             - dtype : cv2 image
             - shape : (h, w, 3)
             - min max : (0, 255)
+            - pad[int]
             
         Output
         ---------
             - FaceBool
                 - dtype : Bool
             - lms_106
                 - dtype : numpy array
                 - shape : (106, 2)
             - lms_5
                 - dtype : numpy array
                 - shape : (5, 2)
         """
         FaceBool = False
-        temp, _ = self.backbone.detect(img)
+        pad_img = np.pad(img, ((pad, pad), (pad,pad), (0,0))) 
+        temp, _ = self.backbone.detect(pad_img)
         
         assert target_face_num < len(temp), 'index is larger than detected face' 
         
         if len(temp):
             FaceBool = True
             bbox = temp[0][0:4]
-            lms_106 = self.lmk_detector.get(img, bbox)
-            if self.align_style == 'ffhq': lms_5 = np.array([lms_106[self.index_5[0]], lms_106[self.index_5[1]], lms_106[self.index_5[2]], lms_106[self.index_5[3]], lms_106[self.index_5[4]]])
-            else: lms_5 = None
+            pad_lms_106 = self.lmk_detector.get(pad_img, bbox)
+            if self.align_style == 'ffhq': pad_lms_5 = np.array([pad_lms_106[self.index_5[0]], pad_lms_106[self.index_5[1]], pad_lms_106[self.index_5[2]], pad_lms_106[self.index_5[3]], pad_lms_106[self.index_5[4]]])
 
         if FaceBool:
+            lms_106 = pad_lms_106 - pad
+            lms_5 = pad_lms_5 - pad if self.align_style=='ffhq' else None
             return FaceBool, lms_106, lms_5
 
         else:
             return FaceBool, None, None
     
     def align_face_from_5(self, img, lms_5p, size = None) :
         """
```

### Comparing `innerverz-0.0.20/innerverz_/face_alignment/retina_face.py` & `innerverz-0.0.21/innerverz_/face_alignment/retina_face.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/face_alignment/test.py` & `innerverz-0.0.21/innerverz_/face_alignment/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/face_alignment/utils/face_align.py` & `innerverz-0.0.21/innerverz_/face_alignment/utils/face_align.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/face_alignment/utils/transform.py` & `innerverz-0.0.21/innerverz_/face_alignment/utils/transform.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/face_color_transfer/main.py` & `innerverz-0.0.21/innerverz_/face_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/face_color_transfer/nets.py` & `innerverz-0.0.21/innerverz_/face_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/face_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.21/innerverz_/face_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/face_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.21/innerverz_/face_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/face_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.21/innerverz_/face_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/face_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.21/innerverz_/face_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/face_color_transfer/test.py` & `innerverz-0.0.21/innerverz_/face_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/face_enhancer/main.py` & `innerverz-0.0.21/innerverz_/face_enhancer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/face_enhancer/nets.py` & `innerverz-0.0.21/innerverz_/face_enhancer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/face_enhancer/test.py` & `innerverz-0.0.21/innerverz_/face_enhancer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/face_parser/main.py` & `innerverz-0.0.21/innerverz_/face_parser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/face_parser/nets.py` & `innerverz-0.0.21/innerverz_/face_parser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/face_parser/test.py` & `innerverz-0.0.21/innerverz_/face_parser/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/head_color_transfer/main.py` & `innerverz-0.0.21/innerverz_/head_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/head_color_transfer/nets.py` & `innerverz-0.0.21/innerverz_/head_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/head_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.21/innerverz_/head_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/head_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.21/innerverz_/head_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/head_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.21/innerverz_/head_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/head_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.21/innerverz_/head_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/head_color_transfer/test.py` & `innerverz-0.0.21/innerverz_/head_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/id_extractor/main.py` & `innerverz-0.0.21/innerverz_/id_extractor/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/id_extractor/nets.py` & `innerverz-0.0.21/innerverz_/id_extractor/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/id_extractor/test.py` & `innerverz-0.0.21/innerverz_/id_extractor/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/relighter/main.py` & `innerverz-0.0.21/innerverz_/relighter/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/relighter/nets.py` & `innerverz-0.0.21/innerverz_/relighter/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/relighter/test.py` & `innerverz-0.0.21/innerverz_/relighter/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/upsampler/main.py` & `innerverz-0.0.21/innerverz_/upsampler/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/upsampler/nets.py` & `innerverz-0.0.21/innerverz_/upsampler/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/upsampler/test.py` & `innerverz-0.0.21/innerverz_/upsampler/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/utils/download.py` & `innerverz-0.0.21/innerverz_/utils/download.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/utils/input.py` & `innerverz-0.0.21/innerverz/utils/input.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,11 +25,14 @@
     elif source_type == 'pillow':
         if target == 'pillow':
             image = source
         elif target == 'cv2':
             image = np.array(source)[:,:,::-1]
     elif source_type == 'cv2':
         if target == 'pillow':
-            image = Image.fromarray(source[:,:,::-1]).convert("RGB")
+            if len(source.shape) == 2:
+                image = Image.fromarray(source.astype(np.uint8))
+            else:
+                image = Image.fromarray(source[:,:,::-1]).convert("RGB")
         elif target == 'cv2':
             image = source
     return image
```

### Comparing `innerverz-0.0.20/innerverz_/utils/utils.py` & `innerverz-0.0.21/innerverz_/utils/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/video_faceparser/main.py` & `innerverz-0.0.21/innerverz_/video_faceparser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/video_faceparser/nets.py` & `innerverz-0.0.21/innerverz_/video_faceparser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/video_faceparser/utils/corr.py` & `innerverz-0.0.21/innerverz_/video_faceparser/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/video_faceparser/utils/extractor.py` & `innerverz-0.0.21/innerverz_/video_faceparser/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/video_faceparser/utils/update.py` & `innerverz-0.0.21/innerverz_/video_faceparser/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/innerverz_/video_faceparser/utils/util.py` & `innerverz-0.0.21/innerverz_/video_faceparser/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.20/setup.py` & `innerverz-0.0.21/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 except (IOError, ImportError, ModuleNotFoundError):
     print('WARNING: pandoc not enabled')
     long_description = open('README.md').read()
     pypandoc_enabled = False
 
 setup(
     name="innerverz",
-    version="0.0.20",
+    version="0.0.21",
     author="Innerverz",
     author_email="study@innerverz.com",
     description="innerverz package",
     long_description=long_description,
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages()
```

