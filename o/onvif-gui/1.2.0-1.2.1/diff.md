# Comparing `tmp/onvif-gui-1.2.0.tar.gz` & `tmp/onvif-gui-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-gui-1.2.0.tar", last modified: Tue May 30 02:27:41 2023, max compression
+gzip compressed data, was "onvif-gui-1.2.1.tar", last modified: Tue May 30 02:46:25 2023, max compression
```

## Comparing `onvif-gui-1.2.0.tar` & `onvif-gui-1.2.1.tar`

### file list

```diff
@@ -1,307 +1,307 @@
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11558 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/LICENSE
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      221 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/MANIFEST.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/PKG-INFO
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8359 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/README.md
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.363506 onvif-gui-1.2.0/detectron2/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       68 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.363506 onvif-gui-1.2.0/detectron2/checkpoint/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      357 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/checkpoint/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18177 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/checkpoint/c2_model_loading.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5800 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/checkpoint/catalog.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5379 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/checkpoint/detection_checkpoint.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.363506 onvif-gui-1.2.0/detectron2/config/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      623 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/config/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8119 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/config/compat.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9476 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/config/config.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    30158 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/config/defaults.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3103 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/config/instantiate.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15786 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/config/lazy.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.363506 onvif-gui-1.2.0/detectron2/configs/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1360 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/configs/Base-RCNN-FPN.yaml
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.367506 onvif-gui-1.2.0/detectron2/configs/COCO-InstanceSegmentation/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/configs/COCO-InstanceSegmentation/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      201 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.367506 onvif-gui-1.2.0/detectron2/configs/COCO-Keypoints/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      542 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/configs/COCO-Keypoints/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      190 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/configs/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x.yaml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/configs/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.367506 onvif-gui-1.2.0/detectron2/data/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      663 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7603 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/benchmark.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21787 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/build.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7460 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/catalog.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9406 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/common.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8360 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/dataset_mapper.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.367506 onvif-gui-1.2.0/detectron2/data/datasets/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      532 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10433 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/builtin.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    22191 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/builtin_meta.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13496 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/cityscapes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8008 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/cityscapes_panoptic.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    24004 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/coco.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9205 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/coco_panoptic.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9864 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/lvis.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)   223770 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/lvis_v0_5_categories.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)   219193 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/lvis_v1_categories.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    39434 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/lvis_v1_category_image_count.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3210 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/pascal_voc.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/datasets/register_coco.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    23487 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/detection_utils.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.367506 onvif-gui-1.2.0/detectron2/data/samplers/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      429 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/samplers/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12067 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/samplers/distributed_sampler.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1991 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/samplers/grouped_batch_sampler.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.367506 onvif-gui-1.2.0/detectron2/data/transforms/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      480 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/transforms/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14492 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/transforms/augmentation.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    23683 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/transforms/augmentation_impl.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12980 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/data/transforms/transform.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.367506 onvif-gui-1.2.0/detectron2/layers/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      900 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5908 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/aspp.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12431 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/batch_norm.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3135 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/blocks.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17492 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/deform_conv.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4335 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/losses.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11154 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/mask_ops.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6629 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/nms.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3172 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/roi_align.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3393 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/roi_align_rotated.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      673 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/rotated_boxes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      555 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/shape_spec.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5271 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/layers/wrappers.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.371506 onvif-gui-1.2.0/detectron2/modeling/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1632 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15825 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/anchor_generator.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.371506 onvif-gui-1.2.0/detectron2/modeling/backbone/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      618 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2586 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/backbone.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1048 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/build.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10628 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/fpn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    16434 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/mvit.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17108 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/regnet.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    24352 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/resnet.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    25785 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/swin.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6546 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/utils.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    19860 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/backbone/vit.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15492 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/box_regression.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6391 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/matcher.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.371506 onvif-gui-1.2.0/detectron2/modeling/meta_arch/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      524 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/meta_arch/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      839 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/meta_arch/build.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11940 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/meta_arch/dense_detector.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13541 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/meta_arch/fcos.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10676 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/meta_arch/panoptic_fpn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14237 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/meta_arch/rcnn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18704 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/meta_arch/retinanet.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10173 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/meta_arch/semantic_seg.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11104 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/mmdet_wrapper.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11575 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/poolers.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4145 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/postprocessing.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.371506 onvif-gui-1.2.0/detectron2/modeling/proposal_generator/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      236 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/proposal_generator/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      860 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/proposal_generator/build.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8333 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/proposal_generator/proposal_utils.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    24347 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/proposal_generator/rpn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9016 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/proposal_generator/rrpn.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.371506 onvif-gui-1.2.0/detectron2/modeling/roi_heads/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      797 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/roi_heads/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4195 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/roi_heads/box_head.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13289 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/roi_heads/cascade_rcnn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    25959 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/roi_heads/fast_rcnn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11428 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/roi_heads/keypoint_head.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12467 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/roi_heads/mask_head.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    38578 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/roi_heads/roi_heads.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11446 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2388 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/sampling.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12723 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/modeling/test_time_augmentation.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1829 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/predictor.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.371506 onvif-gui-1.2.0/detectron2/structures/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      662 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/structures/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14854 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/structures/boxes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5649 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/structures/image_list.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6807 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/structures/instances.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9269 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/structures/keypoints.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    20336 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/structures/masks.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    19356 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/structures/rotated_boxes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2775 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/tracker.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.375506 onvif-gui-1.2.0/detectron2/utils/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       52 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6205 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/analysis.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8633 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/collect_env.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4254 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/colormap.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5807 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/comm.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1911 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/develop.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5814 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/env.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17508 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/events.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1226 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/file_io.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8044 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/logger.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2667 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/memory.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1934 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/registry.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1096 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/serialize.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18576 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/testing.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11606 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/video_visualizer.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    52426 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/detectron2/utils/visualizer.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.375506 onvif-gui-1.2.0/gui/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       28 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.375506 onvif-gui-1.2.0/gui/components/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      286 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/gui/components/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1824 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/components/comboselector.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2459 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/components/directoryselector.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2172 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/components/fileselector.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5508 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/components/labelselector.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4194 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/components/progress.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1962 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/components/thresholdslider.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      831 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/gui/components/waitdialog.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2054 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/glwidget.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15800 2023-05-30 02:26:06.000000 onvif-gui-1.2.0/gui/main.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.375506 onvif-gui-1.2.0/gui/onvif/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      196 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/onvif/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5870 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/onvif/admintab.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4051 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/onvif/imagetab.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2484 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/onvif/logindialog.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5364 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/onvif/networktab.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5241 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/onvif/ptztab.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4640 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/onvif/videotab.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.375506 onvif-gui-1.2.0/gui/panels/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      184 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/panels/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3802 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/gui/panels/audiopanel.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13667 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/gui/panels/camerapanel.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14756 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/gui/panels/filepanel.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14115 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/gui/panels/settingspanel.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3806 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/gui/panels/videopanel.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.383506 onvif-gui-1.2.0/gui/resources/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2021 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/LICENSE
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      252 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/apply.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      245 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/apply_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      244 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/apply_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      911 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/audio.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      536 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/audio_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      920 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/audio_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      203 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/branch_closed.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      219 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/branch_closed_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      211 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/branch_closed_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      199 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/branch_open.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      168 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/branch_open_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/branch_open_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      267 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/checked.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      235 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/checked_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      246 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/checked_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13358 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/gui/resources/darkstyle.qss
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      910 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/discover.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      849 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/discover_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      937 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/discover_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      425 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/fast-forward.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      253 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/fast-forward_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      433 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/fast-forward_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      641 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/mute.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      346 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/mute_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      618 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/mute_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      347 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/next.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      225 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/next_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      348 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/next_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    46084 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/onvif-gui.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/pause.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      144 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/pause_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      149 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/pause_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      321 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/play.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      209 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/play_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      316 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/play_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      349 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/previous.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      232 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/previous_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      348 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/previous_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      324 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/radio-off.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      250 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/radio-off_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      324 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/radio-off_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      350 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/radio-on.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      263 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/radio-on_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      343 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/radio-on_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      395 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/record.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      394 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/record_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      425 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/record_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      408 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/recording.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      435 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/recording_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      532 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/recording_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      454 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/rewind.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      250 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/rewind_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      457 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/rewind_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      187 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/small_arrow_left.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      183 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/small_arrow_left_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      189 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/small_arrow_left_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      162 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/small_arrow_up.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      160 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/small_arrow_up_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      161 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/small_arrow_up_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    19236 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/gui/resources/spinner.gif
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      158 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/stop.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      140 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/stop_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      151 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/stop_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      143 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/unchecked.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      142 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/unchecked_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      143 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/gui/resources/unchecked_lo.png
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.383506 onvif-gui-1.2.0/modules/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/modules/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.383506 onvif-gui-1.2.0/modules/audio/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/modules/audio/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3492 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/modules/audio/sample.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/modules/video/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/modules/video/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7756 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/modules/video/keypoint.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5390 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/modules/video/retinanet.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3234 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/modules/video/sample.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8278 2023-05-30 01:46:34.000000 onvif-gui-1.2.0/modules/video/segment.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12058 2023-05-30 02:16:29.000000 onvif-gui-1.2.0/modules/video/yolov7.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11322 2023-05-30 02:16:20.000000 onvif-gui-1.2.0/modules/video/yolov8.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12641 2023-05-30 02:13:23.000000 onvif-gui-1.2.0/modules/video/yolox.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/onvif_gui.egg-info/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-30 02:27:41.000000 onvif-gui-1.2.0/onvif_gui.egg-info/PKG-INFO
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8447 2023-05-30 02:27:41.000000 onvif-gui-1.2.0/onvif_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-05-30 02:27:41.000000 onvif-gui-1.2.0/onvif_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       39 2023-05-30 02:27:41.000000 onvif-gui-1.2.0/onvif_gui.egg-info/entry_points.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       47 2023-05-30 02:27:41.000000 onvif-gui-1.2.0/onvif_gui.egg-info/requires.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       44 2023-05-30 02:27:41.000000 onvif-gui-1.2.0/onvif_gui.egg-info/top_level.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1688 2023-05-30 02:25:31.000000 onvif-gui-1.2.0/pyproject.toml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       38 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/setup.cfg
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1549 2023-05-30 02:25:19.000000 onvif-gui-1.2.0/setup.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/tracker/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/tracker/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1003 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/tracker/basetrack.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12632 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/tracker/byte_tracker.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9816 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/tracker/kalman_filter.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6304 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/tracker/matching.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/yolov7/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/yolov7/models/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        6 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/models/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    86435 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/models/common.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11177 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/models/experimental.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    40895 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/models/yolo.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/yolov7/utils/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        6 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2320 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/activations.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5771 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/add_nms.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7321 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/autoanchor.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    57559 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/datasets.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    37789 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/general.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4996 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/google_utils.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    76741 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/loss.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9537 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/metrics.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21424 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/plots.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15840 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolov7/utils/torch_utils.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/yolox/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/yolox/models/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      961 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/models/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5019 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/models/build.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6840 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/models/darknet.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2372 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/models/losses.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6944 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/models/network_blocks.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3202 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/models/yolo_fpn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    26204 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/models/yolo_head.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4288 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/models/yolo_pafpn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2054 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/models/yolox.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:27:41.387506 onvif-gui-1.2.0/yolox/utils/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      130 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/utils/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1628 2023-05-25 17:26:34.000000 onvif-gui-1.2.0/yolox/utils/utils.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.150022 onvif-gui-1.2.1/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11558 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/LICENSE
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      221 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/MANIFEST.in
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-30 02:46:25.150022 onvif-gui-1.2.1/PKG-INFO
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8359 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/README.md
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.126022 onvif-gui-1.2.1/detectron2/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       68 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.126022 onvif-gui-1.2.1/detectron2/checkpoint/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      357 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/checkpoint/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18177 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/checkpoint/c2_model_loading.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5800 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/checkpoint/catalog.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5379 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/checkpoint/detection_checkpoint.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.130022 onvif-gui-1.2.1/detectron2/config/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      623 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/config/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8119 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/config/compat.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9476 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/config/config.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    30158 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/config/defaults.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3103 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/config/instantiate.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15786 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/config/lazy.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.130022 onvif-gui-1.2.1/detectron2/configs/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1360 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/configs/Base-RCNN-FPN.yaml
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.130022 onvif-gui-1.2.1/detectron2/configs/COCO-InstanceSegmentation/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/configs/COCO-InstanceSegmentation/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      201 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.130022 onvif-gui-1.2.1/detectron2/configs/COCO-Keypoints/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      542 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/configs/COCO-Keypoints/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      190 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/configs/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x.yaml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/configs/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.130022 onvif-gui-1.2.1/detectron2/data/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      663 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7603 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/benchmark.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21787 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7460 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/catalog.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9406 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/common.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8360 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/dataset_mapper.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.130022 onvif-gui-1.2.1/detectron2/data/datasets/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      532 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/datasets/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10433 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/datasets/builtin.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    22191 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/datasets/builtin_meta.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13496 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/datasets/cityscapes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8008 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/datasets/cityscapes_panoptic.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    24004 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/datasets/coco.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9205 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/datasets/coco_panoptic.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9864 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/datasets/lvis.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)   223770 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/datasets/lvis_v0_5_categories.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)   219193 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/datasets/lvis_v1_categories.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    39434 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/datasets/lvis_v1_category_image_count.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3210 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/datasets/pascal_voc.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/datasets/register_coco.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23487 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/detection_utils.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.130022 onvif-gui-1.2.1/detectron2/data/samplers/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      429 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/samplers/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12067 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/samplers/distributed_sampler.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1991 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/samplers/grouped_batch_sampler.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.130022 onvif-gui-1.2.1/detectron2/data/transforms/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      480 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/transforms/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14492 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/transforms/augmentation.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23683 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/transforms/augmentation_impl.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12980 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/data/transforms/transform.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.134022 onvif-gui-1.2.1/detectron2/layers/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      900 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/layers/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5908 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/layers/aspp.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12431 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/layers/batch_norm.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3135 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/layers/blocks.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17492 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/layers/deform_conv.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4335 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/layers/losses.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11154 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/layers/mask_ops.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6629 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/layers/nms.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3172 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/layers/roi_align.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3393 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/layers/roi_align_rotated.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      673 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/layers/rotated_boxes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      555 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/layers/shape_spec.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5271 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/layers/wrappers.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.134022 onvif-gui-1.2.1/detectron2/modeling/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1632 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15825 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/anchor_generator.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.134022 onvif-gui-1.2.1/detectron2/modeling/backbone/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      618 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/backbone/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2586 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/backbone/backbone.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1048 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/backbone/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10628 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/backbone/fpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    16434 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/backbone/mvit.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17108 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/backbone/regnet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    24352 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/backbone/resnet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    25785 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/backbone/swin.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6546 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/backbone/utils.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    19860 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/backbone/vit.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15492 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/box_regression.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6391 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/matcher.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.134022 onvif-gui-1.2.1/detectron2/modeling/meta_arch/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      524 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/meta_arch/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      839 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/meta_arch/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11940 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/meta_arch/dense_detector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13541 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/meta_arch/fcos.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10676 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/meta_arch/panoptic_fpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14237 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/meta_arch/rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18704 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/meta_arch/retinanet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10173 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/meta_arch/semantic_seg.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11104 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/mmdet_wrapper.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11575 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/poolers.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4145 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/postprocessing.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.134022 onvif-gui-1.2.1/detectron2/modeling/proposal_generator/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      236 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/proposal_generator/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      860 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/proposal_generator/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8333 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/proposal_generator/proposal_utils.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    24347 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/proposal_generator/rpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9016 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/proposal_generator/rrpn.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.134022 onvif-gui-1.2.1/detectron2/modeling/roi_heads/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      797 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/roi_heads/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4195 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/roi_heads/box_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13289 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/roi_heads/cascade_rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    25959 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/roi_heads/fast_rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11428 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/roi_heads/keypoint_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12467 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/roi_heads/mask_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    38578 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/roi_heads/roi_heads.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11446 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2388 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/sampling.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12723 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/modeling/test_time_augmentation.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1829 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/predictor.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.138022 onvif-gui-1.2.1/detectron2/structures/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      662 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/structures/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14854 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/structures/boxes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5649 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/structures/image_list.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6807 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/structures/instances.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9269 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/structures/keypoints.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    20336 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/structures/masks.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    19356 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/structures/rotated_boxes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2775 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/tracker.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.138022 onvif-gui-1.2.1/detectron2/utils/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       52 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/utils/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6205 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/utils/analysis.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8633 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/utils/collect_env.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4254 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/utils/colormap.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5807 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/utils/comm.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1911 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/utils/develop.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5814 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/utils/env.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17508 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/utils/events.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1226 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/utils/file_io.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8044 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/utils/logger.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2667 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/utils/memory.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1934 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/utils/registry.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1096 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/utils/serialize.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18576 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/utils/testing.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11606 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/utils/video_visualizer.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    52426 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/detectron2/utils/visualizer.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.138022 onvif-gui-1.2.1/gui/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       28 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.138022 onvif-gui-1.2.1/gui/components/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      286 2023-05-30 01:46:34.000000 onvif-gui-1.2.1/gui/components/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1824 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/components/comboselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2459 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/components/directoryselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2172 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/components/fileselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5508 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/components/labelselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4194 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/components/progress.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1962 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/components/thresholdslider.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      831 2023-05-30 01:46:34.000000 onvif-gui-1.2.1/gui/components/waitdialog.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2054 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/glwidget.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15800 2023-05-30 02:43:53.000000 onvif-gui-1.2.1/gui/main.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.138022 onvif-gui-1.2.1/gui/onvif/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      196 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/onvif/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5870 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/onvif/admintab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4051 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/onvif/imagetab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2484 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/onvif/logindialog.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5364 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/onvif/networktab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5241 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/onvif/ptztab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4640 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/onvif/videotab.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.138022 onvif-gui-1.2.1/gui/panels/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      184 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/panels/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3802 2023-05-30 01:46:34.000000 onvif-gui-1.2.1/gui/panels/audiopanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13667 2023-05-30 01:46:34.000000 onvif-gui-1.2.1/gui/panels/camerapanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14756 2023-05-30 01:46:34.000000 onvif-gui-1.2.1/gui/panels/filepanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14115 2023-05-30 01:46:34.000000 onvif-gui-1.2.1/gui/panels/settingspanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3806 2023-05-30 01:46:34.000000 onvif-gui-1.2.1/gui/panels/videopanel.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.146022 onvif-gui-1.2.1/gui/resources/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2021 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/LICENSE
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      252 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/apply.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      245 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/apply_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      244 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/apply_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      911 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/audio.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      536 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/audio_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      920 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/audio_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      203 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/branch_closed.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      219 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/branch_closed_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      211 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/branch_closed_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      199 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/branch_open.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      168 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/branch_open_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/branch_open_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      267 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/checked.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      235 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/checked_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      246 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/checked_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13358 2023-05-30 01:46:34.000000 onvif-gui-1.2.1/gui/resources/darkstyle.qss
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      910 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/discover.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      849 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/discover_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      937 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/discover_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      425 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/fast-forward.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      253 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/fast-forward_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      433 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/fast-forward_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      641 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/mute.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      346 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/mute_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      618 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/mute_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      347 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/next.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      225 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/next_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      348 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/next_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    46084 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/onvif-gui.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/pause.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      144 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/pause_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      149 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/pause_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      321 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/play.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      209 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/play_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      316 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/play_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      349 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/previous.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      232 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/previous_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      348 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/previous_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      324 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/radio-off.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      250 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/radio-off_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      324 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/radio-off_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      350 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/radio-on.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      263 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/radio-on_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      343 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/radio-on_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      395 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/record.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      394 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/record_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      425 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/record_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      408 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/recording.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      435 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/recording_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      532 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/recording_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      454 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/rewind.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      250 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/rewind_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      457 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/rewind_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      187 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/small_arrow_left.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      183 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/small_arrow_left_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      189 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/small_arrow_left_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      162 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/small_arrow_up.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      160 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/small_arrow_up_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      161 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/small_arrow_up_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    19236 2023-05-30 01:46:34.000000 onvif-gui-1.2.1/gui/resources/spinner.gif
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      158 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/stop.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      140 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/stop_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      151 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/stop_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      143 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/unchecked.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      142 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/unchecked_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      143 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/gui/resources/unchecked_lo.png
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.146022 onvif-gui-1.2.1/modules/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/modules/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.146022 onvif-gui-1.2.1/modules/audio/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/modules/audio/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3492 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/modules/audio/sample.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.146022 onvif-gui-1.2.1/modules/video/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/modules/video/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7967 2023-05-30 02:38:07.000000 onvif-gui-1.2.1/modules/video/keypoint.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5615 2023-05-30 02:39:35.000000 onvif-gui-1.2.1/modules/video/retinanet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3234 2023-05-30 01:46:34.000000 onvif-gui-1.2.1/modules/video/sample.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8489 2023-05-30 02:40:35.000000 onvif-gui-1.2.1/modules/video/segment.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12083 2023-05-30 02:35:32.000000 onvif-gui-1.2.1/modules/video/yolov7.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11347 2023-05-30 02:35:21.000000 onvif-gui-1.2.1/modules/video/yolov8.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12666 2023-05-30 02:32:57.000000 onvif-gui-1.2.1/modules/video/yolox.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.146022 onvif-gui-1.2.1/onvif_gui.egg-info/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-30 02:46:25.000000 onvif-gui-1.2.1/onvif_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8447 2023-05-30 02:46:25.000000 onvif-gui-1.2.1/onvif_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-05-30 02:46:25.000000 onvif-gui-1.2.1/onvif_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       39 2023-05-30 02:46:25.000000 onvif-gui-1.2.1/onvif_gui.egg-info/entry_points.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       47 2023-05-30 02:46:25.000000 onvif-gui-1.2.1/onvif_gui.egg-info/requires.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       44 2023-05-30 02:46:25.000000 onvif-gui-1.2.1/onvif_gui.egg-info/top_level.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1688 2023-05-30 02:43:48.000000 onvif-gui-1.2.1/pyproject.toml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       38 2023-05-30 02:46:25.150022 onvif-gui-1.2.1/setup.cfg
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1549 2023-05-30 02:43:40.000000 onvif-gui-1.2.1/setup.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.146022 onvif-gui-1.2.1/tracker/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/tracker/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1003 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/tracker/basetrack.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12632 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/tracker/byte_tracker.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9816 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/tracker/kalman_filter.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6304 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/tracker/matching.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.146022 onvif-gui-1.2.1/yolov7/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolov7/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.146022 onvif-gui-1.2.1/yolov7/models/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        6 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolov7/models/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    86435 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolov7/models/common.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11177 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolov7/models/experimental.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    40895 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolov7/models/yolo.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.146022 onvif-gui-1.2.1/yolov7/utils/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        6 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolov7/utils/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2320 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolov7/utils/activations.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5771 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolov7/utils/add_nms.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7321 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolov7/utils/autoanchor.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    57559 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolov7/utils/datasets.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    37789 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolov7/utils/general.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4996 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolov7/utils/google_utils.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    76741 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolov7/utils/loss.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9537 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolov7/utils/metrics.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21424 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolov7/utils/plots.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15840 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolov7/utils/torch_utils.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.146022 onvif-gui-1.2.1/yolox/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolox/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.150022 onvif-gui-1.2.1/yolox/models/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      961 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolox/models/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5019 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolox/models/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6840 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolox/models/darknet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2372 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolox/models/losses.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6944 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolox/models/network_blocks.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3202 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolox/models/yolo_fpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    26204 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolox/models/yolo_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4288 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolox/models/yolo_pafpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2054 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolox/models/yolox.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 02:46:25.150022 onvif-gui-1.2.1/yolox/utils/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      130 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolox/utils/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1628 2023-05-25 17:26:34.000000 onvif-gui-1.2.1/yolox/utils/utils.py
```

### Comparing `onvif-gui-1.2.0/LICENSE` & `onvif-gui-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/PKG-INFO` & `onvif-gui-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-gui
-Version: 1.2.0
+Version: 1.2.1
 Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libonvif
 Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `onvif-gui-1.2.0/README.md` & `onvif-gui-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/checkpoint/c2_model_loading.py` & `onvif-gui-1.2.1/detectron2/checkpoint/c2_model_loading.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/checkpoint/catalog.py` & `onvif-gui-1.2.1/detectron2/checkpoint/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/checkpoint/detection_checkpoint.py` & `onvif-gui-1.2.1/detectron2/checkpoint/detection_checkpoint.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/config/__init__.py` & `onvif-gui-1.2.1/detectron2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/config/compat.py` & `onvif-gui-1.2.1/detectron2/config/compat.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/config/config.py` & `onvif-gui-1.2.1/detectron2/config/config.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/config/defaults.py` & `onvif-gui-1.2.1/detectron2/config/defaults.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/config/instantiate.py` & `onvif-gui-1.2.1/detectron2/config/instantiate.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/config/lazy.py` & `onvif-gui-1.2.1/detectron2/config/lazy.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/configs/Base-RCNN-FPN.yaml` & `onvif-gui-1.2.1/detectron2/configs/Base-RCNN-FPN.yaml`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml` & `onvif-gui-1.2.1/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/__init__.py` & `onvif-gui-1.2.1/detectron2/data/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/benchmark.py` & `onvif-gui-1.2.1/detectron2/data/benchmark.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/build.py` & `onvif-gui-1.2.1/detectron2/data/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/catalog.py` & `onvif-gui-1.2.1/detectron2/data/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/common.py` & `onvif-gui-1.2.1/detectron2/data/common.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/dataset_mapper.py` & `onvif-gui-1.2.1/detectron2/data/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/datasets/__init__.py` & `onvif-gui-1.2.1/detectron2/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/datasets/builtin.py` & `onvif-gui-1.2.1/detectron2/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/datasets/builtin_meta.py` & `onvif-gui-1.2.1/detectron2/data/datasets/builtin_meta.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/datasets/cityscapes.py` & `onvif-gui-1.2.1/detectron2/data/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/datasets/cityscapes_panoptic.py` & `onvif-gui-1.2.1/detectron2/data/datasets/cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/datasets/coco.py` & `onvif-gui-1.2.1/detectron2/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/datasets/coco_panoptic.py` & `onvif-gui-1.2.1/detectron2/data/datasets/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/datasets/lvis.py` & `onvif-gui-1.2.1/detectron2/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/datasets/lvis_v0_5_categories.py` & `onvif-gui-1.2.1/detectron2/data/datasets/lvis_v0_5_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/datasets/lvis_v1_categories.py` & `onvif-gui-1.2.1/detectron2/data/datasets/lvis_v1_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/datasets/lvis_v1_category_image_count.py` & `onvif-gui-1.2.1/detectron2/data/datasets/lvis_v1_category_image_count.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/datasets/pascal_voc.py` & `onvif-gui-1.2.1/detectron2/data/datasets/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/detection_utils.py` & `onvif-gui-1.2.1/detectron2/data/detection_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/samplers/distributed_sampler.py` & `onvif-gui-1.2.1/detectron2/data/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/samplers/grouped_batch_sampler.py` & `onvif-gui-1.2.1/detectron2/data/samplers/grouped_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/transforms/augmentation.py` & `onvif-gui-1.2.1/detectron2/data/transforms/augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/transforms/augmentation_impl.py` & `onvif-gui-1.2.1/detectron2/data/transforms/augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/data/transforms/transform.py` & `onvif-gui-1.2.1/detectron2/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/layers/__init__.py` & `onvif-gui-1.2.1/detectron2/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/layers/aspp.py` & `onvif-gui-1.2.1/detectron2/layers/aspp.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/layers/batch_norm.py` & `onvif-gui-1.2.1/detectron2/layers/batch_norm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/layers/blocks.py` & `onvif-gui-1.2.1/detectron2/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/layers/deform_conv.py` & `onvif-gui-1.2.1/detectron2/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/layers/losses.py` & `onvif-gui-1.2.1/detectron2/layers/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/layers/mask_ops.py` & `onvif-gui-1.2.1/detectron2/layers/mask_ops.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/layers/nms.py` & `onvif-gui-1.2.1/detectron2/layers/nms.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/layers/roi_align.py` & `onvif-gui-1.2.1/detectron2/layers/roi_align.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/layers/roi_align_rotated.py` & `onvif-gui-1.2.1/detectron2/layers/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/layers/rotated_boxes.py` & `onvif-gui-1.2.1/detectron2/layers/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/layers/shape_spec.py` & `onvif-gui-1.2.1/detectron2/layers/shape_spec.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/layers/wrappers.py` & `onvif-gui-1.2.1/detectron2/layers/wrappers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/__init__.py` & `onvif-gui-1.2.1/detectron2/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/anchor_generator.py` & `onvif-gui-1.2.1/detectron2/modeling/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/backbone/__init__.py` & `onvif-gui-1.2.1/detectron2/modeling/backbone/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/backbone/backbone.py` & `onvif-gui-1.2.1/detectron2/modeling/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/backbone/build.py` & `onvif-gui-1.2.1/detectron2/modeling/backbone/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/backbone/fpn.py` & `onvif-gui-1.2.1/detectron2/modeling/backbone/fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/backbone/mvit.py` & `onvif-gui-1.2.1/detectron2/modeling/backbone/mvit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/backbone/regnet.py` & `onvif-gui-1.2.1/detectron2/modeling/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/backbone/resnet.py` & `onvif-gui-1.2.1/detectron2/modeling/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/backbone/swin.py` & `onvif-gui-1.2.1/detectron2/modeling/backbone/swin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/backbone/utils.py` & `onvif-gui-1.2.1/detectron2/modeling/backbone/utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/backbone/vit.py` & `onvif-gui-1.2.1/detectron2/modeling/backbone/vit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/box_regression.py` & `onvif-gui-1.2.1/detectron2/modeling/box_regression.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/matcher.py` & `onvif-gui-1.2.1/detectron2/modeling/matcher.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/meta_arch/__init__.py` & `onvif-gui-1.2.1/detectron2/modeling/meta_arch/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/meta_arch/build.py` & `onvif-gui-1.2.1/detectron2/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/meta_arch/dense_detector.py` & `onvif-gui-1.2.1/detectron2/modeling/meta_arch/dense_detector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/meta_arch/fcos.py` & `onvif-gui-1.2.1/detectron2/modeling/meta_arch/fcos.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/meta_arch/panoptic_fpn.py` & `onvif-gui-1.2.1/detectron2/modeling/meta_arch/panoptic_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/meta_arch/rcnn.py` & `onvif-gui-1.2.1/detectron2/modeling/meta_arch/rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/meta_arch/retinanet.py` & `onvif-gui-1.2.1/detectron2/modeling/meta_arch/retinanet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/meta_arch/semantic_seg.py` & `onvif-gui-1.2.1/detectron2/modeling/meta_arch/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/mmdet_wrapper.py` & `onvif-gui-1.2.1/detectron2/modeling/mmdet_wrapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/poolers.py` & `onvif-gui-1.2.1/detectron2/modeling/poolers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/postprocessing.py` & `onvif-gui-1.2.1/detectron2/modeling/postprocessing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/proposal_generator/build.py` & `onvif-gui-1.2.1/detectron2/modeling/proposal_generator/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/proposal_generator/proposal_utils.py` & `onvif-gui-1.2.1/detectron2/modeling/proposal_generator/proposal_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/proposal_generator/rpn.py` & `onvif-gui-1.2.1/detectron2/modeling/proposal_generator/rpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/proposal_generator/rrpn.py` & `onvif-gui-1.2.1/detectron2/modeling/proposal_generator/rrpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/roi_heads/__init__.py` & `onvif-gui-1.2.1/detectron2/modeling/roi_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/roi_heads/box_head.py` & `onvif-gui-1.2.1/detectron2/modeling/roi_heads/box_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/roi_heads/cascade_rcnn.py` & `onvif-gui-1.2.1/detectron2/modeling/roi_heads/cascade_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/roi_heads/fast_rcnn.py` & `onvif-gui-1.2.1/detectron2/modeling/roi_heads/fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/roi_heads/keypoint_head.py` & `onvif-gui-1.2.1/detectron2/modeling/roi_heads/keypoint_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/roi_heads/mask_head.py` & `onvif-gui-1.2.1/detectron2/modeling/roi_heads/mask_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/roi_heads/roi_heads.py` & `onvif-gui-1.2.1/detectron2/modeling/roi_heads/roi_heads.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/roi_heads/rotated_fast_rcnn.py` & `onvif-gui-1.2.1/detectron2/modeling/roi_heads/rotated_fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/sampling.py` & `onvif-gui-1.2.1/detectron2/modeling/sampling.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/modeling/test_time_augmentation.py` & `onvif-gui-1.2.1/detectron2/modeling/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/predictor.py` & `onvif-gui-1.2.1/detectron2/predictor.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/structures/__init__.py` & `onvif-gui-1.2.1/detectron2/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/structures/boxes.py` & `onvif-gui-1.2.1/detectron2/structures/boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/structures/image_list.py` & `onvif-gui-1.2.1/detectron2/structures/image_list.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/structures/instances.py` & `onvif-gui-1.2.1/detectron2/structures/instances.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/structures/keypoints.py` & `onvif-gui-1.2.1/detectron2/structures/keypoints.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/structures/masks.py` & `onvif-gui-1.2.1/detectron2/structures/masks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/structures/rotated_boxes.py` & `onvif-gui-1.2.1/detectron2/structures/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/tracker.py` & `onvif-gui-1.2.1/detectron2/tracker.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/utils/analysis.py` & `onvif-gui-1.2.1/detectron2/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/utils/collect_env.py` & `onvif-gui-1.2.1/detectron2/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/utils/colormap.py` & `onvif-gui-1.2.1/detectron2/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/utils/comm.py` & `onvif-gui-1.2.1/detectron2/utils/comm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/utils/develop.py` & `onvif-gui-1.2.1/detectron2/utils/develop.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/utils/env.py` & `onvif-gui-1.2.1/detectron2/utils/env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/utils/events.py` & `onvif-gui-1.2.1/detectron2/utils/events.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/utils/file_io.py` & `onvif-gui-1.2.1/detectron2/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/utils/logger.py` & `onvif-gui-1.2.1/detectron2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/utils/memory.py` & `onvif-gui-1.2.1/detectron2/utils/memory.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/utils/registry.py` & `onvif-gui-1.2.1/detectron2/utils/registry.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/utils/serialize.py` & `onvif-gui-1.2.1/detectron2/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/utils/testing.py` & `onvif-gui-1.2.1/detectron2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/utils/video_visualizer.py` & `onvif-gui-1.2.1/detectron2/utils/video_visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/detectron2/utils/visualizer.py` & `onvif-gui-1.2.1/detectron2/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/components/comboselector.py` & `onvif-gui-1.2.1/gui/components/comboselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/components/directoryselector.py` & `onvif-gui-1.2.1/gui/components/directoryselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/components/fileselector.py` & `onvif-gui-1.2.1/gui/components/fileselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/components/labelselector.py` & `onvif-gui-1.2.1/gui/components/labelselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/components/progress.py` & `onvif-gui-1.2.1/gui/components/progress.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/components/thresholdslider.py` & `onvif-gui-1.2.1/gui/components/thresholdslider.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/components/waitdialog.py` & `onvif-gui-1.2.1/gui/components/waitdialog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/glwidget.py` & `onvif-gui-1.2.1/gui/glwidget.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/main.py` & `onvif-gui-1.2.1/gui/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 class MainWindow(QMainWindow):
     def __init__(self, clear_settings=False):
         super().__init__()
         os.environ["QT_FILESYSTEMMODEL_WATCH_FILES"] = "ON"
         QDir.addSearchPath("image", self.getLocation() + "/gui/resources/")
         self.style()
 
