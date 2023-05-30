# Comparing `tmp/PartSeg-0.9b1.tar.gz` & `tmp/PartSeg-0.9b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PartSeg-0.9b1.tar", last modified: Thu Feb 28 12:26:02 2019, max compression
+gzip compressed data, was "dist/PartSeg-0.9b2.tar", last modified: Tue Mar  5 14:49:07 2019, max compression
```

## Comparing `PartSeg-0.9b1.tar` & `PartSeg-0.9b2.tar`

### file list

```diff
@@ -1,229 +1,235 @@
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     4494 2019-02-28 12:26:02.000000 PartSeg-0.9b1/PKG-INFO
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/tests/
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/tests/cython/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      131 2017-11-16 11:31:46.000000 PartSeg-0.9b1/tests/cython/fib.pyx
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      185 2019-02-28 12:21:13.000000 PartSeg-0.9b1/MANIFEST.in
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     4498 2019-02-28 12:21:13.000000 PartSeg-0.9b1/setup.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)       38 2019-02-28 12:26:02.000000 PartSeg-0.9b1/setup.cfg
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      901 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/callback.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      739 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/stackseg_main.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/segmentation_mask/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3186 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/segmentation_mask/stack_settings.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/segmentation_mask/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    31692 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/segmentation_mask/stack_gui_main.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2708 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/segmentation_mask/image_view.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3873 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/segmentation_mask/batch_proceed.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3630 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/update_metadata.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/launcher/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     4503 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/launcher/main_window.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/launcher/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      589 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/genrate_colormaps_map.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/plugins/
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/plugins/multiscale_segmentation/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)       24 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/plugins/multiscale_segmentation/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)       80 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/plugins/multiscale_segmentation/multiscale_segmentation.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/plugins/itk_snap_save/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      865 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/plugins/itk_snap_save/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      400 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/plugins/__init__.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/custom_application/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)       42 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/custom_application/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      838 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/custom_application/application.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      457 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/test-sctipt.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      171 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/__init__.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/utils/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      367 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/cmap_utils.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/utils/analysis/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    26494 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/utils/analysis/statistics_calculation.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/analysis/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      148 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/analysis/save_register.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    10933 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/utils/analysis/save_functions.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      511 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/analysis/io_utils.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     5874 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/utils/analysis/load_functions.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2437 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/utils/analysis/analysis_utils.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    20269 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/analysis/calculation_plan.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/utils/analysis/batch_processing/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     7130 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/utils/analysis/batch_processing/parallel_backed.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/analysis/batch_processing/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    19505 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/utils/analysis/batch_processing/batch_backend.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1468 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/analysis/save_hooks.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2726 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/utils/analysis/algorithm_description.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)       48 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/report_utils.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1024 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/utils/base_argparser.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1451 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/utils/register.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      144 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/class_generate_base.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/utils/segmentation/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2294 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/segmentation/algorithm_base.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     5204 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/utils/segmentation/algorithm_describe_base.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2391 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/utils/segmentation/mu_mid_point.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/segmentation/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    10023 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/segmentation/segmentation_algorithm.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     7906 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/segmentation/threshold.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     6967 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/utils/segmentation/sprawl.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    11975 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/segmentation/segment.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    21475 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/utils/segmentation/restartable_segmentation_algorithms.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2102 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/segmentation/noise_filtering.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/utils/fuzy_segment/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     5682 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/fuzy_segment/fuzzy_segment_cython.pyx
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/utils/multiscale_opening/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)  2024482 2019-02-28 12:21:48.000000 PartSeg-0.9b1/package/PartSeg/utils/multiscale_opening/mso_bind.cpp
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)       50 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/utils/multiscale_opening/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    11709 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/utils/multiscale_opening/mso_bind.pyx
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2081 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/calculate_pipeline.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2901 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/utils/json_hooks.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    38176 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/czifile.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      384 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/universal_const.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)       22 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      980 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/global_settings.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     6966 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/utils/mask_create.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3074 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/convex_fill.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     4509 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/utils/autofit.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/euclieadn.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3110 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/put_borders_in_queue.pyx
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     7537 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/find_split.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     4539 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/fuzzy_distance.pyx
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      665 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/distance_utils.pxd
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)  1298932 2019-02-13 09:51:39.000000 PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/euclidean_cython.cpp
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      100 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)   496356 2019-02-13 09:51:40.000000 PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/path_sprawl_cython.cpp
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)  1445833 2019-02-13 09:51:41.000000 PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/sprawl_utils.cpp
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     5744 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/path_sprawl_cython.pyx
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3957 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/sprawl_utils.pyx
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)   639783 2019-02-13 09:51:40.000000 PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/fuzzy_distance.cpp
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     5191 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/euclidean_cython.pyx
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/distance_calculate.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)       71 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/utils/channel_class.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/utils/mask/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/mask/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     8481 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/utils/mask/io_functions.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      234 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/mask/algorithm_description.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/utils/color_image/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2185 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/color_image/color_image_base.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     5616 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/color_image/color_image.pyx
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)       78 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/color_image/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)  1491657 2019-02-13 09:51:38.000000 PartSeg-0.9b1/package/PartSeg/utils/color_image/color_image.cpp
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    14389 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/class_generator.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1560 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/utils.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2240 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/image_operations.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2337 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/utils/io_utils.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      599 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/border_rim.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/utils/interpolation/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/interpolation/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      342 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/interpolation/setup.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     4022 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/interpolation/bilinear_interpolation.pyx
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      210 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/interpolation/cubic_interpolation.pyx
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1572 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/custom_colormaps.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)       73 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/utils/colors.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2193 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/extract_images.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     7962 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/convert_to_cmap.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1878 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/batch_testing.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1647 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/launcher_main.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/static_files/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)   540852 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/colors.npz
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/static_files/icons/
--rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     1786 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/icons/transform-move.png
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    90226 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/icons/icon.png
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    79907 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/icons/icon.icns
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)   160103 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/icons/icon_stack.png
--rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)      715 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/icons/image-zoom-in.png
--rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     1847 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/icons/zoom-original.png
--rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     1557 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/icons/task-attempt.png
--rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     1589 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/icons/draw-eraser.png
--rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     1219 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/icons/draw-path.png
--rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     5791 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/icons/transform-scale.png
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    92968 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/icons/icon.ico
--rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     1450 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/icons/configure.png
--rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     2152 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/icons/document-save-as.png
--rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     1912 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/icons/task-reject.png
--rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     1798 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/icons/document-open.png
--rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)      924 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/icons/task-accepted.png
--rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     2187 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/icons/zoom-select.png
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/static_files/initial_images/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)   364564 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/initial_images/clean_segment.tiff
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)  6356872 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/static_files/initial_images/stack.tif
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/project_utils_qt/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2363 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/project_utils_qt/main_window.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1126 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/project_utils_qt/execute_function_thread.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      936 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/project_utils_qt/image_read_thread.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3075 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/project_utils_qt/error_dialog.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2613 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/project_utils_qt/segmentation_thread.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      925 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/project_utils_qt/except_hook.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/project_utils_qt/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      370 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/project_utils_qt/progress_thread.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1445 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/project_utils_qt/load_backup.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     8893 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/project_utils_qt/settings.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1256 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/project_utils_qt/list_item_widget_for_exception.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)       96 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/project_utils_qt/abstract_class.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     6113 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/testy.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    11735 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/main_window.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    21102 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/statistics_calculation.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    26025 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/backend.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    50843 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/advanced_window.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    25194 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/batch_window.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    34690 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/image_view.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     4106 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/qt_import.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2409 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/interpolate_dialog.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    10714 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/profile_export.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    10884 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/segment.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    46539 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/prepare_plan_widget.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    13313 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/io_functions.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/batch_processing/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     7109 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/batch_processing/parallel_backed.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/batch_processing/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    17540 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/batch_processing/batch_backend.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    20712 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/batch_processing/calculation_plan.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    46927 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg_old/gui.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/tiff_image/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      100 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/tiff_image/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1854 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/tiff_image/image_writer.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    16810 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/tiff_image/image_reader.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     7529 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/tiff_image/image.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/segmentation_analysis/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    35364 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/segmentation_analysis/main_window.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    40848 2019-02-28 12:20:46.000000 PartSeg-0.9b1/package/PartSeg/segmentation_analysis/advanced_window.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    20111 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/segmentation_analysis/batch_window.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/segmentation_analysis/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     8490 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/segmentation_analysis/image_view.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      958 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/segmentation_analysis/interpolate_thread.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2651 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/segmentation_analysis/interpolate_dialog.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    11112 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/segmentation_analysis/profile_export.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     5994 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/segmentation_analysis/partseg_settings.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    46075 2019-02-28 12:20:36.000000 PartSeg-0.9b1/package/PartSeg/segmentation_analysis/prepare_plan_widget.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    13657 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/segmentation_analysis/statistic_widget.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      912 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/segmentation_analysis/calculation_pipeline_thread.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      673 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg2_main.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg/common_gui/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3858 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/common_gui/colors_choose.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      589 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/common_gui/vetical_scroll_area.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     6269 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/common_gui/flow_layout.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1930 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/common_gui/waiting_dialog.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/common_gui/__init__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     5893 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/common_gui/mask_widget.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    19881 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/common_gui/channel_control.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1485 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/common_gui/custom_load_dialog.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     6198 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/common_gui/select_multiple_files.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     4505 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/common_gui/custom_save_dialog.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3145 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/common_gui/save_dialog.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1451 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/common_gui/show_directory_dialog.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      456 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/common_gui/dim_combobox.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1858 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/common_gui/collapse_checkbox.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1070 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/common_gui/about_dialog.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    20870 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/common_gui/algorithms_description.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      706 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/common_gui/lock_checkbox.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     5007 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/common_gui/universal_gui_part.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)    31560 2019-02-27 09:18:03.000000 PartSeg-0.9b1/package/PartSeg/common_gui/stack_image_view.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)       83 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/__main__.py
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1691 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/PartSeg/partseg_main.py
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/PartSeg.egg-info/
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     4494 2019-02-28 12:26:00.000000 PartSeg-0.9b1/package/PartSeg.egg-info/PKG-INFO
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)     9287 2019-02-28 12:26:00.000000 PartSeg-0.9b1/package/PartSeg.egg-info/SOURCES.txt
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)      135 2019-02-28 12:26:00.000000 PartSeg-0.9b1/package/PartSeg.egg-info/requires.txt
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)        8 2019-02-28 12:26:00.000000 PartSeg-0.9b1/package/PartSeg.egg-info/top_level.txt
--rw-r--r--   0 grzegorzbokota   (501) staff       (20)        1 2019-02-28 12:26:00.000000 PartSeg-0.9b1/package/PartSeg.egg-info/dependency_links.txt
-drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-02-28 12:26:02.000000 PartSeg-0.9b1/package/scripts/
--rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)       77 2019-02-13 09:50:39.000000 PartSeg-0.9b1/package/scripts/PartSeg
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     4494 2019-03-05 14:49:07.000000 PartSeg-0.9b2/PKG-INFO
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/tests/
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/tests/cython/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      131 2017-11-16 11:31:46.000000 PartSeg-0.9b2/tests/cython/fib.pyx
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      185 2019-03-05 12:55:17.000000 PartSeg-0.9b2/MANIFEST.in
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     4498 2019-03-05 12:55:17.000000 PartSeg-0.9b2/setup.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)       38 2019-03-05 14:49:07.000000 PartSeg-0.9b2/setup.cfg
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      901 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/callback.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      739 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/stackseg_main.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/segmentation_mask/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3186 2019-02-27 09:18:03.000000 PartSeg-0.9b2/package/PartSeg/segmentation_mask/stack_settings.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/segmentation_mask/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    31692 2019-03-05 12:55:17.000000 PartSeg-0.9b2/package/PartSeg/segmentation_mask/stack_gui_main.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2708 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/segmentation_mask/image_view.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3873 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/segmentation_mask/batch_proceed.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3630 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/update_metadata.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/launcher/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     4503 2019-03-05 12:55:17.000000 PartSeg-0.9b2/package/PartSeg/launcher/main_window.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/launcher/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      589 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/genrate_colormaps_map.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/plugins/
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/plugins/multiscale_segmentation/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)       24 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/plugins/multiscale_segmentation/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)       80 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/plugins/multiscale_segmentation/multiscale_segmentation.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/plugins/itk_snap_save/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      865 2019-02-27 09:18:03.000000 PartSeg-0.9b2/package/PartSeg/plugins/itk_snap_save/__init__.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/plugins/modeling_save/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3252 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/plugins/modeling_save/save_modeling_data.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      267 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/plugins/modeling_save/__init__.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/plugins/old_partseg/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      266 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/plugins/old_partseg/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3122 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/plugins/old_partseg/old_partseg.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      400 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/plugins/__init__.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/custom_application/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)       42 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/custom_application/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      838 2019-03-05 12:55:17.000000 PartSeg-0.9b2/package/PartSeg/custom_application/application.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      457 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/test-sctipt.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      171 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/__init__.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/utils/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)       75 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/utils/state_store.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      367 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/cmap_utils.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/utils/analysis/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    26494 2019-02-27 09:18:03.000000 PartSeg-0.9b2/package/PartSeg/utils/analysis/statistics_calculation.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/analysis/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      148 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/analysis/save_register.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    12494 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/utils/analysis/save_functions.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      511 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/analysis/io_utils.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     5906 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/utils/analysis/load_functions.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2437 2019-02-28 12:20:46.000000 PartSeg-0.9b2/package/PartSeg/utils/analysis/analysis_utils.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    20269 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/analysis/calculation_plan.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/utils/analysis/batch_processing/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     7130 2019-02-27 09:18:03.000000 PartSeg-0.9b2/package/PartSeg/utils/analysis/batch_processing/parallel_backed.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/analysis/batch_processing/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    19505 2019-02-27 09:18:03.000000 PartSeg-0.9b2/package/PartSeg/utils/analysis/batch_processing/batch_backend.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1468 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/analysis/save_hooks.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2726 2019-02-28 12:20:46.000000 PartSeg-0.9b2/package/PartSeg/utils/analysis/algorithm_description.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1451 2019-02-27 09:18:03.000000 PartSeg-0.9b2/package/PartSeg/utils/register.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      144 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/class_generate_base.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/utils/segmentation/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2294 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/segmentation/algorithm_base.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     5204 2019-02-28 12:20:46.000000 PartSeg-0.9b2/package/PartSeg/utils/segmentation/algorithm_describe_base.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2391 2019-03-05 11:41:04.000000 PartSeg-0.9b2/package/PartSeg/utils/segmentation/mu_mid_point.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/segmentation/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    10023 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/utils/segmentation/segmentation_algorithm.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     7935 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/utils/segmentation/threshold.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     6969 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/utils/segmentation/sprawl.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    11975 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/segmentation/segment.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    21475 2019-03-05 11:41:04.000000 PartSeg-0.9b2/package/PartSeg/utils/segmentation/restartable_segmentation_algorithms.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2102 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/segmentation/noise_filtering.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/utils/fuzy_segment/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     5682 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/fuzy_segment/fuzzy_segment_cython.pyx
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/utils/multiscale_opening/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)  2023726 2019-03-05 14:48:51.000000 PartSeg-0.9b2/package/PartSeg/utils/multiscale_opening/mso_bind.cpp
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)       50 2019-03-05 11:41:04.000000 PartSeg-0.9b2/package/PartSeg/utils/multiscale_opening/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    11794 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/utils/multiscale_opening/mso_bind.pyx
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2081 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/calculate_pipeline.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2901 2019-02-27 09:18:03.000000 PartSeg-0.9b2/package/PartSeg/utils/json_hooks.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    38176 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/czifile.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      384 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/universal_const.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)       22 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      980 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/global_settings.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     6966 2019-02-27 09:18:03.000000 PartSeg-0.9b2/package/PartSeg/utils/mask_create.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3074 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/convex_fill.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     4509 2019-02-27 09:18:03.000000 PartSeg-0.9b2/package/PartSeg/utils/autofit.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/euclieadn.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3110 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/put_borders_in_queue.pyx
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     7537 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/find_split.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     4539 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/fuzzy_distance.pyx
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      665 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/distance_utils.pxd
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)  1298932 2019-02-13 09:51:39.000000 PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/euclidean_cython.cpp
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      100 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)   496356 2019-02-13 09:51:40.000000 PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/path_sprawl_cython.cpp
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)  1445833 2019-02-13 09:51:41.000000 PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/sprawl_utils.cpp
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     5744 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/path_sprawl_cython.pyx
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3957 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/sprawl_utils.pyx
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)   639783 2019-02-13 09:51:40.000000 PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/fuzzy_distance.cpp
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     5191 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/euclidean_cython.pyx
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/distance_calculate.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)       71 2019-02-28 12:20:46.000000 PartSeg-0.9b2/package/PartSeg/utils/channel_class.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/utils/mask/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/mask/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     8481 2019-02-27 09:18:03.000000 PartSeg-0.9b2/package/PartSeg/utils/mask/io_functions.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      234 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/mask/algorithm_description.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/utils/color_image/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2185 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/color_image/color_image_base.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     5616 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/color_image/color_image.pyx
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)       78 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/color_image/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)  1491657 2019-02-13 09:51:38.000000 PartSeg-0.9b2/package/PartSeg/utils/color_image/color_image.cpp
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    14389 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/class_generator.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1560 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/utils.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2240 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/image_operations.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2337 2019-02-27 09:18:03.000000 PartSeg-0.9b2/package/PartSeg/utils/io_utils.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      599 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/border_rim.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/utils/interpolation/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/interpolation/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      342 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/interpolation/setup.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     4022 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/interpolation/bilinear_interpolation.pyx
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      210 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/interpolation/cubic_interpolation.pyx
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1572 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/custom_colormaps.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)       73 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/utils/colors.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2193 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/extract_images.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     7962 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/convert_to_cmap.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1878 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/batch_testing.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2292 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/launcher_main.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/static_files/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)   540852 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/colors.npz
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/static_files/icons/
+-rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     1786 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/icons/transform-move.png
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    90226 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/icons/icon.png
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    79907 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/icons/icon.icns
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)   160103 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/icons/icon_stack.png
+-rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)      715 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/icons/image-zoom-in.png
+-rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     1847 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/icons/zoom-original.png
+-rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     1557 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/icons/task-attempt.png
+-rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     1589 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/icons/draw-eraser.png
+-rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     1219 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/icons/draw-path.png
+-rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     5791 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/icons/transform-scale.png
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    92968 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/icons/icon.ico
+-rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     1450 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/icons/configure.png
+-rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     2152 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/icons/document-save-as.png
+-rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     1912 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/icons/task-reject.png
+-rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     1798 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/icons/document-open.png
+-rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)      924 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/icons/task-accepted.png
+-rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)     2187 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/icons/zoom-select.png
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/static_files/initial_images/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)   364564 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/initial_images/clean_segment.tiff
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)  6356872 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/static_files/initial_images/stack.tif
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/project_utils_qt/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2363 2019-03-05 12:55:17.000000 PartSeg-0.9b2/package/PartSeg/project_utils_qt/main_window.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1126 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/project_utils_qt/execute_function_thread.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      936 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/project_utils_qt/image_read_thread.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1169 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/project_utils_qt/base_argparser.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3071 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/project_utils_qt/error_dialog.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2613 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/project_utils_qt/segmentation_thread.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      923 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/project_utils_qt/except_hook.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/project_utils_qt/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      370 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/project_utils_qt/progress_thread.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1445 2019-03-05 12:55:17.000000 PartSeg-0.9b2/package/PartSeg/project_utils_qt/load_backup.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     8926 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/project_utils_qt/settings.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1256 2019-02-27 09:18:03.000000 PartSeg-0.9b2/package/PartSeg/project_utils_qt/list_item_widget_for_exception.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)       96 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/project_utils_qt/abstract_class.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     6113 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/testy.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    11735 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/main_window.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    21102 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/statistics_calculation.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    26025 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/backend.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    50843 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/advanced_window.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    25194 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/batch_window.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    34690 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/image_view.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     4106 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/qt_import.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2409 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/interpolate_dialog.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    10714 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/profile_export.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    10884 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/segment.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    46539 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/prepare_plan_widget.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    13313 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/io_functions.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/batch_processing/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     7109 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/batch_processing/parallel_backed.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/batch_processing/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    17540 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/batch_processing/batch_backend.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    20712 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/batch_processing/calculation_plan.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    46927 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg_old/gui.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/tiff_image/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      100 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/tiff_image/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1854 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/tiff_image/image_writer.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    16810 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/tiff_image/image_reader.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     7529 2019-02-27 09:18:03.000000 PartSeg-0.9b2/package/PartSeg/tiff_image/image.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/segmentation_analysis/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    35723 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/segmentation_analysis/main_window.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    40848 2019-02-28 12:20:46.000000 PartSeg-0.9b2/package/PartSeg/segmentation_analysis/advanced_window.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    20111 2019-02-27 09:18:03.000000 PartSeg-0.9b2/package/PartSeg/segmentation_analysis/batch_window.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/segmentation_analysis/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     8490 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/segmentation_analysis/image_view.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      973 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/segmentation_analysis/interpolate_thread.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     2651 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/segmentation_analysis/interpolate_dialog.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    11112 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/segmentation_analysis/profile_export.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     6040 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/segmentation_analysis/partseg_settings.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    46537 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/segmentation_analysis/prepare_plan_widget.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    13657 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/segmentation_analysis/statistic_widget.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      912 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/segmentation_analysis/calculation_pipeline_thread.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      673 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg2_main.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg/common_gui/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3858 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/common_gui/colors_choose.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      589 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/common_gui/vetical_scroll_area.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     6269 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/common_gui/flow_layout.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1930 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/common_gui/waiting_dialog.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)        0 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/common_gui/__init__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     5893 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/common_gui/mask_widget.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    20012 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/common_gui/channel_control.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1485 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/common_gui/custom_load_dialog.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     6198 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/common_gui/select_multiple_files.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     4505 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/common_gui/custom_save_dialog.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     3145 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/common_gui/save_dialog.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1451 2019-02-27 09:18:03.000000 PartSeg-0.9b2/package/PartSeg/common_gui/show_directory_dialog.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      456 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/common_gui/dim_combobox.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1858 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/common_gui/collapse_checkbox.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1070 2019-02-27 09:18:03.000000 PartSeg-0.9b2/package/PartSeg/common_gui/about_dialog.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    21358 2019-03-05 14:43:15.000000 PartSeg-0.9b2/package/PartSeg/common_gui/algorithms_description.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      706 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/common_gui/lock_checkbox.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     5007 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/common_gui/universal_gui_part.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)    31560 2019-02-27 09:18:03.000000 PartSeg-0.9b2/package/PartSeg/common_gui/stack_image_view.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)       83 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/__main__.py
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     1691 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/PartSeg/partseg_main.py
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/PartSeg.egg-info/
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     4494 2019-03-05 14:48:51.000000 PartSeg-0.9b2/package/PartSeg.egg-info/PKG-INFO
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)     9506 2019-03-05 14:48:52.000000 PartSeg-0.9b2/package/PartSeg.egg-info/SOURCES.txt
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)      135 2019-03-05 14:48:51.000000 PartSeg-0.9b2/package/PartSeg.egg-info/requires.txt
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)        8 2019-03-05 14:48:51.000000 PartSeg-0.9b2/package/PartSeg.egg-info/top_level.txt
+-rw-r--r--   0 grzegorzbokota   (501) staff       (20)        1 2019-03-05 14:48:51.000000 PartSeg-0.9b2/package/PartSeg.egg-info/dependency_links.txt
+drwxr-xr-x   0 grzegorzbokota   (501) staff       (20)        0 2019-03-05 14:49:07.000000 PartSeg-0.9b2/package/scripts/
+-rwxr-xr-x   0 grzegorzbokota   (501) staff       (20)       77 2019-02-13 09:50:39.000000 PartSeg-0.9b2/package/scripts/PartSeg
```

### Comparing `PartSeg-0.9b1/PKG-INFO` & `PartSeg-0.9b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PartSeg
-Version: 0.9b1
+Version: 0.9b2
 Summary: PartSeg is python GUI for bio imaging analysis
 Home-page: https://4dnucleome.cent.uw.edu.pl/PartSeg/
 Author: Grzegorz Bokota
 Author-email: g.bokota@cent.uw.edu.pl
 License: UNKNOWN
 Description: # PartSeg
         [![Build Status](https://travis-ci.org/4DNucleome/PartSeg.svg?branch=master)](https://travis-ci.org/4DNucleome/PartSeg)
```

### Comparing `PartSeg-0.9b1/setup.py` & `PartSeg-0.9b2/setup.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/callback.py` & `PartSeg-0.9b2/package/PartSeg/callback.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/stackseg_main.py` & `PartSeg-0.9b2/package/PartSeg/stackseg_main.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/segmentation_mask/stack_settings.py` & `PartSeg-0.9b2/package/PartSeg/segmentation_mask/stack_settings.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/segmentation_mask/stack_gui_main.py` & `PartSeg-0.9b2/package/PartSeg/segmentation_mask/stack_gui_main.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/segmentation_mask/image_view.py` & `PartSeg-0.9b2/package/PartSeg/segmentation_mask/image_view.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/segmentation_mask/batch_proceed.py` & `PartSeg-0.9b2/package/PartSeg/segmentation_mask/batch_proceed.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/update_metadata.py` & `PartSeg-0.9b2/package/PartSeg/update_metadata.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/launcher/main_window.py` & `PartSeg-0.9b2/package/PartSeg/launcher/main_window.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/genrate_colormaps_map.py` & `PartSeg-0.9b2/package/PartSeg/genrate_colormaps_map.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/plugins/itk_snap_save/__init__.py` & `PartSeg-0.9b2/package/PartSeg/plugins/itk_snap_save/__init__.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/custom_application/application.py` & `PartSeg-0.9b2/package/PartSeg/custom_application/application.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/analysis/statistics_calculation.py` & `PartSeg-0.9b2/package/PartSeg/utils/analysis/statistics_calculation.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/analysis/save_functions.py` & `PartSeg-0.9b2/package/PartSeg/utils/analysis/save_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from pathlib import Path
 
+import tifffile
+
 from .io_utils import ProjectTuple
 from ..analysis.analysis_utils import HistoryElement
 from ..channel_class import Channel
 from ..segmentation.algorithm_describe_base import AlgorithmProperty
 from ..universal_const import UNIT_SCALE, Units
 from ..analysis.save_hooks import PartEncoder
 import numpy as np
@@ -57,16 +59,16 @@
         if len(el_info) > 0:
             hist_str = json.dumps(el_info, cls=PartEncoder)
             hist_buff = BytesIO(hist_str.encode('utf-8'))
             tar_algorithm = get_tarinfo("history/history.json", hist_buff)
             tar.addfile(tar_algorithm, hist_buff)
 
 
-def save_cmap(file: typing.Union[str, h5py.File], image: Image, segmentation: np.ndarray, cmap_profile: dict,
-              metadata: typing.Optional[dict] = None):
+def save_cmap(file: typing.Union[str, h5py.File], image: Image, segmentation: np.ndarray, full_segmentation: np.ndarray,
+              cmap_profile: dict, metadata: typing.Optional[dict] = None):
     if segmentation is None or segmentation.max() == 0:
         raise ValueError("No segmentation")
     if isinstance(file, (str, BytesIO)):
         if isinstance(file, str) and os.path.exists(file):
             os.remove(file)
         cmap_file = h5py.File(file)
     elif isinstance(file, h5py.File):
@@ -75,21 +77,28 @@
         raise ValueError(f"Wrong type of file argument, type: {type(file)}")
     data = image.get_channel(cmap_profile["channel"])
     """if cmap_profile.gauss_radius > 0 and cmap_profile.gauss_type != RadiusType.NO:
         gauss_radius = calculate_operation_radius(cmap_profile.gauss_radius, image.spacing, cmap_profile.gauss_radius)
         layer = cmap_profile.gauss_type == RadiusType.R2D
         data = gaussian(data, gauss_radius, layer=layer)"""
 
+    if cmap_profile["reverse"]:
+        if full_segmentation is None:
+            full_segmentation = segmentation
+        mean_val = np.mean(data[full_segmentation == 0])
+        data = mean_val - data
+        data[data < 0] = 0
+
     data[segmentation == 0] = 0
     grp = cmap_file.create_group('Chimera/image1')
     if cmap_profile["clip"]:
         points = np.nonzero(segmentation)
         lower_bound = np.min(points, axis=1)
         upper_bound = np.max(points, axis=1)
-        cut_img = np.zeros(upper_bound - lower_bound + [7, 7, 7], dtype=data.dtype)
+        cut_img = np.zeros(upper_bound - lower_bound + np.array([6, 6, 6]), dtype=data.dtype)
         coord = tuple([slice(x, y) for x, y in zip(lower_bound, upper_bound)])
         cut_img[3:-3, 3:-3, 3:-3] = data[coord]
         data = cut_img
     z, y, x = data.shape
     data_set = grp.create_dataset("data_zyx", (z, y, x), dtype='f', compression="gzip")
     data_set[...] = data
 
@@ -103,16 +112,15 @@
     grp.attrs['TITLE'] = np.string_('')
     grp.attrs['VERSION'] = np.string_('1.0')
 
     grp = cmap_file['Chimera/image1']
     grp.attrs['CLASS'] = np.string_('GROUP')
     grp.attrs['TITLE'] = np.string_('')
     grp.attrs['VERSION'] = np.string_('1.0')
-    grp.attrs['step'] = np.array(image._image_spacing, dtype=np.float32)[::-1] * \
-                        UNIT_SCALE[cmap_profile["units"].value]
+    grp.attrs['step'] = np.array(image._image_spacing, dtype=np.float32)[::-1] * UNIT_SCALE[cmap_profile["units"].value]
 
     if isinstance(file, str):
         cmap_file.close()
     pass
 
 
 class SaveProject(SaveBase):
@@ -145,20 +153,23 @@
         return "cmap"
 
     @classmethod
     def get_fields(cls):
         return [AlgorithmProperty("channel", "Channel", 0, property_type=Channel),
                 AlgorithmProperty("separated_objects", "Separate Objects", False),
                 AlgorithmProperty("clip", "Clip area", False),
-                AlgorithmProperty("units", "Units", Units.nm, property_type=Units)]
+                AlgorithmProperty("units", "Units", Units.nm, property_type=Units),
+                AlgorithmProperty('reverse', 'Reverse', False,
+                                  tool_tip="Reverse brightness off image (for electron microscopy)")]
 
     @classmethod
     def save(cls, save_location: typing.Union[str, BytesIO, Path], project_info: ProjectTuple, parameters: dict,
              range_changed=None, step_changed=None):
-        save_cmap(save_location, project_info.image, project_info.segmentation, parameters)
+        save_cmap(save_location, project_info.image, project_info.segmentation, project_info.full_segmentation,
+                  parameters)
 
 
 class SaveXYZ(SaveBase):
     @classmethod
     def get_name(cls):
         return "XYZ text (*.xyz *.txt)"
 
@@ -255,16 +266,14 @@
              range_changed=None, step_changed=None):
         data = project_info.image.get_data()
         if parameters["squeeze"]:
             data = np.squeeze(data)
         np.save(save_location, data)
 
 
