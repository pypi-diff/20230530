# Comparing `tmp/onvif-gui-1.1.9.tar.gz` & `tmp/onvif-gui-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-gui-1.1.9.tar", last modified: Thu May 25 17:33:53 2023, max compression
+gzip compressed data, was "onvif-gui-1.2.0.tar", last modified: Tue May 30 02:27:41 2023, max compression
```

## Comparing `onvif-gui-1.1.9.tar` & `onvif-gui-1.2.0.tar`

### file list

```diff
@@ -1,305 +1,307 @@
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.187840 onvif-gui-1.1.9/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11558 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/LICENSE
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      221 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/MANIFEST.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-25 17:33:53.187840 onvif-gui-1.1.9/PKG-INFO
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8359 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/README.md
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.167840 onvif-gui-1.1.9/detectron2/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       68 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.167840 onvif-gui-1.1.9/detectron2/checkpoint/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      357 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/checkpoint/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18177 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/checkpoint/c2_model_loading.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5800 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/checkpoint/catalog.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5379 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/checkpoint/detection_checkpoint.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.167840 onvif-gui-1.1.9/detectron2/config/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      623 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/config/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8119 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/config/compat.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9476 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/config/config.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    30158 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/config/defaults.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3103 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/config/instantiate.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15786 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/config/lazy.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.167840 onvif-gui-1.1.9/detectron2/configs/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1360 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/configs/Base-RCNN-FPN.yaml
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.167840 onvif-gui-1.1.9/detectron2/configs/COCO-InstanceSegmentation/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/configs/COCO-InstanceSegmentation/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      201 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.167840 onvif-gui-1.1.9/detectron2/configs/COCO-Keypoints/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      542 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/configs/COCO-Keypoints/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      190 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/configs/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x.yaml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/configs/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.171840 onvif-gui-1.1.9/detectron2/data/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      663 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7603 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/benchmark.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21787 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/build.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7460 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/catalog.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9406 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/common.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8360 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/dataset_mapper.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.171840 onvif-gui-1.1.9/detectron2/data/datasets/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      532 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/datasets/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10433 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/datasets/builtin.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    22191 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/datasets/builtin_meta.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13496 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/datasets/cityscapes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8008 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/datasets/cityscapes_panoptic.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    24004 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/datasets/coco.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9205 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/datasets/coco_panoptic.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9864 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/datasets/lvis.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)   223770 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/datasets/lvis_v0_5_categories.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)   219193 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/datasets/lvis_v1_categories.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    39434 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/datasets/lvis_v1_category_image_count.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3210 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/datasets/pascal_voc.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/datasets/register_coco.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    23487 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/detection_utils.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.171840 onvif-gui-1.1.9/detectron2/data/samplers/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      429 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/samplers/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12067 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/samplers/distributed_sampler.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1991 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/samplers/grouped_batch_sampler.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.171840 onvif-gui-1.1.9/detectron2/data/transforms/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      480 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/transforms/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14492 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/transforms/augmentation.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    23683 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/transforms/augmentation_impl.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12980 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/data/transforms/transform.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.171840 onvif-gui-1.1.9/detectron2/layers/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      900 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/layers/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5908 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/layers/aspp.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12431 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/layers/batch_norm.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3135 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/layers/blocks.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17492 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/layers/deform_conv.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4335 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/layers/losses.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11154 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/layers/mask_ops.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6629 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/layers/nms.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3172 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/layers/roi_align.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3393 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/layers/roi_align_rotated.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      673 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/layers/rotated_boxes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      555 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/layers/shape_spec.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5271 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/layers/wrappers.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.171840 onvif-gui-1.1.9/detectron2/modeling/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1632 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15825 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/anchor_generator.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.175840 onvif-gui-1.1.9/detectron2/modeling/backbone/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      618 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/backbone/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2586 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/backbone/backbone.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1048 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/backbone/build.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10628 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/backbone/fpn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    16434 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/backbone/mvit.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17108 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/backbone/regnet.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    24352 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/backbone/resnet.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    25785 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/backbone/swin.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6546 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/backbone/utils.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    19860 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/backbone/vit.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15492 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/box_regression.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6391 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/matcher.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.175840 onvif-gui-1.1.9/detectron2/modeling/meta_arch/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      524 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/meta_arch/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      839 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/meta_arch/build.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11940 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/meta_arch/dense_detector.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13541 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/meta_arch/fcos.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10676 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/meta_arch/panoptic_fpn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14237 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/meta_arch/rcnn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18704 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/meta_arch/retinanet.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10173 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/meta_arch/semantic_seg.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11104 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/mmdet_wrapper.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11575 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/poolers.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4145 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/postprocessing.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.175840 onvif-gui-1.1.9/detectron2/modeling/proposal_generator/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      236 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/proposal_generator/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      860 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/proposal_generator/build.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8333 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/proposal_generator/proposal_utils.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    24347 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/proposal_generator/rpn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9016 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/proposal_generator/rrpn.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.175840 onvif-gui-1.1.9/detectron2/modeling/roi_heads/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      797 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/roi_heads/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4195 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/roi_heads/box_head.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13289 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/roi_heads/cascade_rcnn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    25959 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/roi_heads/fast_rcnn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11428 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/roi_heads/keypoint_head.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12467 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/roi_heads/mask_head.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    38578 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/roi_heads/roi_heads.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11446 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2388 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/sampling.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12723 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/modeling/test_time_augmentation.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1829 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/predictor.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.175840 onvif-gui-1.1.9/detectron2/structures/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      662 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/structures/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14854 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/structures/boxes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5649 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/structures/image_list.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6807 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/structures/instances.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9269 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/structures/keypoints.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    20336 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/structures/masks.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    19356 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/structures/rotated_boxes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2775 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/tracker.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.179840 onvif-gui-1.1.9/detectron2/utils/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       52 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/utils/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6205 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/utils/analysis.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8633 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/utils/collect_env.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4254 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/utils/colormap.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5807 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/utils/comm.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1911 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/utils/develop.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5814 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/utils/env.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17508 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/utils/events.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1226 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/utils/file_io.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8044 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/utils/logger.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2667 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/utils/memory.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1934 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/utils/registry.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1096 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/utils/serialize.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18576 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/utils/testing.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11606 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/utils/video_visualizer.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    52426 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/detectron2/utils/visualizer.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.179840 onvif-gui-1.1.9/gui/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       28 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.179840 onvif-gui-1.1.9/gui/components/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      250 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/components/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1824 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/components/comboselector.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2459 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/components/directoryselector.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2172 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/components/fileselector.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5508 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/components/labelselector.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4194 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/components/progress.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1962 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/components/thresholdslider.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2054 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/glwidget.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14578 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/main.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.179840 onvif-gui-1.1.9/gui/onvif/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      196 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/onvif/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5870 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/onvif/admintab.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4051 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/onvif/imagetab.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2484 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/onvif/logindialog.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5364 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/onvif/networktab.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5241 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/onvif/ptztab.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4640 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/onvif/videotab.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.179840 onvif-gui-1.1.9/gui/panels/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      184 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/panels/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3716 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/panels/audiopanel.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13807 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/panels/camerapanel.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14838 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/panels/filepanel.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13665 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/panels/settingspanel.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3720 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/panels/videopanel.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.183840 onvif-gui-1.1.9/gui/resources/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2021 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/LICENSE
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      252 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/apply.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      245 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/apply_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      244 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/apply_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      911 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/audio.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      536 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/audio_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      920 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/audio_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      203 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/branch_closed.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      219 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/branch_closed_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      211 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/branch_closed_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      199 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/branch_open.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      168 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/branch_open_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/branch_open_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      267 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/checked.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      235 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/checked_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      246 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/checked_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13331 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/darkstyle.qss
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      910 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/discover.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      849 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/discover_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      937 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/discover_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      425 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/fast-forward.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      253 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/fast-forward_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      433 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/fast-forward_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      641 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/mute.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      346 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/mute_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      618 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/mute_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      347 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/next.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      225 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/next_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      348 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/next_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    46084 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/onvif-gui.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/pause.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      144 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/pause_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      149 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/pause_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      321 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/play.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      209 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/play_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      316 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/play_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      349 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/previous.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      232 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/previous_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      348 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/previous_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      324 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/radio-off.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      250 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/radio-off_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      324 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/radio-off_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      350 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/radio-on.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      263 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/radio-on_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      343 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/radio-on_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      395 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/record.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      394 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/record_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      425 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/record_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      408 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/recording.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      435 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/recording_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      532 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/recording_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      454 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/rewind.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      250 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/rewind_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      457 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/rewind_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      187 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/small_arrow_left.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      183 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/small_arrow_left_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      189 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/small_arrow_left_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      162 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/small_arrow_up.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      160 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/small_arrow_up_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      161 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/small_arrow_up_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      158 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/stop.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      140 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/stop_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      151 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/stop_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      143 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/unchecked.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      142 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/unchecked_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      143 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/gui/resources/unchecked_lo.png
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.183840 onvif-gui-1.1.9/modules/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/modules/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.183840 onvif-gui-1.1.9/modules/audio/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/modules/audio/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3492 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/modules/audio/sample.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.183840 onvif-gui-1.1.9/modules/video/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/modules/video/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7094 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/modules/video/keypoint.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4889 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/modules/video/retinanet.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3176 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/modules/video/sample.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7614 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/modules/video/segment.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10910 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/modules/video/yolov7.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9052 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/modules/video/yolov8.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12265 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/modules/video/yolox.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.187840 onvif-gui-1.1.9/onvif_gui.egg-info/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-25 17:33:53.000000 onvif-gui-1.1.9/onvif_gui.egg-info/PKG-INFO
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8392 2023-05-25 17:33:53.000000 onvif-gui-1.1.9/onvif_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-05-25 17:33:53.000000 onvif-gui-1.1.9/onvif_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       39 2023-05-25 17:33:53.000000 onvif-gui-1.1.9/onvif_gui.egg-info/entry_points.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       47 2023-05-25 17:33:53.000000 onvif-gui-1.1.9/onvif_gui.egg-info/requires.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       44 2023-05-25 17:33:53.000000 onvif-gui-1.1.9/onvif_gui.egg-info/top_level.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1709 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/pyproject.toml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       38 2023-05-25 17:33:53.187840 onvif-gui-1.1.9/setup.cfg
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1549 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/setup.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.187840 onvif-gui-1.1.9/tracker/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/tracker/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1003 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/tracker/basetrack.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12632 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/tracker/byte_tracker.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9816 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/tracker/kalman_filter.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6304 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/tracker/matching.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.187840 onvif-gui-1.1.9/yolov7/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolov7/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.187840 onvif-gui-1.1.9/yolov7/models/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        6 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolov7/models/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    86435 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolov7/models/common.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11177 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolov7/models/experimental.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    40895 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolov7/models/yolo.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.187840 onvif-gui-1.1.9/yolov7/utils/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        6 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolov7/utils/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2320 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolov7/utils/activations.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5771 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolov7/utils/add_nms.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7321 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolov7/utils/autoanchor.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    57559 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolov7/utils/datasets.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    37789 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolov7/utils/general.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4996 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolov7/utils/google_utils.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    76741 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolov7/utils/loss.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9537 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolov7/utils/metrics.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21424 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolov7/utils/plots.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15840 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolov7/utils/torch_utils.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.187840 onvif-gui-1.1.9/yolox/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolox/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.187840 onvif-gui-1.1.9/yolox/models/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      961 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolox/models/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5019 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolox/models/build.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6840 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolox/models/darknet.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2372 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolox/models/losses.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6944 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolox/models/network_blocks.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3202 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolox/models/yolo_fpn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    26204 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolox/models/yolo_head.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4288 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolox/models/yolo_pafpn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2054 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolox/models/yolox.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:33:53.187840 onvif-gui-1.1.9/yolox/utils/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      130 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolox/utils/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1628 2023-05-25 17:26:34.000000 onvif-gui-1.1.9/yolox/utils/utils.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11558 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/LICENSE
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      221 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/MANIFEST.in
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/PKG-INFO
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8359 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/README.md
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.363506 onvif-gui-1.2.0/detectron2/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       68 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.363506 onvif-gui-1.2.0/detectron2/checkpoint/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      357 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/checkpoint/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18177 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/checkpoint/c2_model_loading.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5800 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/checkpoint/catalog.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5379 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/checkpoint/detection_checkpoint.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.363506 onvif-gui-1.2.0/detectron2/config/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      623 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/config/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8119 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/config/compat.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9476 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/config/config.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    30158 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/config/defaults.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3103 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/config/instantiate.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15786 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/config/lazy.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.363506 onvif-gui-1.2.0/detectron2/configs/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1360 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/configs/Base-RCNN-FPN.yaml
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.367506 onvif-gui-1.2.0/detectron2/configs/COCO-InstanceSegmentation/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/configs/COCO-InstanceSegmentation/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      201 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.367506 onvif-gui-1.2.0/detectron2/configs/COCO-Keypoints/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      542 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/configs/COCO-Keypoints/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      190 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/configs/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x.yaml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/configs/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.367506 onvif-gui-1.2.0/detectron2/data/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      663 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7603 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/benchmark.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21787 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7460 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/catalog.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9406 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/common.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8360 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/dataset_mapper.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.367506 onvif-gui-1.2.0/detectron2/data/datasets/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      532 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10433 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/builtin.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    22191 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/builtin_meta.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13496 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/cityscapes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8008 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/cityscapes_panoptic.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    24004 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/coco.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9205 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/coco_panoptic.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9864 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/lvis.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)   223770 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/lvis_v0_5_categories.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)   219193 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/lvis_v1_categories.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    39434 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/lvis_v1_category_image_count.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3210 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/pascal_voc.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/register_coco.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23487 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/detection_utils.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.367506 onvif-gui-1.2.0/detectron2/data/samplers/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      429 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/samplers/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12067 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/samplers/distributed_sampler.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1991 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/samplers/grouped_batch_sampler.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.367506 onvif-gui-1.2.0/detectron2/data/transforms/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      480 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/transforms/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14492 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/transforms/augmentation.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23683 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/transforms/augmentation_impl.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12980 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/transforms/transform.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.367506 onvif-gui-1.2.0/detectron2/layers/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      900 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5908 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/aspp.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12431 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/batch_norm.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3135 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/blocks.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17492 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/deform_conv.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4335 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/losses.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11154 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/mask_ops.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6629 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/nms.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3172 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/roi_align.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3393 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/roi_align_rotated.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      673 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/rotated_boxes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      555 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/shape_spec.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5271 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/wrappers.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.371506 onvif-gui-1.2.0/detectron2/modeling/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1632 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15825 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/anchor_generator.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.371506 onvif-gui-1.2.0/detectron2/modeling/backbone/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      618 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2586 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/backbone.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1048 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10628 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/fpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    16434 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/mvit.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17108 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/regnet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    24352 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/resnet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    25785 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/swin.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6546 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/utils.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    19860 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/vit.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15492 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/box_regression.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6391 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/matcher.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.371506 onvif-gui-1.2.0/detectron2/modeling/meta_arch/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      524 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/meta_arch/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      839 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/meta_arch/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11940 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/meta_arch/dense_detector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13541 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/meta_arch/fcos.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10676 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/meta_arch/panoptic_fpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14237 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/meta_arch/rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18704 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/meta_arch/retinanet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10173 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/meta_arch/semantic_seg.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11104 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/mmdet_wrapper.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11575 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/poolers.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4145 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/postprocessing.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.371506 onvif-gui-1.2.0/detectron2/modeling/proposal_generator/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      236 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/proposal_generator/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      860 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/proposal_generator/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8333 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/proposal_generator/proposal_utils.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    24347 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/proposal_generator/rpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9016 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/proposal_generator/rrpn.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.371506 onvif-gui-1.2.0/detectron2/modeling/roi_heads/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      797 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/roi_heads/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4195 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/roi_heads/box_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13289 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/roi_heads/cascade_rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    25959 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/roi_heads/fast_rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11428 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/roi_heads/keypoint_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12467 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/roi_heads/mask_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    38578 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/roi_heads/roi_heads.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11446 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2388 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/sampling.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12723 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/test_time_augmentation.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1829 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/predictor.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.371506 onvif-gui-1.2.0/detectron2/structures/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      662 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/structures/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14854 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/structures/boxes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5649 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/structures/image_list.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6807 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/structures/instances.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9269 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/structures/keypoints.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    20336 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/structures/masks.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    19356 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/structures/rotated_boxes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2775 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/tracker.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.375506 onvif-gui-1.2.0/detectron2/utils/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       52 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6205 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/analysis.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8633 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/collect_env.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4254 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/colormap.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5807 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/comm.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1911 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/develop.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5814 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/env.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17508 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/events.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1226 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/file_io.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8044 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/logger.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2667 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/memory.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1934 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/registry.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1096 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/serialize.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18576 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/testing.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11606 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/video_visualizer.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    52426 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/visualizer.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.375506 onvif-gui-1.2.0/gui/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       28 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.375506 onvif-gui-1.2.0/gui/components/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      286 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/gui/components/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1824 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/components/comboselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2459 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/components/directoryselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2172 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/components/fileselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5508 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/components/labelselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4194 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/components/progress.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1962 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/components/thresholdslider.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      831 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/gui/components/waitdialog.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2054 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/glwidget.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15800 2023-05-30 02:26:06.000000 onvif-gui-1.2.0/gui/main.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.375506 onvif-gui-1.2.0/gui/onvif/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      196 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/onvif/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5870 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/onvif/admintab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4051 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/onvif/imagetab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2484 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/onvif/logindialog.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5364 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/onvif/networktab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5241 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/onvif/ptztab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4640 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/onvif/videotab.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.375506 onvif-gui-1.2.0/gui/panels/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      184 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/panels/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3802 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/gui/panels/audiopanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13667 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/gui/panels/camerapanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14756 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/gui/panels/filepanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14115 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/gui/panels/settingspanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3806 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/gui/panels/videopanel.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.383506 onvif-gui-1.2.0/gui/resources/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2021 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/LICENSE
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      252 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/apply.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      245 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/apply_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      244 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/apply_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      911 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/audio.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      536 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/audio_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      920 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/audio_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      203 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/branch_closed.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      219 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/branch_closed_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      211 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/branch_closed_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      199 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/branch_open.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      168 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/branch_open_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/branch_open_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      267 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/checked.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      235 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/checked_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      246 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/checked_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13358 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/gui/resources/darkstyle.qss
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      910 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/discover.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      849 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/discover_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      937 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/discover_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      425 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/fast-forward.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      253 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/fast-forward_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      433 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/fast-forward_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      641 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/mute.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      346 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/mute_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      618 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/mute_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      347 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/next.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      225 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/next_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      348 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/next_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    46084 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/onvif-gui.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/pause.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      144 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/pause_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      149 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/pause_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      321 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/play.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      209 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/play_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      316 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/play_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      349 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/previous.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      232 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/previous_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      348 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/previous_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      324 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/radio-off.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      250 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/radio-off_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      324 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/radio-off_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      350 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/radio-on.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      263 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/radio-on_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      343 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/radio-on_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      395 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/record.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      394 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/record_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      425 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/record_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      408 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/recording.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      435 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/recording_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      532 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/recording_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      454 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/rewind.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      250 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/rewind_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      457 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/rewind_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      187 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/small_arrow_left.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      183 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/small_arrow_left_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      189 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/small_arrow_left_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      162 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/small_arrow_up.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      160 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/small_arrow_up_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      161 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/small_arrow_up_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    19236 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/gui/resources/spinner.gif
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      158 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/stop.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      140 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/stop_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      151 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/stop_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      143 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/unchecked.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      142 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/unchecked_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      143 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/unchecked_lo.png
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.383506 onvif-gui-1.2.0/modules/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/modules/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.383506 onvif-gui-1.2.0/modules/audio/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/modules/audio/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3492 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/modules/audio/sample.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/modules/video/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/modules/video/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7756 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/modules/video/keypoint.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5390 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/modules/video/retinanet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3234 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/modules/video/sample.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8278 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/modules/video/segment.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12058 2023-05-30 02:16:29.000000 onvif-gui-1.2.0/modules/video/yolov7.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11322 2023-05-30 02:16:20.000000 onvif-gui-1.2.0/modules/video/yolov8.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12641 2023-05-30 02:13:23.000000 onvif-gui-1.2.0/modules/video/yolox.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/onvif_gui.egg-info/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-30 02:27:41.000000 onvif-gui-1.2.0/onvif_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8447 2023-05-30 02:27:41.000000 onvif-gui-1.2.0/onvif_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-05-30 02:27:41.000000 onvif-gui-1.2.0/onvif_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       39 2023-05-30 02:27:41.000000 onvif-gui-1.2.0/onvif_gui.egg-info/entry_points.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       47 2023-05-30 02:27:41.000000 onvif-gui-1.2.0/onvif_gui.egg-info/requires.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       44 2023-05-30 02:27:41.000000 onvif-gui-1.2.0/onvif_gui.egg-info/top_level.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1688 2023-05-30 02:25:31.000000 onvif-gui-1.2.0/pyproject.toml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       38 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/setup.cfg
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1549 2023-05-30 02:25:19.000000 onvif-gui-1.2.0/setup.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/tracker/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/tracker/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1003 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/tracker/basetrack.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12632 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/tracker/byte_tracker.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9816 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/tracker/kalman_filter.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6304 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/tracker/matching.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/yolov7/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/yolov7/models/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        6 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/models/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    86435 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/models/common.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11177 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/models/experimental.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    40895 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/models/yolo.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/yolov7/utils/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        6 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2320 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/activations.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5771 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/add_nms.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7321 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/autoanchor.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    57559 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/datasets.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    37789 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/general.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4996 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/google_utils.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    76741 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/loss.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9537 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/metrics.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21424 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/plots.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15840 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/torch_utils.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/yolox/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/yolox/models/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      961 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/models/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5019 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/models/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6840 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/models/darknet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2372 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/models/losses.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6944 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/models/network_blocks.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3202 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/models/yolo_fpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    26204 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/models/yolo_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4288 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/models/yolo_pafpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2054 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/models/yolox.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/yolox/utils/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      130 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/utils/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1628 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/utils/utils.py
```

### Comparing `onvif-gui-1.1.9/LICENSE` & `onvif-gui-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/PKG-INFO` & `onvif-gui-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-gui
-Version: 1.1.9
+Version: 1.2.0
 Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libonvif
 Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `onvif-gui-1.1.9/README.md` & `onvif-gui-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/checkpoint/c2_model_loading.py` & `onvif-gui-1.2.0/detectron2/checkpoint/c2_model_loading.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/checkpoint/catalog.py` & `onvif-gui-1.2.0/detectron2/checkpoint/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/checkpoint/detection_checkpoint.py` & `onvif-gui-1.2.0/detectron2/checkpoint/detection_checkpoint.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/config/__init__.py` & `onvif-gui-1.2.0/detectron2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/config/compat.py` & `onvif-gui-1.2.0/detectron2/config/compat.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/config/config.py` & `onvif-gui-1.2.0/detectron2/config/config.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/config/defaults.py` & `onvif-gui-1.2.0/detectron2/config/defaults.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/config/instantiate.py` & `onvif-gui-1.2.0/detectron2/config/instantiate.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/config/lazy.py` & `onvif-gui-1.2.0/detectron2/config/lazy.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/configs/Base-RCNN-FPN.yaml` & `onvif-gui-1.2.0/detectron2/configs/Base-RCNN-FPN.yaml`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml` & `onvif-gui-1.2.0/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/__init__.py` & `onvif-gui-1.2.0/detectron2/data/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/benchmark.py` & `onvif-gui-1.2.0/detectron2/data/benchmark.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/build.py` & `onvif-gui-1.2.0/detectron2/data/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/catalog.py` & `onvif-gui-1.2.0/detectron2/data/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/common.py` & `onvif-gui-1.2.0/detectron2/data/common.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/dataset_mapper.py` & `onvif-gui-1.2.0/detectron2/data/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/datasets/__init__.py` & `onvif-gui-1.2.0/detectron2/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/datasets/builtin.py` & `onvif-gui-1.2.0/detectron2/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/datasets/builtin_meta.py` & `onvif-gui-1.2.0/detectron2/data/datasets/builtin_meta.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/datasets/cityscapes.py` & `onvif-gui-1.2.0/detectron2/data/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/datasets/cityscapes_panoptic.py` & `onvif-gui-1.2.0/detectron2/data/datasets/cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/datasets/coco.py` & `onvif-gui-1.2.0/detectron2/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/datasets/coco_panoptic.py` & `onvif-gui-1.2.0/detectron2/data/datasets/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/datasets/lvis.py` & `onvif-gui-1.2.0/detectron2/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/datasets/lvis_v0_5_categories.py` & `onvif-gui-1.2.0/detectron2/data/datasets/lvis_v0_5_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/datasets/lvis_v1_categories.py` & `onvif-gui-1.2.0/detectron2/data/datasets/lvis_v1_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/datasets/lvis_v1_category_image_count.py` & `onvif-gui-1.2.0/detectron2/data/datasets/lvis_v1_category_image_count.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/datasets/pascal_voc.py` & `onvif-gui-1.2.0/detectron2/data/datasets/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/detection_utils.py` & `onvif-gui-1.2.0/detectron2/data/detection_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/samplers/distributed_sampler.py` & `onvif-gui-1.2.0/detectron2/data/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/samplers/grouped_batch_sampler.py` & `onvif-gui-1.2.0/detectron2/data/samplers/grouped_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/transforms/augmentation.py` & `onvif-gui-1.2.0/detectron2/data/transforms/augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/transforms/augmentation_impl.py` & `onvif-gui-1.2.0/detectron2/data/transforms/augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/data/transforms/transform.py` & `onvif-gui-1.2.0/detectron2/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/layers/__init__.py` & `onvif-gui-1.2.0/detectron2/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/layers/aspp.py` & `onvif-gui-1.2.0/detectron2/layers/aspp.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/layers/batch_norm.py` & `onvif-gui-1.2.0/detectron2/layers/batch_norm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/layers/blocks.py` & `onvif-gui-1.2.0/detectron2/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/layers/deform_conv.py` & `onvif-gui-1.2.0/detectron2/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/layers/losses.py` & `onvif-gui-1.2.0/detectron2/layers/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/layers/mask_ops.py` & `onvif-gui-1.2.0/detectron2/layers/mask_ops.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/layers/nms.py` & `onvif-gui-1.2.0/detectron2/layers/nms.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/layers/roi_align.py` & `onvif-gui-1.2.0/detectron2/layers/roi_align.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/layers/roi_align_rotated.py` & `onvif-gui-1.2.0/detectron2/layers/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/layers/rotated_boxes.py` & `onvif-gui-1.2.0/detectron2/layers/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/layers/shape_spec.py` & `onvif-gui-1.2.0/detectron2/layers/shape_spec.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/layers/wrappers.py` & `onvif-gui-1.2.0/detectron2/layers/wrappers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/__init__.py` & `onvif-gui-1.2.0/detectron2/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/anchor_generator.py` & `onvif-gui-1.2.0/detectron2/modeling/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/backbone/__init__.py` & `onvif-gui-1.2.0/detectron2/modeling/backbone/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/backbone/backbone.py` & `onvif-gui-1.2.0/detectron2/modeling/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/backbone/build.py` & `onvif-gui-1.2.0/detectron2/modeling/backbone/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/backbone/fpn.py` & `onvif-gui-1.2.0/detectron2/modeling/backbone/fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/backbone/mvit.py` & `onvif-gui-1.2.0/detectron2/modeling/backbone/mvit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/backbone/regnet.py` & `onvif-gui-1.2.0/detectron2/modeling/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/backbone/resnet.py` & `onvif-gui-1.2.0/detectron2/modeling/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/backbone/swin.py` & `onvif-gui-1.2.0/detectron2/modeling/backbone/swin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/backbone/utils.py` & `onvif-gui-1.2.0/detectron2/modeling/backbone/utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/backbone/vit.py` & `onvif-gui-1.2.0/detectron2/modeling/backbone/vit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/box_regression.py` & `onvif-gui-1.2.0/detectron2/modeling/box_regression.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/matcher.py` & `onvif-gui-1.2.0/detectron2/modeling/matcher.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/meta_arch/__init__.py` & `onvif-gui-1.2.0/detectron2/modeling/meta_arch/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/meta_arch/build.py` & `onvif-gui-1.2.0/detectron2/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/meta_arch/dense_detector.py` & `onvif-gui-1.2.0/detectron2/modeling/meta_arch/dense_detector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/meta_arch/fcos.py` & `onvif-gui-1.2.0/detectron2/modeling/meta_arch/fcos.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/meta_arch/panoptic_fpn.py` & `onvif-gui-1.2.0/detectron2/modeling/meta_arch/panoptic_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/meta_arch/rcnn.py` & `onvif-gui-1.2.0/detectron2/modeling/meta_arch/rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/meta_arch/retinanet.py` & `onvif-gui-1.2.0/detectron2/modeling/meta_arch/retinanet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/meta_arch/semantic_seg.py` & `onvif-gui-1.2.0/detectron2/modeling/meta_arch/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/mmdet_wrapper.py` & `onvif-gui-1.2.0/detectron2/modeling/mmdet_wrapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/poolers.py` & `onvif-gui-1.2.0/detectron2/modeling/poolers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/postprocessing.py` & `onvif-gui-1.2.0/detectron2/modeling/postprocessing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/proposal_generator/build.py` & `onvif-gui-1.2.0/detectron2/modeling/proposal_generator/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/proposal_generator/proposal_utils.py` & `onvif-gui-1.2.0/detectron2/modeling/proposal_generator/proposal_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/proposal_generator/rpn.py` & `onvif-gui-1.2.0/detectron2/modeling/proposal_generator/rpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/proposal_generator/rrpn.py` & `onvif-gui-1.2.0/detectron2/modeling/proposal_generator/rrpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/roi_heads/__init__.py` & `onvif-gui-1.2.0/detectron2/modeling/roi_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/roi_heads/box_head.py` & `onvif-gui-1.2.0/detectron2/modeling/roi_heads/box_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/roi_heads/cascade_rcnn.py` & `onvif-gui-1.2.0/detectron2/modeling/roi_heads/cascade_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/roi_heads/fast_rcnn.py` & `onvif-gui-1.2.0/detectron2/modeling/roi_heads/fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/roi_heads/keypoint_head.py` & `onvif-gui-1.2.0/detectron2/modeling/roi_heads/keypoint_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/roi_heads/mask_head.py` & `onvif-gui-1.2.0/detectron2/modeling/roi_heads/mask_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/roi_heads/roi_heads.py` & `onvif-gui-1.2.0/detectron2/modeling/roi_heads/roi_heads.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/roi_heads/rotated_fast_rcnn.py` & `onvif-gui-1.2.0/detectron2/modeling/roi_heads/rotated_fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/sampling.py` & `onvif-gui-1.2.0/detectron2/modeling/sampling.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/modeling/test_time_augmentation.py` & `onvif-gui-1.2.0/detectron2/modeling/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/predictor.py` & `onvif-gui-1.2.0/detectron2/predictor.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/structures/__init__.py` & `onvif-gui-1.2.0/detectron2/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/structures/boxes.py` & `onvif-gui-1.2.0/detectron2/structures/boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/structures/image_list.py` & `onvif-gui-1.2.0/detectron2/structures/image_list.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/structures/instances.py` & `onvif-gui-1.2.0/detectron2/structures/instances.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/structures/keypoints.py` & `onvif-gui-1.2.0/detectron2/structures/keypoints.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/structures/masks.py` & `onvif-gui-1.2.0/detectron2/structures/masks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/structures/rotated_boxes.py` & `onvif-gui-1.2.0/detectron2/structures/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/tracker.py` & `onvif-gui-1.2.0/detectron2/tracker.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/utils/analysis.py` & `onvif-gui-1.2.0/detectron2/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/utils/collect_env.py` & `onvif-gui-1.2.0/detectron2/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/utils/colormap.py` & `onvif-gui-1.2.0/detectron2/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/utils/comm.py` & `onvif-gui-1.2.0/detectron2/utils/comm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/utils/develop.py` & `onvif-gui-1.2.0/detectron2/utils/develop.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/utils/env.py` & `onvif-gui-1.2.0/detectron2/utils/env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/utils/events.py` & `onvif-gui-1.2.0/detectron2/utils/events.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/utils/file_io.py` & `onvif-gui-1.2.0/detectron2/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/utils/logger.py` & `onvif-gui-1.2.0/detectron2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/utils/memory.py` & `onvif-gui-1.2.0/detectron2/utils/memory.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/utils/registry.py` & `onvif-gui-1.2.0/detectron2/utils/registry.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/utils/serialize.py` & `onvif-gui-1.2.0/detectron2/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/utils/testing.py` & `onvif-gui-1.2.0/detectron2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/utils/video_visualizer.py` & `onvif-gui-1.2.0/detectron2/utils/video_visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/detectron2/utils/visualizer.py` & `onvif-gui-1.2.0/detectron2/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/components/comboselector.py` & `onvif-gui-1.2.0/gui/components/comboselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/components/directoryselector.py` & `onvif-gui-1.2.0/gui/components/directoryselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/components/fileselector.py` & `onvif-gui-1.2.0/gui/components/fileselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/components/labelselector.py` & `onvif-gui-1.2.0/gui/components/labelselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/components/progress.py` & `onvif-gui-1.2.0/gui/components/progress.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/components/thresholdslider.py` & `onvif-gui-1.2.0/gui/components/thresholdslider.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/glwidget.py` & `onvif-gui-1.2.0/gui/glwidget.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/main.py` & `onvif-gui-1.2.0/gui/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,48 +17,49 @@
 #
 #*********************************************************************/
 
 import os
 import sys
 import time
 import importlib.util