-        self.program_name = "onvif gui version 1.2.0"
+        self.program_name = "onvif gui version 1.2.1"
         self.setWindowTitle(self.program_name)
         self.setWindowIcon(QIcon('image:onvif-gui.png'))
         self.settings = QSettings("onvif", "gui")
         if clear_settings:
             self.settings.clear()
         self.volumeKey = "MainWindow/volume"
         self.muteKey = "MainWindow/mute"
```

### Comparing `onvif-gui-1.2.0/gui/onvif/admintab.py` & `onvif-gui-1.2.1/gui/onvif/admintab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/onvif/imagetab.py` & `onvif-gui-1.2.1/gui/onvif/imagetab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/onvif/logindialog.py` & `onvif-gui-1.2.1/gui/onvif/logindialog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/onvif/networktab.py` & `onvif-gui-1.2.1/gui/onvif/networktab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/onvif/ptztab.py` & `onvif-gui-1.2.1/gui/onvif/ptztab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/onvif/videotab.py` & `onvif-gui-1.2.1/gui/onvif/videotab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/panels/audiopanel.py` & `onvif-gui-1.2.1/gui/panels/audiopanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/panels/camerapanel.py` & `onvif-gui-1.2.1/gui/panels/camerapanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/panels/filepanel.py` & `onvif-gui-1.2.1/gui/panels/filepanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/panels/settingspanel.py` & `onvif-gui-1.2.1/gui/panels/settingspanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/panels/videopanel.py` & `onvif-gui-1.2.1/gui/panels/videopanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/resources/LICENSE` & `onvif-gui-1.2.1/gui/resources/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/resources/audio.png` & `onvif-gui-1.2.1/gui/resources/audio.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/resources/audio_hi.png` & `onvif-gui-1.2.1/gui/resources/audio_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/resources/audio_lo.png` & `onvif-gui-1.2.1/gui/resources/audio_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/resources/darkstyle.qss` & `onvif-gui-1.2.1/gui/resources/darkstyle.qss`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/resources/discover.png` & `onvif-gui-1.2.1/gui/resources/discover.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/resources/discover_hi.png` & `onvif-gui-1.2.1/gui/resources/discover_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/resources/discover_lo.png` & `onvif-gui-1.2.1/gui/resources/discover_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/resources/mute.png` & `onvif-gui-1.2.1/gui/resources/mute.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/resources/mute_lo.png` & `onvif-gui-1.2.1/gui/resources/mute_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/resources/onvif-gui.png` & `onvif-gui-1.2.1/gui/resources/onvif-gui.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/resources/recording_lo.png` & `onvif-gui-1.2.1/gui/resources/recording_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/gui/resources/spinner.gif` & `onvif-gui-1.2.1/gui/resources/spinner.gif`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/modules/audio/sample.py` & `onvif-gui-1.2.1/modules/audio/sample.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/modules/video/keypoint.py` & `onvif-gui-1.2.1/modules/video/keypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,17 @@
 
 class VideoWorker:
     def __init__(self, mw):
         try:
             self.mw = mw
             self.last_ex = ""
 