-
-
 class SaveMaskAsTiff(SaveBase):
     @classmethod
     def get_name(cls):
         return "Mask (*.tiff *.tif)"
 
     @classmethod
     def get_short_name(cls):
@@ -276,13 +285,52 @@
 
     @classmethod
     def save(cls, save_location: typing.Union[str, BytesIO, Path], project_info, parameters: dict,
              range_changed=None, step_changed=None):
         ImageWriter.save_mask(project_info.image, save_location)
 
 
+class SaveSegmentationAsTIFF(SaveBase):
+    @classmethod
+    def get_name(cls):
+        return "Segmentation (*.tiff *.tif)"
+
+    @classmethod
+    def get_short_name(cls):
+        return "segmentation_tiff"
+
+    @classmethod
+    def get_fields(cls):
+        return []
+
+    @classmethod
+    def save(cls, save_location: typing.Union[str, BytesIO, Path], project_info, parameters: dict,
+             range_changed=None, step_changed=None):
+        tifffile.imsave(save_location, project_info.segmentation)
+
+class SaveSegmentationAsNumpy(SaveBase):
+    @classmethod
+    def get_name(cls):
+        return "Segmentation (*.npy)"
+
+    @classmethod
+    def get_short_name(cls):
+        return "segmentation_numpy"
+
+    @classmethod
+    def get_fields(cls):
+        return []
+
+    @classmethod
+    def save(cls, save_location: typing.Union[str, BytesIO, Path], project_info, parameters: dict,
+             range_changed=None, step_changed=None):
+        np.save(save_location, project_info.segmentation)
+
+
 save_dict.register(SaveProject)
 save_dict.register(SaveCmap)
 save_dict.register(SaveXYZ)
 save_dict.register(SaveAsTiff)
 save_dict.register(SaveMaskAsTiff)
 save_dict.register(SaveAsNumpy)
+save_dict.register(SaveSegmentationAsTIFF)
+save_dict.register(SaveSegmentationAsNumpy)
```

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/analysis/load_functions.py` & `PartSeg-0.9b2/package/PartSeg/utils/analysis/load_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         raise ValueError(f"wrong type of file_ argument: {type(file)}")
     image_buffer = BytesIO()
     image_tar = tar_file.extractfile(tar_file.getmember("image.tif"))
     image_buffer.write(image_tar.read())
     image_buffer.seek(0)
     reader = ImageReader()
     image = reader.read(image_buffer)
+    image.file_path = file_path
     seg_tar = tar_file.extractfile(tar_file.getmember("segmentation.npz"))
     seg_buffer = BytesIO()
     seg_buffer.write(seg_tar.read())
     seg_buffer.seek(0)
     seg_dict = np.load(seg_buffer)
     if "mask" in seg_dict:
         mask = seg_dict["mask"]
```

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/analysis/analysis_utils.py` & `PartSeg-0.9b2/package/PartSeg/utils/analysis/analysis_utils.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/analysis/calculation_plan.py` & `PartSeg-0.9b2/package/PartSeg/utils/analysis/calculation_plan.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/analysis/batch_processing/parallel_backed.py` & `PartSeg-0.9b2/package/PartSeg/utils/analysis/batch_processing/parallel_backed.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/analysis/batch_processing/batch_backend.py` & `PartSeg-0.9b2/package/PartSeg/utils/analysis/batch_processing/batch_backend.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/analysis/save_hooks.py` & `PartSeg-0.9b2/package/PartSeg/utils/analysis/save_hooks.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/analysis/algorithm_description.py` & `PartSeg-0.9b2/package/PartSeg/utils/analysis/algorithm_description.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/base_argparser.py` & `PartSeg-0.9b2/package/PartSeg/project_utils_qt/base_argparser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import argparse
 import sys
 import sentry_sdk
 from typing import Optional, Sequence, Text
-from . import report_utils
-from ..project_utils_qt.except_hook import my_excepthook
+from PartSeg.utils import state_store
+from PartSeg.project_utils_qt.except_hook import my_excepthook
 
 class CustomParser(argparse.ArgumentParser):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.add_argument("--no_report", action="store_false", help="disable error reporting")
         self.add_argument("--no_dialog", action="store_false", help="disable error reporting and showing error dialog")
+        self.add_argument("--inner_plugins", action="store_true", help=argparse.SUPPRESS)
 
     def parse_args(self, args: Optional[Sequence[Text]] = None,
                    namespace: Optional[argparse.Namespace] = None):
         args = super().parse_args(args, namespace)
-        print(args)
-        report_utils.report_errors = args.no_report
-        report_utils.show_error_dialog = args.no_dialog
+        state_store.report_errors = args.no_report
+        state_store.show_error_dialog = args.no_dialog
+        state_store.custom_plugin_load = args.inner_plugins
         if args.no_report and args.no_dialog:
             sentry_sdk.init("https://d4118280b73d4ee3a0222d0b17637687@sentry.io/1309302")
         sys.excepthook = my_excepthook
         return args
```

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/register.py` & `PartSeg-0.9b2/package/PartSeg/utils/register.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/segmentation/algorithm_base.py` & `PartSeg-0.9b2/package/PartSeg/utils/segmentation/algorithm_base.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/segmentation/algorithm_describe_base.py` & `PartSeg-0.9b2/package/PartSeg/utils/segmentation/algorithm_describe_base.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/segmentation/mu_mid_point.py` & `PartSeg-0.9b2/package/PartSeg/utils/segmentation/mu_mid_point.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/segmentation/segmentation_algorithm.py` & `PartSeg-0.9b2/package/PartSeg/utils/segmentation/segmentation_algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                 AlgorithmProperty("smooth_border", "Smooth borders", True, (True, False)),
                 AlgorithmProperty("smooth_border_radius", "Smooth borders radius", 2, (0, 20), 1),
                 AlgorithmProperty("noise_removal", "Filter", next(iter(noise_removal_dict.keys())),
                                   possible_values=noise_removal_dict, property_type=AlgorithmDescribeBase),
                 AlgorithmProperty("side_connection", "Side by Side connections", False, (True, False),
                                   tool_tip="During calculation of connected components includes"
                                            " only side by side connected pixels"),
-                AlgorithmProperty("use_convex", "Use convex_hull", False, (True, False))]
+                AlgorithmProperty("use_convex", "Use convex hull", False, (True, False))]
 
     def __init__(self):
         super().__init__()
         self.threshold = None
         self.minimum_size = None
         self.sizes = None
         self.noise_removal = None
```

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/segmentation/threshold.py` & `PartSeg-0.9b2/package/PartSeg/utils/segmentation/threshold.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,16 @@
 threshold_dict.register(MomentsThreshold)
 threshold_dict.register(MaximumEntropyThreshold)
 
 
 class DoubleThreshold(BaseThreshold):
     @classmethod
     def get_name(cls):