-import numpy as np
 from pathlib import Path
 from PyQt6.QtWidgets import QApplication, QMainWindow, QLabel, QSplitter, \
     QTabWidget, QMessageBox
 from PyQt6.QtCore import pyqtSignal, QObject, QSettings, QDir, QSize
 from PyQt6.QtGui import QIcon
 from gui.panels import CameraPanel, FilePanel, SettingsPanel, VideoPanel, AudioPanel
 from gui.glwidget import GLWidget
-from loguru import logger
+from gui.components import WaitDialog
+from collections import deque
 
-sys.path.append("../build/libavio")
-sys.path.append("../build/libavio/Release")
 import avio
 
 class MainWindowSignals(QObject):
     started = pyqtSignal(int)
     stopped = pyqtSignal()
     progress = pyqtSignal(float)
     error = pyqtSignal(str)
+    showWait = pyqtSignal()
+    hideWait = pyqtSignal()
 
 class ViewLabel(QLabel):
     def __init__(self):
         super().__init__()
 
     def sizeHint(self):
         return QSize(640, 480)
 
 class MainWindow(QMainWindow):
     def __init__(self, clear_settings=False):
         super().__init__()
         os.environ["QT_FILESYSTEMMODEL_WATCH_FILES"] = "ON"
         QDir.addSearchPath("image", self.getLocation() + "/gui/resources/")
         self.style()