+            if self.mw.configure.name != MODULE_NAME or len(IMPORT_ERROR) > 0:
+                return
+            
             if self.mw.settingsPanel.chkShowWaitBox.isChecked():
                 self.mw.signals.showWait.emit()
 
             self.CONFIDENCE_THRESHOLD = self.mw.configure.sldThreshold.value()
             ckpt_file = "auto"
             fp16 = True
             self.no_back = True
@@ -114,14 +117,17 @@
             logger.exception("Keypoints initialization error")
 
 
     def __call__(self, F):
         try:
             img = np.array(F, copy=False)
 
+            if self.mw.configure.name != MODULE_NAME:
+                return
+            
             predictions = self.predictor(img)["instances"].to(torch.device('cpu'))
             keypoints = predictions.pred_keypoints.numpy().astype(int)
 
             if self.no_back:
                 img *= 0
 
             boxes = predictions.pred_boxes.tensor.numpy()
```

### Comparing `onvif-gui-1.2.0/modules/video/retinanet.py` & `onvif-gui-1.2.1/modules/video/retinanet.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,14 +82,17 @@
 
 class VideoWorker:
     def __init__(self, mw):
         try:
             self.mw = mw
             self.last_ex = ""
 
+            if self.mw.configure.name != MODULE_NAME or len(IMPORT_ERROR) > 0:
+                return
+            
             if self.mw.settingsPanel.chkShowWaitBox.isChecked():
                 self.mw.signals.showWait.emit()
 
             self.model = torchvision.models.detection.retinanet_resnet50_fpn(weights=torchvision.models.detection.RetinaNet_ResNet50_FPN_Weights.DEFAULT)            
             self.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
             self.model.eval().to(self.device)
             with torch.no_grad():