-        return "Double Choose"
+        # return "Double Choose"
+        return "Base/Core"
 
     @classmethod
     def get_fields(cls):
         return [AlgorithmProperty("core_threshold", "Core threshold", next(iter(threshold_dict.keys())),
                                   possible_values=threshold_dict, property_type=AlgorithmDescribeBase),
                 AlgorithmProperty("base_threshold", "Base threshold", next(iter(threshold_dict.keys())),
                                   possible_values=threshold_dict, property_type=AlgorithmDescribeBase)
```

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/segmentation/sprawl.py` & `PartSeg-0.9b2/package/PartSeg/utils/segmentation/sprawl.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,21 +107,21 @@
         mso.set_components(components_arr, components_num+1)
         mso.set_use_background(False)
         mu_array = calculate_mu(data.copy('C'), lower_bound, upper_bound, MuType.base_mu)
         if arguments["reflective"]:
             mu_array[mu_array < 0.5] = 1 - mu_array[mu_array < 0.5]
         mso.set_mu_array(mu_array)
         mso.run_MSO(arguments["step_limits"])
-        print("Steps: ", mso.steps_done(), file=sys.stderr)
+        # print("Steps: ", mso.steps_done(), file=sys.stderr)
         result = mso.get_result_catted()
         result[result > 0] -= 1
         return result
 
 
-sprawl_dict = Register(PathSprawl, DistanceSprawl, PathDistanceSprawl, FDTSprawl, MSOSprawl)
+sprawl_dict = Register(MSOSprawl, PathSprawl, DistanceSprawl, PathDistanceSprawl, FDTSprawl)
 
 
 def get_neigh(sides):
     if sides:
         return NeighType.sides
     else:
         return NeighType.edges
```

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/segmentation/segment.py` & `PartSeg-0.9b2/package/PartSeg/utils/segmentation/segment.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/segmentation/restartable_segmentation_algorithms.py` & `PartSeg-0.9b2/package/PartSeg/utils/segmentation/restartable_segmentation_algorithms.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/segmentation/noise_filtering.py` & `PartSeg-0.9b2/package/PartSeg/utils/segmentation/noise_filtering.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/fuzy_segment/fuzzy_segment_cython.pyx` & `PartSeg-0.9b2/package/PartSeg/utils/fuzy_segment/fuzzy_segment_cython.pyx`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/multiscale_opening/mso_bind.cpp` & `PartSeg-0.9b2/package/PartSeg/utils/multiscale_opening/mso_bind.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 /* Generated by Cython 0.29.3 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/Users/grzegorzbokota/.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/Users/grzegorzbokota/.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/Users/grzegorzbokota/.pyenv/versions/partseg/lib/python3.6/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/Users/grzegorzbokota/.pyenv/versions/partseg/lib/python3.6/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "package/PartSeg/utils/multiscale_opening/mso.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-Wall"
         ],
         "include_dirs": [
             "package/PartSeg/utils/multiscale_opening",
-            "/Users/grzegorzbokota/.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/numpy/core/include"
+            "/Users/grzegorzbokota/.pyenv/versions/partseg/lib/python3.6/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "PartSeg.utils.multiscale_opening.mso_bind",
         "sources": [
             "package/PartSeg/utils/multiscale_opening/mso_bind.pyx"
         ]
     },
@@ -927,26 +927,26 @@
   int is_complex;
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
-/* ForceInitThreads.proto */
-#ifndef __PYX_FORCE_INIT_THREADS
-  #define __PYX_FORCE_INIT_THREADS 0
-#endif
-
 /* NoFastGil.proto */
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
+/* ForceInitThreads.proto */
+#ifndef __PYX_FORCE_INIT_THREADS
+  #define __PYX_FORCE_INIT_THREADS 0
+#endif
+
 /* Atomics.proto */
 #include <pythread.h>
 #ifndef CYTHON_ATOMICS
     #define CYTHON_ATOMICS 1
 #endif
 #define __pyx_atomic_int_type int
 #if CYTHON_ATOMICS && __GNUC__ >= 4 && (__GNUC_MINOR__ > 1 ||\
@@ -1000,195 +1000,195 @@
   Py_ssize_t shape[8];
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":776
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":776
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":777
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":777
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":778
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":778
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":779
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":779
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":783
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":783
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":784
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":784
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":785
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":785
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":786
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":786
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":790
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":790
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":791
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":791
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":800
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":800
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":801
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":801
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":802
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":802
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":804
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":804
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":805
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":805
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":806
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":806
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":808
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":808
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":809
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":809
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":811
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":811
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":812
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":812
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":813
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":813
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1239,42 +1239,42 @@
 struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO;
 struct __pyx_obj___Pyx_EnumMeta;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":815
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":815
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":816
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":816
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":817
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":817
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":819
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":819
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3181,15 +3181,15 @@
 static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_38set_image(struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self, PyArrayObject *__pyx_v_image, __pyx_t_5numpy_float64_t __pyx_v_lower_bound, __pyx_t_5numpy_float64_t __pyx_v_upper_bound, enum __pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_MuType __pyx_v_type_, PyObject *__pyx_v_mask, __pyx_t_5numpy_float64_t __pyx_v_lower_mid_bound, __pyx_t_5numpy_float64_t __pyx_v_upper_mid_bound); /* proto */
 static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_2set_mu_array(struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self, PyArrayObject *__pyx_v_mu); /* proto */
 static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_4set_components(struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self, PyArrayObject *__pyx_v_components, PyObject *__pyx_v_component_num); /* proto */
 static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_6set_neighbourhood(struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self, PyArrayObject *__pyx_v_neighbourhood, PyArrayObject *__pyx_v_distances); /* proto */
 static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_8calculate_FDT(struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_10optimum_erosion_calculate(struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self, PyArrayObject *__pyx_v_fdt_array, PyArrayObject *__pyx_v_components_arr, PyArrayObject *__pyx_v_sprawl_area); /* proto */
 static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_12constrained_dilation(struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self, PyArrayObject *__pyx_v_fdt_array, PyArrayObject *__pyx_v_components_arr, PyArrayObject *__pyx_v_sprawl_area); /* proto */
-static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_14run_MSO(struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self, PyObject *__pyx_v_step_limits); /* proto */
+static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_14run_MSO(struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self, size_t __pyx_v_step_limits); /* proto */
 static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_16steps_done(struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_18set_components_num(struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self, PyObject *__pyx_v_num); /* proto */
 static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_20get_result_catted(struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_22get_fdt(struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_24set_use_background(struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self, PyObject *__pyx_v_use); /* proto */
 static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_42__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_44__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
@@ -14255,15 +14255,15 @@
   __pyx_t_13 = 0;
 
   /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":207
  *         res = numpy.array(components, dtype=np_component_type)
  *         res = res.reshape([components_arr.shape[i] for i in range(components_arr.ndim)])
  *         return res             # <<<<<<<<<<<<<<
  * 
- *     def run_MSO(self, step_limits=1):
+ *     def run_MSO(self, size_t step_limits=1):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_res);
   __pyx_r = __pyx_v_res;
   goto __pyx_L0;
 
   /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":186
@@ -14304,30 +14304,29 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":209
  *         return res
  * 
- *     def run_MSO(self, step_limits=1):             # <<<<<<<<<<<<<<
- *         return self.mso.run_MSO(step_limits)
- * 
+ *     def run_MSO(self, size_t step_limits=1):             # <<<<<<<<<<<<<<
+ *         cdef size_t val
+ *         with nogil:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_15run_MSO(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_15run_MSO(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyObject *__pyx_v_step_limits = 0;
+  size_t __pyx_v_step_limits;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("run_MSO (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_step_limits,0};
     PyObject* values[1] = {0};
-    values[0] = ((PyObject *)__pyx_int_1);
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
@@ -14348,15 +14347,19 @@
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_step_limits = values[0];
+    if (values[0]) {
+      __pyx_v_step_limits = __Pyx_PyInt_As_size_t(values[0]); if (unlikely((__pyx_v_step_limits == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 209, __pyx_L3_error)
+    } else {
+      __pyx_v_step_limits = ((size_t)1);
+    }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("run_MSO", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 209, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("PartSeg.utils.multiscale_opening.mso_bind.PyMSO.run_MSO", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
@@ -14365,64 +14368,120 @@
   __pyx_r = __pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_14run_MSO(((struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *)__pyx_v_self), __pyx_v_step_limits);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_14run_MSO(struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self, PyObject *__pyx_v_step_limits) {
+static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_14run_MSO(struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self, size_t __pyx_v_step_limits) {
+  size_t __pyx_v_val;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   size_t __pyx_t_1;
-  size_t __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("run_MSO", 0);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":210
- * 
- *     def run_MSO(self, step_limits=1):
- *         return self.mso.run_MSO(step_limits)             # <<<<<<<<<<<<<<
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":211
+ *     def run_MSO(self, size_t step_limits=1):
+ *         cdef size_t val
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             val = self.mso.run_MSO(step_limits)
+ *         return val
+ */
+  {
+      #ifdef WITH_THREAD
+      PyThreadState *_save;
+      Py_UNBLOCK_THREADS
+      __Pyx_FastGIL_Remember();
+      #endif
+      /*try:*/ {
+
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":212
+ *         cdef size_t val
+ *         with nogil:
+ *             val = self.mso.run_MSO(step_limits)             # <<<<<<<<<<<<<<
+ *         return val
+ * 
+ */
+        try {
+          __pyx_t_1 = __pyx_v_self->mso.run_MSO(__pyx_v_step_limits);
+        } catch(...) {
+          #ifdef WITH_THREAD
+          PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+          #endif
+          __Pyx_CppExn2PyErr();
+          #ifdef WITH_THREAD
+          __Pyx_PyGILState_Release(__pyx_gilstate_save);
+          #endif
+          __PYX_ERR(0, 212, __pyx_L4_error)
+        }
+        __pyx_v_val = __pyx_t_1;
+      }
+
+      /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":211
+ *     def run_MSO(self, size_t step_limits=1):
+ *         cdef size_t val
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             val = self.mso.run_MSO(step_limits)
+ *         return val
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L4_error: {
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L1_error;
+        }
+        __pyx_L5:;
+      }
+  }
+
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":213
+ *         with nogil:
+ *             val = self.mso.run_MSO(step_limits)
+ *         return val             # <<<<<<<<<<<<<<
  * 
  *     def steps_done(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_size_t(__pyx_v_step_limits); if (unlikely((__pyx_t_1 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L1_error)
-  try {
-    __pyx_t_2 = __pyx_v_self->mso.run_MSO(__pyx_t_1);
-  } catch(...) {
-    __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 210, __pyx_L1_error)
-  }
-  __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 210, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_r = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_val); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":209
  *         return res
  * 
- *     def run_MSO(self, step_limits=1):             # <<<<<<<<<<<<<<
- *         return self.mso.run_MSO(step_limits)
- * 
+ *     def run_MSO(self, size_t step_limits=1):             # <<<<<<<<<<<<<<
+ *         cdef size_t val
+ *         with nogil:
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_AddTraceback("PartSeg.utils.multiscale_opening.mso_bind.PyMSO.run_MSO", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "PartSeg/utils/multiscale_opening/mso_bind.pyx":212
- *         return self.mso.run_MSO(step_limits)
+/* "PartSeg/utils/multiscale_opening/mso_bind.pyx":215
+ *         return val
  * 
  *     def steps_done(self):             # <<<<<<<<<<<<<<
  *         return self.mso.steps_done()
  * 
  */
 
 /* Python wrapper */
@@ -14440,30 +14499,30 @@
 
 static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_16steps_done(struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("steps_done", 0);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":213
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":216
  * 
  *     def steps_done(self):
  *         return self.mso.steps_done()             # <<<<<<<<<<<<<<
  * 
  *     def set_components_num(self, num):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_self->mso.steps_done()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_self->mso.steps_done()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":212
- *         return self.mso.run_MSO(step_limits)
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":215
+ *         return val
  * 
  *     def steps_done(self):             # <<<<<<<<<<<<<<
  *         return self.mso.steps_done()
  * 
  */
 
   /* function exit code */
@@ -14473,15 +14532,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "PartSeg/utils/multiscale_opening/mso_bind.pyx":215
+/* "PartSeg/utils/multiscale_opening/mso_bind.pyx":218
  *         return self.mso.steps_done()
  * 
  *     def set_components_num(self, num):             # <<<<<<<<<<<<<<
  *         self.mso.set_components_num(num+2)
  * 
  */
 
@@ -14501,28 +14560,28 @@
 static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_18set_components_num(struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self, PyObject *__pyx_v_num) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_component_type __pyx_t_2;
   __Pyx_RefNannySetupContext("set_components_num", 0);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":216
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":219
  * 
  *     def set_components_num(self, num):
  *         self.mso.set_components_num(num+2)             # <<<<<<<<<<<<<<
  * 
  *     def get_result_catted(self):
  */
-  __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_num, __pyx_int_2, 2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_num, __pyx_int_2, 2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_npy_uint8(__pyx_t_1); if (unlikely((__pyx_t_2 == ((npy_uint8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_npy_uint8(__pyx_t_1); if (unlikely((__pyx_t_2 == ((npy_uint8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_self->mso.set_components_num(__pyx_t_2);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":215
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":218
  *         return self.mso.steps_done()
  * 
  *     def set_components_num(self, num):             # <<<<<<<<<<<<<<
  *         self.mso.set_components_num(num+2)
  * 
  */
 
@@ -14535,15 +14594,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "PartSeg/utils/multiscale_opening/mso_bind.pyx":218
+/* "PartSeg/utils/multiscale_opening/mso_bind.pyx":221
  *         self.mso.set_components_num(num+2)
  * 
  *     def get_result_catted(self):             # <<<<<<<<<<<<<<
  *         cdef vector[component_type] res = self.mso.get_result_catted()
  *         res_arr = numpy.array(res, dtype=np_component_type)
  */
 
@@ -14571,75 +14630,75 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_t_7;
   __Pyx_RefNannySetupContext("get_result_catted", 0);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":219
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":222
  * 
  *     def get_result_catted(self):
  *         cdef vector[component_type] res = self.mso.get_result_catted()             # <<<<<<<<<<<<<<
  *         res_arr = numpy.array(res, dtype=np_component_type)
  *         res_arr = res_arr.reshape([self.components.shape[i] for i in range(self.components.ndim)])
  */
   __pyx_v_res = ((std::vector<__pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_component_type> )__pyx_v_self->mso.get_result_catted());
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":220
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":223
  *     def get_result_catted(self):
  *         cdef vector[component_type] res = self.mso.get_result_catted()
  *         res_arr = numpy.array(res, dtype=np_component_type)             # <<<<<<<<<<<<<<
  *         res_arr = res_arr.reshape([self.components.shape[i] for i in range(self.components.ndim)])
  *         return res_arr
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_convert_vector_to_py___pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_component_type(__pyx_v_res); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_to_py___pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_component_type(__pyx_v_res); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np_component_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np_component_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_res_arr = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":221
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":224
  *         cdef vector[component_type] res = self.mso.get_result_catted()
  *         res_arr = numpy.array(res, dtype=np_component_type)
  *         res_arr = res_arr.reshape([self.components.shape[i] for i in range(self.components.ndim)])             # <<<<<<<<<<<<<<
  *         return res_arr
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_res_arr, __pyx_n_s_reshape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_res_arr, __pyx_n_s_reshape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   { /* enter inner scope */
-    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 224, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = __pyx_v_self->components->nd;
     __pyx_t_6 = __pyx_t_5;
     for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
       __pyx_8genexpr2__pyx_v_i = __pyx_t_7;
-      __pyx_t_2 = __Pyx_PyInt_From_Py_intptr_t((__pyx_v_self->components->dimensions[__pyx_8genexpr2__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 221, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyInt_From_Py_intptr_t((__pyx_v_self->components->dimensions[__pyx_8genexpr2__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 224, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 221, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 224, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
   } /* exit inner scope */
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_2)) {
@@ -14648,33 +14707,33 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 221, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF_SET(__pyx_v_res_arr, __pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":222
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":225
  *         res_arr = numpy.array(res, dtype=np_component_type)
  *         res_arr = res_arr.reshape([self.components.shape[i] for i in range(self.components.ndim)])
  *         return res_arr             # <<<<<<<<<<<<<<
  * 
  *     def get_fdt(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_res_arr);
   __pyx_r = __pyx_v_res_arr;
   goto __pyx_L0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":218
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":221
  *         self.mso.set_components_num(num+2)
  * 
  *     def get_result_catted(self):             # <<<<<<<<<<<<<<
  *         cdef vector[component_type] res = self.mso.get_result_catted()
  *         res_arr = numpy.array(res, dtype=np_component_type)
  */
 
@@ -14689,15 +14748,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_res_arr);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "PartSeg/utils/multiscale_opening/mso_bind.pyx":224
+/* "PartSeg/utils/multiscale_opening/mso_bind.pyx":227
  *         return res_arr
  * 
  *     def get_fdt(self):             # <<<<<<<<<<<<<<
  *         cdef vector[mu_type] res = self.mso.get_fdt()
  *         res_arr = numpy.array(res, dtype=numpy.float64)
  */
 
@@ -14726,78 +14785,78 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_t_7;
   int __pyx_t_8;
   __Pyx_RefNannySetupContext("get_fdt", 0);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":225
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":228
  * 
  *     def get_fdt(self):
  *         cdef vector[mu_type] res = self.mso.get_fdt()             # <<<<<<<<<<<<<<
  *         res_arr = numpy.array(res, dtype=numpy.float64)
  *         res_arr = res_arr.reshape([self.components.shape[i] for i in range(self.components.ndim)])
  */
   __pyx_v_res = __pyx_v_self->mso.get_fdt();
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":226
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":229
  *     def get_fdt(self):
  *         cdef vector[mu_type] res = self.mso.get_fdt()
  *         res_arr = numpy.array(res, dtype=numpy.float64)             # <<<<<<<<<<<<<<
  *         res_arr = res_arr.reshape([self.components.shape[i] for i in range(self.components.ndim)])
  *         return res_arr
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_convert_vector_to_py___pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_mu_type(__pyx_v_res); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_to_py___pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_mu_type(__pyx_v_res); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 226, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_res_arr = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":227
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":230
  *         cdef vector[mu_type] res = self.mso.get_fdt()
  *         res_arr = numpy.array(res, dtype=numpy.float64)
  *         res_arr = res_arr.reshape([self.components.shape[i] for i in range(self.components.ndim)])             # <<<<<<<<<<<<<<
  *         return res_arr
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_res_arr, __pyx_n_s_reshape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_res_arr, __pyx_n_s_reshape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 230, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   { /* enter inner scope */
-    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 227, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 230, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_6 = __pyx_v_self->components->nd;
     __pyx_t_7 = __pyx_t_6;
     for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
       __pyx_8genexpr3__pyx_v_i = __pyx_t_8;
-      __pyx_t_2 = __Pyx_PyInt_From_Py_intptr_t((__pyx_v_self->components->dimensions[__pyx_8genexpr3__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 227, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyInt_From_Py_intptr_t((__pyx_v_self->components->dimensions[__pyx_8genexpr3__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 230, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 227, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 230, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
   } /* exit inner scope */
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_2)) {
@@ -14806,33 +14865,33 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_5 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 227, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 230, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF_SET(__pyx_v_res_arr, __pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":228
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":231
  *         res_arr = numpy.array(res, dtype=numpy.float64)
  *         res_arr = res_arr.reshape([self.components.shape[i] for i in range(self.components.ndim)])
  *         return res_arr             # <<<<<<<<<<<<<<
  * 
  *     def set_use_background(self, use):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_res_arr);
   __pyx_r = __pyx_v_res_arr;
   goto __pyx_L0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":224
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":227
  *         return res_arr
  * 
  *     def get_fdt(self):             # <<<<<<<<<<<<<<
  *         cdef vector[mu_type] res = self.mso.get_fdt()
  *         res_arr = numpy.array(res, dtype=numpy.float64)
  */
 
@@ -14848,15 +14907,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_res_arr);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "PartSeg/utils/multiscale_opening/mso_bind.pyx":230
+/* "PartSeg/utils/multiscale_opening/mso_bind.pyx":233
  *         return res_arr
  * 
  *     def set_use_background(self, use):             # <<<<<<<<<<<<<<
  *         self.mso.set_use_background(use)
  * 
  */
 
@@ -14875,25 +14934,25 @@
 
 static PyObject *__pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_5PyMSO_24set_use_background(struct __pyx_obj_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO *__pyx_v_self, PyObject *__pyx_v_use) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   bool __pyx_t_1;
   __Pyx_RefNannySetupContext("set_use_background", 0);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":231
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":234
  * 
  *     def set_use_background(self, use):
  *         self.mso.set_use_background(use)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_use); if (unlikely((__pyx_t_1 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 231, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_use); if (unlikely((__pyx_t_1 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 234, __pyx_L1_error)
   __pyx_v_self->mso.set_use_background(__pyx_t_1);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":230
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":233
  *         return res_arr
  * 
  *     def set_use_background(self, use):             # <<<<<<<<<<<<<<
  *         self.mso.set_use_background(use)
  * 
  */
 
@@ -15012,15 +15071,15 @@
   __Pyx_AddTraceback("PartSeg.utils.multiscale_opening.mso_bind.PyMSO.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "PartSeg/utils/multiscale_opening/mso_bind.pyx":235
+/* "PartSeg/utils/multiscale_opening/mso_bind.pyx":238
  * 
  * @cython.boundscheck(False)
  * def calculate_mu_mid(numpy.ndarray[image_types, ndim=3] image, image_types lower_bound, image_types mid_point,             # <<<<<<<<<<<<<<
  *                  image_types upper_bound):
  *     cdef int16_t x_size, y_size, z_size, x, y, z
  */
 
@@ -15058,31 +15117,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signatures)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_args)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 1); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 1); __PYX_ERR(0, 238, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_kwargs)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 2); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 2); __PYX_ERR(0, 238, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_defaults)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 3); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 3); __PYX_ERR(0, 238, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fused_cpdef") < 0)) __PYX_ERR(0, 235, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fused_cpdef") < 0)) __PYX_ERR(0, 238, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -15091,15 +15150,15 @@
     __pyx_v_signatures = values[0];
     __pyx_v_args = values[1];
     __pyx_v_kwargs = values[2];
     __pyx_v_defaults = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 235, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 238, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("PartSeg.utils.multiscale_opening.mso_bind.__pyx_fused_cpdef", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_2calculate_mu_mid(__pyx_self, __pyx_v_signatures, __pyx_v_args, __pyx_v_kwargs, __pyx_v_defaults);
 
@@ -15147,56 +15206,56 @@
   PyObject *__pyx_t_14 = NULL;
   Py_ssize_t __pyx_t_15;
   Py_ssize_t __pyx_t_16;
   Py_ssize_t __pyx_t_17;
   int __pyx_t_18;
   __Pyx_RefNannySetupContext("calculate_mu_mid", 0);
   __Pyx_INCREF(__pyx_v_kwargs);
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyList_SET_ITEM(__pyx_t_1, 0, Py_None);
   __pyx_v_dest_sig = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_v_kwargs != Py_None);
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_kwargs); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_kwargs); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 238, __pyx_L1_error)
   __pyx_t_3 = ((!__pyx_t_4) != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_2) {
     __Pyx_INCREF(Py_None);
     __Pyx_DECREF_SET(__pyx_v_kwargs, Py_None);
   }
-  __pyx_t_1 = ((PyObject *)__Pyx_ImportNumPyArrayTypeIfAvailable()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__Pyx_ImportNumPyArrayTypeIfAvailable()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_ndarray = ((PyTypeObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   __pyx_v_itemsize = -1L;
   __pyx_v____pyx_int8_t_is_signed = (!((((__pyx_t_5numpy_int8_t)-1L) > 0) != 0));
   __pyx_v____pyx_int16_t_is_signed = (!((((__pyx_t_5numpy_int16_t)-1L) > 0) != 0));
   __pyx_v____pyx_uint8_t_is_signed = (!((((__pyx_t_5numpy_uint8_t)-1L) > 0) != 0));
   __pyx_v____pyx_uint16_t_is_signed = (!((((__pyx_t_5numpy_uint16_t)-1L) > 0) != 0));
   __pyx_v____pyx_uint32_t_is_signed = (!((((__pyx_t_5numpy_uint32_t)-1L) > 0) != 0));
   if (unlikely(__pyx_v_args == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 235, __pyx_L1_error)
+    __PYX_ERR(0, 238, __pyx_L1_error)
   }
-  __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 238, __pyx_L1_error)
   __pyx_t_2 = ((0 < __pyx_t_5) != 0);
   if (__pyx_t_2) {
     if (unlikely(__pyx_v_args == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 235, __pyx_L1_error)
+      __PYX_ERR(0, 238, __pyx_L1_error)
     }
     __pyx_t_1 = PyTuple_GET_ITEM(((PyObject*)__pyx_v_args), 0);
     __Pyx_INCREF(__pyx_t_1);
     __pyx_v_arg = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L6;
   }
@@ -15205,85 +15264,85 @@
   if (__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L7_bool_binop_done;
   }
   if (unlikely(__pyx_v_kwargs == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 235, __pyx_L1_error)
+    __PYX_ERR(0, 238, __pyx_L1_error)
   }
-  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_image, ((PyObject*)__pyx_v_kwargs), Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_image, ((PyObject*)__pyx_v_kwargs), Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 238, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_4 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L7_bool_binop_done:;
   if (__pyx_t_2) {
     if (unlikely(__pyx_v_kwargs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 235, __pyx_L1_error)
+      __PYX_ERR(0, 238, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_kwargs), __pyx_n_s_image); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_kwargs), __pyx_n_s_image); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_arg = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L6;
   }
   /*else*/ {
     if (unlikely(__pyx_v_args == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 235, __pyx_L1_error)
+      __PYX_ERR(0, 238, __pyx_L1_error)
     }
-    __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 235, __pyx_L1_error)
-    __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 238, __pyx_L1_error)
+    __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_int_4);
     __Pyx_GIVEREF(__pyx_int_4);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_int_4);
     __Pyx_INCREF(__pyx_n_s_s);
     __Pyx_GIVEREF(__pyx_n_s_s);
     PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_n_s_s);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_Expected_at_least_d_argument_s_g, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_Expected_at_least_d_argument_s_g, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 235, __pyx_L1_error)
+    __PYX_ERR(0, 238, __pyx_L1_error)
   }
   __pyx_L6:;
   while (1) {
     __pyx_t_2 = (__pyx_v_ndarray != ((PyTypeObject*)Py_None));
     __pyx_t_3 = (__pyx_t_2 != 0);
     if (__pyx_t_3) {
       __pyx_t_3 = __Pyx_TypeCheck(__pyx_v_arg, __pyx_v_ndarray); 
       __pyx_t_2 = (__pyx_t_3 != 0);
       if (__pyx_t_2) {
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_dtype = __pyx_t_6;
         __pyx_t_6 = 0;
         goto __pyx_L12;
       }
       __pyx_t_2 = __pyx_memoryview_check(__pyx_v_arg); 
       __pyx_t_3 = (__pyx_t_2 != 0);
       if (__pyx_t_3) {
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_base); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_base); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_arg_base = __pyx_t_6;
         __pyx_t_6 = 0;
         __pyx_t_3 = __Pyx_TypeCheck(__pyx_v_arg_base, __pyx_v_ndarray); 
         __pyx_t_2 = (__pyx_t_3 != 0);
         if (__pyx_t_2) {
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg_base, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg_base, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           __pyx_v_dtype = __pyx_t_6;
           __pyx_t_6 = 0;
           goto __pyx_L13;
         }
         /*else*/ {
           __Pyx_INCREF(Py_None);
@@ -15297,177 +15356,177 @@
         __pyx_v_dtype = Py_None;
       }
       __pyx_L12:;
       __pyx_v_itemsize = -1L;
       __pyx_t_2 = (__pyx_v_dtype != Py_None);
       __pyx_t_3 = (__pyx_t_2 != 0);
       if (__pyx_t_3) {
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_itemsize); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_itemsize); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_v_itemsize = __pyx_t_5;
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_kind); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_kind); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_7 = __Pyx_PyObject_Ord(__pyx_t_6); if (unlikely(__pyx_t_7 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 235, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyObject_Ord(__pyx_t_6); if (unlikely(__pyx_t_7 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 238, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_v_kind = __pyx_t_7;
         __pyx_v_dtype_signed = (__pyx_v_kind == 'i');
         switch (__pyx_v_kind) {
           case 'i':
           case 'u':
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_int8_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L16_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 3) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L16_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_int8_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L16_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 238, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_int16_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L20_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 3) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L20_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_int16_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L20_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 238, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_uint8_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L24_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 3) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L24_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_uint8_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L24_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 238, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_uint16_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L28_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 3) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L28_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_uint16_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L28_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 238, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_uint32_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L32_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 3) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L32_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_uint32_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L32_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 238, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           break;
           case 'f':
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_float32_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L36_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 3) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L36_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 238, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_float64_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L39_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 3) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L39_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 238, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           break;
           case 'c':
           break;
           case 'O':
           break;
@@ -15486,15 +15545,15 @@
     __pyx_L42_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_nn___pyx_t_5numpy_int8_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 238, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -15508,15 +15567,15 @@
     __pyx_L46_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_nn___pyx_t_5numpy_int16_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 238, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -15530,15 +15589,15 @@
     __pyx_L50_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_nn___pyx_t_5numpy_uint8_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 238, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -15552,15 +15611,15 @@
     __pyx_L54_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_nn___pyx_t_5numpy_uint16_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 238, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -15574,15 +15633,15 @@
     __pyx_L58_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_nn___pyx_t_5numpy_uint32_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 238, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -15596,15 +15655,15 @@
     __pyx_L62_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_nn___pyx_t_5numpy_float32_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 238, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -15618,100 +15677,100 @@
     __pyx_L66_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_nn___pyx_t_5numpy_float64_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 238, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, Py_None, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, Py_None, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 238, __pyx_L1_error)
     goto __pyx_L10_break;
   }
   __pyx_L10_break:;
-  __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_v_candidates = ((PyObject*)__pyx_t_6);
   __pyx_t_6 = 0;
   __pyx_t_5 = 0;
   if (unlikely(__pyx_v_signatures == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 235, __pyx_L1_error)
+    __PYX_ERR(0, 238, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_dict_iterator(((PyObject*)__pyx_v_signatures), 1, ((PyObject *)NULL), (&__pyx_t_9), (&__pyx_t_10)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_dict_iterator(((PyObject*)__pyx_v_signatures), 1, ((PyObject *)NULL), (&__pyx_t_9), (&__pyx_t_10)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_6);
   __pyx_t_6 = __pyx_t_1;
   __pyx_t_1 = 0;
   while (1) {
     __pyx_t_11 = __Pyx_dict_iter_next(__pyx_t_6, __pyx_t_9, &__pyx_t_5, &__pyx_t_1, NULL, NULL, __pyx_t_10);
     if (unlikely(__pyx_t_11 == 0)) break;
-    if (unlikely(__pyx_t_11 == -1)) __PYX_ERR(0, 235, __pyx_L1_error)
+    if (unlikely(__pyx_t_11 == -1)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_sig, __pyx_t_1);
     __pyx_t_1 = 0;
     __pyx_v_match_found = 0;
-    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_sig, __pyx_n_s_strip); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 235, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_sig, __pyx_n_s_strip); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     __pyx_t_14 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_13))) {
       __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_13);
       if (likely(__pyx_t_14)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
         __Pyx_INCREF(__pyx_t_14);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_13, function);
       }
     }
     __pyx_t_12 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_13, __pyx_t_14, __pyx_kp_s__22) : __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_kp_s__22);
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-    if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 235, __pyx_L1_error)
+    if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_split); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 235, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_split); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     __pyx_t_12 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_13))) {
       __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_13);
       if (likely(__pyx_t_12)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
         __Pyx_INCREF(__pyx_t_12);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_13, function);
       }
     }
     __pyx_t_1 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_13, __pyx_t_12, __pyx_kp_s__23) : __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_kp_s__23);
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
     __Pyx_XDECREF_SET(__pyx_v_src_sig, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_15 = PyList_GET_SIZE(__pyx_v_dest_sig); if (unlikely(__pyx_t_15 == ((Py_ssize_t)-1))) __PYX_ERR(0, 235, __pyx_L1_error)
+    __pyx_t_15 = PyList_GET_SIZE(__pyx_v_dest_sig); if (unlikely(__pyx_t_15 == ((Py_ssize_t)-1))) __PYX_ERR(0, 238, __pyx_L1_error)
     __pyx_t_16 = __pyx_t_15;
     for (__pyx_t_17 = 0; __pyx_t_17 < __pyx_t_16; __pyx_t_17+=1) {
       __pyx_v_i = __pyx_t_17;
-      __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_dest_sig, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_dest_sig, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_XDECREF_SET(__pyx_v_dst_type, __pyx_t_1);
       __pyx_t_1 = 0;
       __pyx_t_3 = (__pyx_v_dst_type != Py_None);
       __pyx_t_2 = (__pyx_t_3 != 0);
       if (__pyx_t_2) {
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_src_sig, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_src_sig, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_13 = PyObject_RichCompare(__pyx_t_1, __pyx_v_dst_type, Py_EQ); __Pyx_XGOTREF(__pyx_t_13); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 235, __pyx_L1_error)
+        __pyx_t_13 = PyObject_RichCompare(__pyx_t_1, __pyx_v_dst_type, Py_EQ); __Pyx_XGOTREF(__pyx_t_13); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 238, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_13); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_13); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 238, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         if (__pyx_t_2) {
           __pyx_v_match_found = 1;
           goto __pyx_L74;
         }
         /*else*/ {
           __pyx_v_match_found = 0;
@@ -15719,43 +15778,43 @@
         }
         __pyx_L74:;
       }
     }
     __pyx_L72_break:;
     __pyx_t_2 = (__pyx_v_match_found != 0);
     if (__pyx_t_2) {
-      __pyx_t_18 = __Pyx_PyList_Append(__pyx_v_candidates, __pyx_v_sig); if (unlikely(__pyx_t_18 == ((int)-1))) __PYX_ERR(0, 235, __pyx_L1_error)
+      __pyx_t_18 = __Pyx_PyList_Append(__pyx_v_candidates, __pyx_v_sig); if (unlikely(__pyx_t_18 == ((int)-1))) __PYX_ERR(0, 238, __pyx_L1_error)
     }
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_2 = (PyList_GET_SIZE(__pyx_v_candidates) != 0);
   __pyx_t_3 = ((!__pyx_t_2) != 0);
   if (__pyx_t_3) {
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 235, __pyx_L1_error)
+    __PYX_ERR(0, 238, __pyx_L1_error)
   }
-  __pyx_t_9 = PyList_GET_SIZE(__pyx_v_candidates); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_9 = PyList_GET_SIZE(__pyx_v_candidates); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 238, __pyx_L1_error)
   __pyx_t_3 = ((__pyx_t_9 > 1) != 0);
   if (__pyx_t_3) {
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 235, __pyx_L1_error)
+    __PYX_ERR(0, 238, __pyx_L1_error)
   }
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     if (unlikely(__pyx_v_signatures == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 235, __pyx_L1_error)
+      __PYX_ERR(0, 238, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_signatures), PyList_GET_ITEM(__pyx_v_candidates, 0)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_signatures), PyList_GET_ITEM(__pyx_v_candidates, 0)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_r = __pyx_t_6;
     __pyx_t_6 = 0;
     goto __pyx_L0;
   }
 
   /* function exit code */
@@ -15817,54 +15876,54 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_image)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_lower_bound)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 1); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 1); __PYX_ERR(0, 238, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mid_point)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 2); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 2); __PYX_ERR(0, 238, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_upper_bound)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 3); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 3); __PYX_ERR(0, 238, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "calculate_mu_mid") < 0)) __PYX_ERR(0, 235, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "calculate_mu_mid") < 0)) __PYX_ERR(0, 238, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
     __pyx_v_image = ((PyArrayObject *)values[0]);
-    __pyx_v_lower_bound = __Pyx_PyInt_As_npy_int8(values[1]); if (unlikely((__pyx_v_lower_bound == ((npy_int8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L3_error)
-    __pyx_v_mid_point = __Pyx_PyInt_As_npy_int8(values[2]); if (unlikely((__pyx_v_mid_point == ((npy_int8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L3_error)
-    __pyx_v_upper_bound = __Pyx_PyInt_As_npy_int8(values[3]); if (unlikely((__pyx_v_upper_bound == ((npy_int8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 236, __pyx_L3_error)
+    __pyx_v_lower_bound = __Pyx_PyInt_As_npy_int8(values[1]); if (unlikely((__pyx_v_lower_bound == ((npy_int8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L3_error)
+    __pyx_v_mid_point = __Pyx_PyInt_As_npy_int8(values[2]); if (unlikely((__pyx_v_mid_point == ((npy_int8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L3_error)
+    __pyx_v_upper_bound = __Pyx_PyInt_As_npy_int8(values[3]); if (unlikely((__pyx_v_upper_bound == ((npy_int8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 239, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 235, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 238, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("PartSeg.utils.multiscale_opening.mso_bind.calculate_mu_mid", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_image), __pyx_ptype_5numpy_ndarray, 1, "image", 0))) __PYX_ERR(0, 235, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_image), __pyx_ptype_5numpy_ndarray, 1, "image", 0))) __PYX_ERR(0, 238, __pyx_L1_error)
   __pyx_r = __pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_20calculate_mu_mid(__pyx_self, __pyx_v_image, __pyx_v_lower_bound, __pyx_v_mid_point, __pyx_v_upper_bound);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -15920,316 +15979,316 @@
   __pyx_pybuffernd_res.rcbuffer = &__pyx_pybuffer_res;
   __pyx_pybuffer_image.pybuffer.buf = NULL;
   __pyx_pybuffer_image.refcount = 0;
   __pyx_pybuffernd_image.data = NULL;
   __pyx_pybuffernd_image.rcbuffer = &__pyx_pybuffer_image;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_image.rcbuffer->pybuffer, (PyObject*)__pyx_v_image, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int8_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 235, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_image.rcbuffer->pybuffer, (PyObject*)__pyx_v_image, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int8_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 238, __pyx_L1_error)
   }
   __pyx_pybuffernd_image.diminfo[0].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_image.diminfo[0].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_image.diminfo[1].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_image.diminfo[1].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_image.diminfo[2].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_image.diminfo[2].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[2];
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":240
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":243
  *     cdef mu_type res_val
  *     cdef image_types point_val
  *     x_size = image.shape[2]             # <<<<<<<<<<<<<<
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]
  */
   __pyx_v_x_size = (__pyx_v_image->dimensions[2]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":241
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
  *     cdef image_types point_val
  *     x_size = image.shape[2]
  *     y_size = image.shape[1]             # <<<<<<<<<<<<<<
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  */
   __pyx_v_y_size = (__pyx_v_image->dimensions[1]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":242
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":245
  *     x_size = image.shape[2]
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:
  */
   __pyx_v_z_size = (__pyx_v_image->dimensions[0]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":243
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":246
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)             # <<<<<<<<<<<<<<
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_npy_int16(__pyx_v_z_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_npy_int16(__pyx_v_z_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_From_npy_int16(__pyx_v_y_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_npy_int16(__pyx_v_y_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_npy_int16(__pyx_v_x_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_npy_int16(__pyx_v_x_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_4);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 246, __pyx_L1_error)
   __pyx_t_6 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_res.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_mu_type, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 3, 0, __pyx_stack) == -1)) {
       __pyx_v_res = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_res.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 243, __pyx_L1_error)
+      __PYX_ERR(0, 246, __pyx_L1_error)
     } else {__pyx_pybuffernd_res.diminfo[0].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_res.diminfo[0].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_res.diminfo[1].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_res.diminfo[1].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_res.diminfo[2].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_res.diminfo[2].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[2];
     }
   }
   __pyx_t_6 = 0;
   __pyx_v_res = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:             # <<<<<<<<<<<<<<
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  */
   __pyx_t_7 = ((__pyx_v_upper_bound < __pyx_v_lower_bound) != 0);
   if (__pyx_t_7) {
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":245
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":248
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound             # <<<<<<<<<<<<<<
  *         lower_bound = upper_bound
  *         upper_bound = tmp
  */
     __pyx_v_tmp = __pyx_v_lower_bound;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":246
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":249
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound
  *         lower_bound = upper_bound             # <<<<<<<<<<<<<<
  *         upper_bound = tmp
  * 
  */
     __pyx_v_lower_bound = __pyx_v_upper_bound;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":250
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  *         upper_bound = tmp             # <<<<<<<<<<<<<<
  * 
  *     for z in range(z_size):
  */
     __pyx_v_upper_bound = __pyx_v_tmp;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:             # <<<<<<<<<<<<<<
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  */
   }
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":249
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":252
  *         upper_bound = tmp
  * 
  *     for z in range(z_size):             # <<<<<<<<<<<<<<
  *         for y in range(y_size):
  *             for x in range(x_size):
  */
   __pyx_t_8 = __pyx_v_z_size;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_z = __pyx_t_10;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":250
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
  * 
  *     for z in range(z_size):
  *         for y in range(y_size):             # <<<<<<<<<<<<<<
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  */
     __pyx_t_11 = __pyx_v_y_size;
     __pyx_t_12 = __pyx_t_11;
     for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
       __pyx_v_y = __pyx_t_13;
 
-      /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":251
+      /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":254
  *     for z in range(z_size):
  *         for y in range(y_size):
  *             for x in range(x_size):             # <<<<<<<<<<<<<<
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:
  */
       __pyx_t_14 = __pyx_v_x_size;
       __pyx_t_15 = __pyx_t_14;
       for (__pyx_t_16 = 0; __pyx_t_16 < __pyx_t_15; __pyx_t_16+=1) {
         __pyx_v_x = __pyx_t_16;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":252
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":255
  *         for y in range(y_size):
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]             # <<<<<<<<<<<<<<
  *                 if point_val < mid_point:
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  */
         __pyx_t_17 = __pyx_v_z;
         __pyx_t_18 = __pyx_v_y;
         __pyx_t_19 = __pyx_v_x;
         if (__pyx_t_17 < 0) __pyx_t_17 += __pyx_pybuffernd_image.diminfo[0].shape;
         if (__pyx_t_18 < 0) __pyx_t_18 += __pyx_pybuffernd_image.diminfo[1].shape;
         if (__pyx_t_19 < 0) __pyx_t_19 += __pyx_pybuffernd_image.diminfo[2].shape;
         __pyx_v_point_val = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int8_t *, __pyx_pybuffernd_image.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_image.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_image.diminfo[1].strides, __pyx_t_19, __pyx_pybuffernd_image.diminfo[2].strides));
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:             # <<<<<<<<<<<<<<
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  */
         __pyx_t_7 = ((__pyx_v_point_val < __pyx_v_mid_point) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":254
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)             # <<<<<<<<<<<<<<
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  */
           __pyx_t_20 = (__pyx_v_mid_point - __pyx_v_point_val);
           __pyx_t_21 = (__pyx_v_mid_point - __pyx_v_lower_bound);
           if (unlikely(__pyx_t_21 == 0)) {
             PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-            __PYX_ERR(0, 254, __pyx_L1_error)
+            __PYX_ERR(0, 257, __pyx_L1_error)
           }
           __pyx_v_res_val = (((double)__pyx_t_20) / ((double)__pyx_t_21));
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:             # <<<<<<<<<<<<<<
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  */
           goto __pyx_L10;
         }
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)             # <<<<<<<<<<<<<<
  *                 if res_val > 1:
  *                     res_val = 1
  */
         /*else*/ {
           __pyx_t_21 = (__pyx_v_point_val - __pyx_v_mid_point);
           __pyx_t_20 = (__pyx_v_upper_bound - __pyx_v_mid_point);
           if (unlikely(__pyx_t_20 == 0)) {
             PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-            __PYX_ERR(0, 256, __pyx_L1_error)
+            __PYX_ERR(0, 259, __pyx_L1_error)
           }
           __pyx_v_res_val = (((double)__pyx_t_21) / ((double)__pyx_t_20));
         }
         __pyx_L10:;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:             # <<<<<<<<<<<<<<
  *                     res_val = 1
  *                 elif res_val < 0:
  */
         __pyx_t_7 = ((__pyx_v_res_val > 1.0) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":258
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":261
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:
  *                     res_val = 1             # <<<<<<<<<<<<<<
  *                 elif res_val < 0:
  *                     res_val = 0
  */
           __pyx_v_res_val = 1.0;
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:             # <<<<<<<<<<<<<<
  *                     res_val = 1
  *                 elif res_val < 0:
  */
           goto __pyx_L11;
         }
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
  *                 if res_val > 1:
  *                     res_val = 1
  *                 elif res_val < 0:             # <<<<<<<<<<<<<<
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  */
         __pyx_t_7 = ((__pyx_v_res_val < 0.0) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":263
  *                     res_val = 1
  *                 elif res_val < 0:
  *                     res_val = 0             # <<<<<<<<<<<<<<
  *                 res[z, y, x] = res_val
  *     return res
  */
           __pyx_v_res_val = 0.0;
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
  *                 if res_val > 1:
  *                     res_val = 1
  *                 elif res_val < 0:             # <<<<<<<<<<<<<<
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  */
         }
         __pyx_L11:;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":261
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":264
  *                 elif res_val < 0:
  *                     res_val = 0
  *                 res[z, y, x] = res_val             # <<<<<<<<<<<<<<
  *     return res
  * 
  */
         __pyx_t_22 = __pyx_v_z;
@@ -16239,27 +16298,27 @@
         if (__pyx_t_23 < 0) __pyx_t_23 += __pyx_pybuffernd_res.diminfo[1].shape;
         if (__pyx_t_24 < 0) __pyx_t_24 += __pyx_pybuffernd_res.diminfo[2].shape;
         *__Pyx_BufPtrStrided3d(__pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_mu_type *, __pyx_pybuffernd_res.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_res.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_res.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_res.diminfo[2].strides) = __pyx_v_res_val;
       }
     }
   }
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":265
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  *     return res             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_res));
   __pyx_r = ((PyObject *)__pyx_v_res);
   goto __pyx_L0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":235
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":238
  * 
  * @cython.boundscheck(False)
  * def calculate_mu_mid(numpy.ndarray[image_types, ndim=3] image, image_types lower_bound, image_types mid_point,             # <<<<<<<<<<<<<<
  *                  image_types upper_bound):
  *     cdef int16_t x_size, y_size, z_size, x, y, z
  */
 
@@ -16324,54 +16383,54 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_image)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_lower_bound)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 1); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 1); __PYX_ERR(0, 238, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mid_point)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 2); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 2); __PYX_ERR(0, 238, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_upper_bound)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 3); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 3); __PYX_ERR(0, 238, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "calculate_mu_mid") < 0)) __PYX_ERR(0, 235, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "calculate_mu_mid") < 0)) __PYX_ERR(0, 238, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
     __pyx_v_image = ((PyArrayObject *)values[0]);
-    __pyx_v_lower_bound = __Pyx_PyInt_As_npy_int16(values[1]); if (unlikely((__pyx_v_lower_bound == ((npy_int16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L3_error)
-    __pyx_v_mid_point = __Pyx_PyInt_As_npy_int16(values[2]); if (unlikely((__pyx_v_mid_point == ((npy_int16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L3_error)
-    __pyx_v_upper_bound = __Pyx_PyInt_As_npy_int16(values[3]); if (unlikely((__pyx_v_upper_bound == ((npy_int16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 236, __pyx_L3_error)
+    __pyx_v_lower_bound = __Pyx_PyInt_As_npy_int16(values[1]); if (unlikely((__pyx_v_lower_bound == ((npy_int16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L3_error)
+    __pyx_v_mid_point = __Pyx_PyInt_As_npy_int16(values[2]); if (unlikely((__pyx_v_mid_point == ((npy_int16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L3_error)
+    __pyx_v_upper_bound = __Pyx_PyInt_As_npy_int16(values[3]); if (unlikely((__pyx_v_upper_bound == ((npy_int16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 239, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 235, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 238, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("PartSeg.utils.multiscale_opening.mso_bind.calculate_mu_mid", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_image), __pyx_ptype_5numpy_ndarray, 1, "image", 0))) __PYX_ERR(0, 235, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_image), __pyx_ptype_5numpy_ndarray, 1, "image", 0))) __PYX_ERR(0, 238, __pyx_L1_error)
   __pyx_r = __pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_22calculate_mu_mid(__pyx_self, __pyx_v_image, __pyx_v_lower_bound, __pyx_v_mid_point, __pyx_v_upper_bound);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -16427,316 +16486,316 @@
   __pyx_pybuffernd_res.rcbuffer = &__pyx_pybuffer_res;
   __pyx_pybuffer_image.pybuffer.buf = NULL;
   __pyx_pybuffer_image.refcount = 0;
   __pyx_pybuffernd_image.data = NULL;
   __pyx_pybuffernd_image.rcbuffer = &__pyx_pybuffer_image;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_image.rcbuffer->pybuffer, (PyObject*)__pyx_v_image, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int16_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 235, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_image.rcbuffer->pybuffer, (PyObject*)__pyx_v_image, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int16_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 238, __pyx_L1_error)
   }
   __pyx_pybuffernd_image.diminfo[0].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_image.diminfo[0].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_image.diminfo[1].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_image.diminfo[1].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_image.diminfo[2].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_image.diminfo[2].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[2];
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":240
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":243
  *     cdef mu_type res_val
  *     cdef image_types point_val
  *     x_size = image.shape[2]             # <<<<<<<<<<<<<<
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]
  */
   __pyx_v_x_size = (__pyx_v_image->dimensions[2]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":241
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
  *     cdef image_types point_val
  *     x_size = image.shape[2]
  *     y_size = image.shape[1]             # <<<<<<<<<<<<<<
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  */
   __pyx_v_y_size = (__pyx_v_image->dimensions[1]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":242
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":245
  *     x_size = image.shape[2]
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:
  */
   __pyx_v_z_size = (__pyx_v_image->dimensions[0]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":243
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":246
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)             # <<<<<<<<<<<<<<
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_npy_int16(__pyx_v_z_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_npy_int16(__pyx_v_z_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_From_npy_int16(__pyx_v_y_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_npy_int16(__pyx_v_y_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_npy_int16(__pyx_v_x_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_npy_int16(__pyx_v_x_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_4);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 246, __pyx_L1_error)
   __pyx_t_6 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_res.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_mu_type, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 3, 0, __pyx_stack) == -1)) {
       __pyx_v_res = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_res.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 243, __pyx_L1_error)
+      __PYX_ERR(0, 246, __pyx_L1_error)
     } else {__pyx_pybuffernd_res.diminfo[0].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_res.diminfo[0].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_res.diminfo[1].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_res.diminfo[1].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_res.diminfo[2].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_res.diminfo[2].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[2];
     }
   }
   __pyx_t_6 = 0;
   __pyx_v_res = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:             # <<<<<<<<<<<<<<
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  */
   __pyx_t_7 = ((__pyx_v_upper_bound < __pyx_v_lower_bound) != 0);
   if (__pyx_t_7) {
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":245
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":248
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound             # <<<<<<<<<<<<<<
  *         lower_bound = upper_bound
  *         upper_bound = tmp
  */
     __pyx_v_tmp = __pyx_v_lower_bound;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":246
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":249
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound
  *         lower_bound = upper_bound             # <<<<<<<<<<<<<<
  *         upper_bound = tmp
  * 
  */
     __pyx_v_lower_bound = __pyx_v_upper_bound;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":250
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  *         upper_bound = tmp             # <<<<<<<<<<<<<<
  * 
  *     for z in range(z_size):
  */
     __pyx_v_upper_bound = __pyx_v_tmp;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:             # <<<<<<<<<<<<<<
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  */
   }
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":249
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":252
  *         upper_bound = tmp
  * 
  *     for z in range(z_size):             # <<<<<<<<<<<<<<
  *         for y in range(y_size):
  *             for x in range(x_size):
  */
   __pyx_t_8 = __pyx_v_z_size;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_z = __pyx_t_10;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":250
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
  * 
  *     for z in range(z_size):
  *         for y in range(y_size):             # <<<<<<<<<<<<<<
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  */
     __pyx_t_11 = __pyx_v_y_size;
     __pyx_t_12 = __pyx_t_11;
     for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
       __pyx_v_y = __pyx_t_13;
 
-      /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":251
+      /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":254
  *     for z in range(z_size):
  *         for y in range(y_size):
  *             for x in range(x_size):             # <<<<<<<<<<<<<<
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:
  */
       __pyx_t_14 = __pyx_v_x_size;
       __pyx_t_15 = __pyx_t_14;
       for (__pyx_t_16 = 0; __pyx_t_16 < __pyx_t_15; __pyx_t_16+=1) {
         __pyx_v_x = __pyx_t_16;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":252
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":255
  *         for y in range(y_size):
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]             # <<<<<<<<<<<<<<
  *                 if point_val < mid_point:
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  */
         __pyx_t_17 = __pyx_v_z;
         __pyx_t_18 = __pyx_v_y;
         __pyx_t_19 = __pyx_v_x;
         if (__pyx_t_17 < 0) __pyx_t_17 += __pyx_pybuffernd_image.diminfo[0].shape;
         if (__pyx_t_18 < 0) __pyx_t_18 += __pyx_pybuffernd_image.diminfo[1].shape;
         if (__pyx_t_19 < 0) __pyx_t_19 += __pyx_pybuffernd_image.diminfo[2].shape;
         __pyx_v_point_val = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int16_t *, __pyx_pybuffernd_image.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_image.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_image.diminfo[1].strides, __pyx_t_19, __pyx_pybuffernd_image.diminfo[2].strides));
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:             # <<<<<<<<<<<<<<
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  */
         __pyx_t_7 = ((__pyx_v_point_val < __pyx_v_mid_point) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":254
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)             # <<<<<<<<<<<<<<
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  */
           __pyx_t_20 = (__pyx_v_mid_point - __pyx_v_point_val);
           __pyx_t_21 = (__pyx_v_mid_point - __pyx_v_lower_bound);
           if (unlikely(__pyx_t_21 == 0)) {
             PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-            __PYX_ERR(0, 254, __pyx_L1_error)
+            __PYX_ERR(0, 257, __pyx_L1_error)
           }
           __pyx_v_res_val = (((double)__pyx_t_20) / ((double)__pyx_t_21));
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:             # <<<<<<<<<<<<<<
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  */
           goto __pyx_L10;
         }
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)             # <<<<<<<<<<<<<<
  *                 if res_val > 1:
  *                     res_val = 1
  */
         /*else*/ {
           __pyx_t_21 = (__pyx_v_point_val - __pyx_v_mid_point);
           __pyx_t_20 = (__pyx_v_upper_bound - __pyx_v_mid_point);
           if (unlikely(__pyx_t_20 == 0)) {
             PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-            __PYX_ERR(0, 256, __pyx_L1_error)
+            __PYX_ERR(0, 259, __pyx_L1_error)
           }
           __pyx_v_res_val = (((double)__pyx_t_21) / ((double)__pyx_t_20));
         }
         __pyx_L10:;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:             # <<<<<<<<<<<<<<
  *                     res_val = 1
  *                 elif res_val < 0:
  */
         __pyx_t_7 = ((__pyx_v_res_val > 1.0) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":258
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":261
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:
  *                     res_val = 1             # <<<<<<<<<<<<<<
  *                 elif res_val < 0:
  *                     res_val = 0
  */
           __pyx_v_res_val = 1.0;
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:             # <<<<<<<<<<<<<<
  *                     res_val = 1
  *                 elif res_val < 0:
  */
           goto __pyx_L11;
         }
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
  *                 if res_val > 1:
  *                     res_val = 1
  *                 elif res_val < 0:             # <<<<<<<<<<<<<<
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  */
         __pyx_t_7 = ((__pyx_v_res_val < 0.0) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":263
  *                     res_val = 1
  *                 elif res_val < 0:
  *                     res_val = 0             # <<<<<<<<<<<<<<
  *                 res[z, y, x] = res_val
  *     return res
  */
           __pyx_v_res_val = 0.0;
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
  *                 if res_val > 1:
  *                     res_val = 1
  *                 elif res_val < 0:             # <<<<<<<<<<<<<<
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  */
         }
         __pyx_L11:;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":261
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":264
  *                 elif res_val < 0:
  *                     res_val = 0
  *                 res[z, y, x] = res_val             # <<<<<<<<<<<<<<
  *     return res
  * 
  */
         __pyx_t_22 = __pyx_v_z;
@@ -16746,27 +16805,27 @@
         if (__pyx_t_23 < 0) __pyx_t_23 += __pyx_pybuffernd_res.diminfo[1].shape;
         if (__pyx_t_24 < 0) __pyx_t_24 += __pyx_pybuffernd_res.diminfo[2].shape;
         *__Pyx_BufPtrStrided3d(__pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_mu_type *, __pyx_pybuffernd_res.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_res.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_res.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_res.diminfo[2].strides) = __pyx_v_res_val;
       }
     }
   }
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":265
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  *     return res             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_res));
   __pyx_r = ((PyObject *)__pyx_v_res);
   goto __pyx_L0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":235
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":238
  * 
  * @cython.boundscheck(False)
  * def calculate_mu_mid(numpy.ndarray[image_types, ndim=3] image, image_types lower_bound, image_types mid_point,             # <<<<<<<<<<<<<<
  *                  image_types upper_bound):
  *     cdef int16_t x_size, y_size, z_size, x, y, z
  */
 
@@ -16831,54 +16890,54 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_image)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_lower_bound)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 1); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 1); __PYX_ERR(0, 238, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mid_point)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 2); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 2); __PYX_ERR(0, 238, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_upper_bound)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 3); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 3); __PYX_ERR(0, 238, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "calculate_mu_mid") < 0)) __PYX_ERR(0, 235, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "calculate_mu_mid") < 0)) __PYX_ERR(0, 238, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
     __pyx_v_image = ((PyArrayObject *)values[0]);
-    __pyx_v_lower_bound = __Pyx_PyInt_As_npy_uint8(values[1]); if (unlikely((__pyx_v_lower_bound == ((npy_uint8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L3_error)
-    __pyx_v_mid_point = __Pyx_PyInt_As_npy_uint8(values[2]); if (unlikely((__pyx_v_mid_point == ((npy_uint8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L3_error)
-    __pyx_v_upper_bound = __Pyx_PyInt_As_npy_uint8(values[3]); if (unlikely((__pyx_v_upper_bound == ((npy_uint8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 236, __pyx_L3_error)
+    __pyx_v_lower_bound = __Pyx_PyInt_As_npy_uint8(values[1]); if (unlikely((__pyx_v_lower_bound == ((npy_uint8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L3_error)
+    __pyx_v_mid_point = __Pyx_PyInt_As_npy_uint8(values[2]); if (unlikely((__pyx_v_mid_point == ((npy_uint8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L3_error)
+    __pyx_v_upper_bound = __Pyx_PyInt_As_npy_uint8(values[3]); if (unlikely((__pyx_v_upper_bound == ((npy_uint8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 239, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 235, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 238, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("PartSeg.utils.multiscale_opening.mso_bind.calculate_mu_mid", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_image), __pyx_ptype_5numpy_ndarray, 1, "image", 0))) __PYX_ERR(0, 235, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_image), __pyx_ptype_5numpy_ndarray, 1, "image", 0))) __PYX_ERR(0, 238, __pyx_L1_error)
   __pyx_r = __pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_24calculate_mu_mid(__pyx_self, __pyx_v_image, __pyx_v_lower_bound, __pyx_v_mid_point, __pyx_v_upper_bound);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -16934,316 +16993,316 @@
   __pyx_pybuffernd_res.rcbuffer = &__pyx_pybuffer_res;
   __pyx_pybuffer_image.pybuffer.buf = NULL;
   __pyx_pybuffer_image.refcount = 0;
   __pyx_pybuffernd_image.data = NULL;
   __pyx_pybuffernd_image.rcbuffer = &__pyx_pybuffer_image;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_image.rcbuffer->pybuffer, (PyObject*)__pyx_v_image, &__Pyx_TypeInfo_nn___pyx_t_5numpy_uint8_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 235, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_image.rcbuffer->pybuffer, (PyObject*)__pyx_v_image, &__Pyx_TypeInfo_nn___pyx_t_5numpy_uint8_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 238, __pyx_L1_error)
   }
   __pyx_pybuffernd_image.diminfo[0].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_image.diminfo[0].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_image.diminfo[1].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_image.diminfo[1].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_image.diminfo[2].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_image.diminfo[2].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[2];
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":240
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":243
  *     cdef mu_type res_val
  *     cdef image_types point_val
  *     x_size = image.shape[2]             # <<<<<<<<<<<<<<
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]
  */
   __pyx_v_x_size = (__pyx_v_image->dimensions[2]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":241
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
  *     cdef image_types point_val
  *     x_size = image.shape[2]
  *     y_size = image.shape[1]             # <<<<<<<<<<<<<<
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  */
   __pyx_v_y_size = (__pyx_v_image->dimensions[1]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":242
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":245
  *     x_size = image.shape[2]
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:
  */
   __pyx_v_z_size = (__pyx_v_image->dimensions[0]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":243
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":246
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)             # <<<<<<<<<<<<<<
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_npy_int16(__pyx_v_z_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_npy_int16(__pyx_v_z_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_From_npy_int16(__pyx_v_y_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_npy_int16(__pyx_v_y_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_npy_int16(__pyx_v_x_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_npy_int16(__pyx_v_x_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_4);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 246, __pyx_L1_error)
   __pyx_t_6 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_res.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_mu_type, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 3, 0, __pyx_stack) == -1)) {
       __pyx_v_res = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_res.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 243, __pyx_L1_error)
+      __PYX_ERR(0, 246, __pyx_L1_error)
     } else {__pyx_pybuffernd_res.diminfo[0].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_res.diminfo[0].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_res.diminfo[1].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_res.diminfo[1].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_res.diminfo[2].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_res.diminfo[2].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[2];
     }
   }
   __pyx_t_6 = 0;
   __pyx_v_res = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:             # <<<<<<<<<<<<<<
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  */
   __pyx_t_7 = ((__pyx_v_upper_bound < __pyx_v_lower_bound) != 0);
   if (__pyx_t_7) {
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":245
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":248
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound             # <<<<<<<<<<<<<<
  *         lower_bound = upper_bound
  *         upper_bound = tmp
  */
     __pyx_v_tmp = __pyx_v_lower_bound;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":246
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":249
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound
  *         lower_bound = upper_bound             # <<<<<<<<<<<<<<
  *         upper_bound = tmp
  * 
  */
     __pyx_v_lower_bound = __pyx_v_upper_bound;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":250
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  *         upper_bound = tmp             # <<<<<<<<<<<<<<
  * 
  *     for z in range(z_size):
  */
     __pyx_v_upper_bound = __pyx_v_tmp;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:             # <<<<<<<<<<<<<<
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  */
   }
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":249
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":252
  *         upper_bound = tmp
  * 
  *     for z in range(z_size):             # <<<<<<<<<<<<<<
  *         for y in range(y_size):
  *             for x in range(x_size):
  */
   __pyx_t_8 = __pyx_v_z_size;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_z = __pyx_t_10;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":250
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
  * 
  *     for z in range(z_size):
  *         for y in range(y_size):             # <<<<<<<<<<<<<<
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  */
     __pyx_t_11 = __pyx_v_y_size;
     __pyx_t_12 = __pyx_t_11;
     for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
       __pyx_v_y = __pyx_t_13;
 
-      /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":251
+      /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":254
  *     for z in range(z_size):
  *         for y in range(y_size):
  *             for x in range(x_size):             # <<<<<<<<<<<<<<
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:
  */
       __pyx_t_14 = __pyx_v_x_size;
       __pyx_t_15 = __pyx_t_14;
       for (__pyx_t_16 = 0; __pyx_t_16 < __pyx_t_15; __pyx_t_16+=1) {
         __pyx_v_x = __pyx_t_16;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":252
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":255
  *         for y in range(y_size):
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]             # <<<<<<<<<<<<<<
  *                 if point_val < mid_point:
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  */
         __pyx_t_17 = __pyx_v_z;
         __pyx_t_18 = __pyx_v_y;
         __pyx_t_19 = __pyx_v_x;
         if (__pyx_t_17 < 0) __pyx_t_17 += __pyx_pybuffernd_image.diminfo[0].shape;
         if (__pyx_t_18 < 0) __pyx_t_18 += __pyx_pybuffernd_image.diminfo[1].shape;
         if (__pyx_t_19 < 0) __pyx_t_19 += __pyx_pybuffernd_image.diminfo[2].shape;
         __pyx_v_point_val = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_uint8_t *, __pyx_pybuffernd_image.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_image.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_image.diminfo[1].strides, __pyx_t_19, __pyx_pybuffernd_image.diminfo[2].strides));
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:             # <<<<<<<<<<<<<<
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  */
         __pyx_t_7 = ((__pyx_v_point_val < __pyx_v_mid_point) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":254
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)             # <<<<<<<<<<<<<<
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  */
           __pyx_t_20 = (__pyx_v_mid_point - __pyx_v_point_val);
           __pyx_t_21 = (__pyx_v_mid_point - __pyx_v_lower_bound);
           if (unlikely(__pyx_t_21 == 0)) {
             PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-            __PYX_ERR(0, 254, __pyx_L1_error)
+            __PYX_ERR(0, 257, __pyx_L1_error)
           }
           __pyx_v_res_val = (((double)__pyx_t_20) / ((double)__pyx_t_21));
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:             # <<<<<<<<<<<<<<
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  */
           goto __pyx_L10;
         }
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)             # <<<<<<<<<<<<<<
  *                 if res_val > 1:
  *                     res_val = 1
  */
         /*else*/ {
           __pyx_t_21 = (__pyx_v_point_val - __pyx_v_mid_point);
           __pyx_t_20 = (__pyx_v_upper_bound - __pyx_v_mid_point);
           if (unlikely(__pyx_t_20 == 0)) {
             PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-            __PYX_ERR(0, 256, __pyx_L1_error)
+            __PYX_ERR(0, 259, __pyx_L1_error)
           }
           __pyx_v_res_val = (((double)__pyx_t_21) / ((double)__pyx_t_20));
         }
         __pyx_L10:;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:             # <<<<<<<<<<<<<<
  *                     res_val = 1
  *                 elif res_val < 0:
  */
         __pyx_t_7 = ((__pyx_v_res_val > 1.0) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":258
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":261
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:
  *                     res_val = 1             # <<<<<<<<<<<<<<
  *                 elif res_val < 0:
  *                     res_val = 0
  */
           __pyx_v_res_val = 1.0;
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:             # <<<<<<<<<<<<<<
  *                     res_val = 1
  *                 elif res_val < 0:
  */
           goto __pyx_L11;
         }
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
  *                 if res_val > 1:
  *                     res_val = 1
  *                 elif res_val < 0:             # <<<<<<<<<<<<<<
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  */
         __pyx_t_7 = ((__pyx_v_res_val < 0.0) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":263
  *                     res_val = 1
  *                 elif res_val < 0:
  *                     res_val = 0             # <<<<<<<<<<<<<<
  *                 res[z, y, x] = res_val
  *     return res
  */
           __pyx_v_res_val = 0.0;
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
  *                 if res_val > 1:
  *                     res_val = 1
  *                 elif res_val < 0:             # <<<<<<<<<<<<<<
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  */
         }
         __pyx_L11:;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":261
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":264
  *                 elif res_val < 0:
  *                     res_val = 0
  *                 res[z, y, x] = res_val             # <<<<<<<<<<<<<<
  *     return res
  * 
  */
         __pyx_t_22 = __pyx_v_z;
@@ -17253,27 +17312,27 @@
         if (__pyx_t_23 < 0) __pyx_t_23 += __pyx_pybuffernd_res.diminfo[1].shape;
         if (__pyx_t_24 < 0) __pyx_t_24 += __pyx_pybuffernd_res.diminfo[2].shape;
         *__Pyx_BufPtrStrided3d(__pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_mu_type *, __pyx_pybuffernd_res.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_res.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_res.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_res.diminfo[2].strides) = __pyx_v_res_val;
       }
     }
   }
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":265
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  *     return res             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_res));
   __pyx_r = ((PyObject *)__pyx_v_res);
   goto __pyx_L0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":235
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":238
  * 
  * @cython.boundscheck(False)
  * def calculate_mu_mid(numpy.ndarray[image_types, ndim=3] image, image_types lower_bound, image_types mid_point,             # <<<<<<<<<<<<<<
  *                  image_types upper_bound):
  *     cdef int16_t x_size, y_size, z_size, x, y, z
  */
 
@@ -17338,54 +17397,54 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_image)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_lower_bound)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 1); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 1); __PYX_ERR(0, 238, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mid_point)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 2); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 2); __PYX_ERR(0, 238, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_upper_bound)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 3); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 3); __PYX_ERR(0, 238, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "calculate_mu_mid") < 0)) __PYX_ERR(0, 235, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "calculate_mu_mid") < 0)) __PYX_ERR(0, 238, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
     __pyx_v_image = ((PyArrayObject *)values[0]);
-    __pyx_v_lower_bound = __Pyx_PyInt_As_npy_uint16(values[1]); if (unlikely((__pyx_v_lower_bound == ((npy_uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L3_error)
-    __pyx_v_mid_point = __Pyx_PyInt_As_npy_uint16(values[2]); if (unlikely((__pyx_v_mid_point == ((npy_uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L3_error)
-    __pyx_v_upper_bound = __Pyx_PyInt_As_npy_uint16(values[3]); if (unlikely((__pyx_v_upper_bound == ((npy_uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 236, __pyx_L3_error)
+    __pyx_v_lower_bound = __Pyx_PyInt_As_npy_uint16(values[1]); if (unlikely((__pyx_v_lower_bound == ((npy_uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L3_error)
+    __pyx_v_mid_point = __Pyx_PyInt_As_npy_uint16(values[2]); if (unlikely((__pyx_v_mid_point == ((npy_uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L3_error)
+    __pyx_v_upper_bound = __Pyx_PyInt_As_npy_uint16(values[3]); if (unlikely((__pyx_v_upper_bound == ((npy_uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 239, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 235, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 238, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("PartSeg.utils.multiscale_opening.mso_bind.calculate_mu_mid", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_image), __pyx_ptype_5numpy_ndarray, 1, "image", 0))) __PYX_ERR(0, 235, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_image), __pyx_ptype_5numpy_ndarray, 1, "image", 0))) __PYX_ERR(0, 238, __pyx_L1_error)
   __pyx_r = __pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_26calculate_mu_mid(__pyx_self, __pyx_v_image, __pyx_v_lower_bound, __pyx_v_mid_point, __pyx_v_upper_bound);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -17441,316 +17500,316 @@
   __pyx_pybuffernd_res.rcbuffer = &__pyx_pybuffer_res;
   __pyx_pybuffer_image.pybuffer.buf = NULL;
   __pyx_pybuffer_image.refcount = 0;
   __pyx_pybuffernd_image.data = NULL;
   __pyx_pybuffernd_image.rcbuffer = &__pyx_pybuffer_image;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_image.rcbuffer->pybuffer, (PyObject*)__pyx_v_image, &__Pyx_TypeInfo_nn___pyx_t_5numpy_uint16_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 235, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_image.rcbuffer->pybuffer, (PyObject*)__pyx_v_image, &__Pyx_TypeInfo_nn___pyx_t_5numpy_uint16_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 238, __pyx_L1_error)
   }
   __pyx_pybuffernd_image.diminfo[0].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_image.diminfo[0].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_image.diminfo[1].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_image.diminfo[1].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_image.diminfo[2].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_image.diminfo[2].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[2];
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":240
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":243
  *     cdef mu_type res_val
  *     cdef image_types point_val
  *     x_size = image.shape[2]             # <<<<<<<<<<<<<<
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]
  */
   __pyx_v_x_size = (__pyx_v_image->dimensions[2]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":241
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
  *     cdef image_types point_val
  *     x_size = image.shape[2]
  *     y_size = image.shape[1]             # <<<<<<<<<<<<<<
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  */
   __pyx_v_y_size = (__pyx_v_image->dimensions[1]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":242
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":245
  *     x_size = image.shape[2]
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:
  */
   __pyx_v_z_size = (__pyx_v_image->dimensions[0]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":243
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":246
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)             # <<<<<<<<<<<<<<
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_npy_int16(__pyx_v_z_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_npy_int16(__pyx_v_z_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_From_npy_int16(__pyx_v_y_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_npy_int16(__pyx_v_y_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_npy_int16(__pyx_v_x_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_npy_int16(__pyx_v_x_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_4);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 246, __pyx_L1_error)
   __pyx_t_6 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_res.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_mu_type, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 3, 0, __pyx_stack) == -1)) {
       __pyx_v_res = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_res.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 243, __pyx_L1_error)
+      __PYX_ERR(0, 246, __pyx_L1_error)
     } else {__pyx_pybuffernd_res.diminfo[0].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_res.diminfo[0].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_res.diminfo[1].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_res.diminfo[1].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_res.diminfo[2].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_res.diminfo[2].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[2];
     }
   }
   __pyx_t_6 = 0;
   __pyx_v_res = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:             # <<<<<<<<<<<<<<
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  */
   __pyx_t_7 = ((__pyx_v_upper_bound < __pyx_v_lower_bound) != 0);
   if (__pyx_t_7) {
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":245
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":248
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound             # <<<<<<<<<<<<<<
  *         lower_bound = upper_bound
  *         upper_bound = tmp
  */
     __pyx_v_tmp = __pyx_v_lower_bound;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":246
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":249
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound
  *         lower_bound = upper_bound             # <<<<<<<<<<<<<<
  *         upper_bound = tmp
  * 
  */
     __pyx_v_lower_bound = __pyx_v_upper_bound;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":250
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  *         upper_bound = tmp             # <<<<<<<<<<<<<<
  * 
  *     for z in range(z_size):
  */
     __pyx_v_upper_bound = __pyx_v_tmp;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:             # <<<<<<<<<<<<<<
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  */
   }
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":249
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":252
  *         upper_bound = tmp
  * 
  *     for z in range(z_size):             # <<<<<<<<<<<<<<
  *         for y in range(y_size):
  *             for x in range(x_size):
  */
   __pyx_t_8 = __pyx_v_z_size;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_z = __pyx_t_10;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":250
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
  * 
  *     for z in range(z_size):
  *         for y in range(y_size):             # <<<<<<<<<<<<<<
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  */
     __pyx_t_11 = __pyx_v_y_size;
     __pyx_t_12 = __pyx_t_11;
     for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
       __pyx_v_y = __pyx_t_13;
 
-      /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":251
+      /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":254
  *     for z in range(z_size):
  *         for y in range(y_size):
  *             for x in range(x_size):             # <<<<<<<<<<<<<<
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:
  */
       __pyx_t_14 = __pyx_v_x_size;
       __pyx_t_15 = __pyx_t_14;
       for (__pyx_t_16 = 0; __pyx_t_16 < __pyx_t_15; __pyx_t_16+=1) {
         __pyx_v_x = __pyx_t_16;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":252
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":255
  *         for y in range(y_size):
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]             # <<<<<<<<<<<<<<
  *                 if point_val < mid_point:
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  */
         __pyx_t_17 = __pyx_v_z;
         __pyx_t_18 = __pyx_v_y;
         __pyx_t_19 = __pyx_v_x;
         if (__pyx_t_17 < 0) __pyx_t_17 += __pyx_pybuffernd_image.diminfo[0].shape;
         if (__pyx_t_18 < 0) __pyx_t_18 += __pyx_pybuffernd_image.diminfo[1].shape;
         if (__pyx_t_19 < 0) __pyx_t_19 += __pyx_pybuffernd_image.diminfo[2].shape;
         __pyx_v_point_val = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_uint16_t *, __pyx_pybuffernd_image.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_image.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_image.diminfo[1].strides, __pyx_t_19, __pyx_pybuffernd_image.diminfo[2].strides));
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:             # <<<<<<<<<<<<<<
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  */
         __pyx_t_7 = ((__pyx_v_point_val < __pyx_v_mid_point) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":254
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)             # <<<<<<<<<<<<<<
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  */
           __pyx_t_20 = (__pyx_v_mid_point - __pyx_v_point_val);
           __pyx_t_21 = (__pyx_v_mid_point - __pyx_v_lower_bound);
           if (unlikely(__pyx_t_21 == 0)) {
             PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-            __PYX_ERR(0, 254, __pyx_L1_error)
+            __PYX_ERR(0, 257, __pyx_L1_error)
           }
           __pyx_v_res_val = (((double)__pyx_t_20) / ((double)__pyx_t_21));
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:             # <<<<<<<<<<<<<<
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  */
           goto __pyx_L10;
         }
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)             # <<<<<<<<<<<<<<
  *                 if res_val > 1:
  *                     res_val = 1
  */
         /*else*/ {
           __pyx_t_21 = (__pyx_v_point_val - __pyx_v_mid_point);
           __pyx_t_20 = (__pyx_v_upper_bound - __pyx_v_mid_point);
           if (unlikely(__pyx_t_20 == 0)) {
             PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-            __PYX_ERR(0, 256, __pyx_L1_error)
+            __PYX_ERR(0, 259, __pyx_L1_error)
           }
           __pyx_v_res_val = (((double)__pyx_t_21) / ((double)__pyx_t_20));
         }
         __pyx_L10:;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:             # <<<<<<<<<<<<<<
  *                     res_val = 1
  *                 elif res_val < 0:
  */
         __pyx_t_7 = ((__pyx_v_res_val > 1.0) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":258
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":261
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:
  *                     res_val = 1             # <<<<<<<<<<<<<<
  *                 elif res_val < 0:
  *                     res_val = 0
  */
           __pyx_v_res_val = 1.0;
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:             # <<<<<<<<<<<<<<
  *                     res_val = 1
  *                 elif res_val < 0:
  */
           goto __pyx_L11;
         }
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
  *                 if res_val > 1:
  *                     res_val = 1
  *                 elif res_val < 0:             # <<<<<<<<<<<<<<
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  */
         __pyx_t_7 = ((__pyx_v_res_val < 0.0) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":263
  *                     res_val = 1
  *                 elif res_val < 0:
  *                     res_val = 0             # <<<<<<<<<<<<<<
  *                 res[z, y, x] = res_val
  *     return res
  */
           __pyx_v_res_val = 0.0;
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
  *                 if res_val > 1:
  *                     res_val = 1
  *                 elif res_val < 0:             # <<<<<<<<<<<<<<
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  */
         }
         __pyx_L11:;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":261
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":264
  *                 elif res_val < 0:
  *                     res_val = 0
  *                 res[z, y, x] = res_val             # <<<<<<<<<<<<<<
  *     return res
  * 
  */
         __pyx_t_22 = __pyx_v_z;
@@ -17760,27 +17819,27 @@
         if (__pyx_t_23 < 0) __pyx_t_23 += __pyx_pybuffernd_res.diminfo[1].shape;
         if (__pyx_t_24 < 0) __pyx_t_24 += __pyx_pybuffernd_res.diminfo[2].shape;
         *__Pyx_BufPtrStrided3d(__pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_mu_type *, __pyx_pybuffernd_res.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_res.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_res.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_res.diminfo[2].strides) = __pyx_v_res_val;
       }
     }
   }
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":265
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  *     return res             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_res));
   __pyx_r = ((PyObject *)__pyx_v_res);
   goto __pyx_L0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":235
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":238
  * 
  * @cython.boundscheck(False)
  * def calculate_mu_mid(numpy.ndarray[image_types, ndim=3] image, image_types lower_bound, image_types mid_point,             # <<<<<<<<<<<<<<
  *                  image_types upper_bound):
  *     cdef int16_t x_size, y_size, z_size, x, y, z
  */
 
@@ -17845,54 +17904,54 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_image)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_lower_bound)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 1); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 1); __PYX_ERR(0, 238, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mid_point)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 2); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 2); __PYX_ERR(0, 238, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_upper_bound)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 3); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 3); __PYX_ERR(0, 238, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "calculate_mu_mid") < 0)) __PYX_ERR(0, 235, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "calculate_mu_mid") < 0)) __PYX_ERR(0, 238, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
     __pyx_v_image = ((PyArrayObject *)values[0]);
-    __pyx_v_lower_bound = __Pyx_PyInt_As_npy_uint32(values[1]); if (unlikely((__pyx_v_lower_bound == ((npy_uint32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L3_error)
-    __pyx_v_mid_point = __Pyx_PyInt_As_npy_uint32(values[2]); if (unlikely((__pyx_v_mid_point == ((npy_uint32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L3_error)
-    __pyx_v_upper_bound = __Pyx_PyInt_As_npy_uint32(values[3]); if (unlikely((__pyx_v_upper_bound == ((npy_uint32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 236, __pyx_L3_error)
+    __pyx_v_lower_bound = __Pyx_PyInt_As_npy_uint32(values[1]); if (unlikely((__pyx_v_lower_bound == ((npy_uint32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L3_error)
+    __pyx_v_mid_point = __Pyx_PyInt_As_npy_uint32(values[2]); if (unlikely((__pyx_v_mid_point == ((npy_uint32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L3_error)
+    __pyx_v_upper_bound = __Pyx_PyInt_As_npy_uint32(values[3]); if (unlikely((__pyx_v_upper_bound == ((npy_uint32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 239, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 235, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 238, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("PartSeg.utils.multiscale_opening.mso_bind.calculate_mu_mid", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_image), __pyx_ptype_5numpy_ndarray, 1, "image", 0))) __PYX_ERR(0, 235, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_image), __pyx_ptype_5numpy_ndarray, 1, "image", 0))) __PYX_ERR(0, 238, __pyx_L1_error)
   __pyx_r = __pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_28calculate_mu_mid(__pyx_self, __pyx_v_image, __pyx_v_lower_bound, __pyx_v_mid_point, __pyx_v_upper_bound);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -17948,316 +18007,316 @@
   __pyx_pybuffernd_res.rcbuffer = &__pyx_pybuffer_res;
   __pyx_pybuffer_image.pybuffer.buf = NULL;
   __pyx_pybuffer_image.refcount = 0;
   __pyx_pybuffernd_image.data = NULL;
   __pyx_pybuffernd_image.rcbuffer = &__pyx_pybuffer_image;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_image.rcbuffer->pybuffer, (PyObject*)__pyx_v_image, &__Pyx_TypeInfo_nn___pyx_t_5numpy_uint32_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 235, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_image.rcbuffer->pybuffer, (PyObject*)__pyx_v_image, &__Pyx_TypeInfo_nn___pyx_t_5numpy_uint32_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 238, __pyx_L1_error)
   }
   __pyx_pybuffernd_image.diminfo[0].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_image.diminfo[0].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_image.diminfo[1].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_image.diminfo[1].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_image.diminfo[2].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_image.diminfo[2].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[2];
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":240
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":243
  *     cdef mu_type res_val
  *     cdef image_types point_val
  *     x_size = image.shape[2]             # <<<<<<<<<<<<<<
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]
  */
   __pyx_v_x_size = (__pyx_v_image->dimensions[2]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":241
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
  *     cdef image_types point_val
  *     x_size = image.shape[2]
  *     y_size = image.shape[1]             # <<<<<<<<<<<<<<
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  */
   __pyx_v_y_size = (__pyx_v_image->dimensions[1]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":242
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":245
  *     x_size = image.shape[2]
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:
  */
   __pyx_v_z_size = (__pyx_v_image->dimensions[0]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":243
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":246
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)             # <<<<<<<<<<<<<<
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_npy_int16(__pyx_v_z_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_npy_int16(__pyx_v_z_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_From_npy_int16(__pyx_v_y_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_npy_int16(__pyx_v_y_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_npy_int16(__pyx_v_x_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_npy_int16(__pyx_v_x_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_4);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 246, __pyx_L1_error)
   __pyx_t_6 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_res.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_mu_type, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 3, 0, __pyx_stack) == -1)) {
       __pyx_v_res = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_res.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 243, __pyx_L1_error)
+      __PYX_ERR(0, 246, __pyx_L1_error)
     } else {__pyx_pybuffernd_res.diminfo[0].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_res.diminfo[0].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_res.diminfo[1].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_res.diminfo[1].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_res.diminfo[2].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_res.diminfo[2].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[2];
     }
   }
   __pyx_t_6 = 0;
   __pyx_v_res = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:             # <<<<<<<<<<<<<<
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  */
   __pyx_t_7 = ((__pyx_v_upper_bound < __pyx_v_lower_bound) != 0);
   if (__pyx_t_7) {
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":245
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":248
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound             # <<<<<<<<<<<<<<
  *         lower_bound = upper_bound
  *         upper_bound = tmp
  */
     __pyx_v_tmp = __pyx_v_lower_bound;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":246
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":249
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound
  *         lower_bound = upper_bound             # <<<<<<<<<<<<<<
  *         upper_bound = tmp
  * 
  */
     __pyx_v_lower_bound = __pyx_v_upper_bound;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":250
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  *         upper_bound = tmp             # <<<<<<<<<<<<<<
  * 
  *     for z in range(z_size):
  */
     __pyx_v_upper_bound = __pyx_v_tmp;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:             # <<<<<<<<<<<<<<
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  */
   }
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":249
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":252
  *         upper_bound = tmp
  * 
  *     for z in range(z_size):             # <<<<<<<<<<<<<<
  *         for y in range(y_size):
  *             for x in range(x_size):
  */
   __pyx_t_8 = __pyx_v_z_size;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_z = __pyx_t_10;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":250
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
  * 
  *     for z in range(z_size):
  *         for y in range(y_size):             # <<<<<<<<<<<<<<
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  */
     __pyx_t_11 = __pyx_v_y_size;
     __pyx_t_12 = __pyx_t_11;
     for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
       __pyx_v_y = __pyx_t_13;
 
-      /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":251
+      /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":254
  *     for z in range(z_size):
  *         for y in range(y_size):
  *             for x in range(x_size):             # <<<<<<<<<<<<<<
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:
  */
       __pyx_t_14 = __pyx_v_x_size;
       __pyx_t_15 = __pyx_t_14;
       for (__pyx_t_16 = 0; __pyx_t_16 < __pyx_t_15; __pyx_t_16+=1) {
         __pyx_v_x = __pyx_t_16;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":252
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":255
  *         for y in range(y_size):
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]             # <<<<<<<<<<<<<<
  *                 if point_val < mid_point:
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  */
         __pyx_t_17 = __pyx_v_z;
         __pyx_t_18 = __pyx_v_y;
         __pyx_t_19 = __pyx_v_x;
         if (__pyx_t_17 < 0) __pyx_t_17 += __pyx_pybuffernd_image.diminfo[0].shape;
         if (__pyx_t_18 < 0) __pyx_t_18 += __pyx_pybuffernd_image.diminfo[1].shape;
         if (__pyx_t_19 < 0) __pyx_t_19 += __pyx_pybuffernd_image.diminfo[2].shape;
         __pyx_v_point_val = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_uint32_t *, __pyx_pybuffernd_image.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_image.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_image.diminfo[1].strides, __pyx_t_19, __pyx_pybuffernd_image.diminfo[2].strides));
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:             # <<<<<<<<<<<<<<
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  */
         __pyx_t_7 = ((__pyx_v_point_val < __pyx_v_mid_point) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":254
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)             # <<<<<<<<<<<<<<
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  */
           __pyx_t_20 = (__pyx_v_mid_point - __pyx_v_point_val);
           __pyx_t_21 = (__pyx_v_mid_point - __pyx_v_lower_bound);
           if (unlikely(__pyx_t_21 == 0)) {
             PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-            __PYX_ERR(0, 254, __pyx_L1_error)
+            __PYX_ERR(0, 257, __pyx_L1_error)
           }
           __pyx_v_res_val = (((double)__pyx_t_20) / ((double)__pyx_t_21));
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:             # <<<<<<<<<<<<<<
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  */
           goto __pyx_L10;
         }
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)             # <<<<<<<<<<<<<<
  *                 if res_val > 1:
  *                     res_val = 1
  */
         /*else*/ {
           __pyx_t_21 = (__pyx_v_point_val - __pyx_v_mid_point);
           __pyx_t_20 = (__pyx_v_upper_bound - __pyx_v_mid_point);
           if (unlikely(__pyx_t_20 == 0)) {
             PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-            __PYX_ERR(0, 256, __pyx_L1_error)
+            __PYX_ERR(0, 259, __pyx_L1_error)
           }
           __pyx_v_res_val = (((double)__pyx_t_21) / ((double)__pyx_t_20));
         }
         __pyx_L10:;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:             # <<<<<<<<<<<<<<
  *                     res_val = 1
  *                 elif res_val < 0:
  */
         __pyx_t_7 = ((__pyx_v_res_val > 1.0) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":258
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":261
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:
  *                     res_val = 1             # <<<<<<<<<<<<<<
  *                 elif res_val < 0:
  *                     res_val = 0
  */
           __pyx_v_res_val = 1.0;
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:             # <<<<<<<<<<<<<<
  *                     res_val = 1
  *                 elif res_val < 0:
  */
           goto __pyx_L11;
         }
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
  *                 if res_val > 1:
  *                     res_val = 1
  *                 elif res_val < 0:             # <<<<<<<<<<<<<<
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  */
         __pyx_t_7 = ((__pyx_v_res_val < 0.0) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":263
  *                     res_val = 1
  *                 elif res_val < 0:
  *                     res_val = 0             # <<<<<<<<<<<<<<
  *                 res[z, y, x] = res_val
  *     return res
  */
           __pyx_v_res_val = 0.0;
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
  *                 if res_val > 1:
  *                     res_val = 1
  *                 elif res_val < 0:             # <<<<<<<<<<<<<<
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  */
         }
         __pyx_L11:;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":261
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":264
  *                 elif res_val < 0:
  *                     res_val = 0
  *                 res[z, y, x] = res_val             # <<<<<<<<<<<<<<
  *     return res
  * 
  */
         __pyx_t_22 = __pyx_v_z;
@@ -18267,27 +18326,27 @@
         if (__pyx_t_23 < 0) __pyx_t_23 += __pyx_pybuffernd_res.diminfo[1].shape;
         if (__pyx_t_24 < 0) __pyx_t_24 += __pyx_pybuffernd_res.diminfo[2].shape;
         *__Pyx_BufPtrStrided3d(__pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_mu_type *, __pyx_pybuffernd_res.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_res.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_res.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_res.diminfo[2].strides) = __pyx_v_res_val;
       }
     }
   }
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":265
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  *     return res             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_res));
   __pyx_r = ((PyObject *)__pyx_v_res);
   goto __pyx_L0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":235
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":238
  * 
  * @cython.boundscheck(False)
  * def calculate_mu_mid(numpy.ndarray[image_types, ndim=3] image, image_types lower_bound, image_types mid_point,             # <<<<<<<<<<<<<<
  *                  image_types upper_bound):
  *     cdef int16_t x_size, y_size, z_size, x, y, z
  */
 
@@ -18352,54 +18411,54 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_image)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_lower_bound)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 1); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 1); __PYX_ERR(0, 238, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mid_point)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 2); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 2); __PYX_ERR(0, 238, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_upper_bound)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 3); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 3); __PYX_ERR(0, 238, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "calculate_mu_mid") < 0)) __PYX_ERR(0, 235, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "calculate_mu_mid") < 0)) __PYX_ERR(0, 238, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
     __pyx_v_image = ((PyArrayObject *)values[0]);
-    __pyx_v_lower_bound = __pyx_PyFloat_AsFloat(values[1]); if (unlikely((__pyx_v_lower_bound == ((npy_float32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L3_error)
-    __pyx_v_mid_point = __pyx_PyFloat_AsFloat(values[2]); if (unlikely((__pyx_v_mid_point == ((npy_float32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L3_error)
-    __pyx_v_upper_bound = __pyx_PyFloat_AsFloat(values[3]); if (unlikely((__pyx_v_upper_bound == ((npy_float32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 236, __pyx_L3_error)
+    __pyx_v_lower_bound = __pyx_PyFloat_AsFloat(values[1]); if (unlikely((__pyx_v_lower_bound == ((npy_float32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L3_error)
+    __pyx_v_mid_point = __pyx_PyFloat_AsFloat(values[2]); if (unlikely((__pyx_v_mid_point == ((npy_float32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L3_error)
+    __pyx_v_upper_bound = __pyx_PyFloat_AsFloat(values[3]); if (unlikely((__pyx_v_upper_bound == ((npy_float32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 239, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 235, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 238, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("PartSeg.utils.multiscale_opening.mso_bind.calculate_mu_mid", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_image), __pyx_ptype_5numpy_ndarray, 1, "image", 0))) __PYX_ERR(0, 235, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_image), __pyx_ptype_5numpy_ndarray, 1, "image", 0))) __PYX_ERR(0, 238, __pyx_L1_error)
   __pyx_r = __pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_30calculate_mu_mid(__pyx_self, __pyx_v_image, __pyx_v_lower_bound, __pyx_v_mid_point, __pyx_v_upper_bound);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -18455,320 +18514,320 @@
   __pyx_pybuffernd_res.rcbuffer = &__pyx_pybuffer_res;
   __pyx_pybuffer_image.pybuffer.buf = NULL;
   __pyx_pybuffer_image.refcount = 0;
   __pyx_pybuffernd_image.data = NULL;
   __pyx_pybuffernd_image.rcbuffer = &__pyx_pybuffer_image;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_image.rcbuffer->pybuffer, (PyObject*)__pyx_v_image, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float32_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 235, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_image.rcbuffer->pybuffer, (PyObject*)__pyx_v_image, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float32_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 238, __pyx_L1_error)
   }
   __pyx_pybuffernd_image.diminfo[0].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_image.diminfo[0].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_image.diminfo[1].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_image.diminfo[1].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_image.diminfo[2].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_image.diminfo[2].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[2];
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":240
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":243
  *     cdef mu_type res_val
  *     cdef image_types point_val
  *     x_size = image.shape[2]             # <<<<<<<<<<<<<<
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]
  */
   __pyx_v_x_size = (__pyx_v_image->dimensions[2]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":241
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
  *     cdef image_types point_val
  *     x_size = image.shape[2]
  *     y_size = image.shape[1]             # <<<<<<<<<<<<<<
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  */
   __pyx_v_y_size = (__pyx_v_image->dimensions[1]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":242
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":245
  *     x_size = image.shape[2]
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:
  */
   __pyx_v_z_size = (__pyx_v_image->dimensions[0]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":243
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":246
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)             # <<<<<<<<<<<<<<
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_npy_int16(__pyx_v_z_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_npy_int16(__pyx_v_z_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_From_npy_int16(__pyx_v_y_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_npy_int16(__pyx_v_y_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_npy_int16(__pyx_v_x_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_npy_int16(__pyx_v_x_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_4);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 246, __pyx_L1_error)
   __pyx_t_6 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_res.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_mu_type, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 3, 0, __pyx_stack) == -1)) {
       __pyx_v_res = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_res.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 243, __pyx_L1_error)
+      __PYX_ERR(0, 246, __pyx_L1_error)
     } else {__pyx_pybuffernd_res.diminfo[0].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_res.diminfo[0].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_res.diminfo[1].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_res.diminfo[1].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_res.diminfo[2].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_res.diminfo[2].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[2];
     }
   }
   __pyx_t_6 = 0;
   __pyx_v_res = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:             # <<<<<<<<<<<<<<
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  */
   __pyx_t_7 = ((__pyx_v_upper_bound < __pyx_v_lower_bound) != 0);
   if (__pyx_t_7) {
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":245
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":248
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound             # <<<<<<<<<<<<<<
  *         lower_bound = upper_bound
  *         upper_bound = tmp
  */
-    __pyx_t_1 = PyFloat_FromDouble(__pyx_v_lower_bound); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
+    __pyx_t_1 = PyFloat_FromDouble(__pyx_v_lower_bound); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_tmp = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":246
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":249
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound
  *         lower_bound = upper_bound             # <<<<<<<<<<<<<<
  *         upper_bound = tmp
  * 
  */
     __pyx_v_lower_bound = __pyx_v_upper_bound;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":250
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  *         upper_bound = tmp             # <<<<<<<<<<<<<<
  * 
  *     for z in range(z_size):
  */
-    __pyx_t_8 = __pyx_PyFloat_AsFloat(__pyx_v_tmp); if (unlikely((__pyx_t_8 == ((npy_float32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 247, __pyx_L1_error)
+    __pyx_t_8 = __pyx_PyFloat_AsFloat(__pyx_v_tmp); if (unlikely((__pyx_t_8 == ((npy_float32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 250, __pyx_L1_error)
     __pyx_v_upper_bound = __pyx_t_8;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:             # <<<<<<<<<<<<<<
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  */
   }
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":249
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":252
  *         upper_bound = tmp
  * 
  *     for z in range(z_size):             # <<<<<<<<<<<<<<
  *         for y in range(y_size):
  *             for x in range(x_size):
  */
   __pyx_t_9 = __pyx_v_z_size;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_z = __pyx_t_11;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":250
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
  * 
  *     for z in range(z_size):
  *         for y in range(y_size):             # <<<<<<<<<<<<<<
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  */
     __pyx_t_12 = __pyx_v_y_size;
     __pyx_t_13 = __pyx_t_12;
     for (__pyx_t_14 = 0; __pyx_t_14 < __pyx_t_13; __pyx_t_14+=1) {
       __pyx_v_y = __pyx_t_14;
 
-      /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":251
+      /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":254
  *     for z in range(z_size):
  *         for y in range(y_size):
  *             for x in range(x_size):             # <<<<<<<<<<<<<<
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:
  */
       __pyx_t_15 = __pyx_v_x_size;
       __pyx_t_16 = __pyx_t_15;
       for (__pyx_t_17 = 0; __pyx_t_17 < __pyx_t_16; __pyx_t_17+=1) {
         __pyx_v_x = __pyx_t_17;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":252
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":255
  *         for y in range(y_size):
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]             # <<<<<<<<<<<<<<
  *                 if point_val < mid_point:
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  */
         __pyx_t_18 = __pyx_v_z;
         __pyx_t_19 = __pyx_v_y;
         __pyx_t_20 = __pyx_v_x;
         if (__pyx_t_18 < 0) __pyx_t_18 += __pyx_pybuffernd_image.diminfo[0].shape;
         if (__pyx_t_19 < 0) __pyx_t_19 += __pyx_pybuffernd_image.diminfo[1].shape;
         if (__pyx_t_20 < 0) __pyx_t_20 += __pyx_pybuffernd_image.diminfo[2].shape;
         __pyx_v_point_val = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float32_t *, __pyx_pybuffernd_image.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_image.diminfo[0].strides, __pyx_t_19, __pyx_pybuffernd_image.diminfo[1].strides, __pyx_t_20, __pyx_pybuffernd_image.diminfo[2].strides));
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:             # <<<<<<<<<<<<<<
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  */
         __pyx_t_7 = ((__pyx_v_point_val < __pyx_v_mid_point) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":254
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)             # <<<<<<<<<<<<<<
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  */
           __pyx_t_8 = (__pyx_v_mid_point - __pyx_v_point_val);
           __pyx_t_21 = (__pyx_v_mid_point - __pyx_v_lower_bound);
           if (unlikely(__pyx_t_21 == 0)) {
             PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-            __PYX_ERR(0, 254, __pyx_L1_error)
+            __PYX_ERR(0, 257, __pyx_L1_error)
           }
           __pyx_v_res_val = (__pyx_t_8 / __pyx_t_21);
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:             # <<<<<<<<<<<<<<
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  */
           goto __pyx_L10;
         }
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)             # <<<<<<<<<<<<<<
  *                 if res_val > 1:
  *                     res_val = 1
  */
         /*else*/ {
           __pyx_t_21 = (__pyx_v_point_val - __pyx_v_mid_point);
           __pyx_t_8 = (__pyx_v_upper_bound - __pyx_v_mid_point);
           if (unlikely(__pyx_t_8 == 0)) {
             PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-            __PYX_ERR(0, 256, __pyx_L1_error)
+            __PYX_ERR(0, 259, __pyx_L1_error)
           }
           __pyx_v_res_val = (__pyx_t_21 / __pyx_t_8);
         }
         __pyx_L10:;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:             # <<<<<<<<<<<<<<
  *                     res_val = 1
  *                 elif res_val < 0:
  */
         __pyx_t_7 = ((__pyx_v_res_val > 1.0) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":258
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":261
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:
  *                     res_val = 1             # <<<<<<<<<<<<<<
  *                 elif res_val < 0:
  *                     res_val = 0
  */
           __pyx_v_res_val = 1.0;
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:             # <<<<<<<<<<<<<<
  *                     res_val = 1
  *                 elif res_val < 0:
  */
           goto __pyx_L11;
         }
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
  *                 if res_val > 1:
  *                     res_val = 1
  *                 elif res_val < 0:             # <<<<<<<<<<<<<<
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  */
         __pyx_t_7 = ((__pyx_v_res_val < 0.0) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":263
  *                     res_val = 1
  *                 elif res_val < 0:
  *                     res_val = 0             # <<<<<<<<<<<<<<
  *                 res[z, y, x] = res_val
  *     return res
  */
           __pyx_v_res_val = 0.0;
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
  *                 if res_val > 1:
  *                     res_val = 1
  *                 elif res_val < 0:             # <<<<<<<<<<<<<<
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  */
         }
         __pyx_L11:;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":261
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":264
  *                 elif res_val < 0:
  *                     res_val = 0
  *                 res[z, y, x] = res_val             # <<<<<<<<<<<<<<
  *     return res
  * 
  */
         __pyx_t_22 = __pyx_v_z;
@@ -18778,27 +18837,27 @@
         if (__pyx_t_23 < 0) __pyx_t_23 += __pyx_pybuffernd_res.diminfo[1].shape;
         if (__pyx_t_24 < 0) __pyx_t_24 += __pyx_pybuffernd_res.diminfo[2].shape;
         *__Pyx_BufPtrStrided3d(__pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_mu_type *, __pyx_pybuffernd_res.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_res.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_res.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_res.diminfo[2].strides) = __pyx_v_res_val;
       }
     }
   }
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":265
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  *     return res             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_res));
   __pyx_r = ((PyObject *)__pyx_v_res);
   goto __pyx_L0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":235
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":238
  * 
  * @cython.boundscheck(False)
  * def calculate_mu_mid(numpy.ndarray[image_types, ndim=3] image, image_types lower_bound, image_types mid_point,             # <<<<<<<<<<<<<<
  *                  image_types upper_bound):
  *     cdef int16_t x_size, y_size, z_size, x, y, z
  */
 
@@ -18864,54 +18923,54 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_image)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_lower_bound)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 1); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 1); __PYX_ERR(0, 238, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mid_point)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 2); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 2); __PYX_ERR(0, 238, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_upper_bound)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 3); __PYX_ERR(0, 235, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, 3); __PYX_ERR(0, 238, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "calculate_mu_mid") < 0)) __PYX_ERR(0, 235, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "calculate_mu_mid") < 0)) __PYX_ERR(0, 238, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
     __pyx_v_image = ((PyArrayObject *)values[0]);
-    __pyx_v_lower_bound = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_lower_bound == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L3_error)
-    __pyx_v_mid_point = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_mid_point == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L3_error)
-    __pyx_v_upper_bound = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_upper_bound == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 236, __pyx_L3_error)
+    __pyx_v_lower_bound = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_lower_bound == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L3_error)
+    __pyx_v_mid_point = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_mid_point == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L3_error)
+    __pyx_v_upper_bound = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_upper_bound == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 239, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 235, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("calculate_mu_mid", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 238, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("PartSeg.utils.multiscale_opening.mso_bind.calculate_mu_mid", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_image), __pyx_ptype_5numpy_ndarray, 1, "image", 0))) __PYX_ERR(0, 235, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_image), __pyx_ptype_5numpy_ndarray, 1, "image", 0))) __PYX_ERR(0, 238, __pyx_L1_error)
   __pyx_r = __pyx_pf_7PartSeg_5utils_18multiscale_opening_8mso_bind_32calculate_mu_mid(__pyx_self, __pyx_v_image, __pyx_v_lower_bound, __pyx_v_mid_point, __pyx_v_upper_bound);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -18967,320 +19026,320 @@
   __pyx_pybuffernd_res.rcbuffer = &__pyx_pybuffer_res;
   __pyx_pybuffer_image.pybuffer.buf = NULL;
   __pyx_pybuffer_image.refcount = 0;
   __pyx_pybuffernd_image.data = NULL;
   __pyx_pybuffernd_image.rcbuffer = &__pyx_pybuffer_image;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_image.rcbuffer->pybuffer, (PyObject*)__pyx_v_image, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 235, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_image.rcbuffer->pybuffer, (PyObject*)__pyx_v_image, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 238, __pyx_L1_error)
   }
   __pyx_pybuffernd_image.diminfo[0].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_image.diminfo[0].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_image.diminfo[1].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_image.diminfo[1].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_image.diminfo[2].strides = __pyx_pybuffernd_image.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_image.diminfo[2].shape = __pyx_pybuffernd_image.rcbuffer->pybuffer.shape[2];
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":240
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":243
  *     cdef mu_type res_val
  *     cdef image_types point_val
  *     x_size = image.shape[2]             # <<<<<<<<<<<<<<
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]
  */
   __pyx_v_x_size = (__pyx_v_image->dimensions[2]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":241
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
  *     cdef image_types point_val
  *     x_size = image.shape[2]
  *     y_size = image.shape[1]             # <<<<<<<<<<<<<<
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  */
   __pyx_v_y_size = (__pyx_v_image->dimensions[1]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":242
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":245
  *     x_size = image.shape[2]
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:
  */
   __pyx_v_z_size = (__pyx_v_image->dimensions[0]);
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":243
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":246
  *     y_size = image.shape[1]
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)             # <<<<<<<<<<<<<<
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_numpy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_npy_int16(__pyx_v_z_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_npy_int16(__pyx_v_z_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_From_npy_int16(__pyx_v_y_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_npy_int16(__pyx_v_y_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_npy_int16(__pyx_v_x_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_npy_int16(__pyx_v_x_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_4);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 246, __pyx_L1_error)
   __pyx_t_6 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_res.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_mu_type, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 3, 0, __pyx_stack) == -1)) {
       __pyx_v_res = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_res.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 243, __pyx_L1_error)
+      __PYX_ERR(0, 246, __pyx_L1_error)
     } else {__pyx_pybuffernd_res.diminfo[0].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_res.diminfo[0].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_res.diminfo[1].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_res.diminfo[1].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_res.diminfo[2].strides = __pyx_pybuffernd_res.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_res.diminfo[2].shape = __pyx_pybuffernd_res.rcbuffer->pybuffer.shape[2];
     }
   }
   __pyx_t_6 = 0;
   __pyx_v_res = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:             # <<<<<<<<<<<<<<
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  */
   __pyx_t_7 = ((__pyx_v_upper_bound < __pyx_v_lower_bound) != 0);
   if (__pyx_t_7) {
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":245
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":248
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound             # <<<<<<<<<<<<<<
  *         lower_bound = upper_bound
  *         upper_bound = tmp
  */
-    __pyx_t_1 = PyFloat_FromDouble(__pyx_v_lower_bound); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
+    __pyx_t_1 = PyFloat_FromDouble(__pyx_v_lower_bound); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_tmp = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":246
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":249
  *     if upper_bound < lower_bound:
  *         tmp = lower_bound
  *         lower_bound = upper_bound             # <<<<<<<<<<<<<<
  *         upper_bound = tmp
  * 
  */
     __pyx_v_lower_bound = __pyx_v_upper_bound;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":250
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  *         upper_bound = tmp             # <<<<<<<<<<<<<<
  * 
  *     for z in range(z_size):
  */
-    __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_tmp); if (unlikely((__pyx_t_8 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 247, __pyx_L1_error)
+    __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_tmp); if (unlikely((__pyx_t_8 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 250, __pyx_L1_error)
     __pyx_v_upper_bound = __pyx_t_8;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":244
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":247
  *     z_size = image.shape[0]
  *     cdef numpy.ndarray[mu_type, ndim=3] res = numpy.empty((z_size, y_size, x_size), dtype=numpy.float64)
  *     if upper_bound < lower_bound:             # <<<<<<<<<<<<<<
  *         tmp = lower_bound
  *         lower_bound = upper_bound
  */
   }
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":249
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":252
  *         upper_bound = tmp
  * 
  *     for z in range(z_size):             # <<<<<<<<<<<<<<
  *         for y in range(y_size):
  *             for x in range(x_size):
  */
   __pyx_t_9 = __pyx_v_z_size;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_z = __pyx_t_11;
 
-    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":250
+    /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
  * 
  *     for z in range(z_size):
  *         for y in range(y_size):             # <<<<<<<<<<<<<<
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  */
     __pyx_t_12 = __pyx_v_y_size;
     __pyx_t_13 = __pyx_t_12;
     for (__pyx_t_14 = 0; __pyx_t_14 < __pyx_t_13; __pyx_t_14+=1) {
       __pyx_v_y = __pyx_t_14;
 
-      /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":251
+      /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":254
  *     for z in range(z_size):
  *         for y in range(y_size):
  *             for x in range(x_size):             # <<<<<<<<<<<<<<
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:
  */
       __pyx_t_15 = __pyx_v_x_size;
       __pyx_t_16 = __pyx_t_15;
       for (__pyx_t_17 = 0; __pyx_t_17 < __pyx_t_16; __pyx_t_17+=1) {
         __pyx_v_x = __pyx_t_17;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":252
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":255
  *         for y in range(y_size):
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]             # <<<<<<<<<<<<<<
  *                 if point_val < mid_point:
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  */
         __pyx_t_18 = __pyx_v_z;
         __pyx_t_19 = __pyx_v_y;
         __pyx_t_20 = __pyx_v_x;
         if (__pyx_t_18 < 0) __pyx_t_18 += __pyx_pybuffernd_image.diminfo[0].shape;
         if (__pyx_t_19 < 0) __pyx_t_19 += __pyx_pybuffernd_image.diminfo[1].shape;
         if (__pyx_t_20 < 0) __pyx_t_20 += __pyx_pybuffernd_image.diminfo[2].shape;
         __pyx_v_point_val = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_image.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_image.diminfo[0].strides, __pyx_t_19, __pyx_pybuffernd_image.diminfo[1].strides, __pyx_t_20, __pyx_pybuffernd_image.diminfo[2].strides));
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:             # <<<<<<<<<<<<<<
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  */
         __pyx_t_7 = ((__pyx_v_point_val < __pyx_v_mid_point) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":254
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)             # <<<<<<<<<<<<<<
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  */
           __pyx_t_8 = (__pyx_v_mid_point - __pyx_v_point_val);
           __pyx_t_21 = (__pyx_v_mid_point - __pyx_v_lower_bound);
           if (unlikely(__pyx_t_21 == 0)) {
             PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-            __PYX_ERR(0, 254, __pyx_L1_error)
+            __PYX_ERR(0, 257, __pyx_L1_error)
           }
           __pyx_v_res_val = (__pyx_t_8 / __pyx_t_21);
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":253
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
  *             for x in range(x_size):
  *                 point_val = image[z, y, x]
  *                 if point_val < mid_point:             # <<<<<<<<<<<<<<
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  */
           goto __pyx_L10;
         }
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":256
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
  *                     res_val = (mid_point - point_val)/(mid_point - lower_bound)
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)             # <<<<<<<<<<<<<<
  *                 if res_val > 1:
  *                     res_val = 1
  */
         /*else*/ {
           __pyx_t_21 = (__pyx_v_point_val - __pyx_v_mid_point);
           __pyx_t_8 = (__pyx_v_upper_bound - __pyx_v_mid_point);
           if (unlikely(__pyx_t_8 == 0)) {
             PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-            __PYX_ERR(0, 256, __pyx_L1_error)
+            __PYX_ERR(0, 259, __pyx_L1_error)
           }
           __pyx_v_res_val = (__pyx_t_21 / __pyx_t_8);
         }
         __pyx_L10:;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:             # <<<<<<<<<<<<<<
  *                     res_val = 1
  *                 elif res_val < 0:
  */
         __pyx_t_7 = ((__pyx_v_res_val > 1.0) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":258
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":261
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:
  *                     res_val = 1             # <<<<<<<<<<<<<<
  *                 elif res_val < 0:
  *                     res_val = 0
  */
           __pyx_v_res_val = 1.0;
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":257
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
  *                 else:
  *                     res_val = (point_val - mid_point)/(upper_bound - mid_point)
  *                 if res_val > 1:             # <<<<<<<<<<<<<<
  *                     res_val = 1
  *                 elif res_val < 0:
  */
           goto __pyx_L11;
         }
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
  *                 if res_val > 1:
  *                     res_val = 1
  *                 elif res_val < 0:             # <<<<<<<<<<<<<<
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  */
         __pyx_t_7 = ((__pyx_v_res_val < 0.0) != 0);
         if (__pyx_t_7) {
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":260
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":263
  *                     res_val = 1
  *                 elif res_val < 0:
  *                     res_val = 0             # <<<<<<<<<<<<<<
  *                 res[z, y, x] = res_val
  *     return res
  */
           __pyx_v_res_val = 0.0;
 
-          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":259
+          /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
  *                 if res_val > 1:
  *                     res_val = 1
  *                 elif res_val < 0:             # <<<<<<<<<<<<<<
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  */
         }
         __pyx_L11:;
 
-        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":261
+        /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":264
  *                 elif res_val < 0:
  *                     res_val = 0
  *                 res[z, y, x] = res_val             # <<<<<<<<<<<<<<
  *     return res
  * 
  */
         __pyx_t_22 = __pyx_v_z;
@@ -19290,27 +19349,27 @@
         if (__pyx_t_23 < 0) __pyx_t_23 += __pyx_pybuffernd_res.diminfo[1].shape;
         if (__pyx_t_24 < 0) __pyx_t_24 += __pyx_pybuffernd_res.diminfo[2].shape;
         *__Pyx_BufPtrStrided3d(__pyx_t_7PartSeg_5utils_18multiscale_opening_8mso_bind_mu_type *, __pyx_pybuffernd_res.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_res.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_res.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_res.diminfo[2].strides) = __pyx_v_res_val;
       }
     }
   }
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":262
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":265
  *                     res_val = 0
  *                 res[z, y, x] = res_val
  *     return res             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_res));
   __pyx_r = ((PyObject *)__pyx_v_res);
   goto __pyx_L0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":235
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":238
  * 
  * @cython.boundscheck(False)
  * def calculate_mu_mid(numpy.ndarray[image_types, ndim=3] image, image_types lower_bound, image_types mid_point,             # <<<<<<<<<<<<<<
  *                  image_types upper_bound):
  *     cdef int16_t x_size, y_size, z_size, x, y, z
  */
 
@@ -19338,15 +19397,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_res);
   __Pyx_XDECREF(__pyx_v_tmp);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":258
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":258
  *         # experimental exception made for __getbuffer__ and __releasebuffer__
  *         # -- the details of this may change.
  *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
  *             # This implementation of getbuffer is geared towards Cython
  *             # requirements, and does not yet fulfill the PEP.
  */
 
@@ -19387,344 +19446,344 @@
     PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
     return -1;
   }
   __Pyx_RefNannySetupContext("__getbuffer__", 0);
   __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(__pyx_v_info->obj);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":265
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":265
  * 
  *             cdef int i, ndim
  *             cdef int endian_detector = 1             # <<<<<<<<<<<<<<
  *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
  * 
  */
   __pyx_v_endian_detector = 1;
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":266
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":266
  *             cdef int i, ndim
  *             cdef int endian_detector = 1
  *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
  * 
  *             ndim = PyArray_NDIM(self)
  */
   __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":268
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":268
  *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
  * 
  *             ndim = PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  */
   __pyx_v_ndim = PyArray_NDIM(__pyx_v_self);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":270
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":270
  *             ndim = PyArray_NDIM(self)
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")
  */
   __pyx_t_2 = (((__pyx_v_flags & PyBUF_C_CONTIGUOUS) == PyBUF_C_CONTIGUOUS) != 0);
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L4_bool_binop_done;
   }
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":271
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":271
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):             # <<<<<<<<<<<<<<
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  */
   __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_C_CONTIGUOUS) != 0)) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":270
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":270
  *             ndim = PyArray_NDIM(self)
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")
  */
   if (unlikely(__pyx_t_1)) {
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":272
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":272
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  */
     __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__49, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 272, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 272, __pyx_L1_error)
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":270
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":270
  *             ndim = PyArray_NDIM(self)
  * 
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")
  */
   }
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":274
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":274
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  */
   __pyx_t_2 = (((__pyx_v_flags & PyBUF_F_CONTIGUOUS) == PyBUF_F_CONTIGUOUS) != 0);
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L7_bool_binop_done;
   }
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":275
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":275
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):             # <<<<<<<<<<<<<<
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  * 
  */
   __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_F_CONTIGUOUS) != 0)) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L7_bool_binop_done:;
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":274
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":274
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  */
   if (unlikely(__pyx_t_1)) {
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":276
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":276
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
  * 
  *             info.buf = PyArray_DATA(self)
  */
     __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__50, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 276, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 276, __pyx_L1_error)
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":274
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":274
  *                 raise ValueError(u"ndarray is not C contiguous")
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  */
   }
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":278
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":278
  *                 raise ValueError(u"ndarray is not Fortran contiguous")
  * 
  *             info.buf = PyArray_DATA(self)             # <<<<<<<<<<<<<<
  *             info.ndim = ndim
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  */
   __pyx_v_info->buf = PyArray_DATA(__pyx_v_self);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":279
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":279
  * 
  *             info.buf = PyArray_DATA(self)
  *             info.ndim = ndim             # <<<<<<<<<<<<<<
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  *                 # Allocate new buffer for strides and shape info.
  */
   __pyx_v_info->ndim = __pyx_v_ndim;
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":280
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":280
  *             info.buf = PyArray_DATA(self)
  *             info.ndim = ndim
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
  *                 # Allocate new buffer for strides and shape info.
  *                 # This is allocated as one block, strides first.
  */
   __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":283
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":283
  *                 # Allocate new buffer for strides and shape info.
  *                 # This is allocated as one block, strides first.
  *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)             # <<<<<<<<<<<<<<
  *                 info.shape = info.strides + ndim
  *                 for i in range(ndim):
  */
     __pyx_v_info->strides = ((Py_ssize_t *)PyObject_Malloc((((sizeof(Py_ssize_t)) * 2) * ((size_t)__pyx_v_ndim))));
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":284
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":284
  *                 # This is allocated as one block, strides first.
  *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
  *                 info.shape = info.strides + ndim             # <<<<<<<<<<<<<<
  *                 for i in range(ndim):
  *                     info.strides[i] = PyArray_STRIDES(self)[i]
  */
     __pyx_v_info->shape = (__pyx_v_info->strides + __pyx_v_ndim);
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":285
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":285
  *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
  *                 info.shape = info.strides + ndim
  *                 for i in range(ndim):             # <<<<<<<<<<<<<<
  *                     info.strides[i] = PyArray_STRIDES(self)[i]
  *                     info.shape[i] = PyArray_DIMS(self)[i]
  */
     __pyx_t_4 = __pyx_v_ndim;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_i = __pyx_t_6;
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":286
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":286
  *                 info.shape = info.strides + ndim
  *                 for i in range(ndim):
  *                     info.strides[i] = PyArray_STRIDES(self)[i]             # <<<<<<<<<<<<<<
  *                     info.shape[i] = PyArray_DIMS(self)[i]
  *             else:
  */
       (__pyx_v_info->strides[__pyx_v_i]) = (PyArray_STRIDES(__pyx_v_self)[__pyx_v_i]);
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":287
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":287
  *                 for i in range(ndim):
  *                     info.strides[i] = PyArray_STRIDES(self)[i]
  *                     info.shape[i] = PyArray_DIMS(self)[i]             # <<<<<<<<<<<<<<
  *             else:
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
  */
       (__pyx_v_info->shape[__pyx_v_i]) = (PyArray_DIMS(__pyx_v_self)[__pyx_v_i]);
     }
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":280
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":280
  *             info.buf = PyArray_DATA(self)
  *             info.ndim = ndim
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
  *                 # Allocate new buffer for strides and shape info.
  *                 # This is allocated as one block, strides first.
  */
     goto __pyx_L9;
   }
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":289
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":289
  *                     info.shape[i] = PyArray_DIMS(self)[i]
  *             else:
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
  *             info.suboffsets = NULL
  */
   /*else*/ {
     __pyx_v_info->strides = ((Py_ssize_t *)PyArray_STRIDES(__pyx_v_self));
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":290
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":290
  *             else:
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  *             info.suboffsets = NULL
  *             info.itemsize = PyArray_ITEMSIZE(self)
  */
     __pyx_v_info->shape = ((Py_ssize_t *)PyArray_DIMS(__pyx_v_self));
   }
   __pyx_L9:;
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":291
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":291
  *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
  *             info.suboffsets = NULL             # <<<<<<<<<<<<<<
  *             info.itemsize = PyArray_ITEMSIZE(self)
  *             info.readonly = not PyArray_ISWRITEABLE(self)
  */
   __pyx_v_info->suboffsets = NULL;
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":292
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":292
  *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
  *             info.suboffsets = NULL
  *             info.itemsize = PyArray_ITEMSIZE(self)             # <<<<<<<<<<<<<<
  *             info.readonly = not PyArray_ISWRITEABLE(self)
  * 
  */
   __pyx_v_info->itemsize = PyArray_ITEMSIZE(__pyx_v_self);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":293
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":293
  *             info.suboffsets = NULL
  *             info.itemsize = PyArray_ITEMSIZE(self)
  *             info.readonly = not PyArray_ISWRITEABLE(self)             # <<<<<<<<<<<<<<
  * 
  *             cdef int t
  */
   __pyx_v_info->readonly = (!(PyArray_ISWRITEABLE(__pyx_v_self) != 0));
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":296
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":296
  * 
  *             cdef int t
  *             cdef char* f = NULL             # <<<<<<<<<<<<<<
  *             cdef dtype descr = <dtype>PyArray_DESCR(self)
  *             cdef int offset
  */
   __pyx_v_f = NULL;
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":297
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":297
  *             cdef int t
  *             cdef char* f = NULL
  *             cdef dtype descr = <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  *             cdef int offset
  * 
  */
   __pyx_t_7 = PyArray_DESCR(__pyx_v_self);
   __pyx_t_3 = ((PyObject *)__pyx_t_7);
   __Pyx_INCREF(__pyx_t_3);
   __pyx_v_descr = ((PyArray_Descr *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":300
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":300
  *             cdef int offset
  * 
  *             info.obj = self             # <<<<<<<<<<<<<<
  * 
  *             if not PyDataType_HASFIELDS(descr):
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   __Pyx_GOTREF(__pyx_v_info->obj);
   __Pyx_DECREF(__pyx_v_info->obj);
   __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":302
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":302
  *             info.obj = self
  * 
  *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or
  */
   __pyx_t_1 = ((!(PyDataType_HASFIELDS(__pyx_v_descr) != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":303
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":303
  * 
  *             if not PyDataType_HASFIELDS(descr):
  *                 t = descr.type_num             # <<<<<<<<<<<<<<
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):
  */
     __pyx_t_4 = __pyx_v_descr->type_num;
     __pyx_v_t = __pyx_t_4;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":304
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":304
  *             if not PyDataType_HASFIELDS(descr):
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  */
     __pyx_t_2 = ((__pyx_v_descr->byteorder == '>') != 0);
@@ -19736,15 +19795,15 @@
     if (!__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L14_bool_binop_done;
     }
     __pyx_L15_next_or:;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":305
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":305
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
  *                     raise ValueError(u"Non-native byte order not supported")
  *                 if   t == NPY_BYTE:        f = "b"
  */
     __pyx_t_2 = ((__pyx_v_descr->byteorder == '<') != 0);
@@ -19753,235 +19812,235 @@
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L14_bool_binop_done;
     }
     __pyx_t_2 = ((!(__pyx_v_little_endian != 0)) != 0);
     __pyx_t_1 = __pyx_t_2;
     __pyx_L14_bool_binop_done:;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":304
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":304
  *             if not PyDataType_HASFIELDS(descr):
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  */
     if (unlikely(__pyx_t_1)) {
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":306
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":306
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"
  */
       __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__51, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 306, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __PYX_ERR(2, 306, __pyx_L1_error)
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":304
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":304
  *             if not PyDataType_HASFIELDS(descr):
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  */
     }
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":307
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":307
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")
  *                 if   t == NPY_BYTE:        f = "b"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_UBYTE:       f = "B"
  *                 elif t == NPY_SHORT:       f = "h"
  */
     switch (__pyx_v_t) {
       case NPY_BYTE:
       __pyx_v_f = ((char *)"b");
       break;
       case NPY_UBYTE:
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":308
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":308
  *                     raise ValueError(u"Non-native byte order not supported")
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_SHORT:       f = "h"
  *                 elif t == NPY_USHORT:      f = "H"
  */
       __pyx_v_f = ((char *)"B");
       break;
       case NPY_SHORT:
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":309
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":309
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"
  *                 elif t == NPY_SHORT:       f = "h"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_USHORT:      f = "H"
  *                 elif t == NPY_INT:         f = "i"
  */
       __pyx_v_f = ((char *)"h");
       break;
       case NPY_USHORT:
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":310
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":310
  *                 elif t == NPY_UBYTE:       f = "B"
  *                 elif t == NPY_SHORT:       f = "h"
  *                 elif t == NPY_USHORT:      f = "H"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_INT:         f = "i"
  *                 elif t == NPY_UINT:        f = "I"
  */
       __pyx_v_f = ((char *)"H");
       break;
       case NPY_INT:
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":311
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":311
  *                 elif t == NPY_SHORT:       f = "h"
  *                 elif t == NPY_USHORT:      f = "H"
  *                 elif t == NPY_INT:         f = "i"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_UINT:        f = "I"
  *                 elif t == NPY_LONG:        f = "l"
  */
       __pyx_v_f = ((char *)"i");
       break;
       case NPY_UINT:
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":312
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":312
  *                 elif t == NPY_USHORT:      f = "H"
  *                 elif t == NPY_INT:         f = "i"
  *                 elif t == NPY_UINT:        f = "I"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_LONG:        f = "l"
  *                 elif t == NPY_ULONG:       f = "L"
  */
       __pyx_v_f = ((char *)"I");
       break;
       case NPY_LONG:
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":313
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":313
  *                 elif t == NPY_INT:         f = "i"
  *                 elif t == NPY_UINT:        f = "I"
  *                 elif t == NPY_LONG:        f = "l"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_ULONG:       f = "L"
  *                 elif t == NPY_LONGLONG:    f = "q"
  */
       __pyx_v_f = ((char *)"l");
       break;
       case NPY_ULONG:
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":314
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":314
  *                 elif t == NPY_UINT:        f = "I"
  *                 elif t == NPY_LONG:        f = "l"
  *                 elif t == NPY_ULONG:       f = "L"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_LONGLONG:    f = "q"
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  */
       __pyx_v_f = ((char *)"L");
       break;
       case NPY_LONGLONG:
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":315
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":315
  *                 elif t == NPY_LONG:        f = "l"
  *                 elif t == NPY_ULONG:       f = "L"
  *                 elif t == NPY_LONGLONG:    f = "q"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  *                 elif t == NPY_FLOAT:       f = "f"
  */
       __pyx_v_f = ((char *)"q");
       break;
       case NPY_ULONGLONG:
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":316
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":316
  *                 elif t == NPY_ULONG:       f = "L"
  *                 elif t == NPY_LONGLONG:    f = "q"
  *                 elif t == NPY_ULONGLONG:   f = "Q"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_FLOAT:       f = "f"
  *                 elif t == NPY_DOUBLE:      f = "d"
  */
       __pyx_v_f = ((char *)"Q");
       break;
       case NPY_FLOAT:
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":317
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":317
  *                 elif t == NPY_LONGLONG:    f = "q"
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  *                 elif t == NPY_FLOAT:       f = "f"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_DOUBLE:      f = "d"
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  */
       __pyx_v_f = ((char *)"f");
       break;
       case NPY_DOUBLE:
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":318
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":318
  *                 elif t == NPY_ULONGLONG:   f = "Q"
  *                 elif t == NPY_FLOAT:       f = "f"
  *                 elif t == NPY_DOUBLE:      f = "d"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  */
       __pyx_v_f = ((char *)"d");
       break;
       case NPY_LONGDOUBLE:
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":319
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":319
  *                 elif t == NPY_FLOAT:       f = "f"
  *                 elif t == NPY_DOUBLE:      f = "d"
  *                 elif t == NPY_LONGDOUBLE:  f = "g"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  */
       __pyx_v_f = ((char *)"g");
       break;
       case NPY_CFLOAT:
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":320
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":320
  *                 elif t == NPY_DOUBLE:      f = "d"
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  *                 elif t == NPY_CFLOAT:      f = "Zf"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
  */
       __pyx_v_f = ((char *)"Zf");
       break;
       case NPY_CDOUBLE:
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":321
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":321
  *                 elif t == NPY_LONGDOUBLE:  f = "g"
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  *                 elif t == NPY_CDOUBLE:     f = "Zd"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
  *                 elif t == NPY_OBJECT:      f = "O"
  */
       __pyx_v_f = ((char *)"Zd");
       break;
       case NPY_CLONGDOUBLE:
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":322
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":322
  *                 elif t == NPY_CFLOAT:      f = "Zf"
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"             # <<<<<<<<<<<<<<
  *                 elif t == NPY_OBJECT:      f = "O"
  *                 else:
  */
       __pyx_v_f = ((char *)"Zg");
       break;
       case NPY_OBJECT:
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":323
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":323
  *                 elif t == NPY_CDOUBLE:     f = "Zd"
  *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
  *                 elif t == NPY_OBJECT:      f = "O"             # <<<<<<<<<<<<<<
  *                 else:
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  */
       __pyx_v_f = ((char *)"O");
       break;
       default:
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":325
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":325
  *                 elif t == NPY_OBJECT:      f = "O"
  *                 else:
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
  *                 info.format = f
  *                 return
  */
       __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 325, __pyx_L1_error)
@@ -19994,91 +20053,91 @@
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __PYX_ERR(2, 325, __pyx_L1_error)
       break;
     }
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":326
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":326
  *                 else:
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  *                 info.format = f             # <<<<<<<<<<<<<<
  *                 return
  *             else:
  */
     __pyx_v_info->format = __pyx_v_f;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":327
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":327
  *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  *                 info.format = f
  *                 return             # <<<<<<<<<<<<<<
  *             else:
  *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
  */
     __pyx_r = 0;
     goto __pyx_L0;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":302
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":302
  *             info.obj = self
  * 
  *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
  *                 t = descr.type_num
  *                 if ((descr.byteorder == c'>' and little_endian) or
  */
   }
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":329
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":329
  *                 return
  *             else:
  *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)             # <<<<<<<<<<<<<<
  *                 info.format[0] = c'^' # Native data types, manual alignment
  *                 offset = 0
  */
   /*else*/ {
     __pyx_v_info->format = ((char *)PyObject_Malloc(0xFF));
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":330
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":330
  *             else:
  *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
  *                 info.format[0] = c'^' # Native data types, manual alignment             # <<<<<<<<<<<<<<
  *                 offset = 0
  *                 f = _util_dtypestring(descr, info.format + 1,
  */
     (__pyx_v_info->format[0]) = '^';
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":331
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":331
  *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
  *                 info.format[0] = c'^' # Native data types, manual alignment
  *                 offset = 0             # <<<<<<<<<<<<<<
  *                 f = _util_dtypestring(descr, info.format + 1,
  *                                       info.format + _buffer_format_string_len,
  */
     __pyx_v_offset = 0;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":332
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":332
  *                 info.format[0] = c'^' # Native data types, manual alignment
  *                 offset = 0
  *                 f = _util_dtypestring(descr, info.format + 1,             # <<<<<<<<<<<<<<
  *                                       info.format + _buffer_format_string_len,
  *                                       &offset)
  */
     __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_descr, (__pyx_v_info->format + 1), (__pyx_v_info->format + 0xFF), (&__pyx_v_offset)); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(2, 332, __pyx_L1_error)
     __pyx_v_f = __pyx_t_9;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":335
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":335
  *                                       info.format + _buffer_format_string_len,
  *                                       &offset)
  *                 f[0] = c'\0' # Terminate format string             # <<<<<<<<<<<<<<
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  */
     (__pyx_v_f[0]) = '\x00';
   }
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":258
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":258
  *         # experimental exception made for __getbuffer__ and __releasebuffer__
  *         # -- the details of this may change.
  *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
  *             # This implementation of getbuffer is geared towards Cython
  *             # requirements, and does not yet fulfill the PEP.
  */
 
@@ -20102,15 +20161,15 @@
   }
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_descr);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":337
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":337
  *                 f[0] = c'\0' # Terminate format string
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)
  */
 
@@ -20126,111 +20185,111 @@
 }
 
 static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__releasebuffer__", 0);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":338
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":338
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  */
   __pyx_t_1 = (PyArray_HASFIELDS(__pyx_v_self) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":339
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":339
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)             # <<<<<<<<<<<<<<
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  *                 PyObject_Free(info.strides)
  */
     PyObject_Free(__pyx_v_info->format);
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":338
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":338
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):
  *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  */
   }
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":340
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":340
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
  *                 PyObject_Free(info.strides)
  *                 # info.shape was stored after info.strides in the same block
  */
   __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":341
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":341
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
  *                 PyObject_Free(info.strides)             # <<<<<<<<<<<<<<
  *                 # info.shape was stored after info.strides in the same block
  * 
  */
     PyObject_Free(__pyx_v_info->strides);
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":340
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":340
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)
  *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
  *                 PyObject_Free(info.strides)
  *                 # info.shape was stored after info.strides in the same block
  */
   }
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":337
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":337
  *                 f[0] = c'\0' # Terminate format string
  * 
  *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
  *             if PyArray_HASFIELDS(self):
  *                 PyObject_Free(info.format)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":821
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":821
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":822
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":822
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 822, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":821
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":821
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -20241,43 +20300,43 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":824
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":824
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":825
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":825
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 825, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":824
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":824
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -20288,43 +20347,43 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":827
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":827
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":828
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":828
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 828, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":827
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":827
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -20335,43 +20394,43 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":830
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":830
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":831
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":831
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 831, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":830
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":830
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -20382,43 +20441,43 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":833
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":833
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":834
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":834
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 834, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":833
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":833
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -20429,89 +20488,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":836
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":836
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":837
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":837
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":838
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":838
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":837
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":837
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":840
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":840
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":836
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":836
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":842
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":842
  *         return ()
  * 
  * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
  *     # Recursive utility function used in __getbuffer__ to get format
  *     # string. The new location in the format string is returned.
  */
 
@@ -20532,33 +20591,33 @@
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_t_7;
   long __pyx_t_8;
   char *__pyx_t_9;
   __Pyx_RefNannySetupContext("_util_dtypestring", 0);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":847
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":847
  * 
  *     cdef dtype child
  *     cdef int endian_detector = 1             # <<<<<<<<<<<<<<
  *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
  *     cdef tuple fields
  */
   __pyx_v_endian_detector = 1;
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":848
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":848
  *     cdef dtype child
  *     cdef int endian_detector = 1
  *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
  *     cdef tuple fields
  * 
  */
   __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":851
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":851
  *     cdef tuple fields
  * 
  *     for childname in descr.names:             # <<<<<<<<<<<<<<
  *         fields = descr.fields[childname]
  *         child, new_offset = fields
  */
   if (unlikely(__pyx_v_descr->names == Py_None)) {
@@ -20573,15 +20632,15 @@
     #else
     __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 851, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_childname, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":852
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":852
  * 
  *     for childname in descr.names:
  *         fields = descr.fields[childname]             # <<<<<<<<<<<<<<
  *         child, new_offset = fields
  * 
  */
     if (unlikely(__pyx_v_descr->fields == Py_None)) {
@@ -20590,15 +20649,15 @@
     }
     __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_descr->fields, __pyx_v_childname); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 852, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (!(likely(PyTuple_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(2, 852, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_fields, ((PyObject*)__pyx_t_3));
     __pyx_t_3 = 0;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":853
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":853
  *     for childname in descr.names:
  *         fields = descr.fields[childname]
  *         child, new_offset = fields             # <<<<<<<<<<<<<<
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:
  */
     if (likely(__pyx_v_fields != Py_None)) {
@@ -20625,15 +20684,15 @@
     }
     if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_dtype))))) __PYX_ERR(2, 853, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_child, ((PyArray_Descr *)__pyx_t_3));
     __pyx_t_3 = 0;
     __Pyx_XDECREF_SET(__pyx_v_new_offset, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":855
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":855
  *         child, new_offset = fields
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  */
     __pyx_t_4 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 855, __pyx_L1_error)
@@ -20642,37 +20701,37 @@
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 855, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_6 = ((((__pyx_v_end - __pyx_v_f) - ((int)__pyx_t_5)) < 15) != 0);
     if (unlikely(__pyx_t_6)) {
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":856
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":856
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
  * 
  *         if ((child.byteorder == c'>' and little_endian) or
  */
       __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__52, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 856, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __PYX_ERR(2, 856, __pyx_L1_error)
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":855
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":855
  *         child, new_offset = fields
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  */
     }
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":858
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":858
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")
  */
     __pyx_t_7 = ((__pyx_v_child->byteorder == '>') != 0);
@@ -20684,15 +20743,15 @@
     if (!__pyx_t_7) {
     } else {
       __pyx_t_6 = __pyx_t_7;
       goto __pyx_L7_bool_binop_done;
     }
     __pyx_L8_next_or:;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":859
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":859
  * 
  *         if ((child.byteorder == c'>' and little_endian) or
  *             (child.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
  *             raise ValueError(u"Non-native byte order not supported")
  *             # One could encode it in the format string and have Cython
  */
     __pyx_t_7 = ((__pyx_v_child->byteorder == '<') != 0);
@@ -20701,46 +20760,46 @@
       __pyx_t_6 = __pyx_t_7;
       goto __pyx_L7_bool_binop_done;
     }
     __pyx_t_7 = ((!(__pyx_v_little_endian != 0)) != 0);
     __pyx_t_6 = __pyx_t_7;
     __pyx_L7_bool_binop_done:;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":858
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":858
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")
  */
     if (unlikely(__pyx_t_6)) {
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":860
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":860
  *         if ((child.byteorder == c'>' and little_endian) or
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
  *             # One could encode it in the format string and have Cython
  *             # complain instead, BUT: < and > in format strings also imply
  */
       __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__51, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 860, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __PYX_ERR(2, 860, __pyx_L1_error)
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":858
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":858
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
  * 
  *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
  *             (child.byteorder == c'<' and not little_endian)):
  *             raise ValueError(u"Non-native byte order not supported")
  */
     }
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":870
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":870
  * 
  *         # Output padding bytes
  *         while offset[0] < new_offset:             # <<<<<<<<<<<<<<
  *             f[0] = 120 # "x"; pad byte
  *             f += 1
  */
     while (1) {
@@ -20748,108 +20807,108 @@
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_v_new_offset, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 870, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 870, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (!__pyx_t_6) break;
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":871
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":871
  *         # Output padding bytes
  *         while offset[0] < new_offset:
  *             f[0] = 120 # "x"; pad byte             # <<<<<<<<<<<<<<
  *             f += 1
  *             offset[0] += 1
  */
       (__pyx_v_f[0]) = 0x78;
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":872
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":872
  *         while offset[0] < new_offset:
  *             f[0] = 120 # "x"; pad byte
  *             f += 1             # <<<<<<<<<<<<<<
  *             offset[0] += 1
  * 
  */
       __pyx_v_f = (__pyx_v_f + 1);
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":873
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":873
  *             f[0] = 120 # "x"; pad byte
  *             f += 1
  *             offset[0] += 1             # <<<<<<<<<<<<<<
  * 
  *         offset[0] += child.itemsize
  */
       __pyx_t_8 = 0;
       (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + 1);
     }
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":875
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":875
  *             offset[0] += 1
  * 
  *         offset[0] += child.itemsize             # <<<<<<<<<<<<<<
  * 
  *         if not PyDataType_HASFIELDS(child):
  */
     __pyx_t_8 = 0;
     (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + __pyx_v_child->elsize);
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":877
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":877
  *         offset[0] += child.itemsize
  * 
  *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
  *             t = child.type_num
  *             if end - f < 5:
  */
     __pyx_t_6 = ((!(PyDataType_HASFIELDS(__pyx_v_child) != 0)) != 0);
     if (__pyx_t_6) {
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":878
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":878
  * 
  *         if not PyDataType_HASFIELDS(child):
  *             t = child.type_num             # <<<<<<<<<<<<<<
  *             if end - f < 5:
  *                 raise RuntimeError(u"Format string allocated too short.")
  */
       __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_child->type_num); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 878, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_XDECREF_SET(__pyx_v_t, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":879
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":879
  *         if not PyDataType_HASFIELDS(child):
  *             t = child.type_num
  *             if end - f < 5:             # <<<<<<<<<<<<<<
  *                 raise RuntimeError(u"Format string allocated too short.")
  * 
  */
       __pyx_t_6 = (((__pyx_v_end - __pyx_v_f) < 5) != 0);
       if (unlikely(__pyx_t_6)) {
 
-        /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":880
+        /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":880
  *             t = child.type_num
  *             if end - f < 5:
  *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
  * 
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  */
         __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__53, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 880, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_Raise(__pyx_t_4, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __PYX_ERR(2, 880, __pyx_L1_error)
 
-        /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":879
+        /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":879
  *         if not PyDataType_HASFIELDS(child):
  *             t = child.type_num
  *             if end - f < 5:             # <<<<<<<<<<<<<<
  *                 raise RuntimeError(u"Format string allocated too short.")
  * 
  */
       }
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":883
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":883
  * 
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  *             if   t == NPY_BYTE:        f[0] =  98 #"b"             # <<<<<<<<<<<<<<
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_BYTE); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 883, __pyx_L1_error)
@@ -20859,15 +20918,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 883, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 98;
         goto __pyx_L15;
       }
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":884
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":884
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  *             if   t == NPY_BYTE:        f[0] =  98 #"b"
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"             # <<<<<<<<<<<<<<
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UBYTE); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 884, __pyx_L1_error)
@@ -20877,15 +20936,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 884, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 66;
         goto __pyx_L15;
       }
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":885
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":885
  *             if   t == NPY_BYTE:        f[0] =  98 #"b"
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"             # <<<<<<<<<<<<<<
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_SHORT); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 885, __pyx_L1_error)
@@ -20895,15 +20954,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 885, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x68;
         goto __pyx_L15;
       }
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":886
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":886
  *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"             # <<<<<<<<<<<<<<
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_USHORT); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 886, __pyx_L1_error)
@@ -20913,15 +20972,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 886, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 72;
         goto __pyx_L15;
       }
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":887
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":887
  *             elif t == NPY_SHORT:       f[0] = 104 #"h"
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  *             elif t == NPY_INT:         f[0] = 105 #"i"             # <<<<<<<<<<<<<<
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_INT); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 887, __pyx_L1_error)
@@ -20931,15 +20990,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 887, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x69;
         goto __pyx_L15;
       }
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":888
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":888
  *             elif t == NPY_USHORT:      f[0] =  72 #"H"
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  *             elif t == NPY_UINT:        f[0] =  73 #"I"             # <<<<<<<<<<<<<<
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UINT); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 888, __pyx_L1_error)
@@ -20949,15 +21008,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 888, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 73;
         goto __pyx_L15;
       }
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":889
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":889
  *             elif t == NPY_INT:         f[0] = 105 #"i"
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  *             elif t == NPY_LONG:        f[0] = 108 #"l"             # <<<<<<<<<<<<<<
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 889, __pyx_L1_error)
@@ -20967,15 +21026,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 889, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x6C;
         goto __pyx_L15;
       }
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":890
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":890
  *             elif t == NPY_UINT:        f[0] =  73 #"I"
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"             # <<<<<<<<<<<<<<
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 890, __pyx_L1_error)
@@ -20985,15 +21044,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 890, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 76;
         goto __pyx_L15;
       }
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":891
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":891
  *             elif t == NPY_LONG:        f[0] = 108 #"l"
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"             # <<<<<<<<<<<<<<
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGLONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 891, __pyx_L1_error)
@@ -21003,15 +21062,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 891, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x71;
         goto __pyx_L15;
       }
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":892
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":892
  *             elif t == NPY_ULONG:       f[0] = 76  #"L"
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"             # <<<<<<<<<<<<<<
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONGLONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 892, __pyx_L1_error)
@@ -21021,15 +21080,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 892, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 81;
         goto __pyx_L15;
       }
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":893
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":893
  *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"             # <<<<<<<<<<<<<<
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_FLOAT); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 893, __pyx_L1_error)
@@ -21039,15 +21098,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 893, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x66;
         goto __pyx_L15;
       }
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":894
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":894
  *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"             # <<<<<<<<<<<<<<
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_DOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 894, __pyx_L1_error)
@@ -21057,15 +21116,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 894, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x64;
         goto __pyx_L15;
       }
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":895
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":895
  *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"             # <<<<<<<<<<<<<<
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 895, __pyx_L1_error)
@@ -21075,15 +21134,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 895, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 0x67;
         goto __pyx_L15;
       }
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":896
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":896
  *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf             # <<<<<<<<<<<<<<
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CFLOAT); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 896, __pyx_L1_error)
@@ -21095,15 +21154,15 @@
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 90;
         (__pyx_v_f[1]) = 0x66;
         __pyx_v_f = (__pyx_v_f + 1);
         goto __pyx_L15;
       }
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":897
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":897
  *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd             # <<<<<<<<<<<<<<
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 897, __pyx_L1_error)
@@ -21115,15 +21174,15 @@
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 90;
         (__pyx_v_f[1]) = 0x64;
         __pyx_v_f = (__pyx_v_f + 1);
         goto __pyx_L15;
       }
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":898
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":898
  *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg             # <<<<<<<<<<<<<<
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
  *             else:
  */
       __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CLONGDOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 898, __pyx_L1_error)
@@ -21135,15 +21194,15 @@
       if (__pyx_t_6) {
         (__pyx_v_f[0]) = 90;
         (__pyx_v_f[1]) = 0x67;
         __pyx_v_f = (__pyx_v_f + 1);
         goto __pyx_L15;
       }
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":899
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":899
  *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
  *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"             # <<<<<<<<<<<<<<
  *             else:
  *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  */
       __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_OBJECT); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 899, __pyx_L1_error)
@@ -21153,15 +21212,15 @@
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 899, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (likely(__pyx_t_6)) {
         (__pyx_v_f[0]) = 79;
         goto __pyx_L15;
       }
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":901
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":901
  *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
  *             else:
  *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
  *             f += 1
  *         else:
  */
       /*else*/ {
@@ -21172,67 +21231,67 @@
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_Raise(__pyx_t_4, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __PYX_ERR(2, 901, __pyx_L1_error)
       }
       __pyx_L15:;
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":902
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":902
  *             else:
  *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
  *             f += 1             # <<<<<<<<<<<<<<
  *         else:
  *             # Cython ignores struct boundary information ("T{...}"),
  */
       __pyx_v_f = (__pyx_v_f + 1);
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":877
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":877
  *         offset[0] += child.itemsize
  * 
  *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
  *             t = child.type_num
  *             if end - f < 5:
  */
       goto __pyx_L13;
     }
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":906
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":906
  *             # Cython ignores struct boundary information ("T{...}"),
  *             # so don't output it
  *             f = _util_dtypestring(child, f, end, offset)             # <<<<<<<<<<<<<<
  *     return f
  * 
  */
     /*else*/ {
       __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_child, __pyx_v_f, __pyx_v_end, __pyx_v_offset); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(2, 906, __pyx_L1_error)
       __pyx_v_f = __pyx_t_9;
     }
     __pyx_L13:;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":851
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":851
  *     cdef tuple fields
  * 
  *     for childname in descr.names:             # <<<<<<<<<<<<<<
  *         fields = descr.fields[childname]
  *         child, new_offset = fields
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":907
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":907
  *             # so don't output it
  *             f = _util_dtypestring(child, f, end, offset)
  *     return f             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_f;
   goto __pyx_L0;
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":842
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":842
  *         return ()
  * 
  * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
  *     # Recursive utility function used in __getbuffer__ to get format
  *     # string. The new location in the format string is returned.
  */
 
@@ -21249,138 +21308,138 @@
   __Pyx_XDECREF(__pyx_v_childname);
   __Pyx_XDECREF(__pyx_v_new_offset);
   __Pyx_XDECREF(__pyx_v_t);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1022
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1022
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1023
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1023
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1024
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1024
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1022
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1022
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1026
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1026
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1027
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1027
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1028
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1028
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1029
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1029
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1028
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1028
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1030
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1030
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1026
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1026
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1034
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_array()
  */
 
@@ -21393,15 +21452,15 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1035
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1035
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_array()
  *     except Exception:
  */
   {
@@ -21409,53 +21468,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1036
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1036
  * cdef inline int import_array() except -1:
  *     try:
  *         _import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1036, __pyx_L3_error)
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1035
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1035
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1037
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1037
  *     try:
  *         _import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1037, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1038
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1038
  *         _import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__54, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1038, __pyx_L5_except_error)
@@ -21463,30 +21522,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 1038, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1035
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1035
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1034
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_array()
  */
 
@@ -21501,15 +21560,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1040
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -21522,15 +21581,15 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1041
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1041
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -21538,53 +21597,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1042
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1042
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1042, __pyx_L3_error)
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1041
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1041
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1043
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1043
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1043, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1044
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1044
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__55, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1044, __pyx_L5_except_error)
@@ -21592,30 +21651,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 1044, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1041
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1041
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1040
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -21630,15 +21689,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+/* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1046
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -21651,15 +21710,15 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1047
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1047
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -21667,81 +21726,81 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1048
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1048
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1048, __pyx_L3_error)
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1047
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1047
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1049
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1049
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1049, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1050
+      /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1050
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__55, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1050, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 1050, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1047
+    /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1047
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1046
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -37386,81 +37445,81 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.mso cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__48 = PyTuple_Pack(1, __pyx_kp_s_self_mso_cannot_be_converted_to); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__48);
   __Pyx_GIVEREF(__pyx_tuple__48);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":272
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":272
  *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
  * 
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  */
   __pyx_tuple__49 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_C_contiguous); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(2, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__49);
   __Pyx_GIVEREF(__pyx_tuple__49);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":276
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":276
  *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
  *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
  *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
  * 
  *             info.buf = PyArray_DATA(self)
  */
   __pyx_tuple__50 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_Fortran_contiguou); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(2, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__50);
   __Pyx_GIVEREF(__pyx_tuple__50);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":306
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":306
  *                 if ((descr.byteorder == c'>' and little_endian) or
  *                     (descr.byteorder == c'<' and not little_endian)):
  *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
  *                 if   t == NPY_BYTE:        f = "b"
  *                 elif t == NPY_UBYTE:       f = "B"
  */
   __pyx_tuple__51 = PyTuple_Pack(1, __pyx_kp_u_Non_native_byte_order_not_suppor); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(2, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__51);
   __Pyx_GIVEREF(__pyx_tuple__51);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":856
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":856
  * 
  *         if (end - f) - <int>(new_offset - offset[0]) < 15:
  *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
  * 
  *         if ((child.byteorder == c'>' and little_endian) or
  */
   __pyx_tuple__52 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(2, 856, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__52);
   __Pyx_GIVEREF(__pyx_tuple__52);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":880
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":880
  *             t = child.type_num
  *             if end - f < 5:
  *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
  * 
  *             # Until ticket #99 is fixed, use integers to avoid warnings
  */
   __pyx_tuple__53 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor_2); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(2, 880, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__53);
   __Pyx_GIVEREF(__pyx_tuple__53);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1038
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1038
  *         _import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__54 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(2, 1038, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__54);
   __Pyx_GIVEREF(__pyx_tuple__54);
 
-  /* "../../../.pyenv/versions/3.6.6/envs/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1044
+  /* "../../../.pyenv/versions/partseg/lib/python3.6/site-packages/Cython/Includes/numpy/__init__.pxd":1044
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__55 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(2, 1044, __pyx_L1_error)
@@ -37679,25 +37738,25 @@
  *                   image_types lower_mid_bound=0, image_types upper_mid_bound=0):
  */
   __pyx_tuple__76 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_image, __pyx_n_s_lower_bound, __pyx_n_s_upper_bound, __pyx_n_s_type, __pyx_n_s_mask, __pyx_n_s_lower_mid_bound, __pyx_n_s_upper_mid_bound, __pyx_n_s_mu); if (unlikely(!__pyx_tuple__76)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__76);
   __Pyx_GIVEREF(__pyx_tuple__76);
   __pyx_codeobj__77 = (PyObject*)__Pyx_PyCode_New(8, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__76, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_package_PartSeg_utils_multiscale, __pyx_n_s_set_image, 133, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__77)) __PYX_ERR(0, 133, __pyx_L1_error)
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":235
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":238
  * 
  * @cython.boundscheck(False)
  * def calculate_mu_mid(numpy.ndarray[image_types, ndim=3] image, image_types lower_bound, image_types mid_point,             # <<<<<<<<<<<<<<
  *                  image_types upper_bound):
  *     cdef int16_t x_size, y_size, z_size, x, y, z
  */
-  __pyx_tuple__78 = PyTuple_Pack(14, __pyx_n_s_image, __pyx_n_s_lower_bound, __pyx_n_s_mid_point, __pyx_n_s_upper_bound, __pyx_n_s_x_size, __pyx_n_s_y_size, __pyx_n_s_z_size, __pyx_n_s_x, __pyx_n_s_y, __pyx_n_s_z, __pyx_n_s_res_val, __pyx_n_s_point_val, __pyx_n_s_res, __pyx_n_s_tmp); if (unlikely(!__pyx_tuple__78)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_tuple__78 = PyTuple_Pack(14, __pyx_n_s_image, __pyx_n_s_lower_bound, __pyx_n_s_mid_point, __pyx_n_s_upper_bound, __pyx_n_s_x_size, __pyx_n_s_y_size, __pyx_n_s_z_size, __pyx_n_s_x, __pyx_n_s_y, __pyx_n_s_z, __pyx_n_s_res_val, __pyx_n_s_point_val, __pyx_n_s_res, __pyx_n_s_tmp); if (unlikely(!__pyx_tuple__78)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__78);
   __Pyx_GIVEREF(__pyx_tuple__78);
-  __pyx_codeobj__79 = (PyObject*)__Pyx_PyCode_New(4, 0, 14, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__78, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_package_PartSeg_utils_multiscale, __pyx_n_s_calculate_mu_mid, 235, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__79)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_codeobj__79 = (PyObject*)__Pyx_PyCode_New(4, 0, 14, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__78, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_package_PartSeg_utils_multiscale, __pyx_n_s_calculate_mu_mid, 238, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__79)) __PYX_ERR(0, 238, __pyx_L1_error)
 
   /* "EnumBase":28
  * class __Pyx_EnumBase(int):
  *     __metaclass__ = __Pyx_EnumMeta
  *     def __new__(cls, value, name=None):             # <<<<<<<<<<<<<<
  *         for v in cls:
  *             if v == value:
@@ -38516,64 +38575,64 @@
   ((__pyx_FusedFunctionObject *) __pyx_t_4)->__signatures__ = __pyx_t_5;
   __Pyx_GIVEREF(__pyx_t_5);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO->tp_dict, __pyx_n_s_set_image, __pyx_t_4) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
   PyType_Modified(__pyx_ptype_7PartSeg_5utils_18multiscale_opening_8mso_bind_PyMSO);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":235
+  /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":238
  * 
  * @cython.boundscheck(False)
  * def calculate_mu_mid(numpy.ndarray[image_types, ndim=3] image, image_types lower_bound, image_types mid_point,             # <<<<<<<<<<<<<<
  *                  image_types upper_bound):
  *     cdef int16_t x_size, y_size, z_size, x, y, z
  */
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __pyx_FusedFunction_NewEx(&__pyx_fuse_0__pyx_mdef_7PartSeg_5utils_18multiscale_opening_8mso_bind_21calculate_mu_mid, 0, __pyx_n_s_calculate_mu_mid, NULL, __pyx_n_s_PartSeg_utils_multiscale_opening, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_8 = __pyx_FusedFunction_NewEx(&__pyx_fuse_0__pyx_mdef_7PartSeg_5utils_18multiscale_opening_8mso_bind_21calculate_mu_mid, 0, __pyx_n_s_calculate_mu_mid, NULL, __pyx_n_s_PartSeg_utils_multiscale_opening, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_8, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_int8_t, __pyx_t_8) < 0) __PYX_ERR(0, 235, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_int8_t, __pyx_t_8) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __pyx_FusedFunction_NewEx(&__pyx_fuse_1__pyx_mdef_7PartSeg_5utils_18multiscale_opening_8mso_bind_23calculate_mu_mid, 0, __pyx_n_s_calculate_mu_mid, NULL, __pyx_n_s_PartSeg_utils_multiscale_opening, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_8 = __pyx_FusedFunction_NewEx(&__pyx_fuse_1__pyx_mdef_7PartSeg_5utils_18multiscale_opening_8mso_bind_23calculate_mu_mid, 0, __pyx_n_s_calculate_mu_mid, NULL, __pyx_n_s_PartSeg_utils_multiscale_opening, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_8, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_int16_t, __pyx_t_8) < 0) __PYX_ERR(0, 235, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_int16_t, __pyx_t_8) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __pyx_FusedFunction_NewEx(&__pyx_fuse_2__pyx_mdef_7PartSeg_5utils_18multiscale_opening_8mso_bind_25calculate_mu_mid, 0, __pyx_n_s_calculate_mu_mid, NULL, __pyx_n_s_PartSeg_utils_multiscale_opening, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_8 = __pyx_FusedFunction_NewEx(&__pyx_fuse_2__pyx_mdef_7PartSeg_5utils_18multiscale_opening_8mso_bind_25calculate_mu_mid, 0, __pyx_n_s_calculate_mu_mid, NULL, __pyx_n_s_PartSeg_utils_multiscale_opening, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_8, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_uint8_t, __pyx_t_8) < 0) __PYX_ERR(0, 235, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_uint8_t, __pyx_t_8) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __pyx_FusedFunction_NewEx(&__pyx_fuse_3__pyx_mdef_7PartSeg_5utils_18multiscale_opening_8mso_bind_27calculate_mu_mid, 0, __pyx_n_s_calculate_mu_mid, NULL, __pyx_n_s_PartSeg_utils_multiscale_opening, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_8 = __pyx_FusedFunction_NewEx(&__pyx_fuse_3__pyx_mdef_7PartSeg_5utils_18multiscale_opening_8mso_bind_27calculate_mu_mid, 0, __pyx_n_s_calculate_mu_mid, NULL, __pyx_n_s_PartSeg_utils_multiscale_opening, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_8, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_uint16_t, __pyx_t_8) < 0) __PYX_ERR(0, 235, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_uint16_t, __pyx_t_8) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __pyx_FusedFunction_NewEx(&__pyx_fuse_4__pyx_mdef_7PartSeg_5utils_18multiscale_opening_8mso_bind_29calculate_mu_mid, 0, __pyx_n_s_calculate_mu_mid, NULL, __pyx_n_s_PartSeg_utils_multiscale_opening, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_8 = __pyx_FusedFunction_NewEx(&__pyx_fuse_4__pyx_mdef_7PartSeg_5utils_18multiscale_opening_8mso_bind_29calculate_mu_mid, 0, __pyx_n_s_calculate_mu_mid, NULL, __pyx_n_s_PartSeg_utils_multiscale_opening, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_8, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_uint32_t, __pyx_t_8) < 0) __PYX_ERR(0, 235, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_uint32_t, __pyx_t_8) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __pyx_FusedFunction_NewEx(&__pyx_fuse_5__pyx_mdef_7PartSeg_5utils_18multiscale_opening_8mso_bind_31calculate_mu_mid, 0, __pyx_n_s_calculate_mu_mid, NULL, __pyx_n_s_PartSeg_utils_multiscale_opening, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_8 = __pyx_FusedFunction_NewEx(&__pyx_fuse_5__pyx_mdef_7PartSeg_5utils_18multiscale_opening_8mso_bind_31calculate_mu_mid, 0, __pyx_n_s_calculate_mu_mid, NULL, __pyx_n_s_PartSeg_utils_multiscale_opening, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_8, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_float32_t, __pyx_t_8) < 0) __PYX_ERR(0, 235, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_float32_t, __pyx_t_8) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __pyx_FusedFunction_NewEx(&__pyx_fuse_6__pyx_mdef_7PartSeg_5utils_18multiscale_opening_8mso_bind_33calculate_mu_mid, 0, __pyx_n_s_calculate_mu_mid, NULL, __pyx_n_s_PartSeg_utils_multiscale_opening, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_8 = __pyx_FusedFunction_NewEx(&__pyx_fuse_6__pyx_mdef_7PartSeg_5utils_18multiscale_opening_8mso_bind_33calculate_mu_mid, 0, __pyx_n_s_calculate_mu_mid, NULL, __pyx_n_s_PartSeg_utils_multiscale_opening, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_8, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_float64_t, __pyx_t_8) < 0) __PYX_ERR(0, 235, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_float64_t, __pyx_t_8) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __pyx_FusedFunction_NewEx(&__pyx_mdef_7PartSeg_5utils_18multiscale_opening_8mso_bind_3calculate_mu_mid, 0, __pyx_n_s_calculate_mu_mid, NULL, __pyx_n_s_PartSeg_utils_multiscale_opening, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_8 = __pyx_FusedFunction_NewEx(&__pyx_mdef_7PartSeg_5utils_18multiscale_opening_8mso_bind_3calculate_mu_mid, 0, __pyx_n_s_calculate_mu_mid, NULL, __pyx_n_s_PartSeg_utils_multiscale_opening, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_8, __pyx_empty_tuple);
   ((__pyx_FusedFunctionObject *) __pyx_t_8)->__signatures__ = __pyx_t_7;
   __Pyx_GIVEREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_calculate_mu_mid, __pyx_t_8) < 0) __PYX_ERR(0, 235, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_calculate_mu_mid, __pyx_t_8) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
   /* "PartSeg/utils/multiscale_opening/mso_bind.pyx":1
  * # distutils: language = c++             # <<<<<<<<<<<<<<
  * # cython: language_level=3
  * 
  */
```

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/multiscale_opening/mso_bind.pyx` & `PartSeg-0.9b2/package/PartSeg/utils/multiscale_opening/mso_bind.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,16 @@
         void set_neighbourhood(int8_t * neighbourhood, M * distances, size_t neigh_size) except +
         void set_components_num(T components_num)
         void compute_FDT(vector[M] & array) except +
         void set_use_background(bool val)
         size_t optimum_erosion_calculate(vector[M] &fdt_array, vector[T] &components_arr, vector[bool] & sprawl_area) except +
         size_t constrained_dilation(vector[M] &fdt_array, vector[T] &components_arr, vector[bool] & sprawl_area) except +
         size_t get_length()
-        size_t run_MSO() except +
-        size_t run_MSO(size_t steps_limits) except +
+        size_t run_MSO() nogil except +
+        size_t run_MSO(size_t steps_limits) nogil except +
         void set_data[W](T * components, W size, T background_component)
         void set_data[W](T * components, W size)
         size_t steps_done()
         vector[mu_type] get_fdt()
         vector[T] get_result_catted()
 
     cdef cppclass MuCalc[R, T]:
@@ -202,16 +202,19 @@
         self.mso.set_components_num(components_arr.max())
 
         count = self.mso.constrained_dilation(fdt, components, sprawl_vec)
         res = numpy.array(components, dtype=np_component_type)
         res = res.reshape([components_arr.shape[i] for i in range(components_arr.ndim)])
         return res
 
-    def run_MSO(self, step_limits=1):
-        return self.mso.run_MSO(step_limits)
+    def run_MSO(self, size_t step_limits=1):
+        cdef size_t val
+        with nogil:
+            val = self.mso.run_MSO(step_limits)
+        return val
 
     def steps_done(self):
         return self.mso.steps_done()
 
     def set_components_num(self, num):
         self.mso.set_components_num(num+2)
```

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/calculate_pipeline.py` & `PartSeg-0.9b2/package/PartSeg/utils/calculate_pipeline.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/json_hooks.py` & `PartSeg-0.9b2/package/PartSeg/utils/json_hooks.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/czifile.py` & `PartSeg-0.9b2/package/PartSeg/utils/czifile.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/global_settings.py` & `PartSeg-0.9b2/package/PartSeg/utils/global_settings.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/mask_create.py` & `PartSeg-0.9b2/package/PartSeg/utils/mask_create.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/convex_fill.py` & `PartSeg-0.9b2/package/PartSeg/utils/convex_fill.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/autofit.py` & `PartSeg-0.9b2/package/PartSeg/utils/autofit.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/put_borders_in_queue.pyx` & `PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/put_borders_in_queue.pyx`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/find_split.py` & `PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/find_split.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/fuzzy_distance.pyx` & `PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/fuzzy_distance.pyx`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/distance_utils.pxd` & `PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/distance_utils.pxd`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/euclidean_cython.cpp` & `PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/euclidean_cython.cpp`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/path_sprawl_cython.cpp` & `PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/path_sprawl_cython.cpp`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/sprawl_utils.cpp` & `PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/sprawl_utils.cpp`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/path_sprawl_cython.pyx` & `PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/path_sprawl_cython.pyx`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/sprawl_utils.pyx` & `PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/sprawl_utils.pyx`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/fuzzy_distance.cpp` & `PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/fuzzy_distance.cpp`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/distance_in_structure/euclidean_cython.pyx` & `PartSeg-0.9b2/package/PartSeg/utils/distance_in_structure/euclidean_cython.pyx`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/mask/io_functions.py` & `PartSeg-0.9b2/package/PartSeg/utils/mask/io_functions.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/color_image/color_image_base.py` & `PartSeg-0.9b2/package/PartSeg/utils/color_image/color_image_base.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/color_image/color_image.pyx` & `PartSeg-0.9b2/package/PartSeg/utils/color_image/color_image.pyx`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/color_image/color_image.cpp` & `PartSeg-0.9b2/package/PartSeg/utils/color_image/color_image.cpp`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/class_generator.py` & `PartSeg-0.9b2/package/PartSeg/utils/class_generator.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/utils.py` & `PartSeg-0.9b2/package/PartSeg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/image_operations.py` & `PartSeg-0.9b2/package/PartSeg/utils/image_operations.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/io_utils.py` & `PartSeg-0.9b2/package/PartSeg/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/border_rim.py` & `PartSeg-0.9b2/package/PartSeg/utils/border_rim.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/interpolation/bilinear_interpolation.pyx` & `PartSeg-0.9b2/package/PartSeg/utils/interpolation/bilinear_interpolation.pyx`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/utils/custom_colormaps.py` & `PartSeg-0.9b2/package/PartSeg/utils/custom_colormaps.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/extract_images.py` & `PartSeg-0.9b2/package/PartSeg/extract_images.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/convert_to_cmap.py` & `PartSeg-0.9b2/package/PartSeg/convert_to_cmap.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/batch_testing.py` & `PartSeg-0.9b2/package/PartSeg/batch_testing.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/launcher_main.py` & `PartSeg-0.9b2/package/PartSeg/launcher_main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import argparse
 import sys
 import logging
+from functools import partial
 
+from PartSeg.tiff_image import ImageReader
 from .custom_application import CustomApplication
-from .utils.base_argparser import CustomParser
+from PartSeg.project_utils_qt.base_argparser import CustomParser
 import multiprocessing
 
 multiprocessing.freeze_support()
 
 
 def main():
     parser = CustomParser("PartSeg")
@@ -15,30 +17,39 @@
                         help=argparse.SUPPRESS)  # Windows bug fix
     sp = parser.add_subparsers()
     sp_a = sp.add_parser("segmentation_analysis", help="Starts GUI for segmentation analysis")
     sp_s = sp.add_parser("segmentation", help="Starts GUI for segmentation")
     parser.set_defaults(gui="launcher")
     sp_a.set_defaults(gui="segmentation_analysis")
     sp_s.set_defaults(gui="segmentation")