-        self.program_name = "onvif gui version 1.1.9"
+
+        self.program_name = "onvif gui version 1.2.0"
         self.setWindowTitle(self.program_name)
         self.setWindowIcon(QIcon('image:onvif-gui.png'))
         self.settings = QSettings("onvif", "gui")
         if clear_settings:
             self.settings.clear()
         self.volumeKey = "MainWindow/volume"
         self.muteKey = "MainWindow/mute"
@@ -94,15 +95,14 @@
         self.signals.started.connect(self.settingsPanel.onMediaStarted)
         self.signals.stopped.connect(self.settingsPanel.onMediaStopped)
         self.tab.addTab(self.cameraPanel, "Cameras")
         self.tab.addTab(self.filePanel, "Files")
         self.tab.addTab(self.settingsPanel, "Settings")
         self.tab.addTab(self.videoPanel, "Video")
         self.tab.addTab(self.audioPanel, "Audio")
-        self.tab.setCurrentIndex(int(self.settings.value(self.tabIndexKey, 0)))
 
         if self.settings.value(self.settingsPanel.renderKey, 0) == 0:
             self.glWidget = GLWidget()
         else:
             self.glWidget = ViewLabel()
 
         self.split = QSplitter()
@@ -117,87 +117,125 @@
         if rect is not None:
             if rect.width() > 0 and rect.height() > 0 and rect.x() > 0 and rect.y() > 0:
                 self.setGeometry(rect)
 
         if self.settingsPanel.chkAutoDiscover.isChecked():
             self.cameraPanel.btnDiscoverClicked()
 
-        self.videoHook = None
+        self.dlgWait = WaitDialog(self)
+        self.signals.showWait.connect(self.dlgWait.show)
+        self.signals.hideWait.connect(self.dlgWait.hide)
+
+        self.videoRuntimes = deque()
+        self.videoWorkerHook = None
         self.videoWorker = None
+        self.videoConfigureHook = None
         self.videoConfigure = None
         videoWorkerName = self.videoPanel.cmbWorker.currentText()
         if len(videoWorkerName) > 0:
-            self.loadVideoWorker(videoWorkerName)
             self.loadVideoConfigure(videoWorkerName)
 
-        self.audioHook = None
+        self.audioRuntimes = deque()
+        self.audioWorkerHook = None
         self.audioWorker = None
+        self.audioConfigureHook = None
         self.audioConfigure = None
         audioWorkerName = self.audioPanel.cmbWorker.currentText()
         if len(audioWorkerName) > 0:
-            self.loadAudioWorker(audioWorkerName)
             self.loadAudioConfigure(audioWorkerName)
 
         if splitterState is not None:
             self.split.restoreState(splitterState)
 
+        self.tab.setCurrentIndex(int(self.settings.value(self.tabIndexKey, 0)))
+
     def loadVideoConfigure(self, workerName):
         spec = importlib.util.spec_from_file_location("VideoConfigure", self.videoPanel.dirModules.text() + "/" + workerName)
-        videoHook = importlib.util.module_from_spec(spec)
-        sys.modules["VideoConfigure"] = videoHook
-        spec.loader.exec_module(videoHook)
-        self.configure = videoHook.VideoConfigure(self)
+        videoConfigureHook = importlib.util.module_from_spec(spec)
+        sys.modules["VideoConfigure"] = videoConfigureHook
+        spec.loader.exec_module(videoConfigureHook)
+        self.configure = videoConfigureHook.VideoConfigure(self)
         self.videoPanel.setPanel(self.configure)
 
     def loadVideoWorker(self, workerName):
         spec = importlib.util.spec_from_file_location("VideoWorker", self.videoPanel.dirModules.text() + "/" + workerName)