@@ -100,14 +103,18 @@
 
         except:
             logger.exception("retinanet worker load error")
 
     def __call__(self, F):
         try:
             img = np.array(F, copy = False)
+            
+            if self.mw.configure.name != MODULE_NAME:
+                return
+            
             tensor = transform(img).to(self.device)
             tensor = tensor.unsqueeze(0)
 
             with torch.no_grad():
                 outputs = self.model(tensor)
 
             threshold = self.mw.configure.sldThreshold.value()
```

### Comparing `onvif-gui-1.2.0/modules/video/sample.py` & `onvif-gui-1.2.1/modules/video/sample.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/modules/video/segment.py` & `onvif-gui-1.2.1/modules/video/segment.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,17 @@
 
 class VideoWorker:
     def __init__(self, mw):
         try:
             self.mw = mw
             self.last_ex = ""
 
+            if self.mw.configure.name != MODULE_NAME or len(IMPORT_ERROR) > 0:
+                return
+            
             if self.mw.settingsPanel.chkShowWaitBox.isChecked():
                 self.mw.signals.showWait.emit()
 
             self.CONFIDENCE_THRESHOLD = self.mw.configure.sldThreshold.value()
             ckpt_file = 'auto'
             fp16 = True
             self.simple = True
@@ -145,14 +148,17 @@
             if self.first_pass:
                 if self.mw.configure.sldThreshold.value() != self.CONFIDENCE_THRESHOLD:
                     self.predictor = None
                     self.__init__(self.mw)
 
             img = np.array(F, copy=False)
 