+    sp_a.add_argument("image", nargs="?", help="image to read on begin", default="")
+    sp_a.add_argument("mask", nargs="?", help="mask to read on begin", default=None)
+    sp_s.add_argument("image", nargs="?", help="image to read on begin", default="")
     argv = [x for x in sys.argv[1:] if not (x.startswith("parent") or x.startswith("pipe"))]
     args = parser.parse_args(argv)
     # print(args)
 
     logging.basicConfig(level=logging.INFO)
     my_app = CustomApplication(sys.argv)
     if args.gui == "segmentation_analysis" or args.mf:
         from . import plugins
         plugins.register()
         from .segmentation_analysis.main_window import MainWindow
         title = "PartSeg Segmentation Analysis"
+        if args.image:
+            image = ImageReader.read_image(args.image, args.mask)
+            MainWindow = partial(MainWindow, initial_image=image)
     elif args.gui == "segmentation":
         from . import plugins
         plugins.register()
         from .segmentation_mask.stack_gui_main import MainWindow
         title = "PartSeg Mask Segmentation"
+        if args.image:
+            image = ImageReader.read_image(args.image)
+            MainWindow = partial(MainWindow, initial_image=image)
     else:
         from .launcher.main_window import MainWindow
         title = "PartSeg Launcher"
     wind = MainWindow(title=title)
     wind.show()
     my_app.exec_()
     del wind