-        self.videoHook = importlib.util.module_from_spec(spec)
-        sys.modules["VideoWorker"] = self.videoHook
-        spec.loader.exec_module(self.videoHook)
+        self.videoWorkerHook = importlib.util.module_from_spec(spec)
+        sys.modules["VideoWorker"] = self.videoWorkerHook
+        spec.loader.exec_module(self.videoWorkerHook)
         self.worker = None
 
     def pyVideoCallback(self, F):
         if self.videoPanel.chkEngage.isChecked():
-            if self.videoHook is not None:
+
+            if self.videoWorkerHook is None:
+                videoWorkerName = self.videoPanel.cmbWorker.currentText()
+                if len(videoWorkerName) > 0:
+                    self.loadVideoWorker(videoWorkerName)
+
+            if self.videoWorkerHook is not None:
                 if self.worker is None:
-                    self.worker = self.videoHook.VideoWorker(self)
+                    self.worker = self.videoWorkerHook.VideoWorker(self)
+
                 start = time.time()
                 self.worker(F)
                 finish = time.time()
                 elapsed = int((finish - start) * 1000)
-                self.videoPanel.lblElapsed.setText("Elapsed Time (ms)  " + str(elapsed))
+                self.videoRuntimes.append(elapsed)
+                if len(self.videoRuntimes) > 60:
+                    self.videoRuntimes.popleft()
+                sum = 0
+                for x in self.videoRuntimes:
+                    sum += x
+                display = str(int(sum / len(self.videoRuntimes)))
+                self.videoPanel.lblElapsed.setText("Avg Rumtime (ms)  " + display)
+
         else:
             self.videoPanel.lblElapsed.setText("")
         return F
     
     def loadAudioConfigure(self, workerName):
         spec = importlib.util.spec_from_file_location("AudioConfigure", self.audioPanel.dirModules.text() + "/" + workerName)
-        audioHook = importlib.util.module_from_spec(spec)
-        sys.modules["AudioConfigure"] = audioHook
-        spec.loader.exec_module(audioHook)
-        self.audioConfigure = audioHook.AudioConfigure(self)
+        audioConfigureHook = importlib.util.module_from_spec(spec)
+        sys.modules["AudioConfigure"] = audioConfigureHook
+        spec.loader.exec_module(audioConfigureHook)
+        self.audioConfigure = audioConfigureHook.AudioConfigure(self)
         self.audioPanel.setPanel(self.audioConfigure)
     
     def loadAudioWorker(self, workerName):
         spec = importlib.util.spec_from_file_location("AudioWorker", self.audioPanel.dirModules.text() + "/" + workerName)
-        self.audioHook = importlib.util.module_from_spec(spec)
-        sys.modules["AudioWorker"] = self.audioHook
-        spec.loader.exec_module(self.audioHook)
+        self.audioWorkerHook = importlib.util.module_from_spec(spec)
+        sys.modules["AudioWorker"] = self.audioWorkerHook
+        spec.loader.exec_module(self.audioWorkerHook)
         self.audioWorker = None
 
     def pyAudioCallback(self, F):
         if self.audioPanel.chkEngage.isChecked():
-            if self.audioHook is not None:
+
+            if self.audioWorkerHook is None:
+                audioWorkerName = self.audioPanel.cmbWorker.currentText()
+                if len(audioWorkerName) > 0:
+                    self.loadAudioWorker(audioWorkerName)
+
+            if self.audioWorkerHook is not None:
                 if self.audioWorker is None:
-                    self.audioWorker = self.audioHook.AudioWorker(self)
+                    self.audioWorker = self.audioWorkerHook.AudioWorker(self)
+                
                 start = time.time()
                 self.audioWorker(F)
                 finish = time.time()
                 elapsed = int((finish - start) * 1000)
-                self.audioPanel.lblElapsed.setText("Elapsed Time (ms)  " + str(elapsed))
+                self.audioRuntimes.append(elapsed)
+                if len(self.audioRuntimes) > 100:
+                    self.audioRuntimes.popleft()
+                sum = 0
+                for x in self.audioRuntimes:
+                    sum += x
+                display = str(int(sum / len(self.audioRuntimes)))
+                self.audioPanel.lblElapsed.setText("Avg Runtime (ms)  " + display)
+
         else:
             self.audioPanel.lblElapsed.setText("")
         return F
 
     def playMedia(self, uri):
         self.stopMedia()
         self.player = avio.Player()
@@ -292,16 +330,16 @@
 
     def mediaProgress(self, f):
         self.signals.progress.emit(f)
 
     def infoCallback(self, msg):
         print(msg)
 
-    def errorCallback(self, s):
-        self.signals.error.emit(s)
+    def errorCallback(self, msg):
+        self.signals.error.emit(msg)
 
     def onError(self, msg):
         msgBox = QMessageBox(self)
         msgBox.setText(msg)
         msgBox.setWindowTitle(self.program_name)
         msgBox.setIcon(QMessageBox.Icon.Warning)
         msgBox.exec()
@@ -311,22 +349,18 @@
 
     def splitterMoved(self, pos, index):
         self.settings.setValue(self.splitKey, self.split.saveState())
 
     def getLocation(self):
         path = Path(os.path.dirname(__file__))
         return str(path.parent.absolute())
-        #return os.path.dirname(__file__)
-
+    
     def style(self):
-        #blDefault = "#566170"
         blDefault = "#5B5B5B"
-        #bmDefault = "#3E4754"
         bmDefault = "#4B4B4B"
-        #bdDefault = "#283445"
         bdDefault = "#3B3B3B"
         flDefault = "#C6D9F2"
         fmDefault = "#9DADC2"
         fdDefault = "#808D9E"
         slDefault = "#FFFFFF"
         smDefault = "#DDEEFF"
         sdDefault = "#306294"
@@ -336,21 +370,17 @@
         strStyle = strStyle.replace("background_dark",   bdDefault)
         strStyle = strStyle.replace("foreground_light",  flDefault)
         strStyle = strStyle.replace("foreground_medium", fmDefault)
         strStyle = strStyle.replace("foreground_dark",   fdDefault)
         strStyle = strStyle.replace("selection_light",   slDefault)
         strStyle = strStyle.replace("selection_medium",  smDefault)
         strStyle = strStyle.replace("selection_dark",    sdDefault)
-        #print(strStyle)
         self.setStyleSheet(strStyle)
 
 def run():
-    #if sys.platform == "win32":
-    #    sys.argv += ['-platform', 'windows:darkmode=2']
-
     clear_settings = False
     if len(sys.argv) > 1:
         if str(sys.argv[1]) == "--clear":
             clear_settings = True
 
     app = QApplication(sys.argv)
     app.setStyle('Fusion')
```

### Comparing `onvif-gui-1.1.9/gui/onvif/admintab.py` & `onvif-gui-1.2.0/gui/onvif/admintab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/onvif/imagetab.py` & `onvif-gui-1.2.0/gui/onvif/imagetab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/onvif/logindialog.py` & `onvif-gui-1.2.0/gui/onvif/logindialog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/onvif/networktab.py` & `onvif-gui-1.2.0/gui/onvif/networktab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/onvif/ptztab.py` & `onvif-gui-1.2.0/gui/onvif/ptztab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/onvif/videotab.py` & `onvif-gui-1.2.0/gui/onvif/videotab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/panels/audiopanel.py` & `onvif-gui-1.2.0/gui/panels/audiopanel.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,16 @@
         self.panel.setMaximumWidth(self.mw.tab.width())
         self.layout.addWidget(panel)
         self.layout.setStretch(1, 10)
 
     def cmbWorkerChanged(self, worker):
         if self.cmbWorkerConnected:
             self.mw.settings.setValue(self.workerKey, worker)
+            self.mw.audioFirstPass = True
+            self.mw.audioRuntimes.clear()
             self.mw.loadAudioConfigure(worker)
             self.mw.loadAudioWorker(worker)
 
     def chkEngageClicked(self, state):
         self.mw.settings.setValue(self.engageKey, state)
 
     def dirModulesChanged(self, path):
```

### Comparing `onvif-gui-1.1.9/gui/panels/camerapanel.py` & `onvif-gui-1.2.0/gui/panels/camerapanel.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #*********************************************************************/
 
-import sys
 from time import sleep
 import datetime
 from PyQt6.QtWidgets import QPushButton, QGridLayout, QWidget, QSlider, \
-QListWidget, QTabWidget, QMessageBox
-from PyQt6.QtGui import QIcon
+QListWidget, QTabWidget
 from PyQt6.QtCore import Qt, pyqtSignal, QObject, QSettings, QTimer
 from gui.onvif import AdminTab, NetworkTab, ImageTab, VideoTab, PTZTab, LoginDialog
 
-sys.path.append("../build/libonvif")
-sys.path.append("../build/libonvif/Release")
 import libonvif as onvif
 
 ICON_SIZE = 26
 
 class CameraPanelSignals(QObject):
     fill = pyqtSignal(onvif.Data)
     login = pyqtSignal(onvif.Data)
```

### Comparing `onvif-gui-1.1.9/gui/panels/filepanel.py` & `onvif-gui-1.2.0/gui/panels/filepanel.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 from PyQt6.QtWidgets import QLineEdit, QPushButton, \
 QGridLayout, QWidget, QSlider, QLabel, QMessageBox, \
 QTreeView, QFileDialog, QMenu
 from PyQt6.QtGui import QFileSystemModel, QAction
 from PyQt6.QtCore import Qt, QStandardPaths, QFile
 from gui.components import Progress
 
-sys.path.append("../build/libavio")
-sys.path.append("../build/libavio/Release")
 import avio
 
 ICON_SIZE = 26
 
 class TreeView(QTreeView):
     def __init__(self, mw):
         super().__init__()
```

### Comparing `onvif-gui-1.1.9/gui/panels/settingspanel.py` & `onvif-gui-1.2.0/gui/panels/settingspanel.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,19 +19,15 @@
 
 import os
 import sys
 from PyQt6.QtWidgets import QMessageBox, QLineEdit, QSpinBox, \
 QGridLayout, QWidget, QCheckBox, QLabel, QComboBox
 from PyQt6.QtCore import Qt
 
-sys.path.append("../build/libonvif")
-sys.path.append("../build/libonvif/Release")
 import libonvif as onvif
-sys.path.append("../build/libavio")
-sys.path.append("../build/libavio/Release")
 import avio
 
 class SettingsPanel(QWidget):
     def __init__(self, mw):
         super().__init__()
         self.mw = mw
         self.autoDiscoverKey = "settings/autoDiscover"
@@ -48,14 +44,15 @@
         self.hardwareEncodeKey = "settings/hardwareEncode"
         self.processPauseKey = "settings/processPause"
         self.processFrameKey = "settings/processFrame"
         self.cacheSizeKey = "settings/cacheSize"
         self.interfaceKey = "settings/interface"
         self.videoFilterKey = "settings/videoFilter"
         self.audioFilterKey = "settings/audioFilter"
+        self.showWaitBoxKey = "settings/showWaitBox"
 
         decoders = ["NONE", "CUDA", "VAAPI", "VDPAU", "DXVA2", "D3D11VA"]
 
         self.chkAutoDiscover = QCheckBox("Enable Auto Discovery")
         self.chkAutoDiscover.setChecked(int(mw.settings.value(self.autoDiscoverKey, 0)))
         self.chkAutoDiscover.stateChanged.connect(self.autoDiscoverChecked)
         
@@ -105,36 +102,44 @@
                 self.chkDisableAudio.setEnabled(False)
 
         self.chkPostEncode = QCheckBox("Post Process Record")
         self.chkPostEncode.setChecked(int(mw.settings.value(self.postEncodeKey, 0)))
         self.chkPostEncode.stateChanged.connect(self.postEncodeChecked)
 
         self.chkHardwareEncode = QCheckBox("Hardware Encode")
-        self.chkHardwareEncode.setChecked(int(mw.settings.value(self.hardwareEncodeKey, 0)))
-        self.chkHardwareEncode.setEnabled(self.chkPostEncode.isChecked())
-        self.chkHardwareEncode.stateChanged.connect(self.hardwareEncodeChecked)
+        if sys.platform == "win32":
+            self.chkHardwareEncode.setEnabled(False)
+        else:
+            self.chkHardwareEncode.setChecked(int(mw.settings.value(self.hardwareEncodeKey, 0)))
+            self.chkHardwareEncode.setEnabled(self.chkPostEncode.isChecked())
+            self.chkHardwareEncode.stateChanged.connect(self.hardwareEncodeChecked)
 
         self.chkProcessPause = QCheckBox("Process Pause")
         self.chkProcessPause.setChecked(int(mw.settings.value(self.processPauseKey, 0)))
         self.chkProcessPause.stateChanged.connect(self.processPauseChecked)
 
         self.chkLowLatency = QCheckBox("Low Latency")
         self.chkLowLatency.setChecked(int(mw.settings.value(self.latencyKey, 0)))
         self.chkLowLatency.stateChanged.connect(self.lowLatencyChecked)
 