+            if self.mw.configure.name != MODULE_NAME:
+                return
+            
             predictions = self.predictor(img)["instances"]
 
             test_classes = predictions.pred_classes.cpu().numpy()
             test_boxes = predictions.pred_boxes.tensor.cpu().numpy().astype(int)
 
             masks = []
             classes = []
```

### Comparing `onvif-gui-1.2.0/modules/video/yolov7.py` & `onvif-gui-1.2.1/modules/video/yolov7.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
 class VideoWorker:
     def __init__(self, mw):
         try:
             self.mw = mw
             self.last_ex = ""
 
-            if self.mw.configure.name != MODULE_NAME:
+            if self.mw.configure.name != MODULE_NAME or len(IMPORT_ERROR) > 0:
                 return
             
             if self.mw.settingsPanel.chkShowWaitBox.isChecked():
                 self.mw.signals.showWait.emit()
 
             self.ckpt_file = None
             if self.mw.configure.chkAuto.isChecked():
```

### Comparing `onvif-gui-1.2.0/modules/video/yolov8.py` & `onvif-gui-1.2.1/modules/video/yolov8.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             
 class VideoWorker:
     def __init__(self, mw):
         try:
             self.mw = mw
             self.last_ex = ""
 
-            if self.mw.configure.name != MODULE_NAME:
+            if self.mw.configure.name != MODULE_NAME or len(IMPORT_ERROR) > 0:
                 return
             
             if self.mw.settingsPanel.chkShowWaitBox.isChecked():
                 self.mw.signals.showWait.emit()
 
             self.ckpt_file = None
             if self.mw.configure.chkAuto.isChecked():