```

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/colors.npz` & `PartSeg-0.9b2/package/PartSeg/static_files/colors.npz`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/icons/transform-move.png` & `PartSeg-0.9b2/package/PartSeg/static_files/icons/transform-move.png`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/icons/icon.png` & `PartSeg-0.9b2/package/PartSeg/static_files/icons/icon.png`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/icons/icon.icns` & `PartSeg-0.9b2/package/PartSeg/static_files/icons/icon.icns`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/icons/icon_stack.png` & `PartSeg-0.9b2/package/PartSeg/static_files/icons/icon_stack.png`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/icons/image-zoom-in.png` & `PartSeg-0.9b2/package/PartSeg/static_files/icons/image-zoom-in.png`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/icons/zoom-original.png` & `PartSeg-0.9b2/package/PartSeg/static_files/icons/zoom-original.png`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/icons/task-attempt.png` & `PartSeg-0.9b2/package/PartSeg/static_files/icons/task-attempt.png`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/icons/draw-eraser.png` & `PartSeg-0.9b2/package/PartSeg/static_files/icons/draw-eraser.png`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/icons/draw-path.png` & `PartSeg-0.9b2/package/PartSeg/static_files/icons/draw-path.png`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/icons/transform-scale.png` & `PartSeg-0.9b2/package/PartSeg/static_files/icons/transform-scale.png`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/icons/icon.ico` & `PartSeg-0.9b2/package/PartSeg/static_files/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/icons/configure.png` & `PartSeg-0.9b2/package/PartSeg/static_files/icons/configure.png`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/icons/document-save-as.png` & `PartSeg-0.9b2/package/PartSeg/static_files/icons/document-save-as.png`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/icons/task-reject.png` & `PartSeg-0.9b2/package/PartSeg/static_files/icons/task-reject.png`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/icons/document-open.png` & `PartSeg-0.9b2/package/PartSeg/static_files/icons/document-open.png`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/icons/task-accepted.png` & `PartSeg-0.9b2/package/PartSeg/static_files/icons/task-accepted.png`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/icons/zoom-select.png` & `PartSeg-0.9b2/package/PartSeg/static_files/icons/zoom-select.png`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/initial_images/clean_segment.tiff` & `PartSeg-0.9b2/package/PartSeg/static_files/initial_images/clean_segment.tiff`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/static_files/initial_images/stack.tif` & `PartSeg-0.9b2/package/PartSeg/static_files/initial_images/stack.tif`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/project_utils_qt/main_window.py` & `PartSeg-0.9b2/package/PartSeg/project_utils_qt/main_window.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/project_utils_qt/execute_function_thread.py` & `PartSeg-0.9b2/package/PartSeg/project_utils_qt/execute_function_thread.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/project_utils_qt/image_read_thread.py` & `PartSeg-0.9b2/package/PartSeg/project_utils_qt/image_read_thread.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/project_utils_qt/error_dialog.py` & `PartSeg-0.9b2/package/PartSeg/project_utils_qt/error_dialog.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import sys
 
 from qtpy.QtWidgets import QDialog, QPushButton, QTextEdit, QHBoxLayout, QVBoxLayout, QLabel, QLineEdit
 import traceback