+        self.chkShowWaitBox = QCheckBox("Show Wait Box")
+        self.chkShowWaitBox.setChecked(int(mw.settings.value(self.showWaitBoxKey, 1)))
+        self.chkShowWaitBox.stateChanged.connect(self.showWaitBoxChecked)
+
         pnlChecks = QWidget()
         lytChecks = QGridLayout(pnlChecks)
         lytChecks.addWidget(self.chkDirectRender,   0, 0, 1, 1)
         lytChecks.addWidget(self.chkConvert2RGB,    0, 1, 1, 1)
         lytChecks.addWidget(self.chkDisableAudio,   1, 0, 1, 1)
         lytChecks.addWidget(self.chkDisableVideo,   1, 1, 1, 1)
         lytChecks.addWidget(self.chkPostEncode,     2, 0, 1, 1)
         lytChecks.addWidget(self.chkHardwareEncode, 2, 1, 1, 1)
         lytChecks.addWidget(self.chkProcessPause,   3, 0, 1, 1)
         lytChecks.addWidget(self.chkLowLatency,     3, 1, 1, 1)
+        lytChecks.addWidget(self.chkShowWaitBox,    4, 0, 1, 1)
 
         self.spnCacheSize = QSpinBox()
         self.spnCacheSize.setMinimum(1)
         self.spnCacheSize.setMaximum(10)
         self.spnCacheSize.setMaximumWidth(80)
         self.spnCacheSize.setValue(int(self.mw.settings.value(self.cacheSizeKey, 1)))
         self.spnCacheSize.valueChanged.connect(self.spnCacheSizeChanged)
@@ -190,16 +195,16 @@
         lytMain.addWidget(lblDecoders,            3, 0, 1, 1)
         lytMain.addWidget(self.cmbDecoder,        3, 1, 1, 1)
         lytMain.addWidget(pnlFilter,              6, 0, 1, 3)
         lytMain.addWidget(pnlChecks,              7, 0, 1, 3)
         lytMain.addWidget(lblCacheSize,           8, 0, 1, 1)
         lytMain.addWidget(self.spnCacheSize,      8, 1, 1, 1)
         lytMain.addWidget(pnlInterface,           9, 0, 1, 3)
-        lytMain.addWidget(self.lblSpacer,        10, 0, 1, 3, Qt.AlignmentFlag.AlignCenter)
-        lytMain.setRowStretch(10, 10)
+        lytMain.addWidget(self.lblSpacer,        11, 0, 1, 3, Qt.AlignmentFlag.AlignCenter)
+        lytMain.setRowStretch(11, 10)
 
     def autoDiscoverChecked(self, state):
         self.mw.settings.setValue(self.autoDiscoverKey, state)
 
     def usernameChanged(self, username):
         self.mw.settings.setValue(self.usernameKey, username)
 
@@ -245,27 +250,31 @@
         if state == 0:
             self.chkDisableAudio.setEnabled(True)
         else:
             self.chkDisableAudio.setEnabled(False)
 
     def postEncodeChecked(self, state):
         self.mw.settings.setValue(self.postEncodeKey, state)
-        if state == 0:
-            self.chkHardwareEncode.setChecked(False)
-        self.chkHardwareEncode.setEnabled(state)
+        if sys.platform != "win32":
+            if state == 0:
+                self.chkHardwareEncode.setChecked(False)
+            self.chkHardwareEncode.setEnabled(state)
 
     def hardwareEncodeChecked(self, state):
         self.mw.settings.setValue(self.hardwareEncodeKey, state)
 
     def processPauseChecked(self, state):
         self.mw.settings.setValue(self.processPauseKey, state)
 
     def lowLatencyChecked(self, state):
         self.mw.settings.setValue(self.latencyKey, state)
 
+    def showWaitBoxChecked(self, state):
+        self.mw.settings.setValue(self.showWaitBoxKey, state)
+
     def radioFilenameChecked(self):
         if self.radGenerateFilename.isChecked():
             self.mw.settings.setValue(self.generateKey, 1)
         else:
             self.mw.settings.setValue(self.generateKey, 0)
 
     def spnCacheSizeChanged(self, i):
```

### Comparing `onvif-gui-1.1.9/gui/panels/videopanel.py` & `onvif-gui-1.2.0/gui/panels/videopanel.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,14 +76,16 @@
         self.panel.setMaximumWidth(self.mw.tab.width())
         self.layout.addWidget(panel)
         self.layout.setStretch(1, 10)
 
     def cmbWorkerChanged(self, worker):
         if self.cmbWorkerConnected:
             self.mw.settings.setValue(self.workerKey, worker)
+            self.mw.videoFirstPass = True
+            self.mw.videoRuntimes.clear()
             self.mw.loadVideoConfigure(worker)
             self.mw.loadVideoWorker(worker)
 
     def chkEngageClicked(self, state):
         self.mw.settings.setValue(self.engageKey, state)
 
     def dirModulesChanged(self, path):
```

### Comparing `onvif-gui-1.1.9/gui/resources/LICENSE` & `onvif-gui-1.2.0/gui/resources/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/resources/audio.png` & `onvif-gui-1.2.0/gui/resources/audio.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/resources/audio_hi.png` & `onvif-gui-1.2.0/gui/resources/audio_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/resources/audio_lo.png` & `onvif-gui-1.2.0/gui/resources/audio_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/resources/darkstyle.qss` & `onvif-gui-1.2.0/gui/resources/darkstyle.qss`

 * *Files 0% similar despite different names*

```diff
@@ -609,8 +609,9 @@
 
 QSlider::sub-page:horizontal {
     background: foreground_medium;
 }
 
 QToolTip {
     color : black;
+    background : #ffffbb;
 }
```

### Comparing `onvif-gui-1.1.9/gui/resources/discover.png` & `onvif-gui-1.2.0/gui/resources/discover.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/resources/discover_hi.png` & `onvif-gui-1.2.0/gui/resources/discover_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/resources/discover_lo.png` & `onvif-gui-1.2.0/gui/resources/discover_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/resources/mute.png` & `onvif-gui-1.2.0/gui/resources/mute.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/resources/mute_lo.png` & `onvif-gui-1.2.0/gui/resources/mute_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/resources/onvif-gui.png` & `onvif-gui-1.2.0/gui/resources/onvif-gui.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/gui/resources/recording_lo.png` & `onvif-gui-1.2.0/gui/resources/recording_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/modules/audio/sample.py` & `onvif-gui-1.2.0/modules/audio/sample.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/modules/video/keypoint.py` & `onvif-gui-1.2.0/modules/video/keypoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,25 +12,30 @@
     from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QMessageBox
     from gui.components import ThresholdSlider
 
     import torch
     from detectron2.config import get_cfg
     from detectron2.predictor import Predictor
     from detectron2.tracker import DetectedInstance, SimpleTracker
+
+    import ssl
+    ssl._create_default_https_context = ssl._create_unverified_context
+
 except ModuleNotFoundError as ex:
     IMPORT_ERROR = str(ex)
     print("Import Error has occurred, missing modules need to be installed, please consult documentation: ", ex)
 
 MODULE_NAME = "detectron2/keypoint"
 
 class VideoConfigure(QWidget):
     def __init__(self, mw):
         try:
             super().__init__()
             self.mw = mw
+            logger.add("errors.txt", retention="1 days")
             self.name = MODULE_NAME
             self.sldThreshold = ThresholdSlider(mw, MODULE_NAME, "Confidence", 50)
             lytMain = QGridLayout(self)
             lytMain.addWidget(self.sldThreshold,   0, 0, 1, 1)
             lytMain.addWidget(QLabel(""),          1, 0, 1, 1)
             lytMain.setRowStretch(1, 10)
 
@@ -52,29 +57,37 @@
         self.sldThreshold.setEnabled(True)
 
 class VideoWorker:
     def __init__(self, mw):
         try:
             self.mw = mw
             self.last_ex = ""
+
+            if self.mw.settingsPanel.chkShowWaitBox.isChecked():
+                self.mw.signals.showWait.emit()
+
             self.CONFIDENCE_THRESHOLD = self.mw.configure.sldThreshold.value()
             ckpt_file = "auto"
             fp16 = True
             self.no_back = True
             self.simple = True
 
             if ckpt_file is not None:
                 if ckpt_file.lower() == "auto":
                     ckpt_file = self.get_auto_ckpt_filename()
                     print("ckpt_file:", ckpt_file)
                     cache = Path(ckpt_file)
 
                     if not cache.is_file():
                         cache.parent.mkdir(parents=True, exist_ok=True)
-                        torch.hub.download_url_to_file("https://dl.fbaipublicfiles.com/detectron2/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x/137849621/model_final_a6e10b.pkl", ckpt_file)
+                        link = "https://dl.fbaipublicfiles.com/detectron2/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x/137849621/model_final_a6e10b.pkl"
+                        if sys.platform == "win32":
+                            torch.hub.download_url_to_file(link, ckpt_file, progress=False)
+                        else:
+                            torch.hub.download_url_to_file(link, ckpt_file)
 
             cfg = get_cfg()
             config_file = ""
             yaml_file = 'detectron2/configs/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x.yaml'
             if not os.path.isfile(yaml_file):
                 for path in sys.path:
                     config_file = os.path.join(path, yaml_file)
@@ -88,14 +101,19 @@
             cfg.MODEL.ROI_HEADS.SCORE_THRESH_TEST = self.CONFIDENCE_THRESHOLD
             cfg.MODEL.WEIGHTS = ckpt_file
             cfg.MODEL.PANOPTIC_FPN.COMBINE.INSTANCES_CONFIDENCE_THRESH = self.CONFIDENCE_THRESHOLD
             cfg.freeze()
 
             self.tracker = SimpleTracker()
             self.predictor = Predictor(cfg, fp16)
+            self.predictor(np.zeros([1280, 720, 3]))
+
+            if self.mw.settingsPanel.chkShowWaitBox.isChecked():
+                self.mw.signals.hideWait.emit()
+
         except:
             logger.exception("Keypoints initialization error")
 
 
     def __call__(self, F):
         try:
             img = np.array(F, copy=False)
@@ -118,14 +136,15 @@
 
             if len(detected):
                 colors = np.asarray(self.tracker.assign_colors(detected)) * 255
                 colors = colors.astype(np.int32)
                 for idx, keypoint in enumerate(keypoints):
                     self.draw_keypoint(img, keypoint, colors[idx])
 
+
         except Exception as ex:
             if self.last_ex != str(ex) and self.mw.configure.name == MODULE_NAME:
                 logger.exception("Keypoints runtime error")
             self.last_ex = str(ex)
 
     def get_auto_ckpt_filename(self):
         filename = None
```

### Comparing `onvif-gui-1.1.9/modules/video/retinanet.py` & `onvif-gui-1.2.0/modules/video/retinanet.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,28 +27,33 @@
     from gui.components.thresholdslider import ThresholdSlider
     from gui.components.labelselector import LabelSelector
 
     import torch
     import torchvision
     import torchvision.transforms as transforms
 
+    import ssl
+    ssl._create_default_https_context = ssl._create_unverified_context
+
     transform = transforms.Compose([
         transforms.ToTensor(),
     ])
+    
 except ModuleNotFoundError as ex:
     IMPORT_ERROR = str(ex)
     print("Import Error has occurred, missing modules need to be installed, please consult documentation: ", ex)
 
 MODULE_NAME = "retinanet"
 
 class VideoConfigure(QWidget):
     def __init__(self, mw):
         try:
             super().__init__()
             self.mw = mw
+            logger.add("errors.txt", retention="1 days")
             self.name = MODULE_NAME
 
             self.sldThreshold = ThresholdSlider(mw, MODULE_NAME, "Confidence", 35)
             
             number_of_labels = 5
             self.labels = []
             for i in range(number_of_labels):
@@ -76,17 +81,27 @@
             logger.exception("retinanet configuration load error")
 
 class VideoWorker:
     def __init__(self, mw):
         try:
             self.mw = mw
             self.last_ex = ""
+
+            if self.mw.settingsPanel.chkShowWaitBox.isChecked():
+                self.mw.signals.showWait.emit()
+
             self.model = torchvision.models.detection.retinanet_resnet50_fpn(weights=torchvision.models.detection.RetinaNet_ResNet50_FPN_Weights.DEFAULT)            
             self.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
             self.model.eval().to(self.device)
+            with torch.no_grad():
+                self.model(torch.zeros(1, 3, 1280, 720).to(self.device))
+
+            if self.mw.settingsPanel.chkShowWaitBox.isChecked():
+                self.mw.signals.hideWait.emit()
+
         except:
             logger.exception("retinanet worker load error")
 
     def __call__(self, F):
         try:
             img = np.array(F, copy = False)
             tensor = transform(img).to(self.device)
```

### Comparing `onvif-gui-1.1.9/modules/video/sample.py` & `onvif-gui-1.2.0/modules/video/sample.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 MODULE_NAME = "sample"
 
 class VideoConfigure(QWidget):
     def __init__(self, mw):
         try:
             super().__init__()
             self.mw = mw
+            logger.add("errors.txt", retention="1 days")
             self.name = MODULE_NAME
             self.showBorderKey = "Module/" + MODULE_NAME + "/showBorder"
             self.chkShowBorder = QCheckBox("Show Border")
             self.chkShowBorder.setChecked(int(self.mw.settings.value(self.showBorderKey, 0)))
             self.chkShowBorder.stateChanged.connect(self.chkShowBorderClicked)
             lytMain = QGridLayout(self)
             lytMain.addWidget(self.chkShowBorder, 0, 0, 1, 1)