```

### Comparing `onvif-gui-1.2.0/modules/video/yolox.py` & `onvif-gui-1.2.1/modules/video/yolox.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
 class VideoWorker:
     def __init__(self, mw):
         try:
             self.mw = mw
             self.last_ex = ""
 
-            if self.mw.configure.name != MODULE_NAME:
+            if self.mw.configure.name != MODULE_NAME or len(IMPORT_ERROR) > 0:
                 return
             
             if self.mw.settingsPanel.chkShowWaitBox.isChecked():
                 self.mw.signals.showWait.emit()
             device_name = "cpu"
             if torch.cuda.is_available():
                 device_name = "cuda"
```

### Comparing `onvif-gui-1.2.0/onvif_gui.egg-info/PKG-INFO` & `onvif-gui-1.2.1/onvif_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-gui
-Version: 1.2.0
+Version: 1.2.1
 Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libonvif
 Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `onvif-gui-1.2.0/onvif_gui.egg-info/SOURCES.txt` & `onvif-gui-1.2.1/onvif_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/pyproject.toml` & `onvif-gui-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #*********************************************************************/
 
 [project]
 name = "onvif-gui" 
-version = "1.2.0"  
+version = "1.2.1"  
 description = "A client gui for Onvif"  
 readme = "README.md" 
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]  
 authors = [
   {name = "Stephen Rhodes", email = "sr99622@gmail.com" }
```