-from ..utils import report_utils
+from ..utils import state_store
 import sentry_sdk
 
 from PartSeg import __version__
 
 
 class ErrorDialog(QDialog):
     def __init__(self, exception: Exception, description: str, additional_notes: str = "", traceback_summary=None):
         super().__init__()
         self.exception = exception
         self.additional_notes = additional_notes
         self.send_report_btn = QPushButton("Send information")
-        self.send_report_btn.setDisabled(not report_utils.report_errors)
+        self.send_report_btn.setDisabled(not state_store.report_errors)
         self.cancel_btn = QPushButton("Cancel")
         self.error_description = QTextEdit()
         if traceback_summary is None:
             self.error_description.setText("".join(
                 traceback.format_exception(type(exception), exception, exception.__traceback__)))
         elif isinstance(traceback_summary, traceback.StackSummary):
             self.error_description.setText("".join(traceback_summary.format()))
@@ -35,26 +35,26 @@
         self.desc.setWordWrap(True)
         layout.addWidget(self.desc)
         layout.addWidget(self.error_description)
         layout.addWidget(QLabel("Contact information"))
         layout.addWidget(self.contact_info)
         layout.addWidget(QLabel("Additional information from user:"))
         layout.addWidget(self.additional_info)
-        if not report_utils.report_errors:
+        if not state_store.report_errors:
             layout.addWidget(QLabel("Sending reports was disabled by runtime flag. "
                                     "You can report it manually by creating report on"
                                     "https://github.com/4DNucleome/PartSeg/issues"))
         btn_layout = QHBoxLayout()
         btn_layout.addWidget(self.cancel_btn)
         btn_layout.addWidget(self.send_report_btn)
         layout.addLayout(btn_layout)
         self.setLayout(layout)
 
     def exec(self):