```

### Comparing `onvif-gui-1.1.9/modules/video/segment.py` & `onvif-gui-1.2.0/modules/video/segment.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,25 +12,30 @@
     from PyQt6.QtCore import Qt
     from gui.components import ThresholdSlider, LabelSelector
 
     import torch
     from detectron2.config import get_cfg
     from detectron2.predictor import Predictor
     from detectron2.tracker import DetectedInstance, SimpleTracker
+
+    import ssl
+    ssl._create_default_https_context = ssl._create_unverified_context
+
 except ModuleNotFoundError as ex:
     IMPORT_ERROR = str(ex)
     print("Import Error has occurred, missing modules need to be installed, please consult documentation: ", ex)
 
 MODULE_NAME = "detectron2/segment"
 
 class VideoConfigure(QWidget):
     def __init__(self, mw):
         try:
             super().__init__()
             self.mw = mw
+            logger.add("errors.txt", retention="1 days")
             self.name = MODULE_NAME
             self.sldThreshold = ThresholdSlider(mw, MODULE_NAME, "Confidence", 50)
 
             self.number_of_labels = 5
             self.labels = []
             for i in range(self.number_of_labels):
                 lbl = LabelSelector(mw, self.name, i)
@@ -70,14 +75,18 @@
         self.sldThreshold.setEnabled(True)
 
 class VideoWorker:
     def __init__(self, mw):
         try:
             self.mw = mw
             self.last_ex = ""
+
+            if self.mw.settingsPanel.chkShowWaitBox.isChecked():
+                self.mw.signals.showWait.emit()
+
             self.CONFIDENCE_THRESHOLD = self.mw.configure.sldThreshold.value()
             ckpt_file = 'auto'
             fp16 = True
             self.simple = True
             self.draw_overlay = False
             self.first_pass = True
 
@@ -85,15 +94,19 @@
                 if ckpt_file.lower() == "auto":
                     ckpt_file = self.get_auto_ckpt_filename()
                     print("ckpt_file:", ckpt_file)
                     cache = Path(ckpt_file)
 
                     if not cache.is_file():
                         cache.parent.mkdir(parents=True, exist_ok=True)
-                        torch.hub.download_url_to_file("https://dl.fbaipublicfiles.com/detectron2/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x/137849600/model_final_f10217.pkl", ckpt_file)
+                        link = "https://dl.fbaipublicfiles.com/detectron2/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x/137849600/model_final_f10217.pkl"
+                        if sys.platform == "win32":
+                            torch.hub.download_url_to_file(link, ckpt_file, progress=False)
+                        else:
+                            torch.hub.download_url_to_file(link, ckpt_file)
 
             cfg = get_cfg()
             config_file = ""
             yaml_file = 'detectron2/configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml'
             if not os.path.isfile(yaml_file):
                 for path in sys.path:
                     config_file = os.path.join(path, yaml_file)
@@ -109,17 +122,24 @@
             cfg.MODEL.ROI_HEADS.SCORE_THRESH_TEST = self.CONFIDENCE_THRESHOLD
             cfg.MODEL.PANOPTIC_FPN.COMBINE.INSTANCES_CONFIDENCE_THRESH = self.CONFIDENCE_THRESHOLD
             cfg.freeze()
 
             self.tracker = SimpleTracker()
             self.predictor = Predictor(cfg, fp16)
 
+            self.predictor(np.zeros([1280, 720, 3]))
+
             self.first_pass = False
             self.mw.signals.stopped.connect(self.stopped)
 
+            if self.mw.settingsPanel.chkShowWaitBox.isChecked():
+                self.mw.signals.hideWait.emit()
+
+
+
         except:
             logger.exception("Instance Segmentation initialization error")
 
     def __call__(self, F):
         try:
 
             if self.first_pass:
```

### Comparing `onvif-gui-1.1.9/modules/video/yolov7.py` & `onvif-gui-1.2.0/modules/video/yolov7.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,17 +54,19 @@
 MODULE_NAME = "yolov7"
 
 class VideoConfigure(QWidget):
     def __init__(self, mw):
         try:
             super().__init__()
             self.mw = mw
+            logger.add("errors.txt", retention="1 days")
             self.name = MODULE_NAME
             self.autoKey = "Module/" + MODULE_NAME + "/autoDownload"
             self.trackKey = "Module/" + MODULE_NAME + "/track"
+            self.showIDKey = "Module/" + MODULE_NAME + "/showID"
 
             self.chkAuto = QCheckBox("Automatically download model")
             self.chkAuto.setChecked(int(self.mw.settings.value(self.autoKey, 1)))
             self.chkAuto.stateChanged.connect(self.chkAutoClicked)
 
             self.txtFilename = FileSelector(mw, MODULE_NAME)
             self.txtFilename.setEnabled(not self.chkAuto.isChecked())
@@ -72,14 +74,21 @@
             self.cmbRes = ComboSelector(mw, "Model Size", ("320", "480", "640", "960", "1280"), "640", MODULE_NAME)
             self.cmbType = ComboSelector(mw, "Model Name", ("yolov7", "yolov7x"), "yolov7", MODULE_NAME)
 
             self.chkTrack = QCheckBox("Track Objects")
             self.chkTrack.setChecked(int(self.mw.settings.value(self.trackKey, 0)))
             self.chkTrack.stateChanged.connect(self.chkTrackClicked)
 
+            self.chkShowID = QCheckBox("Show Object ID")
+            self.chkShowID.setChecked(int(self.mw.settings.value(self.showIDKey, 1)))
+            self.chkShowID.stateChanged.connect(self.chkShowIDClicked)
+
+            if not self.chkTrack.isChecked():
+                self.chkShowID.setVisible(False)
+
             self.sldConfThre = ThresholdSlider(mw, MODULE_NAME + "/confidence", "Confidence", 25)
 
             number_of_labels = 5
             self.labels = []
             for i in range(number_of_labels):
                 self.labels.append(LabelSelector(mw, MODULE_NAME, i+1))
             pnlLabels = QWidget()
@@ -88,63 +97,76 @@
             lblPanel.setAlignment(Qt.AlignmentFlag.AlignCenter)
             lytLabels.addWidget(lblPanel,        0, 0, 1, 1)
             for i in range(number_of_labels):
                 lytLabels.addWidget(self.labels[i], i+1, 0, 1, 1)
             lytLabels.setContentsMargins(0, 0, 0, 0)
 
             lytMain = QGridLayout(self)
-            lytMain.addWidget(self.chkAuto,      0, 0, 1, 1)
-            lytMain.addWidget(self.cmbType,      1, 0, 1, 1)
-            lytMain.addWidget(self.txtFilename,  2, 0, 1, 1)
-            lytMain.addWidget(self.cmbRes,       3, 0, 1, 1)
-            lytMain.addWidget(self.sldConfThre,  4, 0, 1, 1)
+            lytMain.addWidget(self.chkAuto,      0, 0, 1, 2)
+            lytMain.addWidget(self.cmbType,      1, 0, 1, 2)
+            lytMain.addWidget(self.txtFilename,  2, 0, 1, 2)
+            lytMain.addWidget(self.cmbRes,       3, 0, 1, 2)
+            lytMain.addWidget(self.sldConfThre,  4, 0, 1, 2)
             lytMain.addWidget(self.chkTrack,     6, 0, 1, 1)
-            lytMain.addWidget(pnlLabels,         7, 0, 1, 1)
-            lytMain.addWidget(QLabel(),          8, 0, 1, 1)
+            lytMain.addWidget(self.chkShowID,    6, 1, 1, 1)
+            lytMain.addWidget(pnlLabels,         7, 0, 1, 2)
+            lytMain.addWidget(QLabel(),          8, 0, 1, 2)
             lytMain.setRowStretch(8, 10)
 
             if len(IMPORT_ERROR) > 0:
                 QMessageBox.critical(None, MODULE_NAME + " Import Error", "Modules required for running this function are missing: " + IMPORT_ERROR)
 
         except:
             logger.exception(MODULE_NAME + " configure failed to load")
 
     def chkAutoClicked(self, state):
         self.mw.settings.setValue(self.autoKey, state)
         self.txtFilename.setEnabled(not self.chkAuto.isChecked())
 
     def chkTrackClicked(self, state):
         self.mw.settings.setValue(self.trackKey, state)
+        self.chkShowID.setVisible(state)
+
+    def chkShowIDClicked(self, state):
+        self.mw.settings.setValue(self.showIDKey, state)
 
     def getLabel(self, cls):
         for lbl in self.labels:
             if lbl.label() == cls:
                 return lbl
 
 class VideoWorker:
     def __init__(self, mw):
         try:
             self.mw = mw
             self.last_ex = ""
 
+            if self.mw.configure.name != MODULE_NAME:
+                return
+            
+            if self.mw.settingsPanel.chkShowWaitBox.isChecked():
+                self.mw.signals.showWait.emit()
+
             self.ckpt_file = None
             if self.mw.configure.chkAuto.isChecked():
                 self.ckpt_file = self.get_auto_ckpt_filename()
                 print("cpkt_file:", self.ckpt_file)
                 cache = Path(self.ckpt_file)
 
                 if not cache.is_file():
                     cache.parent.mkdir(parents=True, exist_ok=True)
                     model_name = self.mw.configure.cmbType.currentText()
                     link = "https://github.com/WongKinYiu/yolov7/releases/download/v0.1/" + model_name + ".pt"
-                    torch.hub.download_url_to_file(link, self.ckpt_file)
+                    if os.path.split(sys.executable)[1] == "pythonw.exe":
+                        torch.hub.download_url_to_file(link, self.ckpt_file, progress=False)
+                    else:
+                        torch.hub.download_url_to_file(link, self.ckpt_file)
             else:
                 self.ckpt_file = self.mw.configure.txtFilename.text()
 
-
             weights = self.ckpt_file
             res = int(self.mw.configure.cmbRes.currentText())
             self.iou_thres = 0.45
 
             self.device = select_device('')
             self.half = self.device.type != 'cpu'
 
@@ -154,30 +176,36 @@
                 torch.cuda.empty_cache()
 
             self.model = attempt_load(weights, map_location=self.device)
             self.stride = int(self.model.stride.max())
             if self.half:
                 self.model.half()
             self.names = self.model.module.names if hasattr(self.model, 'module') else self.model.names
+
             with torch.no_grad():
                 self.model(torch.zeros(1, 3, res, res).to(self.device).type_as(next(self.model.parameters())))
 
             self.track_thresh = self.mw.configure.sldConfThre.value()
             self.track_buffer = 30
             self.match_thresh = 0.8
 
             self.tracker = BYTETracker(self.track_thresh, self.track_buffer, self.match_thresh)
 
+            if self.mw.settingsPanel.chkShowWaitBox.isChecked():
+                self.mw.signals.hideWait.emit()
         except:
             logger.exception(MODULE_NAME + " initialization failure")
 
     def __call__(self, F):
         try:
             original_img = np.array(F, copy=False)
 
+            if self.mw.configure.name != MODULE_NAME:
+                return
+            
             res = int(self.mw.configure.cmbRes.currentText())
             img = letterbox(original_img, res, stride=self.stride)[0]
             img = img[:, :, ::-1].transpose(2, 0, 1)
             img = np.ascontiguousarray(img)
             img = torch.from_numpy(img).to(self.device)
             img = img.half() if self.half else img.float()
             img /= 255.0
@@ -217,16 +245,17 @@
                         label_counts[t.label] += 1
                         track_id = int(t.track_id)
                         id_text = '{}'.format(int(track_id)).zfill(5)
                         box_color = ((37 * track_id) % 255, (17 * track_id) % 255, (29 * track_id) % 255)
 
                         x, y, w, h = t.tlwh.astype(int)
                         cv2.rectangle(original_img, (x, y), (x+w, y+h), box_color, 2)
-                        label_color = self.mw.configure.getLabel(t.label).color()
-                        cv2.putText(original_img, id_text, (x, y), cv2.FONT_HERSHEY_PLAIN, 2, label_color, 2)
+                        if self.mw.configure.chkShowID.isChecked():
+                            label_color = self.mw.configure.getLabel(t.label).color()
+                            cv2.putText(original_img, id_text, (x, y), cv2.FONT_HERSHEY_PLAIN, 2, label_color, 2)
 
                 else:
                     for box in boxes:
                         x1, y1, x2, y2 = box[:4].astype(int)
                         cls = box[5].astype(int)
                         label_counts[cls] += 1
                         color = self.mw.configure.getLabel(cls).color()
@@ -245,17 +274,10 @@
 
         except Exception as ex:
             if self.last_ex != str(ex) and self.mw.configure.name == MODULE_NAME:
                 logger.exception(MODULE_NAME + " runtime error")
             self.last_ex = str(ex)
 
     def get_auto_ckpt_filename(self):