### Comparing `onvif-gui-1.2.0/setup.py` & `onvif-gui-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from setuptools.command.install import install
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="onvif-gui",
-    version="1.2.0",
+    version="1.2.1",
     author="Stephen Rhodes",
     author_email="sr99622@gmail.com",
     description="GUI program for onvif",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

### Comparing `onvif-gui-1.2.0/tracker/basetrack.py` & `onvif-gui-1.2.1/tracker/basetrack.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/tracker/byte_tracker.py` & `onvif-gui-1.2.1/tracker/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/tracker/kalman_filter.py` & `onvif-gui-1.2.1/tracker/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/tracker/matching.py` & `onvif-gui-1.2.1/tracker/matching.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolov7/models/common.py` & `onvif-gui-1.2.1/yolov7/models/common.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolov7/models/experimental.py` & `onvif-gui-1.2.1/yolov7/models/experimental.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolov7/models/yolo.py` & `onvif-gui-1.2.1/yolov7/models/yolo.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolov7/utils/activations.py` & `onvif-gui-1.2.1/yolov7/utils/activations.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolov7/utils/add_nms.py` & `onvif-gui-1.2.1/yolov7/utils/add_nms.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolov7/utils/autoanchor.py` & `onvif-gui-1.2.1/yolov7/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolov7/utils/datasets.py` & `onvif-gui-1.2.1/yolov7/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolov7/utils/general.py` & `onvif-gui-1.2.1/yolov7/utils/general.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolov7/utils/google_utils.py` & `onvif-gui-1.2.1/yolov7/utils/google_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolov7/utils/loss.py` & `onvif-gui-1.2.1/yolov7/utils/loss.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolov7/utils/metrics.py` & `onvif-gui-1.2.1/yolov7/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolov7/utils/plots.py` & `onvif-gui-1.2.1/yolov7/utils/plots.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolov7/utils/torch_utils.py` & `onvif-gui-1.2.1/yolov7/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolox/models/__init__.py` & `onvif-gui-1.2.1/yolox/models/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolox/models/build.py` & `onvif-gui-1.2.1/yolox/models/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolox/models/darknet.py` & `onvif-gui-1.2.1/yolox/models/darknet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolox/models/losses.py` & `onvif-gui-1.2.1/yolox/models/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolox/models/network_blocks.py` & `onvif-gui-1.2.1/yolox/models/network_blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolox/models/yolo_fpn.py` & `onvif-gui-1.2.1/yolox/models/yolo_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolox/models/yolo_head.py` & `onvif-gui-1.2.1/yolox/models/yolo_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolox/models/yolo_pafpn.py` & `onvif-gui-1.2.1/yolox/models/yolo_pafpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolox/models/yolox.py` & `onvif-gui-1.2.1/yolox/models/yolox.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.0/yolox/utils/utils.py` & `onvif-gui-1.2.1/yolox/utils/utils.py`

 * *Files identical despite different names*