-        if not report_utils.show_error_dialog:
+        if not state_store.show_error_dialog:
             sys.__excepthook__(type(self.exception), self.exception, self.exception.__traceback__)
             return False
         super().exec()
 
     def send_information(self):
         text = self.desc.text() + "\n\nVersion: " + __version__ + "\n"
         if len(self.additional_notes) > 0:
```

### Comparing `PartSeg-0.9b1/package/PartSeg/project_utils_qt/segmentation_thread.py` & `PartSeg-0.9b2/package/PartSeg/project_utils_qt/segmentation_thread.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/project_utils_qt/load_backup.py` & `PartSeg-0.9b2/package/PartSeg/project_utils_qt/load_backup.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/project_utils_qt/settings.py` & `PartSeg-0.9b2/package/PartSeg/project_utils_qt/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,14 +172,15 @@
     file_name: str
     values: typing.Union[dict, ProfileDict]
 
 
 class BaseSettings(ViewSettings):
     json_encoder_class = ProfileEncoder
     decode_hook = staticmethod(profile_hook)
+    algorithm_changed = Signal()
 
     def get_save_list(self) -> typing.List[SaveSettingsDescription]:
         return [SaveSettingsDescription("segmentation_settings.json", self.segmentation_dict),
                 SaveSettingsDescription("view_settings.json", self.view_settings_dict)]
 
     def __init__(self, json_path):
         super().__init__()