-        filename = None
-        if sys.platform == "win32":
-            filename = os.environ['HOMEPATH']
-        else:
-            filename = os.environ['HOME']
-
-        filename += "/.cache/torch/hub/checkpoints/" + self.mw.configure.cmbType.currentText() + ".pt"
-        return filename
+        return torch.hub.get_dir() +  "/checkpoints/" + self.mw.configure.cmbType.currentText() + ".pt"
```

### Comparing `onvif-gui-1.1.9/modules/video/yolov8.py` & `onvif-gui-1.2.0/modules/video/yolov8.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,17 +16,19 @@
 # limitations under the License.
 #
 #*********************************************************************/
 
 IMPORT_ERROR = ""
 try:
     import cv2
+    import sys
     import os
     import numpy as np
     from loguru import logger
+    from pathlib import Path
 
     from gui.components import ComboSelector, FileSelector, LabelSelector, ThresholdSlider
     from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QCheckBox, QMessageBox
     from PyQt6.QtCore import Qt
 
     import torch
     from ultralytics import YOLO
@@ -40,18 +42,20 @@
 MODULE_NAME = "yolov8"
 
 class VideoConfigure(QWidget):
     def __init__(self, mw):
         try:
             super().__init__()
             self.mw = mw
+            logger.add("errors.txt", retention="1 days")
             self.name = MODULE_NAME
             self.last_ex = ""
             self.autoKey = "Module/" + MODULE_NAME + "/autoDownload"
             self.trackKey = "Module/" + MODULE_NAME + "/track"
+            self.showIDKey = "Module/" + MODULE_NAME + "/showID"
 
             self.model_names = {"nano" : "yolov8n.pt", "small" : "yolov8s.pt", "medium" : "yolov8m.pt", "large" : "yolov8l.pt", "XL" : "yolov8x.pt"}
 
             self.chkAuto = QCheckBox("Automatically download model")
             self.chkAuto.setChecked(int(self.mw.settings.value(self.autoKey, 1)))
             self.chkAuto.stateChanged.connect(self.chkAutoClicked)
 
@@ -65,51 +69,63 @@
 
             self.sldConfThre = ThresholdSlider(mw, MODULE_NAME + "/confidence", "Confidence", 25)
 
             self.chkTrack = QCheckBox("Track Objects")
             self.chkTrack.setChecked(int(self.mw.settings.value(self.trackKey, 0)))
             self.chkTrack.stateChanged.connect(self.chkTrackClicked)
 
+            self.chkShowID = QCheckBox("Show Object ID")
+            self.chkShowID.setChecked(int(self.mw.settings.value(self.showIDKey, 1)))
+            self.chkShowID.stateChanged.connect(self.chkShowIDClicked)
+
+            if not self.chkTrack.isChecked():
+                self.chkShowID.setVisible(False)
+
             number_of_labels = 5
             self.labels = []
             for i in range(number_of_labels):
                 self.labels.append(LabelSelector(mw, MODULE_NAME, i+1))
             pnlLabels = QWidget()
             lytLabels = QGridLayout(pnlLabels)
             lblPanel = QLabel("Select classes to be identified")
             lblPanel.setAlignment(Qt.AlignmentFlag.AlignCenter)
             lytLabels.addWidget(lblPanel,        0, 0, 1, 1)
             for i in range(number_of_labels):
                 lytLabels.addWidget(self.labels[i], i+1, 0, 1, 1)
             lytLabels.setContentsMargins(0, 0, 0, 0)
 
             lytMain = QGridLayout(self)
-            lytMain.addWidget(self.chkAuto,      0, 0, 1, 1)
-            lytMain.addWidget(self.cmbModel,     1, 0, 1, 1)
-            lytMain.addWidget(self.txtModelFile, 2, 0, 1, 1)
-            lytMain.addWidget(self.cmbRes,       3, 0, 1, 1)
-            lytMain.addWidget(self.sldConfThre,  4, 0, 1, 1)
+            lytMain.addWidget(self.chkAuto,      0, 0, 1, 2)
+            lytMain.addWidget(self.cmbModel,     1, 0, 1, 2)
+            lytMain.addWidget(self.txtModelFile, 2, 0, 1, 2)
+            lytMain.addWidget(self.cmbRes,       3, 0, 1, 2)
+            lytMain.addWidget(self.sldConfThre,  4, 0, 1, 2)
             lytMain.addWidget(self.chkTrack,     5, 0, 1, 1)
-            lytMain.addWidget(pnlLabels,         6, 0, 1, 1)
-            lytMain.addWidget(QLabel(),          7, 0, 1, 1)
+            lytMain.addWidget(self.chkShowID,    5, 1, 1, 1)
+            lytMain.addWidget(pnlLabels,         6, 0, 1, 2)
+            lytMain.addWidget(QLabel(),          7, 0, 1, 2)
             lytMain.setRowStretch(7, 10)
 
             if len(IMPORT_ERROR) > 0:
                 QMessageBox.critical(None, MODULE_NAME + " Import Error", "Modules required for running this function are missing: " + IMPORT_ERROR)
 
         except:
             logger.exception(MODULE_NAME + " configure failed to load")
 
     def chkAutoClicked(self, state):
         self.mw.settings.setValue(self.autoKey, state)
         self.cmbModel.setEnabled(self.chkAuto.isChecked())
         self.txtModelFile.setEnabled(not self.chkAuto.isChecked())
 
-    def chkTrackClicked(self,state):
+    def chkTrackClicked(self, state):
         self.mw.settings.setValue(self.trackKey, state)
+        self.chkShowID.setVisible(state)
+
+    def chkShowIDClicked(self, state):
+        self.mw.settings.setValue(self.showIDKey, state)
 
     def getModelName(self):
         if self.chkAuto.isChecked():
             return self.model_names[self.cmbModel.currentText()]
         else:
             return self.txtModelFile.text()
         
@@ -119,30 +135,59 @@
                 return lbl
             
 class VideoWorker:
     def __init__(self, mw):
         try:
             self.mw = mw
             self.last_ex = ""
+
+            if self.mw.configure.name != MODULE_NAME:
+                return
+            
+            if self.mw.settingsPanel.chkShowWaitBox.isChecked():
+                self.mw.signals.showWait.emit()
+
+            self.ckpt_file = None
+            if self.mw.configure.chkAuto.isChecked():
+                self.ckpt_file = self.get_auto_ckpt_filename()
+                cache = Path(self.ckpt_file)
+
+                if not cache.is_file():
+                    cache.parent.mkdir(parents=True, exist_ok=True)
+                    model_name = self.mw.configure.getModelName()
+                    link = "https://github.com/ultralytics/assets/releases/download/v0.0.0/" + model_name
+                    if os.path.split(sys.executable)[1] == "pythonw.exe":
+                        torch.hub.download_url_to_file(link, self.ckpt_file, progress=False)
+                    else:
+                        torch.hub.download_url_to_file(link, self.ckpt_file)
+            else:
+                self.ckpt_file = self.configure.txtFilename.text()
+
             self.model_name = self.mw.configure.getModelName()
-            self.model = YOLO(self.model_name)
+            self.model = YOLO(Path(self.ckpt_file))
+            self.model.predict(np.zeros([1920, 1080, 3], dtype=np.uint8), stream=True, verbose=False)
 
             self.track_thresh = self.mw.configure.sldConfThre.value()
             self.track_buffer = 30
             self.match_thresh = 0.8
-
             self.tracker = BYTETracker(self.track_thresh, self.track_buffer, self.match_thresh)
 
+            if self.mw.settingsPanel.chkShowWaitBox.isChecked():
+                self.mw.signals.hideWait.emit()
+
         except:
             logger.exception(MODULE_NAME + " initialization failure")
 
     def __call__(self, F):
         try:
             img = np.array(F, copy=False)
 
+            if self.mw.configure.name != MODULE_NAME:
+                return
+            
             label_counts = {}
             label_filter = []
             for lbl in self.mw.configure.labels:
                 if lbl.chkBox.isChecked():
                     label_filter.append(lbl.label())
                     label_counts[lbl.label()] = 0
 
@@ -150,22 +195,23 @@
             if self.mw.configure.chkTrack.isChecked():
                 confthre = 0.001
 
             if self.model_name != self.mw.configure.getModelName():
                 self.model_name = self.mw.configure.getModelName()
                 with torch.no_grad():
                     torch.cuda.empty_cache()
-                self.model = YOLO(self.model_name)
+                self.__init__(self.mw)
 
             res = int(self.mw.configure.cmbRes.currentText())
                 
             results = self.model.predict(img, stream=True, verbose=False, 
                                          classes=label_filter,
                                          conf=confthre, 
                                          imgsz=res)
+
             for result in results:
                 if self.mw.configure.chkTrack.isChecked():
                     output = result.boxes.xyxy
                     scores = result.boxes.conf.reshape(-1, 1)
                     labels = result.boxes.cls.reshape(-1, 1)
                     output = torch.hstack((output, scores))
                     output = torch.hstack((output, labels))
@@ -182,16 +228,17 @@
 
                         track_id = int(t.track_id)
                         id_text = '{}'.format(int(track_id)).zfill(5)
                         box_color = ((37 * track_id) % 255, (17 * track_id) % 255, (29 * track_id) % 255)
 
                         x, y, w, h = t.tlwh.astype(int)
                         cv2.rectangle(img, (x, y), (x+w, y+h), box_color, 2)
-                        label_color = self.mw.configure.getLabel(t.label).color()
-                        cv2.putText(img, id_text, (x, y), cv2.FONT_HERSHEY_PLAIN, 2, label_color, 2)
+                        if self.mw.configure.chkShowID.isChecked():
+                            label_color = self.mw.configure.getLabel(t.label).color()
+                            cv2.putText(img, id_text, (x, y), cv2.FONT_HERSHEY_PLAIN, 2, label_color, 2)
                 else:
                     boxes = result.boxes.cpu().numpy()
                     for box in boxes:
                         r = box.xyxy[0].astype(int)
                         class_id = int(box.cls[0])
                         color = self.mw.configure.getLabel(class_id).color()
                         label_counts[class_id] += 1
@@ -200,7 +247,11 @@
                 for lbl in label_filter:
                     self.mw.configure.getLabel(lbl).setCount(label_counts[lbl])
             
         except Exception as ex:
             if self.last_ex != str(ex) and self.mw.configure.name == MODULE_NAME:
                 logger.exception(MODULE_NAME + " runtime error")
             self.last_ex = str(ex)
+
+    def get_auto_ckpt_filename(self):
+        return torch.hub.get_dir() +  "/checkpoints/" + self.mw.configure.getModelName()
+
```

### Comparing `onvif-gui-1.1.9/modules/video/yolox.py` & `onvif-gui-1.2.0/modules/video/yolox.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,37 +46,38 @@
 MODULE_NAME = "yolox"
 
 class VideoConfigure(QWidget):
     def __init__(self, mw):
         try:
             super().__init__()
             self.mw = mw
+            logger.add("errors.txt", retention="1 days")
             self.name = MODULE_NAME
             self.autoKey = "Module/" + MODULE_NAME + "/autoDownload"
-            #self.fp16Key = "Module/" + MODULE_NAME + "/fp16"
             self.trackKey = "Module/" + MODULE_NAME + "/track"
+            self.showIDKey = "Module/" + MODULE_NAME + "/showID"
 
             self.chkAuto = QCheckBox("Automatically download model")
             self.chkAuto.setChecked(int(self.mw.settings.value(self.autoKey, 1)))
             self.chkAuto.stateChanged.connect(self.chkAutoClicked)
 
             self.txtFilename = FileSelector(mw, MODULE_NAME)
             self.txtFilename.setEnabled(not self.chkAuto.isChecked())
 
             self.cmbRes = ComboSelector(mw, "Model Size", ("320", "480", "640", "960", "1280", "1440"), "640", MODULE_NAME)
             self.cmbType = ComboSelector(mw, "Model Name", ("yolox_s", "yolox_m", "yolox_l", "yolox_x"), "yolox_s", MODULE_NAME)
 
-            #self.chkFP16 = QCheckBox("Use half precision math")
-            #self.chkFP16.setChecked(int(self.mw.settings.value(self.fp16Key, 1)))
-            #self.chkFP16.stateChanged.connect(self.chkFP16Clicked)
-
             self.chkTrack = QCheckBox("Track Objects")
             self.chkTrack.setChecked(int(self.mw.settings.value(self.trackKey, 0)))
             self.chkTrack.stateChanged.connect(self.chkTrackClicked)
 
+            self.chkShowID = QCheckBox("Show Object ID")
+            self.chkShowID.setChecked(int(self.mw.settings.value(self.showIDKey, 1)))
+            self.chkShowID.stateChanged.connect(self.chkShowIDClicked)
+
             self.sldConfThre = ThresholdSlider(mw, MODULE_NAME + "/confidence", "Confidence", 25)
 
             number_of_labels = 5
             self.labels = []
             for i in range(number_of_labels):
                 self.labels.append(LabelSelector(mw, MODULE_NAME, i+1))
             pnlLabels = QWidget()
@@ -85,56 +86,59 @@
             lblPanel.setAlignment(Qt.AlignmentFlag.AlignCenter)
             lytLabels.addWidget(lblPanel,        0, 0, 1, 1)
             for i in range(number_of_labels):
                 lytLabels.addWidget(self.labels[i], i+1, 0, 1, 1)
             lytLabels.setContentsMargins(0, 0, 0, 0)
 
             lytMain = QGridLayout(self)
-            lytMain.addWidget(self.chkAuto,      0, 0, 1, 1)
-            lytMain.addWidget(self.cmbType,      1, 0, 1, 1)
-            lytMain.addWidget(self.txtFilename,  2, 0, 1, 1)
-            lytMain.addWidget(self.cmbRes,       3, 0, 1, 1)
-            lytMain.addWidget(self.sldConfThre,  4, 0, 1, 1)
-            #lytMain.addWidget(self.chkFP16,      5, 0, 1, 1)
+            lytMain.addWidget(self.chkAuto,      0, 0, 1, 2)
+            lytMain.addWidget(self.cmbType,      1, 0, 1, 2)
+            lytMain.addWidget(self.txtFilename,  2, 0, 1, 2)
+            lytMain.addWidget(self.cmbRes,       3, 0, 1, 2)
+            lytMain.addWidget(self.sldConfThre,  4, 0, 1, 2)
             lytMain.addWidget(self.chkTrack,     6, 0, 1, 1)
-            lytMain.addWidget(pnlLabels,         7, 0, 1, 1)
-            lytMain.addWidget(QLabel(),          8, 0, 1, 1)
+            lytMain.addWidget(self.chkShowID,    6, 1, 1, 1)
+            lytMain.addWidget(pnlLabels,         7, 0, 1, 2)
+            lytMain.addWidget(QLabel(),          8, 0, 1, 2)
             lytMain.setRowStretch(8, 10)
 
             if len(IMPORT_ERROR) > 0:
                 QMessageBox.critical(None, MODULE_NAME + " Import Error", "Modules required for running this function are missing: " + IMPORT_ERROR)
 
         except:
             logger.exception(MODULE_NAME + " configure failed to load")
 
     def chkAutoClicked(self, state):
         self.mw.settings.setValue(self.autoKey, state)
         self.txtFilename.setEnabled(not self.chkAuto.isChecked())
 
-    #def chkFP16Clicked(self, state):
-    #    self.mw.settings.setValue(self.fp16Key, state)
-
     def chkTrackClicked(self, state):
         self.mw.settings.setValue(self.trackKey, state)
 
+    def chkShowIDClicked(self, state):
+        self.mw.settings.setValue(self.showIDKey, state)
+
 class VideoWorker:
     def __init__(self, mw):
         try:
             self.mw = mw
             self.last_ex = ""
+
+            if self.mw.configure.name != MODULE_NAME:
+                return
+            
+            if self.mw.settingsPanel.chkShowWaitBox.isChecked():
+                self.mw.signals.showWait.emit()
             device_name = "cpu"
             if torch.cuda.is_available():
                 device_name = "cuda"
             self.device = torch.device(device_name)
 
             self.num_classes = 80
 
-            #self.fp16 = self.mw.configure.chkFP16.isChecked()
-            #self.track = self.mw.configure.chkTrack.isChecked()
-
             size = {'yolox_s': [0.33, 0.50], 
                     'yolox_m': [0.67, 0.75],
                     'yolox_l': [1.00, 1.00],
                     'yolox_x': [1.33, 1.25]}[self.mw.configure.cmbType.currentText()]
 
             self.model = None
             self.model = self.get_model(self.num_classes, size[0], size[1], None).to(self.device)
@@ -145,35 +149,43 @@
                 self.ckpt_file = self.get_auto_ckpt_filename()
                 cache = Path(self.ckpt_file)
 
                 if not cache.is_file():
                     cache.parent.mkdir(parents=True, exist_ok=True)
                     model_name = self.mw.configure.cmbType.currentText()
                     link = "https://github.com/Megvii-BaseDetection/YOLOX/releases/download/0.1.1rc0/" + model_name + ".pth"
-                    torch.hub.download_url_to_file(link, self.ckpt_file)
+                    if os.path.split(sys.executable)[1] == "pythonw.exe":
+                        torch.hub.download_url_to_file(link, self.ckpt_file, progress=False)
+                    else:
+                        torch.hub.download_url_to_file(link, self.ckpt_file)
             else:
                 self.ckpt_file = self.mw.configure.txtFilename.text()
 
             self.model.load_state_dict(torch.load(self.ckpt_file, map_location="cpu")["model"])
 
-            #if self.fp16:
-            #    self.model = self.model.half()
+            res = int(self.mw.configure.cmbRes.currentText())
+            self.model(torch.zeros(1, 3, res, res).to(self.device))
 
             self.track_thresh = self.mw.configure.sldConfThre.value()
             self.track_buffer = 30
             self.match_thresh = 0.8
-
             self.tracker = BYTETracker(self.track_thresh, self.track_buffer, self.match_thresh)
 
+            if self.mw.settingsPanel.chkShowWaitBox.isChecked():
+                self.mw.signals.hideWait.emit()
+
         except:
             logger.exception(MODULE_NAME + " initialization failure")
 
     def __call__(self, F):
         try:
             img = np.array(F, copy=False)
+
+            if self.mw.configure.name != MODULE_NAME:
+                return
             
             res = int(self.mw.configure.cmbRes.currentText())
             test_size = (res, res)
             ratio = min(test_size[0] / img.shape[0], test_size[1] / img.shape[1])
             inf_shape = (int(img.shape[0] * ratio), int(img.shape[1] * ratio))
             bottom = test_size[0] - inf_shape[0]
             side = test_size[1] - inf_shape[1]
@@ -181,17 +193,14 @@
 
             timg = functional.to_tensor(img.copy()).to(self.device)
             timg *= 255
             timg = functional.resize(timg, inf_shape)
             timg = functional.pad(timg, pad, 114)
             timg = timg.unsqueeze(0)
 
-            #if self.fp16:
-            #    timg = timg.half()  # to FP16
-
             if self.mw.configure.chkTrack.isChecked():
                 confthre = 0.001
             else:
                 confthre = self.mw.configure.sldConfThre.value()
             
             nmsthre = 0.65
 
@@ -260,30 +269,23 @@
             track_id = int(t.track_id)
             id_text = '{}'.format(int(track_id)).zfill(5)
             color = ((37 * track_id) % 255, (17 * track_id) % 255, (29 * track_id) % 255)
 
             tlwh = t.tlwh
             x, y, w, h = tlwh.astype(int)
             cv2.rectangle(img, (x, y), (x+w, y+h), color, 2)
-            cv2.putText(img, id_text, (x, y), cv2.FONT_HERSHEY_PLAIN, 2, label_colors[t.label], 2)
+            if self.mw.configure.chkShowID.isChecked():
+                cv2.putText(img, id_text, (x, y), cv2.FONT_HERSHEY_PLAIN, 2, label_colors[t.label], 2)
 
         for lbl in self.mw.configure.labels:
             if lbl.chkBox.isChecked():
                 lbl.setCount(count[lbl.label()])
 
-
     def get_auto_ckpt_filename(self):
-        filename = None
-        if sys.platform == "win32":
-            filename = os.environ['HOMEPATH']
-        else:
-            filename = os.environ['HOME']
-
-        filename += "/.cache/torch/hub/checkpoints/" + self.mw.configure.cmbType.currentText() + ".pth"
-        return filename
+        return torch.hub.get_dir() + "/checkpoints/" + self.mw.configure.cmbType.currentText() + ".pth"
 
     def get_model(self, num_classes, depth, width, act):
         def init_yolo(M):
             for m in M.modules():
                 if isinstance(m, nn.BatchNorm2d):
                     m.eps = 1e-3
                     m.momentum = 0.03
```

### Comparing `onvif-gui-1.1.9/onvif_gui.egg-info/PKG-INFO` & `onvif-gui-1.2.0/onvif_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-gui
-Version: 1.1.9
+Version: 1.2.0
 Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libonvif
 Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `onvif-gui-1.1.9/onvif_gui.egg-info/SOURCES.txt` & `onvif-gui-1.2.0/onvif_gui.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -132,14 +132,15 @@
 gui/components/__init__.py
 gui/components/comboselector.py
 gui/components/directoryselector.py
 gui/components/fileselector.py
 gui/components/labelselector.py
 gui/components/progress.py
 gui/components/thresholdslider.py
+gui/components/waitdialog.py
 gui/onvif/__init__.py
 gui/onvif/admintab.py
 gui/onvif/imagetab.py
 gui/onvif/logindialog.py
 gui/onvif/networktab.py
 gui/onvif/ptztab.py
 gui/onvif/videotab.py
@@ -206,14 +207,15 @@
 gui/resources/rewind_lo.png
 gui/resources/small_arrow_left.png
 gui/resources/small_arrow_left_hi.png
 gui/resources/small_arrow_left_lo.png
 gui/resources/small_arrow_up.png
 gui/resources/small_arrow_up_hi.png
 gui/resources/small_arrow_up_lo.png
+gui/resources/spinner.gif
 gui/resources/stop.png
 gui/resources/stop_hi.png
 gui/resources/stop_lo.png
 gui/resources/unchecked.png
 gui/resources/unchecked_hi.png
 gui/resources/unchecked_lo.png
 modules/__init__.py
```

### Comparing `onvif-gui-1.1.9/pyproject.toml` & `onvif-gui-1.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #*********************************************************************/
 
 [project]
 name = "onvif-gui" 
-version = "1.1.9"  
+version = "1.2.0"  
 description = "A client gui for Onvif"  
 readme = "README.md" 
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]  
 authors = [
   {name = "Stephen Rhodes", email = "sr99622@gmail.com" } 
@@ -32,19 +32,19 @@
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "Topic :: Software Development :: Build Tools",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3",
 ]
 
-dependencies = [ # Optional
+dependencies = [
   "libonvif", "avio", "pyqt6", "numpy", "loguru", "opencv-python"
 ]
 
-[project.urls]  # Optional
+[project.urls]  
 "Homepage" = "https://github.com/sr99622/libonvif"
 "Bug Reports" = "https://github.com/sr99622/libonvif/issues"
 
 [tool.setuptools]
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
```

### Comparing `onvif-gui-1.1.9/setup.py` & `onvif-gui-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from setuptools.command.install import install
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="onvif-gui",
-    version="1.1.9",
+    version="1.2.0",
     author="Stephen Rhodes",
     author_email="sr99622@gmail.com",
     description="GUI program for onvif",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

### Comparing `onvif-gui-1.1.9/tracker/basetrack.py` & `onvif-gui-1.2.0/tracker/basetrack.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/tracker/byte_tracker.py` & `onvif-gui-1.2.0/tracker/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/tracker/kalman_filter.py` & `onvif-gui-1.2.0/tracker/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/tracker/matching.py` & `onvif-gui-1.2.0/tracker/matching.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolov7/models/common.py` & `onvif-gui-1.2.0/yolov7/models/common.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolov7/models/experimental.py` & `onvif-gui-1.2.0/yolov7/models/experimental.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolov7/models/yolo.py` & `onvif-gui-1.2.0/yolov7/models/yolo.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolov7/utils/activations.py` & `onvif-gui-1.2.0/yolov7/utils/activations.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolov7/utils/add_nms.py` & `onvif-gui-1.2.0/yolov7/utils/add_nms.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolov7/utils/autoanchor.py` & `onvif-gui-1.2.0/yolov7/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolov7/utils/datasets.py` & `onvif-gui-1.2.0/yolov7/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolov7/utils/general.py` & `onvif-gui-1.2.0/yolov7/utils/general.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolov7/utils/google_utils.py` & `onvif-gui-1.2.0/yolov7/utils/google_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolov7/utils/loss.py` & `onvif-gui-1.2.0/yolov7/utils/loss.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolov7/utils/metrics.py` & `onvif-gui-1.2.0/yolov7/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolov7/utils/plots.py` & `onvif-gui-1.2.0/yolov7/utils/plots.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolov7/utils/torch_utils.py` & `onvif-gui-1.2.0/yolov7/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolox/models/__init__.py` & `onvif-gui-1.2.0/yolox/models/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolox/models/build.py` & `onvif-gui-1.2.0/yolox/models/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolox/models/darknet.py` & `onvif-gui-1.2.0/yolox/models/darknet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolox/models/losses.py` & `onvif-gui-1.2.0/yolox/models/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolox/models/network_blocks.py` & `onvif-gui-1.2.0/yolox/models/network_blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolox/models/yolo_fpn.py` & `onvif-gui-1.2.0/yolox/models/yolo_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolox/models/yolo_head.py` & `onvif-gui-1.2.0/yolox/models/yolo_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolox/models/yolo_pafpn.py` & `onvif-gui-1.2.0/yolox/models/yolo_pafpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolox/models/yolox.py` & `onvif-gui-1.2.0/yolox/models/yolox.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.9/yolox/utils/utils.py` & `onvif-gui-1.2.0/yolox/utils/utils.py`

 * *Files identical despite different names*