```

### Comparing `PartSeg-0.9b1/package/PartSeg/project_utils_qt/list_item_widget_for_exception.py` & `PartSeg-0.9b2/package/PartSeg/project_utils_qt/list_item_widget_for_exception.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/testy.py` & `PartSeg-0.9b2/package/PartSeg/testy.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/partseg_old/main_window.py` & `PartSeg-0.9b2/package/PartSeg/partseg_old/main_window.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/partseg_old/statistics_calculation.py` & `PartSeg-0.9b2/package/PartSeg/partseg_old/statistics_calculation.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/partseg_old/backend.py` & `PartSeg-0.9b2/package/PartSeg/partseg_old/backend.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/partseg_old/advanced_window.py` & `PartSeg-0.9b2/package/PartSeg/partseg_old/advanced_window.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/partseg_old/batch_window.py` & `PartSeg-0.9b2/package/PartSeg/partseg_old/batch_window.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/partseg_old/image_view.py` & `PartSeg-0.9b2/package/PartSeg/partseg_old/image_view.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/partseg_old/qt_import.py` & `PartSeg-0.9b2/package/PartSeg/partseg_old/qt_import.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/partseg_old/interpolate_dialog.py` & `PartSeg-0.9b2/package/PartSeg/partseg_old/interpolate_dialog.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/partseg_old/profile_export.py` & `PartSeg-0.9b2/package/PartSeg/partseg_old/profile_export.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/partseg_old/segment.py` & `PartSeg-0.9b2/package/PartSeg/partseg_old/segment.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/partseg_old/prepare_plan_widget.py` & `PartSeg-0.9b2/package/PartSeg/partseg_old/prepare_plan_widget.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/partseg_old/io_functions.py` & `PartSeg-0.9b2/package/PartSeg/partseg_old/io_functions.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/partseg_old/batch_processing/parallel_backed.py` & `PartSeg-0.9b2/package/PartSeg/partseg_old/batch_processing/parallel_backed.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/partseg_old/batch_processing/batch_backend.py` & `PartSeg-0.9b2/package/PartSeg/partseg_old/batch_processing/batch_backend.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/partseg_old/batch_processing/calculation_plan.py` & `PartSeg-0.9b2/package/PartSeg/partseg_old/batch_processing/calculation_plan.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/partseg_old/gui.py` & `PartSeg-0.9b2/package/PartSeg/partseg_old/gui.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/tiff_image/image_writer.py` & `PartSeg-0.9b2/package/PartSeg/tiff_image/image_writer.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/tiff_image/image_reader.py` & `PartSeg-0.9b2/package/PartSeg/tiff_image/image_reader.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/tiff_image/image.py` & `PartSeg-0.9b2/package/PartSeg/tiff_image/image.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/segmentation_analysis/main_window.py` & `PartSeg-0.9b2/package/PartSeg/segmentation_analysis/main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 from pathlib import Path
 
 import numpy as np
 from qtpy.QtCore import Qt, QByteArray, QEvent
 from qtpy.QtGui import QIcon, QKeyEvent, QKeySequence, QResizeEvent
 from qtpy.QtWidgets import QLabel, QWidget, QPushButton, QHBoxLayout, QVBoxLayout, QGridLayout, \
     QMessageBox, QCheckBox, QComboBox, QInputDialog, QDialog
@@ -398,15 +399,16 @@
             if self._settings.mask is not None:
                 mask = self._settings.mask.astype(np.uint8)
                 mask[mask > 0] = 255
                 args.append(mask)
             interp_ob.set_arrays(args)
             interp_ob.set_scaling(scale_factor)
             if dial.exec():
-                image = Image(interp_ob.result[0], [x / y for x, y in zip(self._settings.image_spacing, scale_factor)],
+                # WARNING time !!!!!
+                image = Image(interp_ob.result[0], [x / y for x, y in zip(self._settings.image_spacing, scale_factor[1:])],
                               self._settings.image.file_path,
                               None if len(interp_ob.result) == 1 else interp_ob.result[2],
                               self._settings.image.default_coloring, self._settings.image.ranges,
                               self._settings.image.labels)
                 # print(interp_ob.result[0].shape)
                 self._settings.image = image
             else:
@@ -423,19 +425,23 @@
 
     def load_data(self):
         def exception_hook(exception):
             from qtpy.QtWidgets import QApplication
             from qtpy.QtCore import QMetaObject
             instance = QApplication.instance()
             if isinstance(exception, MemoryError):
-                instance.warning = "Open error", "Not enough memory to read this image"
+                instance.warning = "Open error", f"Not enough memory to read this image: {exception}"
                 QMetaObject.invokeMethod(instance, "show_warning", Qt.QueuedConnection)
             elif isinstance(exception, IOError):
-                instance.warning = "Open error", "Some problem with reading from disc"
+                instance.warning = "Open error", f"Some problem with reading from disc: {exception}"
                 QMetaObject.invokeMethod(instance, "show_warning", Qt.QueuedConnection)
+            elif isinstance(exception, KeyError):
+                instance.warning = "Open error", f"Some problem project file: {exception}"
+                QMetaObject.invokeMethod(instance, "show_warning", Qt.QueuedConnection)
+                print(exception, file=sys.stderr)
             else:
                 raise exception
 
         try:
             dial = CustomLoadDialog(load_dict)
             dial.setDirectory(self._settings.get("io.open_directory", str(Path.home())))
             dial.selectNameFilter(self._settings.get("io.open_filter", next(iter(load_dict.keys()))))
```

### Comparing `PartSeg-0.9b1/package/PartSeg/segmentation_analysis/advanced_window.py` & `PartSeg-0.9b2/package/PartSeg/segmentation_analysis/advanced_window.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/segmentation_analysis/batch_window.py` & `PartSeg-0.9b2/package/PartSeg/segmentation_analysis/batch_window.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/segmentation_analysis/image_view.py` & `PartSeg-0.9b2/package/PartSeg/segmentation_analysis/image_view.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/segmentation_analysis/interpolate_thread.py` & `PartSeg-0.9b2/package/PartSeg/segmentation_analysis/interpolate_thread.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     def set_arrays(self, arrays_list):
         self.arrays = arrays_list
 
     def run(self):
         self.result = []
         for el in self.arrays:
             if len(el.shape) == len(self.scaling):
-                self.result.append(zoom(el, self.scaling))
+                cache = zoom(el, self.scaling, mode="mirror")
+
             else:
                 shape = [round(x * y) for x, y in zip(self.scaling, el.shape)] + list(el.shape[len(self.scaling):])
                 cache = np.zeros(shape, dtype=el.dtype)
                 for i in range(el.shape[-1]):
-                    cache[..., i] = zoom(el[..., i], self.scaling)
-                self.result.append(cache)
+                    cache[..., i] = zoom(el[..., i], self.scaling, mode="mirror")
+            self.result.append(cache)
         return
```

### Comparing `PartSeg-0.9b1/package/PartSeg/segmentation_analysis/interpolate_dialog.py` & `PartSeg-0.9b2/package/PartSeg/segmentation_analysis/interpolate_dialog.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/segmentation_analysis/profile_export.py` & `PartSeg-0.9b2/package/PartSeg/segmentation_analysis/profile_export.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/segmentation_analysis/partseg_settings.py` & `PartSeg-0.9b2/package/PartSeg/segmentation_analysis/partseg_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
             self.image = data.image
             self.segmentation = data.segmentation
             self.full_segmentation = data.full_segmentation
             self.segmentation_history = data.history
             if data.algorithm_parameters:
                 self.last_executed_algorithm = data.algorithm_parameters["name"]
                 self.set(f"algorithms.{self.last_executed_algorithm}", data.algorithm_parameters["values"])
+                self.algorithm_changed.emit()
         if isinstance(data, MaskInfo):
             self.mask = data.mask_array
 
     def save_project(self, file_path):
         dkt = dict()
         dkt["segmentation"] = self.segmentation
         algorithm_name = self.last_executed_algorithm
```

### Comparing `PartSeg-0.9b1/package/PartSeg/segmentation_analysis/prepare_plan_widget.py` & `PartSeg-0.9b2/package/PartSeg/segmentation_analysis/prepare_plan_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     QListWidget, QSpinBox, QTextEdit, QVBoxLayout, QGroupBox, QLabel, QHBoxLayout, QInputDialog, QMessageBox, \
     QTreeWidget, QTreeWidgetItem, QFileDialog, QSplitter, QTabWidget, QListWidgetItem
 
 from PartSeg.common_gui.universal_gui_part import EnumComboBox
 from ..common_gui.custom_save_dialog import FormDialog
 from ..common_gui.mask_widget import MaskWidget
 from ..common_gui.universal_gui_part import right_label
-from PartSeg.utils.analysis.algorithm_description import SegmentationProfile
+from PartSeg.utils.analysis.algorithm_description import SegmentationProfile, analysis_algorithm_dict
 from PartSeg.utils.analysis.save_functions import save_dict
 from ..utils.io_utils import SaveBase
 from ..utils.segmentation.algorithm_describe_base import AlgorithmProperty
 from ..utils.universal_const import Units
 
 from PartSeg.utils.analysis.calculation_plan import CalculationPlan, MaskCreate, MaskUse, Operations, \
     MaskSuffix, MaskSub, MaskFile, PlanChanges, NodeType, ChooseChanel, MaskIntersection, MaskSum, \
@@ -747,15 +747,15 @@
         if self.protect:
             return
         if text is None:
             if self.segment_profile.currentItem() is not None:
                 text = str(self.segment_profile.currentItem().text())
             else:
                 return
-        self.information.setText(str(self.settings.segmentation_profiles[text]))
+        self.information.setText(self.settings.segmentation_profiles[text].pretty_print(analysis_algorithm_dict))
 
     def show_segment(self):
         if self.update_element_btn.isChecked():
             self.get_big_btn.setDisabled(True)
             if self.node_type == NodeType.segment:
                 self.chose_profile_btn.setEnabled(True)
             else:
@@ -842,15 +842,19 @@
         """
         widget = QTreeWidgetItem(up_widget)
         widget.setText(0, CalculationPlan.get_el_name(node_plan.operation))
         self.setCurrentItem(widget)
         if isinstance(node_plan.operation, (StatisticCalculate, SegmentationProfile, MaskCreate)):
             desc = QTreeWidgetItem(widget)
             desc.setText(0, "Description")
-            for line in str(node_plan.operation).split("\n")[1:]:
+            if isinstance(node_plan.operation, SegmentationProfile):
+                txt = node_plan.operation.pretty_print(analysis_algorithm_dict)
+            else:
+                txt = str(node_plan.operation)
+            for line in txt.split("\n")[1:]:
                 QTreeWidgetItem(desc, [line])
         if deep:
             for el in node_plan.children:
                 self.explore_tree(widget, el)
         up_widget.setExpanded(True)
 
     def get_node(self, path):
@@ -888,15 +892,19 @@
                 node.removeChild(node.child(index))
             elif op_type == PlanChanges.replace_node:
                 node = self.get_node(path)
                 node.setText(0, CalculationPlan.get_el_name(el.operation))
                 if isinstance(el.operation, (StatisticProfile, SegmentationProfile, MaskCreate)):
                     child = node.child(0)
                     child.takeChildren()
-                    for line in str(el.operation).split("\n")[1:]:
+                    if isinstance(el.operation, SegmentationProfile):
+                        txt = el.operation.pretty_print(analysis_algorithm_dict)
+                    else:
+                        txt = str(el.operation)
+                    for line in txt.split("\n")[1:]:
                         QTreeWidgetItem(child, [line])
 
             else:
                 logging.error("Unknown operation {}".format(op_type))
         self.blockSignals(False)
         self.set_path()
         self.changed_node.emit()
```

### Comparing `PartSeg-0.9b1/package/PartSeg/segmentation_analysis/statistic_widget.py` & `PartSeg-0.9b2/package/PartSeg/segmentation_analysis/statistic_widget.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/segmentation_analysis/calculation_pipeline_thread.py` & `PartSeg-0.9b2/package/PartSeg/segmentation_analysis/calculation_pipeline_thread.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/partseg2_main.py` & `PartSeg-0.9b2/package/PartSeg/partseg2_main.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/common_gui/colors_choose.py` & `PartSeg-0.9b2/package/PartSeg/common_gui/colors_choose.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/common_gui/vetical_scroll_area.py` & `PartSeg-0.9b2/package/PartSeg/common_gui/vetical_scroll_area.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/common_gui/flow_layout.py` & `PartSeg-0.9b2/package/PartSeg/common_gui/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/common_gui/waiting_dialog.py` & `PartSeg-0.9b2/package/PartSeg/common_gui/waiting_dialog.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/common_gui/mask_widget.py` & `PartSeg-0.9b2/package/PartSeg/common_gui/mask_widget.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/common_gui/channel_control.py` & `PartSeg-0.9b2/package/PartSeg/common_gui/channel_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     def hidePopup(self):
         super().hidePopup()
         self.hide_popup.emit()
 
 
 class ChannelChooseBase(QWidget):
     coloring_update = Signal(bool)  # gave info if it is new image
-    channel_change = Signal(int)
+    channel_change = Signal(int, bool) # TODO something better for remove error during load different z-sizes images
 
     def __init__(self, settings: ViewSettings, parent=None, name="channelcontrol", text=""):
         super().__init__(parent)
         self._settings = settings
         self._name = name
         self._main_name = name
         self.text = text
@@ -293,15 +293,15 @@
         self.gauss_radius.setValue(self._settings.get_from_profile(f"{self._name}.gauss_radius_{chanel_id}", 1))
 
         self.channels_widgets[chanel_id].set_active()
         self.fixed.setChecked(self.channels_widgets[chanel_id].locked)
         self.image = self.channels_widgets[chanel_id].image
         self.colormap_chose.setCurrentText(self.channels_widgets[chanel_id].color)
         self.channel_preview_widget.repaint()
-        self.channel_change.emit(chanel_id)
+        self.channel_change.emit(chanel_id, False)
 
     def change_closed(self):
         text = self.colormap_chose.currentText()
         self.change_color_preview(text)
 
     def change_color_preview(self, value):
         img = color_image(np.arange(0, 256).reshape((1, 256, 1)), [value], [(0, 256)])
@@ -346,15 +346,15 @@
         self.maximum_value.setValue(self._settings.get_from_profile(f"{self._name}.range_{index}", (0, 65000))[1])
         self.use_gauss.setChecked(self._settings.get_from_profile(f"{self._name}.use_gauss_{index}", False))
         self.gauss_radius.setValue(self._settings.get_from_profile(f"{self._name}.gauss_radius_{index}", 1))
         self.current_channel = 0
         self.image = self.channels_widgets[0].image
         self.colormap_chose.setCurrentText(self.channels_widgets[0].color)
         self.send_info(True)
-        self.channel_change.emit(self.current_channel)
+        self.channel_change.emit(self.current_channel, True)
 
     def get_current_colors(self):
         channels_num = len(self.channels_widgets)
         resp = []
         for i in range(channels_num):
             resp.append(self._settings.get_from_profile(f"{self._name}.cmap{i}", self.channels_widgets[i].color))
         return resp
@@ -411,23 +411,23 @@
         self.main_channel_control.channel_change.connect(self.color_change)
         self.main_channel_control.coloring_update.connect(self.coloring_update_resend)
         self._set_layout()
 
     def coloring_update_resend(self, val):
         self.coloring_update.emit(val)
 
-    def color_change(self, val):
+    def color_change(self, val, new=False):
         if val >= len(self.channels_widgets):
             return
         colormap = self._settings.get_from_profile(f"{self.main_channel_control.name}.cmap{val}")
         self.channels_widgets[val].set_color(colormap)
         value = self._settings.get_from_profile(f"{self.name}.lock_{val}")
         self.channels_widgets[val].set_locked(value)
-        self.send_info()
-        self.channel_change.emit(val)
+        self.send_info(new)
+        self.channel_change.emit(val, False)
 
     def get_limits(self):
         return self.main_channel_control.get_limits()
 
     def get_gauss(self):
         return self.main_channel_control.get_gauss()
 
@@ -462,24 +462,24 @@
             self.channels_widgets[-1].clicked.connect(self.change_chanel)
             self.channels_widgets[-1].chosen.stateChanged.connect(self.send_info_wrap)
         self.channels_widgets[0].set_active()
         self.image = self.channels_widgets[0].image
 
         self.current_channel = 0
         self.send_info(True)
-        self.channel_change.emit(self.current_channel)
+        self.channel_change.emit(self.current_channel, True)
 
     def change_chanel(self, chanel_id):
         if chanel_id == self.current_channel:
             return
         self.channels_widgets[self.current_channel].set_inactive()
         self.current_channel = chanel_id
         self.channels_widgets[chanel_id].set_active()
         self.image = self.channels_widgets[chanel_id].image
-        self.channel_change.emit(chanel_id)
+        self.channel_change.emit(chanel_id, False)
 
 
     def active_channel(self, index):
         return self.channels_widgets[index].chosen.isChecked()
 
     @property
     def name(self):
```

### Comparing `PartSeg-0.9b1/package/PartSeg/common_gui/custom_load_dialog.py` & `PartSeg-0.9b2/package/PartSeg/common_gui/custom_load_dialog.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/common_gui/select_multiple_files.py` & `PartSeg-0.9b2/package/PartSeg/common_gui/select_multiple_files.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/common_gui/custom_save_dialog.py` & `PartSeg-0.9b2/package/PartSeg/common_gui/custom_save_dialog.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/common_gui/save_dialog.py` & `PartSeg-0.9b2/package/PartSeg/common_gui/save_dialog.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/common_gui/show_directory_dialog.py` & `PartSeg-0.9b2/package/PartSeg/common_gui/show_directory_dialog.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/common_gui/collapse_checkbox.py` & `PartSeg-0.9b2/package/PartSeg/common_gui/collapse_checkbox.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/common_gui/about_dialog.py` & `PartSeg-0.9b2/package/PartSeg/common_gui/about_dialog.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/common_gui/algorithms_description.py` & `PartSeg-0.9b2/package/PartSeg/common_gui/algorithms_description.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,16 @@
 
     def set_values(self, val: dict):
         if not isinstance(val, dict):
             return
         self.choose.setCurrentText(val["name"])
         if val["name"] not in self.widgets_dict:
             self.algorithm_choose(val["name"])
-        self.widgets_dict[val["name"]].set_values(val["values"])
+        if val["name"] in self.widgets_dict:
+            self.widgets_dict[val["name"]].set_values(val["values"])
 
     def recursive_get_values(self):
         return dict(((name, el.recursive_get_values()) for name, el in self.widgets_dict.items()))
 
     def get_values(self):
         name = self.choose.currentText()
         values = self.widgets_dict[name].get_values()
@@ -280,17 +281,22 @@
         for i in range(self.layout().count()):
             el = self.layout().itemAt(i)
             if el.widget() and isinstance(el.widget(), FormWidget):
                 el.widget().image_changed(image)
 
     def algorithm_choose(self, name):
         if name not in self.widgets_dict:
+            if name not in self.property.possible_values:
+                return
             start_dict = {} if name not in self.starting_values else self.starting_values[name]
-            self.widgets_dict[name] = FormWidget(self.property.possible_values[name].get_fields(),
-                                                 start_values=start_dict)
+            try:
+                self.widgets_dict[name] = FormWidget(self.property.possible_values[name].get_fields(),
+                                                     start_values=start_dict)
+            except KeyError as e:
+                raise  e
             self.widgets_dict[name].layout().setContentsMargins(0, 0, 0, 0)
             self.layout().addWidget(self.widgets_dict[name])
             self.widgets_dict[name].value_changed.connect(self.values_changed)
         widget = self.widgets_dict[name]
         for i in range(self.layout().count()):
             lay_elem = self.layout().itemAt(i)
             if lay_elem.widget():
@@ -437,14 +443,15 @@
     value_changed = Signal()
     algorithm_changed = Signal(str)
 
     def __init__(self, settings: BaseSettings, algorithms: Dict[str, Type[SegmentationAlgorithm]],
                  parent=None):
         super().__init__(parent)
         self.settings = settings
+        settings.algorithm_changed.connect(self.updated_algorithm)
         self.stack_layout = QStackedLayout()
         self.algorithm_choose = QComboBox()
         self.algorithm_dict: typing.Dict[str, BaseAlgorithmSettingsWidget] = {}
         widgets_list = []
         for name, val in algorithms.items():
             self.algorithm_choose.addItem(name)
             widget = InteractiveAlgorithmSettingsWidget(settings, name, val, [])
@@ -469,14 +476,18 @@
         self.setContentsMargins(0, 0, 0, 0)
         layout = QVBoxLayout()
         layout.setContentsMargins(0, 0, 0, 0)
         layout.addWidget(self.algorithm_choose)
         layout.addLayout(self.stack_layout)
         self.setLayout(layout)
 
+    def updated_algorithm(self):
+        self.change_algorithm(self.settings.last_executed_algorithm,
+                              self.settings.get(f"algorithms.{self.settings.last_executed_algorithm}"))
+
     def recursive_get_values(self):
         result = {}
         for key, widget in self.algorithm_dict.items():
             result[key] = widget.recursive_get_values()
         self.settings.set("algorithm_widget_state", update(self.settings.get("algorithm_widget_state", dict), result))
         return result
```

### Comparing `PartSeg-0.9b1/package/PartSeg/common_gui/lock_checkbox.py` & `PartSeg-0.9b2/package/PartSeg/common_gui/lock_checkbox.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/common_gui/universal_gui_part.py` & `PartSeg-0.9b2/package/PartSeg/common_gui/universal_gui_part.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/common_gui/stack_image_view.py` & `PartSeg-0.9b2/package/PartSeg/common_gui/stack_image_view.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg/partseg_main.py` & `PartSeg-0.9b2/package/PartSeg/partseg_main.py`

 * *Files identical despite different names*

### Comparing `PartSeg-0.9b1/package/PartSeg.egg-info/PKG-INFO` & `PartSeg-0.9b2/package/PartSeg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PartSeg
-Version: 0.9b1
+Version: 0.9b2
 Summary: PartSeg is python GUI for bio imaging analysis
 Home-page: https://4dnucleome.cent.uw.edu.pl/PartSeg/
 Author: Grzegorz Bokota
 Author-email: g.bokota@cent.uw.edu.pl
 License: UNKNOWN
 Description: # PartSeg
         [![Build Status](https://travis-ci.org/4DNucleome/PartSeg.svg?branch=master)](https://travis-ci.org/4DNucleome/PartSeg)
```

### Comparing `PartSeg-0.9b1/package/PartSeg.egg-info/SOURCES.txt` & `PartSeg-0.9b2/package/PartSeg.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,18 +58,23 @@
 package/PartSeg/partseg_old/statistics_calculation.py
 package/PartSeg/partseg_old/batch_processing/__init__.py
 package/PartSeg/partseg_old/batch_processing/batch_backend.py
 package/PartSeg/partseg_old/batch_processing/calculation_plan.py
 package/PartSeg/partseg_old/batch_processing/parallel_backed.py
 package/PartSeg/plugins/__init__.py
 package/PartSeg/plugins/itk_snap_save/__init__.py
+package/PartSeg/plugins/modeling_save/__init__.py
+package/PartSeg/plugins/modeling_save/save_modeling_data.py
 package/PartSeg/plugins/multiscale_segmentation/__init__.py
 package/PartSeg/plugins/multiscale_segmentation/multiscale_segmentation.py
+package/PartSeg/plugins/old_partseg/__init__.py
+package/PartSeg/plugins/old_partseg/old_partseg.py
 package/PartSeg/project_utils_qt/__init__.py
 package/PartSeg/project_utils_qt/abstract_class.py
+package/PartSeg/project_utils_qt/base_argparser.py
 package/PartSeg/project_utils_qt/error_dialog.py
 package/PartSeg/project_utils_qt/except_hook.py
 package/PartSeg/project_utils_qt/execute_function_thread.py
 package/PartSeg/project_utils_qt/image_read_thread.py
 package/PartSeg/project_utils_qt/list_item_widget_for_exception.py
 package/PartSeg/project_utils_qt/load_backup.py
 package/PartSeg/project_utils_qt/main_window.py
@@ -115,15 +120,14 @@
 package/PartSeg/static_files/initial_images/stack.tif
 package/PartSeg/tiff_image/__init__.py
 package/PartSeg/tiff_image/image.py
 package/PartSeg/tiff_image/image_reader.py
 package/PartSeg/tiff_image/image_writer.py
 package/PartSeg/utils/__init__.py
 package/PartSeg/utils/autofit.py
-package/PartSeg/utils/base_argparser.py
 package/PartSeg/utils/border_rim.py
 package/PartSeg/utils/calculate_pipeline.py
 package/PartSeg/utils/channel_class.py
 package/PartSeg/utils/class_generate_base.py
 package/PartSeg/utils/class_generator.py
 package/PartSeg/utils/cmap_utils.py
 package/PartSeg/utils/colors.py
@@ -132,15 +136,15 @@
 package/PartSeg/utils/czifile.py
 package/PartSeg/utils/global_settings.py
 package/PartSeg/utils/image_operations.py
 package/PartSeg/utils/io_utils.py
 package/PartSeg/utils/json_hooks.py
 package/PartSeg/utils/mask_create.py
 package/PartSeg/utils/register.py
-package/PartSeg/utils/report_utils.py
+package/PartSeg/utils/state_store.py
 package/PartSeg/utils/universal_const.py
 package/PartSeg/utils/utils.py
 package/PartSeg/utils/analysis/__init__.py
 package/PartSeg/utils/analysis/algorithm_description.py
 package/PartSeg/utils/analysis/analysis_utils.py
 package/PartSeg/utils/analysis/calculation_plan.py
 package/PartSeg/utils/analysis/io_utils.py
```

