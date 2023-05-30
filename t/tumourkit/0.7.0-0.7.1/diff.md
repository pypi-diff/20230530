# Comparing `tmp/tumourkit-0.7.0.tar.gz` & `tmp/tumourkit-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tumourkit-0.7.0.tar", last modified: Thu May 25 07:57:36 2023, max compression
+gzip compressed data, was "tumourkit-0.7.1.tar", last modified: Tue May 30 20:01:02 2023, max compression
```

## Comparing `tumourkit-0.7.0.tar` & `tumourkit-0.7.1.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.458661 tumourkit-0.7.0/
--rw-r--r--   0 joseperezcano   (501) staff       (20)    34523 2022-12-31 13:00:33.000000 tumourkit-0.7.0/LICENSE
--rw-r--r--   0 joseperezcano   (501) staff       (20)    42041 2023-05-25 07:57:36.458279 tumourkit-0.7.0/PKG-INFO
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1269 2023-03-25 17:22:23.000000 tumourkit-0.7.0/README.md
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.349341 tumourkit-0.7.0/docs/
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.349161 tumourkit-0.7.0/docs/buildenv/
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.364651 tumourkit-0.7.0/docs/buildenv/bin/
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      675 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2html.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      795 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2html4.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1163 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2html5.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      872 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2latex.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      680 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2man.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      845 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2odt.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1807 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      682 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      718 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2s5.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      952 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2xetex.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      683 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2xml.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      751 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rstpep2html.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.365470 tumourkit-0.7.0/docs/source/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1151 2023-04-11 15:21:40.000000 tumourkit-0.7.0/docs/source/conf.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2282 2023-05-25 06:24:46.000000 tumourkit-0.7.0/pyproject.toml
--rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-05-04 18:20:19.000000 tumourkit-0.7.0/requirements.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-05-25 07:57:36.458820 tumourkit-0.7.0/setup.cfg
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.383471 tumourkit-0.7.0/tests/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1596 2023-03-20 09:45:58.000000 tumourkit-0.7.0/tests/centroidspng2csv_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1871 2023-03-06 07:41:04.000000 tumourkit-0.7.0/tests/conf_matrix_sum_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2043 2023-03-06 07:25:02.000000 tumourkit-0.7.0/tests/cpairs_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)      805 2023-03-06 07:25:20.000000 tumourkit-0.7.0/tests/example_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3927 2022-12-31 13:06:14.000000 tumourkit-0.7.0/tests/generate_centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3403 2022-12-31 13:06:04.000000 tumourkit-0.7.0/tests/generate_rswoosh.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1517 2023-03-06 07:25:59.000000 tumourkit-0.7.0/tests/get_conn_comp_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1827 2023-03-28 15:20:41.000000 tumourkit-0.7.0/tests/graph2centroids_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1707 2023-03-20 10:39:44.000000 tumourkit-0.7.0/tests/graph_idx_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2199 2023-03-23 19:39:56.000000 tumourkit-0.7.0/tests/hov_prob_pipe_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2098 2023-03-06 07:27:57.000000 tumourkit-0.7.0/tests/hov_prob_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2503 2023-03-23 07:08:34.000000 tumourkit-0.7.0/tests/hovernet_patches_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1844 2023-03-06 07:41:02.000000 tumourkit-0.7.0/tests/metrics_pairs_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1974 2023-03-06 07:41:00.000000 tumourkit-0.7.0/tests/metrics_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1898 2023-03-20 10:58:10.000000 tumourkit-0.7.0/tests/png2graph_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2240 2023-03-06 07:30:23.000000 tumourkit-0.7.0/tests/pngcsv2geojson_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1829 2023-03-20 10:39:00.000000 tumourkit-0.7.0/tests/pngcsv2graph_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1978 2023-04-12 10:40:07.000000 tumourkit-0.7.0/tests/read_nodes_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1374 2023-03-06 07:31:03.000000 tumourkit-0.7.0/tests/remove_idx_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1577 2023-03-06 07:31:28.000000 tumourkit-0.7.0/tests/rswoosh_test.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.389875 tumourkit-0.7.0/tumourkit/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      154 2023-05-25 06:25:28.000000 tumourkit-0.7.0/tumourkit/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.398324 tumourkit-0.7.0/tumourkit/classification/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      155 2023-04-11 15:25:33.000000 tumourkit-0.7.0/tumourkit/classification/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1356 2023-05-18 07:19:54.000000 tumourkit-0.7.0/tumourkit/classification/compute_imbalance.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     6104 2023-05-18 07:21:56.000000 tumourkit-0.7.0/tumourkit/classification/evaluate.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5305 2023-05-18 07:22:57.000000 tumourkit-0.7.0/tumourkit/classification/infer.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.402069 tumourkit-0.7.0/tumourkit/classification/models/
--rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-11-28 08:50:03.000000 tumourkit-0.7.0/tumourkit/classification/models/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2532 2023-03-23 17:44:30.000000 tumourkit-0.7.0/tumourkit/classification/models/gat.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2008 2022-12-31 13:10:31.000000 tumourkit-0.7.0/tumourkit/classification/models/gcn.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7769 2022-12-31 13:10:48.000000 tumourkit-0.7.0/tumourkit/classification/models/hgao.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2840 2022-12-19 09:14:00.000000 tumourkit-0.7.0/tumourkit/classification/models/norm.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7575 2023-05-18 07:24:15.000000 tumourkit-0.7.0/tumourkit/classification/read_graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    20658 2023-05-18 07:28:33.000000 tumourkit-0.7.0/tumourkit/classification/train_graphs.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    10426 2023-05-18 07:32:33.000000 tumourkit-0.7.0/tumourkit/classification/train_xgboost.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.403464 tumourkit-0.7.0/tumourkit/demo/
--rw-r--r--   0 joseperezcano   (501) staff       (20)    12884 2023-05-18 07:16:15.000000 tumourkit-0.7.0/tumourkit/demo/app.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     6349 2023-05-18 07:55:33.000000 tumourkit-0.7.0/tumourkit/eval_pipe.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     8197 2023-05-18 07:55:46.000000 tumourkit-0.7.0/tumourkit/infer_pipe.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3924 2023-05-18 07:56:05.000000 tumourkit-0.7.0/tumourkit/make_dirs.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.408799 tumourkit-0.7.0/tumourkit/postprocessing/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      180 2023-05-03 07:48:49.000000 tumourkit-0.7.0/tumourkit/postprocessing/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2591 2023-05-25 07:56:12.000000 tumourkit-0.7.0/tumourkit/postprocessing/draw_cells.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5344 2023-05-25 07:55:08.000000 tumourkit-0.7.0/tumourkit/postprocessing/draw_graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3623 2023-05-18 07:05:34.000000 tumourkit-0.7.0/tumourkit/postprocessing/join_graph_gt.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5472 2023-05-18 07:06:54.000000 tumourkit-0.7.0/tumourkit/postprocessing/join_hovprob_graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5407 2023-05-18 07:10:02.000000 tumourkit-0.7.0/tumourkit/postprocessing/merge_cells.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1660 2023-05-18 07:11:45.000000 tumourkit-0.7.0/tumourkit/postprocessing/rswoosh.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.418893 tumourkit-0.7.0/tumourkit/preprocessing/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      616 2023-03-20 11:26:08.000000 tumourkit-0.7.0/tumourkit/preprocessing/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2307 2023-05-18 06:57:47.000000 tumourkit-0.7.0/tumourkit/preprocessing/centroids2png.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4660 2023-05-18 06:58:20.000000 tumourkit-0.7.0/tumourkit/preprocessing/centroidspng2csv.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3892 2023-05-18 07:00:03.000000 tumourkit-0.7.0/tumourkit/preprocessing/geojson2pngcsv.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3289 2023-05-18 07:00:16.000000 tumourkit-0.7.0/tumourkit/preprocessing/graph2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2825 2023-05-18 07:00:48.000000 tumourkit-0.7.0/tumourkit/preprocessing/hovernet2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3720 2023-05-18 07:01:18.000000 tumourkit-0.7.0/tumourkit/preprocessing/hovernet2geojson.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4731 2023-05-18 07:02:17.000000 tumourkit-0.7.0/tumourkit/preprocessing/png2graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2777 2023-05-18 07:02:32.000000 tumourkit-0.7.0/tumourkit/preprocessing/pngcsv2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5041 2023-05-18 07:02:55.000000 tumourkit-0.7.0/tumourkit/preprocessing/pngcsv2geojson.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3945 2023-05-18 07:03:41.000000 tumourkit-0.7.0/tumourkit/preprocessing/pngcsv2graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1861 2023-05-18 07:42:25.000000 tumourkit-0.7.0/tumourkit/preprocessing/remove_uncertain.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.420685 tumourkit-0.7.0/tumourkit/profiling/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2747 2023-05-18 07:35:28.000000 tumourkit-0.7.0/tumourkit/profiling/cpairs_profile.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1915 2023-05-18 07:36:50.000000 tumourkit-0.7.0/tumourkit/profiling/rswoosh_profile.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    15312 2023-05-18 07:56:19.000000 tumourkit-0.7.0/tumourkit/research_pipe.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.422293 tumourkit-0.7.0/tumourkit/segmentation/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      182 2023-03-08 12:07:32.000000 tumourkit-0.7.0/tumourkit/segmentation/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    12362 2023-05-18 07:40:19.000000 tumourkit-0.7.0/tumourkit/segmentation/evaluate.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.426797 tumourkit-0.7.0/tumourkit/segmentation/hovernet/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2023-03-08 08:02:19.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     2380 2023-03-20 14:44:06.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/config.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.429271 tumourkit-0.7.0/tumourkit/segmentation/hovernet/dataloader/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:49.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/dataloader/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     3322 2023-04-13 06:48:37.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/dataloader/augs.py
--rwx------   0 joseperezcano   (501) staff       (20)     3608 2023-01-26 12:04:04.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/dataloader/infer_loader.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     6632 2023-03-15 12:03:08.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/dataloader/train_loader.py
--rwx------   0 joseperezcano   (501) staff       (20)     8251 2023-03-08 08:12:38.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/extract_patches.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.431527 tumourkit-0.7.0/tumourkit/segmentation/hovernet/infer/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/infer/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     3497 2023-05-03 12:16:27.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/infer/base.py
--rwx------   0 joseperezcano   (501) staff       (20)    14233 2023-03-08 12:23:40.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/infer/tile.py
--rwx------   0 joseperezcano   (501) staff       (20)    30145 2023-03-23 17:33:09.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/infer/wsi.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.433636 tumourkit-0.7.0/tumourkit/segmentation/hovernet/metrics/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/metrics/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)    16129 2023-01-10 14:25:36.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/metrics/stats_utils.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.437934 tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     5473 2023-01-10 14:24:57.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/patch_extractor.py
--rwx------   0 joseperezcano   (501) staff       (20)     4951 2023-01-10 14:25:05.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     5727 2023-01-10 14:25:12.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/viz_utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     7419 2023-01-10 14:25:19.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/wsi_handler.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.438793 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.444226 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     5421 2023-01-10 14:23:15.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py
--rwx------   0 joseperezcano   (501) staff       (20)     9731 2023-01-10 14:23:26.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     6130 2023-03-15 07:07:22.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/opt.py
--rwx------   0 joseperezcano   (501) staff       (20)     7784 2023-03-22 08:36:42.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py
--rwx------   0 joseperezcano   (501) staff       (20)    13296 2023-03-13 19:48:31.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py
--rwx------   0 joseperezcano   (501) staff       (20)     5117 2023-04-25 06:50:35.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/targets.py
--rwx------   0 joseperezcano   (501) staff       (20)     4903 2023-01-10 16:18:24.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     8325 2023-05-03 12:12:19.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_infer.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.446066 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.448182 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/callbacks/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/callbacks/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     6991 2023-01-11 07:50:22.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py
--rwx------   0 joseperezcano   (501) staff       (20)     6145 2022-09-15 10:27:54.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py
--rwx------   0 joseperezcano   (501) staff       (20)     5955 2023-01-13 16:18:56.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py
--rwx------   0 joseperezcano   (501) staff       (20)     7482 2023-04-13 06:55:55.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/engine.py
--rwx------   0 joseperezcano   (501) staff       (20)     6834 2023-01-10 14:22:13.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)    10663 2023-03-23 18:07:29.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/train.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    10454 2023-05-18 07:56:27.000000 tumourkit-0.7.0/tumourkit/train_pipe.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.457319 tumourkit-0.7.0/tumourkit/utils/
--rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-09-26 11:04:45.000000 tumourkit-0.7.0/tumourkit/utils/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5934 2023-05-18 06:31:59.000000 tumourkit-0.7.0/tumourkit/utils/calibration_error.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5658 2023-05-18 06:37:18.000000 tumourkit-0.7.0/tumourkit/utils/classification.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3611 2023-05-18 06:39:27.000000 tumourkit-0.7.0/tumourkit/utils/folder2txt.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5321 2023-05-18 06:43:10.000000 tumourkit-0.7.0/tumourkit/utils/nearest.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3074 2023-05-18 06:43:40.000000 tumourkit-0.7.0/tumourkit/utils/pipes.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7053 2023-05-18 06:46:21.000000 tumourkit-0.7.0/tumourkit/utils/postprocessing.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    21855 2023-05-18 06:54:22.000000 tumourkit-0.7.0/tumourkit/utils/preprocessing.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5798 2023-05-18 06:56:50.000000 tumourkit-0.7.0/tumourkit/utils/read_nodes.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.392578 tumourkit-0.7.0/tumourkit.egg-info/
--rw-r--r--   0 joseperezcano   (501) staff       (20)    42041 2023-05-25 07:57:36.000000 tumourkit-0.7.0/tumourkit.egg-info/PKG-INFO
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4948 2023-05-25 07:57:36.000000 tumourkit-0.7.0/tumourkit.egg-info/SOURCES.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)        1 2023-05-25 07:57:36.000000 tumourkit-0.7.0/tumourkit.egg-info/dependency_links.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1054 2023-05-25 07:57:36.000000 tumourkit-0.7.0/tumourkit.egg-info/entry_points.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-05-25 07:57:36.000000 tumourkit-0.7.0/tumourkit.egg-info/requires.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-05-25 07:57:36.000000 tumourkit-0.7.0/tumourkit.egg-info/top_level.txt
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.341325 tumourkit-0.7.1/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    34523 2022-12-31 13:00:33.000000 tumourkit-0.7.1/LICENSE
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    42041 2023-05-30 20:01:02.340822 tumourkit-0.7.1/PKG-INFO
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1269 2023-03-25 17:22:23.000000 tumourkit-0.7.1/README.md
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.210515 tumourkit-0.7.1/docs/
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.210246 tumourkit-0.7.1/docs/buildenv/
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.228543 tumourkit-0.7.1/docs/buildenv/bin/
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      675 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2html.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      795 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2html4.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1163 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2html5.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      872 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2latex.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      680 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2man.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      845 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2odt.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1807 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      682 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      718 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2s5.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      952 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2xetex.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      683 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rst2xml.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      751 2023-03-25 16:44:11.000000 tumourkit-0.7.1/docs/buildenv/bin/rstpep2html.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.229235 tumourkit-0.7.1/docs/source/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1151 2023-04-11 15:21:40.000000 tumourkit-0.7.1/docs/source/conf.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2282 2023-05-25 06:24:46.000000 tumourkit-0.7.1/pyproject.toml
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-05-04 18:20:19.000000 tumourkit-0.7.1/requirements.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-05-30 20:01:02.341447 tumourkit-0.7.1/setup.cfg
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.248959 tumourkit-0.7.1/tests/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1596 2023-03-20 09:45:58.000000 tumourkit-0.7.1/tests/centroidspng2csv_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1871 2023-03-06 07:41:04.000000 tumourkit-0.7.1/tests/conf_matrix_sum_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2043 2023-03-06 07:25:02.000000 tumourkit-0.7.1/tests/cpairs_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      805 2023-03-06 07:25:20.000000 tumourkit-0.7.1/tests/example_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3927 2022-12-31 13:06:14.000000 tumourkit-0.7.1/tests/generate_centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3403 2022-12-31 13:06:04.000000 tumourkit-0.7.1/tests/generate_rswoosh.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1517 2023-03-06 07:25:59.000000 tumourkit-0.7.1/tests/get_conn_comp_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1827 2023-03-28 15:20:41.000000 tumourkit-0.7.1/tests/graph2centroids_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1707 2023-03-20 10:39:44.000000 tumourkit-0.7.1/tests/graph_idx_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2183 2023-05-30 17:37:56.000000 tumourkit-0.7.1/tests/hov_prob_pipe_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2098 2023-03-06 07:27:57.000000 tumourkit-0.7.1/tests/hov_prob_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2503 2023-03-23 07:08:34.000000 tumourkit-0.7.1/tests/hovernet_patches_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1844 2023-03-06 07:41:02.000000 tumourkit-0.7.1/tests/metrics_pairs_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1974 2023-03-06 07:41:00.000000 tumourkit-0.7.1/tests/metrics_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1898 2023-03-20 10:58:10.000000 tumourkit-0.7.1/tests/png2graph_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2240 2023-03-06 07:30:23.000000 tumourkit-0.7.1/tests/pngcsv2geojson_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1829 2023-03-20 10:39:00.000000 tumourkit-0.7.1/tests/pngcsv2graph_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1978 2023-04-12 10:40:07.000000 tumourkit-0.7.1/tests/read_nodes_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1374 2023-03-06 07:31:03.000000 tumourkit-0.7.1/tests/remove_idx_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1577 2023-03-06 07:31:28.000000 tumourkit-0.7.1/tests/rswoosh_test.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.256270 tumourkit-0.7.1/tumourkit/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      154 2023-05-30 19:59:52.000000 tumourkit-0.7.1/tumourkit/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.266972 tumourkit-0.7.1/tumourkit/classification/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      155 2023-04-11 15:25:33.000000 tumourkit-0.7.1/tumourkit/classification/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1356 2023-05-18 07:19:54.000000 tumourkit-0.7.1/tumourkit/classification/compute_imbalance.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     8132 2023-05-30 18:36:23.000000 tumourkit-0.7.1/tumourkit/classification/evaluate.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     6654 2023-05-30 18:28:05.000000 tumourkit-0.7.1/tumourkit/classification/infer.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.271271 tumourkit-0.7.1/tumourkit/classification/models/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-11-28 08:50:03.000000 tumourkit-0.7.1/tumourkit/classification/models/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2532 2023-03-23 17:44:30.000000 tumourkit-0.7.1/tumourkit/classification/models/gat.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2008 2022-12-31 13:10:31.000000 tumourkit-0.7.1/tumourkit/classification/models/gcn.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7769 2022-12-31 13:10:48.000000 tumourkit-0.7.1/tumourkit/classification/models/hgao.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2840 2022-12-19 09:14:00.000000 tumourkit-0.7.1/tumourkit/classification/models/norm.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7575 2023-05-18 07:24:15.000000 tumourkit-0.7.1/tumourkit/classification/read_graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    20658 2023-05-18 07:28:33.000000 tumourkit-0.7.1/tumourkit/classification/train_graphs.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    10426 2023-05-18 07:32:33.000000 tumourkit-0.7.1/tumourkit/classification/train_xgboost.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.272706 tumourkit-0.7.1/tumourkit/demo/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    17409 2023-05-30 18:03:04.000000 tumourkit-0.7.1/tumourkit/demo/app.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7305 2023-05-30 18:04:56.000000 tumourkit-0.7.1/tumourkit/eval_pipe.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     9512 2023-05-30 18:06:38.000000 tumourkit-0.7.1/tumourkit/infer_pipe.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4131 2023-05-30 18:12:51.000000 tumourkit-0.7.1/tumourkit/make_dirs.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.281880 tumourkit-0.7.1/tumourkit/postprocessing/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      195 2023-05-30 17:38:57.000000 tumourkit-0.7.1/tumourkit/postprocessing/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3411 2023-05-30 18:20:10.000000 tumourkit-0.7.1/tumourkit/postprocessing/draw_cells.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     6896 2023-05-30 17:55:03.000000 tumourkit-0.7.1/tumourkit/postprocessing/draw_graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4198 2023-05-30 18:20:42.000000 tumourkit-0.7.1/tumourkit/postprocessing/join_graph_gt.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     6977 2023-05-30 18:21:29.000000 tumourkit-0.7.1/tumourkit/postprocessing/join_hovprob_graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     6510 2023-05-30 18:23:48.000000 tumourkit-0.7.1/tumourkit/postprocessing/merge_cells.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2094 2023-05-30 18:24:14.000000 tumourkit-0.7.1/tumourkit/postprocessing/rswoosh.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.301299 tumourkit-0.7.1/tumourkit/preprocessing/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      666 2023-05-30 17:35:42.000000 tumourkit-0.7.1/tumourkit/preprocessing/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2307 2023-05-18 06:57:47.000000 tumourkit-0.7.1/tumourkit/preprocessing/centroids2png.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4660 2023-05-18 06:58:20.000000 tumourkit-0.7.1/tumourkit/preprocessing/centroidspng2csv.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3892 2023-05-18 07:00:03.000000 tumourkit-0.7.1/tumourkit/preprocessing/geojson2pngcsv.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3289 2023-05-18 07:00:16.000000 tumourkit-0.7.1/tumourkit/preprocessing/graph2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2825 2023-05-18 07:00:48.000000 tumourkit-0.7.1/tumourkit/preprocessing/hovernet2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3720 2023-05-18 07:01:18.000000 tumourkit-0.7.1/tumourkit/preprocessing/hovernet2geojson.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4731 2023-05-18 07:02:17.000000 tumourkit-0.7.1/tumourkit/preprocessing/png2graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2777 2023-05-18 07:02:32.000000 tumourkit-0.7.1/tumourkit/preprocessing/pngcsv2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5041 2023-05-18 07:02:55.000000 tumourkit-0.7.1/tumourkit/preprocessing/pngcsv2geojson.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4452 2023-05-30 18:18:32.000000 tumourkit-0.7.1/tumourkit/preprocessing/pngcsv2graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2434 2023-05-30 18:19:10.000000 tumourkit-0.7.1/tumourkit/preprocessing/remove_uncertain.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.302852 tumourkit-0.7.1/tumourkit/profiling/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2747 2023-05-18 07:35:28.000000 tumourkit-0.7.1/tumourkit/profiling/cpairs_profile.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1915 2023-05-18 07:36:50.000000 tumourkit-0.7.1/tumourkit/profiling/rswoosh_profile.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    18656 2023-05-30 18:35:31.000000 tumourkit-0.7.1/tumourkit/research_pipe.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.306229 tumourkit-0.7.1/tumourkit/segmentation/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      182 2023-03-08 12:07:32.000000 tumourkit-0.7.1/tumourkit/segmentation/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    14370 2023-05-30 18:17:43.000000 tumourkit-0.7.1/tumourkit/segmentation/evaluate.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.311297 tumourkit-0.7.1/tumourkit/segmentation/hovernet/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2023-03-08 08:02:19.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     2380 2023-03-20 14:44:06.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/config.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.314455 tumourkit-0.7.1/tumourkit/segmentation/hovernet/dataloader/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:49.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/dataloader/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3322 2023-04-13 06:48:37.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/dataloader/augs.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3608 2023-01-26 12:04:04.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/dataloader/infer_loader.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     6632 2023-03-15 12:03:08.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/dataloader/train_loader.py
+-rwx------   0 joseperezcano   (501) staff       (20)     8251 2023-03-08 08:12:38.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/extract_patches.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.316652 tumourkit-0.7.1/tumourkit/segmentation/hovernet/infer/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/infer/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3497 2023-05-03 12:16:27.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/infer/base.py
+-rwx------   0 joseperezcano   (501) staff       (20)    14233 2023-03-08 12:23:40.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/infer/tile.py
+-rwx------   0 joseperezcano   (501) staff       (20)    30145 2023-03-23 17:33:09.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/infer/wsi.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.317992 tumourkit-0.7.1/tumourkit/segmentation/hovernet/metrics/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/metrics/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)    16129 2023-01-10 14:25:36.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/metrics/stats_utils.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.321515 tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5473 2023-01-10 14:24:57.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/patch_extractor.py
+-rwx------   0 joseperezcano   (501) staff       (20)     4951 2023-01-10 14:25:05.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5727 2023-01-10 14:25:12.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/viz_utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7419 2023-01-10 14:25:19.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/wsi_handler.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.322050 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.328526 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5421 2023-01-10 14:23:15.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py
+-rwx------   0 joseperezcano   (501) staff       (20)     9731 2023-01-10 14:23:26.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6130 2023-03-15 07:07:22.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/opt.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7784 2023-03-22 08:36:42.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py
+-rwx------   0 joseperezcano   (501) staff       (20)    13296 2023-03-13 19:48:31.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5117 2023-04-25 06:50:35.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/targets.py
+-rwx------   0 joseperezcano   (501) staff       (20)     4903 2023-01-10 16:18:24.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     8325 2023-05-03 12:12:19.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_infer.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.330104 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.332281 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/callbacks/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/callbacks/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6991 2023-01-11 07:50:22.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6145 2022-09-15 10:27:54.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5955 2023-01-13 16:18:56.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7482 2023-04-13 06:55:55.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/engine.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6834 2023-01-10 14:22:13.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)    10663 2023-03-23 18:07:29.000000 tumourkit-0.7.1/tumourkit/segmentation/hovernet/train.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    12250 2023-05-30 18:35:15.000000 tumourkit-0.7.1/tumourkit/train_pipe.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.339837 tumourkit-0.7.1/tumourkit/utils/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-09-26 11:04:45.000000 tumourkit-0.7.1/tumourkit/utils/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5934 2023-05-18 06:31:59.000000 tumourkit-0.7.1/tumourkit/utils/calibration_error.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5658 2023-05-18 06:37:18.000000 tumourkit-0.7.1/tumourkit/utils/classification.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3611 2023-05-18 06:39:27.000000 tumourkit-0.7.1/tumourkit/utils/folder2txt.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5321 2023-05-18 06:43:10.000000 tumourkit-0.7.1/tumourkit/utils/nearest.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4402 2023-05-30 18:14:32.000000 tumourkit-0.7.1/tumourkit/utils/pipes.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7053 2023-05-18 06:46:21.000000 tumourkit-0.7.1/tumourkit/utils/postprocessing.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    21855 2023-05-18 06:54:22.000000 tumourkit-0.7.1/tumourkit/utils/preprocessing.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5798 2023-05-18 06:56:50.000000 tumourkit-0.7.1/tumourkit/utils/read_nodes.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-30 20:01:02.260659 tumourkit-0.7.1/tumourkit.egg-info/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    42041 2023-05-30 20:01:02.000000 tumourkit-0.7.1/tumourkit.egg-info/PKG-INFO
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4948 2023-05-30 20:01:02.000000 tumourkit-0.7.1/tumourkit.egg-info/SOURCES.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        1 2023-05-30 20:01:02.000000 tumourkit-0.7.1/tumourkit.egg-info/dependency_links.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1054 2023-05-30 20:01:02.000000 tumourkit-0.7.1/tumourkit.egg-info/entry_points.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-05-30 20:01:02.000000 tumourkit-0.7.1/tumourkit.egg-info/requires.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-05-30 20:01:02.000000 tumourkit-0.7.1/tumourkit.egg-info/top_level.txt
```

### Comparing `tumourkit-0.7.0/LICENSE` & `tumourkit-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/PKG-INFO` & `tumourkit-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumourkit
-Version: 0.7.0
+Version: 0.7.1
 Summary: A SDK for tumour study
 Author-email: Jose Pérez Cano <joseperez2000@hotmail.es>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `tumourkit-0.7.0/README.md` & `tumourkit-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/docs/buildenv/bin/rst2html.py` & `tumourkit-0.7.1/docs/buildenv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/docs/buildenv/bin/rst2html4.py` & `tumourkit-0.7.1/docs/buildenv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/docs/buildenv/bin/rst2html5.py` & `tumourkit-0.7.1/docs/buildenv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/docs/buildenv/bin/rst2latex.py` & `tumourkit-0.7.1/docs/buildenv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/docs/buildenv/bin/rst2man.py` & `tumourkit-0.7.1/docs/buildenv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/docs/buildenv/bin/rst2odt.py` & `tumourkit-0.7.1/docs/buildenv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/docs/buildenv/bin/rst2odt_prepstyles.py` & `tumourkit-0.7.1/docs/buildenv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/docs/buildenv/bin/rst2pseudoxml.py` & `tumourkit-0.7.1/docs/buildenv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/docs/buildenv/bin/rst2s5.py` & `tumourkit-0.7.1/docs/buildenv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/docs/buildenv/bin/rst2xetex.py` & `tumourkit-0.7.1/docs/buildenv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/docs/buildenv/bin/rst2xml.py` & `tumourkit-0.7.1/docs/buildenv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/docs/buildenv/bin/rstpep2html.py` & `tumourkit-0.7.1/docs/buildenv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/docs/source/conf.py` & `tumourkit-0.7.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/pyproject.toml` & `tumourkit-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/requirements.txt` & `tumourkit-0.7.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tests/centroidspng2csv_test.py` & `tumourkit-0.7.1/tests/centroidspng2csv_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tests/conf_matrix_sum_test.py` & `tumourkit-0.7.1/tests/conf_matrix_sum_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tests/cpairs_test.py` & `tumourkit-0.7.1/tests/cpairs_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tests/example_test.py` & `tumourkit-0.7.1/tests/example_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tests/generate_centroids.py` & `tumourkit-0.7.1/tests/generate_centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tests/generate_rswoosh.py` & `tumourkit-0.7.1/tests/generate_rswoosh.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tests/get_conn_comp_test.py` & `tumourkit-0.7.1/tests/get_conn_comp_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tests/graph2centroids_test.py` & `tumourkit-0.7.1/tests/graph2centroids_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tests/graph_idx_test.py` & `tumourkit-0.7.1/tests/graph_idx_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tests/hov_prob_pipe_test.py` & `tumourkit-0.7.1/tests/hov_prob_pipe_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 """
 import shutil
 import os
 from argparse import Namespace
 import pandas as pd
 
 from tumourkit.utils.preprocessing import parse_path, create_dir
-from tumourkit.postprocessing import join_graph_gt
-from tumourkit.postprocessing import join_hovprob_graph
+from tumourkit.postprocessing import join_graph_gt_main, join_hovprob_graph_main
 from tumourkit import eval_class
 
 TEST_DIR = os.path.dirname(os.path.abspath(__file__))
 TEST_DIR = parse_path(TEST_DIR)
 JSON_DIR = TEST_DIR + 'json/'
 GRAPHS_DIR = TEST_DIR + 'pipe_graphs/'
 CENTROIDS_DIR = TEST_DIR + 'pipe_centroids/'
@@ -36,25 +35,25 @@
 
 def test_hov_prob_pipe():
     create_dir(TMP_DIR)
     args = Namespace()
     args.graph_dir = GRAPHS_DIR
     args.centroids_dir = CENTROIDS_DIR
     args.output_dir = TMP_DIR
-    join_graph_gt(args)
+    join_graph_gt_main(args)
     args.node_dir = TMP_DIR
     args.save_file = TEST_DIR + 'tmp'
     args.by_img = False
     args.draw = False
     eval_class(args)
     args.json_dir = JSON_DIR
     args.graph_dir = TMP_DIR
     args.output_dir = TMP_DIR
     args.num_classes = 2
-    join_hovprob_graph(args)
+    join_hovprob_graph_main(args)
     args.node_dir = TMP_DIR
     args.save_file = TEST_DIR + 'tmp2'
     eval_class(args)
     res1 = pd.read_csv(TEST_DIR + 'tmp.csv')
     res2 = pd.read_csv(TEST_DIR + 'tmp2.csv')
     assert (abs(res1['Accuracy'] - res2['Accuracy']) < 0.01)[0]
     assert (abs(res1['F1-score'] - res2['F1-score']) < 0.01)[0]
```

### Comparing `tumourkit-0.7.0/tests/hov_prob_test.py` & `tumourkit-0.7.1/tests/hov_prob_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tests/hovernet_patches_test.py` & `tumourkit-0.7.1/tests/hovernet_patches_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tests/metrics_pairs_test.py` & `tumourkit-0.7.1/tests/metrics_pairs_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tests/metrics_test.py` & `tumourkit-0.7.1/tests/metrics_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tests/png2graph_test.py` & `tumourkit-0.7.1/tests/png2graph_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tests/pngcsv2geojson_test.py` & `tumourkit-0.7.1/tests/pngcsv2geojson_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tests/pngcsv2graph_test.py` & `tumourkit-0.7.1/tests/pngcsv2graph_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tests/read_nodes_test.py` & `tumourkit-0.7.1/tests/read_nodes_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tests/remove_idx_test.py` & `tumourkit-0.7.1/tests/remove_idx_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tests/rswoosh_test.py` & `tumourkit-0.7.1/tests/rswoosh_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/classification/compute_imbalance.py` & `tumourkit-0.7.1/tumourkit/classification/compute_imbalance.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/classification/infer.py` & `tumourkit-0.7.1/tumourkit/classification/infer.py`

 * *Files 24% similar despite different names*

```diff
@@ -33,37 +33,63 @@
 import pandas as pd
 import argparse
 import os
 
 
 def load_saved_model(weights_path: str, conf_path: str, num_classes: int, num_feats: int) -> nn.Module:
     """
-    Loads state_dict into a torch module.
-    Configuration file must match with state_dict.
+    Loads a saved model from the given weights_path and conf_path.
+
+    :param weights_path: The path to the saved weights file.
+    :type weights_path: str
+    :param conf_path: The path to the configuration file.
+    :type conf_path: str
+    :param num_classes: The number of classes for the model.
+    :type num_classes: int
+    :param num_feats: The number of features for the model.
+    :type num_feats: int
+    :return: The loaded model.
+    :rtype: nn.Module
     """
     state_dict = torch.load(weights_path, map_location='cpu')
     with open(conf_path, 'r') as f:
         conf = json.load(f)
     model = load_model(conf, num_classes, num_feats)
     model.load_state_dict(state_dict)
     return model
 
 
 def load_normalizer(norm_path: str) -> Tuple[Any]:
     """
-    Returns normalizers used in training save at norm_path.
+    Loads the normalizers used in training from the given norm_path.
+
+    :param norm_path: The path to the saved normalizers file.
+    :type norm_path: str
+    :return: The loaded normalizers.
+    :rtype: Tuple[Any]
     """
     with open(norm_path, 'rb') as f:
         normalizers = pickle.load(f)
     return normalizers
 
 
 def run_inference(model: nn.Module, loader: GraphDataLoader, device: str, num_classes: int) -> Dict[str, np.ndarray]:
     """
-    Computes probabilities for all the nodes.
+    Runs inference using the specified model on the provided data loader.
+
+    :param model: The model used for inference.
+    :type model: nn.Module
+    :param loader: The graph data loader.
+    :type loader: GraphDataLoader
+    :param device: The device used for inference (e.g., 'cpu' or 'cuda').
+    :type device: str
+    :param num_classes: The number of classes.
+    :type num_classes: int
+    :return: The probabilities for all the nodes.
+    :rtype: Dict[str, np.ndarray]
     """
     probs = {}
     for g, name in loader:
         # self-loops
         g = dgl.remove_self_loop(g)
         g = dgl.add_self_loop(g)
         # data
@@ -76,16 +102,24 @@
             prob = F.softmax(logits, dim=1).detach().numpy()
         probs[name[0]] = prob
     return probs
 
 
 def save_probs(probs: Dict[str, np.ndarray], node_dir: str, output_dir: str, num_classes: int) -> None:
     """
-    Saves probabilities in .nodes.csv files.
-    It appends a column to original .nodes.csv file.
+    Saves the probabilities in .nodes.csv files by appending a column to the original .nodes.csv file.
+
+    :param probs: The probabilities for each graph.
+    :type probs: Dict[str, np.ndarray]
+    :param node_dir: The directory containing the original .nodes.csv files.
+    :type node_dir: str
+    :param output_dir: The directory where the updated .nodes.csv files will be saved.
+    :type output_dir: str
+    :param num_classes: The number of classes.
+    :type num_classes: int
     """
     for name, prob in probs.items():
         orig = pd.read_csv(os.path.join(node_dir, name))
         if num_classes == 2:
             orig['prob1'] = prob
         else:
             for k in range(1, num_classes + 1):
```

### Comparing `tumourkit-0.7.0/tumourkit/classification/models/gat.py` & `tumourkit-0.7.1/tumourkit/classification/models/gat.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/classification/models/gcn.py` & `tumourkit-0.7.1/tumourkit/classification/models/gcn.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/classification/models/hgao.py` & `tumourkit-0.7.1/tumourkit/classification/models/hgao.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/classification/models/norm.py` & `tumourkit-0.7.1/tumourkit/classification/models/norm.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/classification/read_graph.py` & `tumourkit-0.7.1/tumourkit/classification/read_graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/classification/train_graphs.py` & `tumourkit-0.7.1/tumourkit/classification/train_graphs.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/classification/train_xgboost.py` & `tumourkit-0.7.1/tumourkit/classification/train_xgboost.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/eval_pipe.py` & `tumourkit-0.7.1/tumourkit/eval_pipe.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,32 +22,40 @@
 from argparse import Namespace
 import logging
 from logging import Logger
 import numpy as np
 import pandas as pd
 from . import eval_segment
 import os
-from .preprocessing import hovernet2centroids, geojson2pngcsv, pngcsv2centroids
+from .preprocessing import hovernet2centroids_main, geojson2pngcsv_main, pngcsv2centroids_main
 from .utils.preprocessing import get_names
 from .utils.pipes import HovernetNotFoundError, check_void
 from .utils.classification import metrics_from_predictions
 
 
 def run_preprocessing(args: Namespace, logger: Logger) -> None:
     """
-    Converts the gson format to the rest of formats.
+    Runs the preprocessing steps to convert the gson format to other formats.
+
+    :param args: The arguments for the preprocessing.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
+
+    :raises HovernetNotFoundError: If the Hovernet centroids are not found in the training output.
     """
     logger.info('Extracting Hovernet centroids from training output.')
     if not os.path.isdir(os.path.join(args.root_dir, 'data', 'tmp_hov', 'json')):
         raise HovernetNotFoundError('Please, train again or extract hovernet outputs.')
     newargs = Namespace(
         json_dir=os.path.join(args.root_dir, 'data', 'tmp_hov', 'json'),
         output_path=os.path.join(args.root_dir, 'data', 'tmp_hov', 'centroids_hov'),
     )
-    hovernet2centroids(newargs)
+    hovernet2centroids_main(newargs)
     for split in ['train', 'validation', 'test']:
         if check_void(os.path.join(args.root_dir, 'data', split, 'names.txt')):
             logger.info(f'Preprocessing split {split}.')
             split_names = get_names(os.path.join(args.root_dir, 'data', split, 'gson'), '.geojson')
             with open(os.path.join(args.root_dir, 'data', split, 'names.txt'), 'w') as f:
                 for name in split_names:
                     print(name, file=f)
@@ -55,27 +63,39 @@
             logger.info('   From geojson to pngcsv.')
             newargs = Namespace(
                 gson_dir=os.path.join(args.root_dir, 'data', split, 'gson'),
                 png_dir=os.path.join(args.root_dir, 'data', split, 'png'),
                 csv_dir=os.path.join(args.root_dir, 'data', split, 'csv'),
                 num_classes=args.num_classes,
             )
-            geojson2pngcsv(newargs)
+            geojson2pngcsv_main(newargs)
         if check_void(os.path.join(args.root_dir, 'data', split, 'centroids')):
             logger.info('   Extracting centroids from GT.')
             newargs = Namespace(
                 png_dir=os.path.join(args.root_dir, 'data', split, 'png'),
                 csv_dir=os.path.join(args.root_dir, 'data', split, 'csv'),
                 output_path=os.path.join(args.root_dir, 'data', split, 'centroids')
             )
-            pngcsv2centroids(newargs)
+            pngcsv2centroids_main(newargs)
     return
 
 
 def compute_ece(args: Namespace, logger: Logger, split: str) -> None:
+    """
+    Computes Expected Calibration Error (ECE) and other metrics for the given split.
+
+    :param args: The arguments for computing ECE and metrics.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
+
+    :param split: The name of the split (e.g., 'train', 'validation', 'test').
+    :type split: str
+    """
     folder = os.path.join(args.root_dir, 'data', split, 'graphs', 'preds')
     trues, probs = None, None
     for file in os.listdir(folder):
         df = pd.read_csv(os.path.join(folder, file))
         _trues = df['class'].to_numpy() - 1
         if trues is None:
             trues = _trues.reshape((-1, 1))
@@ -104,14 +124,23 @@
             'Macro F1': [macro], 'Weighted F1': [weighted], 'Micro F1': [micro], 'ECE': [ece]
         }
     metrics_df = pd.DataFrame(dic_metrics)
     metrics_df.to_csv(args.save_name + '_' + split + '_ece.csv', index=False)
 
 
 def run_evaluation(args: Namespace, logger: Logger) -> None:
+    """
+    Runs the evaluation of Hovernet output for different splits.
+
+    :param args: The arguments for the evaluation.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
+    """
     logger.info('Starting evaluation of Hovernet output.')
     for split in ['train', 'validation', 'test']:
         logger.info(f'    Evaluating {split} split')
         newargs = Namespace(
             names=os.path.join(args.root_dir, 'data', split, 'names.txt'),
             gt_path=os.path.join(args.root_dir, 'data', split, 'centroids'),
             pred_path=os.path.join(args.root_dir, 'data', 'tmp_hov', 'centroids_hov'),
```

### Comparing `tumourkit-0.7.0/tumourkit/infer_pipe.py` & `tumourkit-0.7.1/tumourkit/infer_pipe.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,22 +20,31 @@
 """
 import argparse
 from argparse import Namespace
 import logging
 from logging import Logger
 from .segmentation import hov_infer
 import os
-from .preprocessing import geojson2pngcsv, png2graph, hovernet2geojson, graph2centroids, centroidspng2csv, pngcsv2geojson
-from .postprocessing import join_hovprob_graph
+from .preprocessing import geojson2pngcsv_main, png2graph_main, hovernet2geojson_main, graph2centroids_main, centroidspng2csv_main, pngcsv2geojson_main
+from .postprocessing import join_hovprob_graph_main
 from .utils.preprocessing import create_dir
 from .classification import infer_gnn
 import pandas as pd
 
 
 def set_best_configuration(args: Namespace, logger: Logger) -> None:
+    """
+    Sets the best configuration from training based on the F1 score.
+
+    :param args: The arguments for setting the best configuration.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
+    """
     logger.info('Configuration not provided, using best configuration from training based on F1 score.')
     if args.best_arch == 'GCN':
         save_file = os.path.join(args.root_dir, 'gnn_logs', 'gcn_results.csv')
     elif args.best_arch == 'ATT':
         save_file = os.path.join(args.root_dir, 'gnn_logs', 'gat_results.csv')
     else:
         assert False, 'Architecture not supported'
@@ -47,14 +56,23 @@
     args.best_num_layers = str(best_conf['NUM_LAYERS'])
     args.best_dropout = str(best_conf['DROPOUT'])
     args.best_norm_type = str(best_conf['NORM_TYPE'])
     return
 
 
 def run_hovernet(args: Namespace, logger: Logger) -> None:
+    """
+    Runs the Hovernet inference.
+
+    :param args: The arguments for running Hovernet inference.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
+    """
     logger.info('Starting hovernet inference.')
     newargs = {
         'nr_types': str(args.num_classes + 1),
         'type_info_path': os.path.join(args.root_dir, 'weights', 'segmentation', 'hovernet', 'type_info.json'),
         'gpu': args.gpu,
         'nr_inference_workers': '0',
         'model_path': os.path.join(args.root_dir, 'weights', 'segmentation', 'hovernet', '01', 'net_epoch=50.tar'),
@@ -73,51 +91,69 @@
         'mem_usage': '0.2'
     }
     hov_infer(newargs, newsubargs, 'tile')
     return
 
 
 def run_posthov(args: Namespace, logger: Logger) -> None:
+    """
+    Performs post-processing steps on Hovernet output.
+
+    :param args: The arguments for running post-processing on Hovernet output.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
+    """
     logger.info('Parsing Hovernet output')
     logger.info('   From json to geojson.')
     newargs = Namespace(
         json_dir=os.path.join(args.output_dir, 'tmp_hov', 'json'),
         gson_dir=os.path.join(args.output_dir, 'gson_hov'),
         num_classes=args.num_classes
     )
-    hovernet2geojson(newargs)
+    hovernet2geojson_main(newargs)
     logger.info('   From geojson to pngcsv.')
     newargs = Namespace(
         gson_dir=os.path.join(args.output_dir, 'gson_hov'),
         png_dir=os.path.join(args.output_dir, 'png_hov'),
         csv_dir=os.path.join(args.output_dir, 'csv_hov'),
         num_classes=args.num_classes
     )
-    geojson2pngcsv(newargs)
+    geojson2pngcsv_main(newargs)
     logger.info('   From pngcsv to nodes.csv.')
     create_dir(os.path.join(args.output_dir, 'graphs'))
     newargs = Namespace(
         png_dir=os.path.join(args.output_dir, 'png_hov'),
         orig_dir=args.input_dir,
         output_path=os.path.join(args.output_dir, 'graphs', 'raw'),
         num_workers=args.num_workers
     )
-    png2graph(newargs)
+    png2graph_main(newargs)
     logger.info('   Adding hovernet predictions to .nodes.csv.')
     newargs = Namespace(
         json_dir=os.path.join(args.output_dir, 'tmp_hov', 'json'),
         graph_dir=os.path.join(args.output_dir, 'graphs', 'raw'),
         output_dir=os.path.join(args.output_dir, 'graphs', 'hovpreds'),
         num_classes=args.num_classes
     )
-    join_hovprob_graph(newargs, logger)
+    join_hovprob_graph_main(newargs, logger)
     return
 
 
 def run_graphs(args: Namespace, logger: Logger) -> None:
+    """
+    Runs the graph inference.
+
+    :param args: The arguments for running graph inference.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
+    """
     logger.info('Starting graph inference.')
     model_name = 'best_' + args.best_arch + '_' + args.best_num_layers + '_' \
         + args.best_dropout + '_' + args.best_norm_type
     newargs = Namespace(
         node_dir=os.path.join(args.output_dir, 'graphs', 'hovpreds'),
         output_dir=os.path.join(args.output_dir, 'gnn_preds'),
         weights=os.path.join(args.root_dir, 'weights', 'classification', 'gnn', 'weights', model_name + '.pth'),
@@ -128,37 +164,46 @@
         disable_morph_feats=False,
     )
     infer_gnn(newargs)
     return
 
 
 def run_postgraphs(args: Namespace, logger: Logger) -> None:
+    """
+    Performs post-processing steps on GNN output.
+
+    :param args: The arguments for running post-processing on GNN output.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
+    """
     logger.info('Parsing gnn output.')
     logger.info('   Converting .nodes.csv to .centroids.csv.')
     newargs = Namespace(
         graph_dir=os.path.join(args.output_dir, 'gnn_preds'),
         centroids_dir=os.path.join(args.output_dir, 'centroids'),
         num_classes=args.num_classes,
     )
-    graph2centroids(newargs)
+    graph2centroids_main(newargs)
     logger.info('   Converting .centroids.csv and .GT_cells.png to .class.csv.')
     newargs = Namespace(
         centroids_dir=os.path.join(args.output_dir, 'centroids'),
         png_dir=os.path.join(args.output_dir, 'png_hov'),
         csv_dir=os.path.join(args.output_dir, 'csv_gnn'),
     )
-    centroidspng2csv(newargs)
+    centroidspng2csv_main(newargs)
     logger.info('   Converting png/csv to geojson.')
     newargs = Namespace(
         png_dir=os.path.join(args.output_dir, 'png_hov'),
         csv_dir=os.path.join(args.output_dir, 'csv_gnn'),
         gson_dir=os.path.join(args.output_dir, 'gson_gnn'),
         num_classes=args.num_classes
     )
-    pngcsv2geojson(newargs)
+    pngcsv2geojson_main(newargs)
     return
 
 
 def _create_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument('--root-dir', type=str, help='Internal data and weights directory.', default='./.internals/')
     parser.add_argument('--input-dir', type=str, help='Folder containing patches to process.', required=True)
```

### Comparing `tumourkit-0.7.0/tumourkit/make_dirs.py` & `tumourkit-0.7.1/tumourkit/make_dirs.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,15 +30,21 @@
     parser.add_argument('--root-dir', type=str, default='./.internals/', help='Root folder to save data and models.')
     parser.add_argument('--num-classes', type=int, default=2, help='Number of classes (up to 7) to consider in the classification problem.')
     return parser
 
 
 def create_subfolders(node: Union[Dict, List], current_folder: str) -> None:
     """
-    Creates folders and subfolders recursively. The leaf nodes must be lists.
+    Creates folders and subfolders recursively.
+
+    :param node: The folder structure represented as a dictionary or list.
+    :type node: Union[Dict, List]
+
+    :param current_folder: The current folder where the folders and subfolders will be created.
+    :type current_folder: str
     """
     if isinstance(node, Dict):
         for key, value in node.items():
             subfolder = os.path.join(current_folder, key)
             os.mkdir(subfolder)
             create_subfolders(value, subfolder)
     elif isinstance(node, List):
```

### Comparing `tumourkit-0.7.0/tumourkit/postprocessing/draw_cells.py` & `tumourkit-0.7.1/tumourkit/postprocessing/draw_cells.py`

 * *Files 21% similar despite different names*

```diff
@@ -28,15 +28,38 @@
 import numpy as np
 import pandas as pd
 import json
 from typing import Dict, Tuple, List
 from ..utils.preprocessing import get_names, read_labels
 
 
-def draw_cells(orig: np.ndarray, png: np.ndarray, csv: pd.DataFrame, type_info: Dict[str, Tuple[str, List[int]]]) -> np.ndarray:
+def draw_cells(
+        orig: np.ndarray,
+        png: np.ndarray,
+        csv: pd.DataFrame,
+        type_info: Dict[str, Tuple[str, List[int]]]
+        ) -> np.ndarray:
+    """
+    Draws cell labels on the original image based on the PNG labels and CSV data.
+
+    Given the original image, PNG labels, CSV data containing cell labels,
+    and type information, this function draws the cell labels on the original image.
+    The cell labels are blended with the original image by alpha compositing.
+
+    :param orig: The original image.
+    :type orig: np.ndarray
+    :param png: The PNG labels representing cell IDs.
+    :type png: np.ndarray
+    :param csv: The CSV data containing cell labels.
+    :type csv: pd.DataFrame
+    :param type_info: The type information dictionary mapping cell labels to colors.
+    :type type_info: Dict[str, Tuple[str, List[int]]]
+    :return: The image with cell labels drawn on it.
+    :rtype: np.ndarray
+    """
     blend = orig.copy()
     for i, (idx, cell_label) in csv.iterrows():
         blend[png == idx] = 0.3 * np.array(type_info[str(cell_label)][1]) \
             + 0.7 * blend[png == idx]
     return blend
```

### Comparing `tumourkit-0.7.0/tumourkit/postprocessing/join_graph_gt.py` & `tumourkit-0.7.1/tumourkit/postprocessing/join_graph_gt.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,16 +27,27 @@
 import os
 from ..utils.preprocessing import parse_path, create_dir, get_names, read_centroids, save_graph
 from ..utils.nearest import generate_tree, find_nearest
 
 
 def merge_labels(graph: pd.DataFrame, centroids: np.ndarray) -> pd.DataFrame:
     """
-    Finds 1-1 matchings of nodes and substitutes labels in graph
-    by those in centroids. Internally uses KD-trees.
+    Matches nodes in the graph to centroids and updates their labels.
+
+    Given a graph DataFrame and a centroids array, this function finds 1-1 matchings
+    between nodes in the graph and centroids based on their coordinates.
+    It substitutes the labels of the graph nodes with the labels from the centroids.
+    The matching is performed using KD-trees for efficient nearest neighbor search.
+
+    :param graph: The graph DataFrame containing nodes with labels.
+    :type graph: pd.DataFrame
+    :param centroids: The centroids array containing coordinates and labels.
+    :type centroids: np.ndarray
+    :return: The updated graph DataFrame with matched labels.
+    :rtype: pd.DataFrame
     """
     assert len(centroids) > 0, 'GT must contain at least one cell.'
     graph = graph.copy()
     graph['prob1'] = graph['class'] - 1
     gt_tree = generate_tree(centroids[:, :2])
     pred_centroids = graph[['X', 'Y']].to_numpy(dtype=int)
     pred_tree = generate_tree(pred_centroids)
```

### Comparing `tumourkit-0.7.0/tumourkit/postprocessing/join_hovprob_graph.py` & `tumourkit-0.7.1/tumourkit/postprocessing/join_hovprob_graph.py`

 * *Files 19% similar despite different names*

```diff
@@ -30,16 +30,28 @@
 from ..utils.nearest import generate_tree, find_nearest
 import logging
 from logging import Logger
 
 
 def parse_centroids_probs(nuc: Dict[str, Any], logger: Optional[Logger] = None, num_classes: Optional[int] = 2) -> List[Tuple[int, int, int]]:
     """
-    Input: Hovernet json nuclei dictionary as given by modified run_infer.py.
-    Output: List of (X,Y,prob1) tuples representing centroids.
+    Parses the centroids and probabilities from the Hovernet JSON nuclei dictionary.
+
+    This function takes the Hovernet JSON nuclei dictionary as input, which is obtained from the modified run_infer.py script.
+    It extracts the centroids and probabilities from the dictionary and returns them as a list of tuples.
+    Each tuple represents a centroid and consists of (X, Y, prob1) for binary classification or (X, Y, prob1, prob2, ..., probN) for multiclass classification.
+
+    :param nuc: The Hovernet JSON nuclei dictionary.
+    :type nuc: Dict[str, Any]
+    :param logger: Optional logger object to log warnings.
+    :type logger: Optional[Logger]
+    :param num_classes: Optional number of classes. Defaults to 2 for binary classification.
+    :type num_classes: Optional[int]
+    :return: The list of centroids with probabilities.
+    :rtype: List[Tuple[int, int, int]]
     """
     centroids_ = []
     for inst in nuc:
         inst_info = nuc[inst]
         inst_centroid = inst_info['centroid']
         inst_prob1 = inst_info['prob1']
         if num_classes > 2:
@@ -58,16 +70,29 @@
             else:
                 centroids_.append((inst_centroid[1], inst_centroid[0], *inst_probs))
     return centroids_
 
 
 def add_probability(graph: pd.DataFrame, hov_json: Dict[str, Any], logger: Optional[Logger] = None, num_classes: Optional[int] = 2) -> pd.DataFrame:
     """
-    Extracts type_prob from json and adds it as column prob1.
-    Makes the join based on id.
+    Adds probability information from the Hovernet JSON nuclei dictionary to the graph DataFrame.
+
+    This function extracts the type probabilities from the Hovernet JSON nuclei dictionary (`hov_json`) and adds them as columns to the `graph` DataFrame.
+    The join between the `graph` DataFrame and the `hov_json` dictionary is based on the 'id' field.
+
+    :param graph: The graph DataFrame containing the nodes.
+    :type graph: pd.DataFrame
+    :param hov_json: The Hovernet JSON nuclei dictionary.
+    :type hov_json: Dict[str, Any]
+    :param logger: Optional logger object to log warnings.
+    :type logger: Optional[Logger]
+    :param num_classes: Optional number of classes. Defaults to 2 for binary classification.
+    :type num_classes: Optional[int]
+    :return: The updated graph DataFrame with probability information.
+    :rtype: pd.DataFrame
     """
     centroids = parse_centroids_probs(hov_json, logger, num_classes)
     centroids = np.array(centroids)
     assert len(centroids) > 0, 'Hov json must contain at least one cell.'
     graph = graph.copy()
     if 'prob1' not in graph.columns:
         n_cols = len(graph.columns)
```

### Comparing `tumourkit-0.7.0/tumourkit/postprocessing/merge_cells.py` & `tumourkit-0.7.1/tumourkit/postprocessing/merge_cells.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,18 +32,20 @@
 
 
 MAX_CELLS = 1500
 
 
 def create_id_map() -> Tuple[Callable[[np.ndarray], np.ndarray], Dict[int, Tuple[int, int]]]:
     """
-    Map index to some function so that difference is unique per pair.
-    Also returns the inverse mapping of the differences and the
-    inverse mapping of the function itself.
+    Creates an index mapping function and its inverse mapping based on a unique difference per pair.
+    The index mapping function `f` is defined as `f(x) = x^5`, ensuring that the difference between function values for each pair of indices is unique.
     Extra information: https://math.stackexchange.com/questions/4565014/injectivity-of-given-integer-function/4567383#4567383
+
+    :return: A tuple containing the index mapping function `f` and the inverse mapping of the differences.
+    :rtype: Tuple[Callable[[np.ndarray], np.ndarray], Dict[int, Tuple[int, int]]]
     """
     def f(x: int) -> int:
         return x**5
     sq_dif = []
     inv_diff_mapping = {}
     for i in range(MAX_CELLS):
         for j in range(i + 1, MAX_CELLS):
@@ -52,16 +54,22 @@
     assert (len(sq_dif) - len(set(sq_dif))) == 0, 'Defined function is not injective.'
 
     vec_mapping = np.vectorize(f)
     return vec_mapping, inv_diff_mapping
 
 
 def get_gradient(png: np.ndarray) -> np.ndarray:
-    """
-    Apply a dilation, subtract the image and remove pixels in background.
+    """"
+    Computes the morphological gradient of a binary image.
+
+    :param png: The binary image for which the gradient is computed.
+    :type png: np.ndarray
+
+    :return: The gradient image.
+    :rtype: np.ndarray
     """
     mask = png.copy()
     mask[mask > 0] = 1
     dilation = skimage.morphology.dilation(png, np.ones((3, 3)))
     grad = dilation - png
     grad_bkgr = grad * mask
     return grad_bkgr
@@ -69,15 +77,25 @@
 
 def merge_cells(
         png: np.ndarray,
         vec_mapping: Callable[[np.ndarray], np.ndarray],
         inv_diff_mapping: Dict[int, Tuple[int, int]]
         ) -> np.ndarray:
     """
-    Merges all the cells that share a frontier of more than 13 pixels.
+    Merges cells in a binary image based on the shared frontier length.
+
+    :param png: The binary image containing cells.
+    :type png: np.ndarray
+    :param vec_mapping: The vectorized mapping function to map indices.
+    :type vec_mapping: Callable[[np.ndarray], np.ndarray]
+    :param inv_diff_mapping: The inverse mapping of differences between indices.
+    :type inv_diff_mapping: Dict[int, Tuple[int, int]]
+
+    :return: The merged binary image.
+    :rtype: np.ndarray
     """
     png_cp = png.copy()
     png_cp = vec_mapping(png_cp)  # Indices mapping
     grad_bkgr = get_gradient(png_cp)  # Morphological gradient
     # Select pairs with long frontier
     unique, counts = np.unique(grad_bkgr, return_counts=True)
     component = [-1 for _ in range(MAX_CELLS)]
@@ -100,15 +118,23 @@
             png[png == pair[0]] = M
             png[png == pair[1]] = M
     return png
 
 
 def remove_lost_ids(png: np.ndarray, csv: pd.DataFrame) -> pd.DataFrame:
     """
-    Removes identifiers in csv that are not in png.
+    Removes identifiers in csv that are not present in the png.
+
+    :param png: The binary image containing cell identifiers.
+    :type png: np.ndarray
+    :param csv: The DataFrame containing cell information with identifiers.
+    :type csv: pd.DataFrame
+
+    :return: The updated DataFrame with removed identifiers.
+    :rtype: pd.DataFrame
     """
     next_ids = set(np.unique(png))
     curr_ids = set(csv.id)
     assert next_ids.difference(curr_ids) == set([0]), "Indices doesn't match"
     remove_ids = curr_ids.difference(next_ids)
     csv.set_index('id', inplace=True)
     csv.drop(remove_ids, axis='index', inplace=True)
```

### Comparing `tumourkit-0.7.0/tumourkit/postprocessing/rswoosh.py` & `tumourkit-0.7.1/tumourkit/postprocessing/rswoosh.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,15 +27,27 @@
 def rswoosh(
         I: List[Cell],
         isEqual: Callable[[Contour, Contour], bool],
         merge: Callable[[Cell, Cell], Cell]
         ) -> List[Cell]:
     """
     Given a list of cells, returns the same list without duplicates.
-    Must provide a function to check equality and another to merge cells.
+
+    The `rswoosh` function takes a list of cells `I`, a function `isEqual` to check equality between contours,
+    and a function `merge` to merge two cells.
+
+    :param I: The list of cells.
+    :type I: List[Cell]
+    :param isEqual: A function to check equality between contours.
+    :type isEqual: Callable[[Contour, Contour], bool]
+    :param merge: A function to merge two cells.
+    :type merge: Callable[[Cell, Cell], Cell]
+
+    :return: The list of cells without duplicates.
+    :rtype: List[Cell]
     """
     out = {}  # Hash Table
     while (len(I) > 0):
         key_r, class_r, r = I.pop()  # O(1)
         exist_equal = False
         for key_s, (class_s, s) in out.items():
             if isEqual(r, s):
```

### Comparing `tumourkit-0.7.0/tumourkit/preprocessing/__init__.py` & `tumourkit-0.7.1/tumourkit/preprocessing/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from .centroids2png import main_with_args as centroids2png
-from .geojson2pngcsv import main_with_args as geojson2pngcsv
-from .hovernet2centroids import main_with_args as hovernet2centroids
-from .hovernet2geojson import main_with_args as hovernet2geojson
-from .pngcsv2centroids import main_with_args as pngcsv2centroids
-from .pngcsv2geojson import main_with_args as pngcsv2geojson
-from .pngcsv2graph import main_with_args as pngcsv2graph
-from .graph2centroids import main_with_args as graph2centroids
-from .centroidspng2csv import main_with_args as centroidspng2csv
-from .png2graph import main_with_args as png2graph
+from .centroids2png import main_with_args as centroids2png_main
+from .geojson2pngcsv import main_with_args as geojson2pngcsv_main
+from .hovernet2centroids import main_with_args as hovernet2centroids_main
+from .hovernet2geojson import main_with_args as hovernet2geojson_main
+from .pngcsv2centroids import main_with_args as pngcsv2centroids_main
+from .pngcsv2geojson import main_with_args as pngcsv2geojson_main
+from .pngcsv2graph import main_with_args as pngcsv2graph_main
+from .graph2centroids import main_with_args as graph2centroids_main
+from .centroidspng2csv import main_with_args as centroidspng2csv_main
+from .png2graph import main_with_args as png2graph_main
```

### Comparing `tumourkit-0.7.0/tumourkit/preprocessing/centroids2png.py` & `tumourkit-0.7.1/tumourkit/preprocessing/centroids2png.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/preprocessing/centroidspng2csv.py` & `tumourkit-0.7.1/tumourkit/preprocessing/centroidspng2csv.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/preprocessing/geojson2pngcsv.py` & `tumourkit-0.7.1/tumourkit/preprocessing/geojson2pngcsv.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/preprocessing/graph2centroids.py` & `tumourkit-0.7.1/tumourkit/preprocessing/graph2centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/preprocessing/hovernet2centroids.py` & `tumourkit-0.7.1/tumourkit/preprocessing/hovernet2centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/preprocessing/hovernet2geojson.py` & `tumourkit-0.7.1/tumourkit/preprocessing/hovernet2geojson.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/preprocessing/png2graph.py` & `tumourkit-0.7.1/tumourkit/preprocessing/png2graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/preprocessing/pngcsv2centroids.py` & `tumourkit-0.7.1/tumourkit/preprocessing/pngcsv2centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/preprocessing/pngcsv2geojson.py` & `tumourkit-0.7.1/tumourkit/preprocessing/pngcsv2geojson.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/preprocessing/pngcsv2graph.py` & `tumourkit-0.7.1/tumourkit/preprocessing/pngcsv2graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,23 +26,35 @@
 import logging
 from tqdm import tqdm
 from ..utils.preprocessing import get_mask, read_labels, parse_path, create_dir, save_graph, get_names, apply_mask, extract_features, add_node, read_image
 
 
 def pngcsv2graph(img: np.ndarray, png: np.ndarray, csv: pd.DataFrame) -> pd.DataFrame:
     """
-    Given original image and pngcsv labels,
-    returns nodes with extracted attributes in a DataFrame.
-    Current attributes are:
-        - X, Y of centroid
+    Converts an original image and PNGCSV labels into a graph representation.
+
+    Given the original image and PNGCSV labels, this function extracts attributes
+    from each label and constructs a graph representation in the form of a DataFrame.
+
+    The current attributes extracted for each label include:
+        - X, Y coordinates of the centroid
         - Area
         - Perimeter
         - Variance
-        - Regularity (not yet)
+        - Regularity (not yet implemented)
         - Histogram (5 bins)
+
+    :param img: The original image.
+    :type img: np.ndarray
+    :param png: The PNGCSV labels.
+    :type png: np.ndarray
+    :param csv: The CSV file containing label information.
+    :type csv: pd.DataFrame
+    :return: The graph representation in the form of a DataFrame.
+    :rtype: pd.DataFrame
     """
     graph = {}
     for idx, cls in csv.itertuples(index=False, name=None):
         mask = get_mask(png, idx)
         msk_img, msk, X, Y = apply_mask(img, mask)
         try:
             feats = extract_features(msk_img, msk)
```

### Comparing `tumourkit-0.7.0/tumourkit/preprocessing/remove_uncertain.py` & `tumourkit-0.7.1/tumourkit/preprocessing/remove_uncertain.py`

 * *Files 23% similar despite different names*

```diff
@@ -23,14 +23,26 @@
 from tqdm import tqdm
 import argparse
 from argparse import Namespace
 from ..utils.preprocessing import get_names, read_gson, save_geojson
 
 
 def process_gson(gson: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
+    """
+    Filters out uncertain classifications from a list of GeoJSON dictionaries.
+
+    Given a list of GeoJSON dictionaries, this function filters out the GeoJSON objects
+    that have an uncertain classification. The uncertain classification is determined
+    based on the 'name' property under the 'classification' key in the GeoJSON dictionary.
+
+    :param gson: The list of GeoJSON dictionaries.
+    :type gson: List[Dict[str, Any]]
+    :return: The filtered list of GeoJSON dictionaries without uncertain classifications.
+    :rtype: List[Dict[str, Any]]
+    """
     return list(filter(lambda x: x['properties']['classification']['name'] != 'uncertain', gson))
 
 
 def main_with_args(args: Namespace) -> None:
     os.makedirs(args.output_dir, exist_ok=True)
     names = get_names(args.input_dir, '.geojson')
     for name in tqdm(names):
```

### Comparing `tumourkit-0.7.0/tumourkit/profiling/cpairs_profile.py` & `tumourkit-0.7.1/tumourkit/profiling/cpairs_profile.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/profiling/rswoosh_profile.py` & `tumourkit-0.7.1/tumourkit/profiling/rswoosh_profile.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/research_pipe.py` & `tumourkit-0.7.1/tumourkit/research_pipe.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,48 +22,66 @@
 import argparse
 from argparse import Namespace
 import logging
 from logging import Logger
 import os
 from .segmentation import hov_train, hov_infer
 from .utils.pipes import check_training, WrongConfigurationError, HovernetNotFoundError, check_void
-from .preprocessing import hovernet2centroids, geojson2pngcsv, pngcsv2centroids
+from .preprocessing import hovernet2centroids_main, geojson2pngcsv_main, pngcsv2centroids_main
 from .segmentation import pngcsv2npy
 from .utils.preprocessing import get_names
 from . import eval_segment
 from .classification import train_xgb, train_gnn
 
 
 def run_preprocessing(args: Namespace, logger: Logger) -> None:
+    """
+    Runs the preprocessing steps.
+
+    :param args: The arguments for running the preprocessing.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
+    """
     if args.experiment == 'cnn-gnn' or args.experiment == 'xgb-gnn' or args.experiment == 'void-gnn':
         check_training(args, logger)
     os.makedirs(args.output_dir, exist_ok=True)
     if args.experiment == 'scaling':
         if args.pretrained_path is None:
             raise WrongConfigurationError('You must provide a path to pretrained Hovernet weights for the scaling experiment.')
     return
 
 
 def hovernet_preproc_with_shape(shape: str, args: Namespace, logger: Logger) -> None:
     """
-    Converts the gson format to the rest of formats.
+    Converts the Hovernet gson format to the rest of formats.
+
+    :param shape: The shape of the Hovernet model.
+    :type shape: str
+
+    :param args: The arguments for running Hovernet preprocessing.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
     """
     real_shape = shape[:-2] if 'FT' in shape else shape
     os.makedirs(os.path.join(args.output_dir, 'hovernet', 'data', real_shape), exist_ok=True)
     for split in ['train', 'validation', 'test']:
         logger.info(f'Parsing {split} split')
         if check_void(os.path.join(args.root_dir, 'data', split, 'png')) or check_void(os.path.join(args.root_dir, 'data', split, 'csv')):
             logger.info('   From geojson to pngcsv.')
             newargs = Namespace(
                 gson_dir=os.path.join(args.root_dir, 'data', split, 'gson'),
                 png_dir=os.path.join(args.root_dir, 'data', split, 'png'),
                 csv_dir=os.path.join(args.root_dir, 'data', split, 'csv'),
                 num_classes=args.num_classes,
             )
-            geojson2pngcsv(newargs)
+            geojson2pngcsv_main(newargs)
         os.makedirs(os.path.join(args.output_dir, 'hovernet', 'data', real_shape, split), exist_ok=True)
         os.makedirs(os.path.join(args.output_dir, 'hovernet', 'data', real_shape, split, 'npy'), exist_ok=True)
         if check_void(os.path.join(args.output_dir, 'hovernet', 'data', real_shape, split, 'npy')):
             newargs = Namespace(
                 orig_dir=os.path.join(args.root_dir, 'data', 'orig'),
                 png_dir=os.path.join(args.root_dir, 'data', split, 'png'),
                 csv_dir=os.path.join(args.root_dir, 'data', split, 'csv'),
@@ -72,14 +90,26 @@
                 shape=real_shape
             )
             pngcsv2npy(newargs)
     return
 
 
 def train_hovernet_with_shape(shape: str, args: Namespace, logger: Logger) -> None:
+    """
+    Performs Hovernet preprocessing and training with the specified shape.
+
+    :param shape: The shape of the Hovernet model.
+    :type shape: str
+
+    :param args: The arguments for Hovernet preprocessing and training.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
+    """
     logger.info(f'Starting hovernet preprocessing of {shape}.')
     hovernet_preproc_with_shape(shape, args, logger)
     logger.info(f'Starting training of {shape}.')
     os.makedirs(os.path.join(args.output_dir, 'hovernet', 'weights', shape), exist_ok=True)
     real_shape = shape[:-2] if 'FT' in shape else shape
     newargs = Namespace(
         gpu=args.gpu, view=None, save_name=None,
@@ -90,14 +120,26 @@
         shape=real_shape,
         num_classes=args.num_classes,
     )
     hov_train(newargs)
 
 
 def infer_hovernet_with_shape(shape: str, args: Namespace, logger: Logger) -> None:
+    """
+    Performs inference with the specified Hovernet model shape.
+
+    :param shape: The shape of the Hovernet model.
+    :type shape: str
+
+    :param args: The arguments for Hovernet inference.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
+    """
     logger.info(f'Starting inference of {shape}.')
     newargs = {
         'nr_types': str(args.num_classes + 1),
         'type_info_path': os.path.join(args.root_dir, 'weights', 'segmentation', 'hovernet', 'type_info.json'),
         'gpu': args.gpu,
         'nr_inference_workers': '0',
         'model_path': os.path.join(args.output_dir, 'hovernet', 'weights', shape, '01', 'net_epoch=50.tar'),
@@ -117,24 +159,33 @@
         'mem_usage': '0.2'
     }
     hov_infer(newargs, newsubargs, 'tile')
 
 
 def run_postprocessing_with_shape(shape: str, args: Namespace, logger: Logger) -> None:
     """
-    Converts the gson format to the rest of formats.
+    Performs post-processing after Hovernet training with the specified shape.
+
+    :param shape: The shape of the Hovernet model.
+    :type shape: str
+
+    :param args: The arguments for post-processing.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
     """
     logger.info('Extracting Hovernet centroids from training output.')
     if not os.path.isdir(os.path.join(args.output_dir, 'hovernet', 'output', shape, 'json')):
         raise HovernetNotFoundError('Please, train again or extract hovernet outputs.')
     newargs = Namespace(
         json_dir=os.path.join(args.output_dir, 'hovernet', 'output', shape, 'json'),
         output_path=os.path.join(args.output_dir, 'hovernet', 'output', shape, 'centroids_hov'),
     )
-    hovernet2centroids(newargs)
+    hovernet2centroids_main(newargs)
     for split in ['train', 'validation', 'test']:
         if check_void(os.path.join(args.root_dir, 'data', split, 'names.txt')):
             logger.info(f'Preprocessing split {split}.')
             split_names = get_names(os.path.join(args.root_dir, 'data', split, 'gson'), '.geojson')
             with open(os.path.join(args.root_dir, 'data', split, 'names.txt'), 'w') as f:
                 for name in split_names:
                     print(name, file=f)
@@ -142,26 +193,38 @@
             logger.info('   From geojson to pngcsv.')
             newargs = Namespace(
                 gson_dir=os.path.join(args.root_dir, 'data', split, 'gson'),
                 png_dir=os.path.join(args.root_dir, 'data', split, 'png'),
                 csv_dir=os.path.join(args.root_dir, 'data', split, 'csv'),
                 num_classes=args.num_classes,
             )
-            geojson2pngcsv(newargs)
+            geojson2pngcsv_main(newargs)
         if check_void(os.path.join(args.root_dir, 'data', split, 'centroids')):
             logger.info('   Extracting centroids from GT.')
             newargs = Namespace(
                 png_dir=os.path.join(args.root_dir, 'data', split, 'png'),
                 csv_dir=os.path.join(args.root_dir, 'data', split, 'csv'),
                 output_path=os.path.join(args.root_dir, 'data', split, 'centroids')
             )
-            pngcsv2centroids(newargs)
+            pngcsv2centroids_main(newargs)
 
 
 def evaluate_hovernet_with_shape(shape: str, args: Namespace, logger: Logger) -> None:
+    """
+    Performs evaluation of Hovernet outputs with the specified shape.
+
+    :param shape: The shape of the Hovernet model.
+    :type shape: str
+
+    :param args: The arguments for evaluation.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
+    """
     logger.info(f'Starting evaluation of {shape}.')
     os.makedirs(os.path.join(args.output_dir, 'hovernet', 'output', shape, 'results'), exist_ok=True)
     for split in ['train', 'validation', 'test']:
         logger.info(f'    Evaluating {split} split')
         newargs = Namespace(
             names=os.path.join(args.root_dir, 'data', split, 'names.txt'),
             gt_path=os.path.join(args.root_dir, 'data', split, 'centroids'),
@@ -170,14 +233,29 @@
             debug_path=None,
             num_classes=args.num_classes
         )
         eval_segment(newargs, logger)
 
 
 def run_scaling(args: Namespace, logger: Logger) -> None:
+    """
+    Runs the scaling experiment for Hovernet.
+
+    This function performs the following steps:
+        1. Trains Hovernet models with different shapes: '270', '270FT', '518', '518FT'.
+        2. Performs inference with the trained models on the input data.
+        3. Runs post-processing on the Hovernet output.
+        4. Evaluates the Hovernet output using the ground truth data.
+
+    :param args: The arguments for the scaling experiment.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
+    """
     os.makedirs(os.path.join(args.output_dir, 'hovernet'), exist_ok=True)
     os.makedirs(os.path.join(args.output_dir, 'hovernet', 'weights'), exist_ok=True)
     os.makedirs(os.path.join(args.output_dir, 'hovernet', 'data'), exist_ok=True)
     train_hovernet_with_shape('270', args, logger)
     train_hovernet_with_shape('270FT', args, logger)
     train_hovernet_with_shape('518', args, logger)
     train_hovernet_with_shape('518FT', args, logger)
@@ -196,14 +274,28 @@
     evaluate_hovernet_with_shape('270', args, logger)
     evaluate_hovernet_with_shape('270FT', args, logger)
     evaluate_hovernet_with_shape('518', args, logger)
     evaluate_hovernet_with_shape('518FT', args, logger)
 
 
 def run_xgb(args: Namespace, logger: Logger) -> None:
+    """
+    Runs the XGBoost training and evaluation.
+
+    This function performs the following steps:
+        1. Moves the graph files into a single folder for training and validation.
+        2. Trains XGBoost using the merged graph files.
+        3. Saves the cross-validation results.
+
+    :param args: The arguments for the XGBoost training.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
+    """
     logger.info('Moving graphs files into one single folder.')
     all_graphs_dir = os.path.join(args.root_dir, 'data', 'train_validation', 'graphs', 'preds')
     os.makedirs(all_graphs_dir, exist_ok=True)
     tr_graphs_dir = os.path.join(args.root_dir, 'data', 'train', 'graphs', 'preds')
     val_graphs_dir = os.path.join(args.root_dir, 'data', 'validation', 'graphs', 'preds')
     files = [os.path.join(tr_graphs_dir, f) for f in os.listdir(tr_graphs_dir)] + \
             [os.path.join(val_graphs_dir, f) for f in os.listdir(val_graphs_dir)]
@@ -221,14 +313,28 @@
         save_name=os.path.join(args.output_dir, 'xgb', 'cv_results'),
         num_classes=args.num_classes,
     )
     train_xgb(newargs, logger)
 
 
 def run_void(args: Namespace, logger: Logger) -> None:
+    """
+    Runs the training of GNN models without prior and morphological features.
+
+    This function performs the following steps:
+        1. Trains a GNN model without prior.
+        2. Trains a GNN model without morphological features.
+        3. Trains a void GNN model (without prior and morphological features).
+
+    :param args: The arguments for the GNN training.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
+    """
     logger.info('Training GNN without prior.')
     newargs = Namespace(
         train_node_dir=os.path.join(args.root_dir, 'data', 'train', 'graphs', 'preds'),
         validation_node_dir=os.path.join(args.root_dir, 'data', 'validation', 'graphs', 'preds'),
         test_node_dir=os.path.join(args.root_dir, 'data', 'test', 'graphs', 'preds'),
         log_dir=os.path.join(args.output_dir, 'gnn_no_prior_logs'),
         early_stopping_rounds=10,
```

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/evaluate.py` & `tumourkit-0.7.1/tumourkit/segmentation/evaluate.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,17 +41,27 @@
 
 
 def get_confusion_matrix(
         gt_centroids: List[Tuple[int, int, int]],
         pred_centroids: List[Tuple[int, int, int]]
         ) -> np.ndarray:
     """
+    Calculates the confusion matrix based on the ground truth and predicted centroids.
+
     Each centroid is represented by a 3-tuple with (X, Y, class).
-    Matrix has (N+1)x(N+1) entries, one more for background when no match is found.
-    N is the maximum value encountered for class.
+    The confusion matrix has (N+1)x(N+1) entries, where N is the maximum value encountered for the class.
+    There is one additional entry for the background class when no match is found.
+
+    :param gt_centroids: The ground truth centroids represented as a list of 3-tuples (X, Y, class).
+    :type gt_centroids: List[Tuple[int, int, int]]
+    :param pred_centroids: The predicted centroids represented as a list of 3-tuples (X, Y, class).
+    :type pred_centroids: List[Tuple[int, int, int]]
+
+    :return: The confusion matrix.
+    :rtype: np.ndarray
     """
     if len(gt_centroids) == 0 and len(pred_centroids) == 0:
         return np.array([[0]])
     if len(gt_centroids) == 0:
         N = np.max(pred_centroids[:, 2])
         M = np.zeros((N + 1, N + 1))
         classes, freqs = np.unique(pred_centroids[:, 2], return_counts=True)
@@ -88,18 +98,27 @@
 
 
 def get_pairs(
         gt_centroids: List[Tuple[int, int, int]],
         pred_centroids: List[Tuple[int, int, int]]
         ) -> Tuple[np.ndarray, np.ndarray]:
     """
+    Retrieves true and predicted labels ordered by their correspondences.
+
     Each centroid is represented by a 3-tuple with (X, Y, class).
-    Class is 1=non-tumour, 2=tumour.
-    Returns true and predicted labels ordered by their correspondences.
-    Returned labels start at 0.
+    The class is represented as 1=non-tumour, 2=tumour.
+    The returned labels are ordered starting from 0.
+
+    :param gt_centroids: The ground truth centroids represented as a list of 3-tuples (X, Y, class).
+    :type gt_centroids: List[Tuple[int, int, int]]
+    :param pred_centroids: The predicted centroids represented as a list of 3-tuples (X, Y, class).
+    :type pred_centroids: List[Tuple[int, int, int]]
+
+    :return: A tuple containing the true labels and predicted labels ordered by their correspondences.
+    :rtype: Tuple[np.ndarray, np.ndarray]
     """
     if len(gt_centroids) == 0:
         return None, None
 
     gt_tree = generate_tree(gt_centroids[:, :2])
     pred_tree = generate_tree(pred_centroids[:, :2])
     true_labels, pred_labels = [], []
@@ -110,16 +129,23 @@
             true_labels.append(point[2] - 1)
             pred_labels.append(closest[2] - 1)
     return np.array(true_labels), np.array(pred_labels)
 
 
 def compute_f1_score_from_matrix(conf_mat: np.ndarray, cls: int) -> float:
     """
-    Returns f1 score of given class against the rest.
-    If no positive or predictive positive classes are found, None is returned.
+    Computes the F1 score of a given class against the rest.
+
+    :param conf_mat: The confusion matrix.
+    :type conf_mat: np.ndarray
+    :param cls: The class for which to compute the F1 score.
+    :type cls: int
+
+    :return: The F1 score of the given class against the rest.
+    :rtype: float
     """
     if cls == 0:
         return None
     TP = conf_mat[cls, cls]
     PP = conf_mat[:, cls].sum()
     if PP == 0:
         return None
@@ -131,16 +157,24 @@
     if TP == 0:
         return 0
     return 2 * precision * recall / (precision + recall)
 
 
 def compute_metrics_from_matrix(conf_mat: np.ndarray) -> Tuple[float, float, float, float]:
     """
-    Given confusion matrix,
-    returns F1 score, Accuracy, ROC AUC and percentage error.
+    Computes various evaluation metrics from a confusion matrix.
+
+    Given a confusion matrix, this function calculates the F1 score, accuracy,
+    ROC AUC, and percentage error.
+
+    :param conf_mat: The confusion matrix.
+    :type conf_mat: np.ndarray
+
+    :return: A tuple containing the F1 score, accuracy, ROC AUC, and percentage error.
+    :rtype: Tuple[float, float, float, float]
     """
     total = np.sum(conf_mat)
     acc = np.matrix.trace(conf_mat) / total
     n_classes = len(conf_mat)
     macro, weighted = 0, 0
     real_n_classes = n_classes
     adjust_weighted = 1
@@ -159,14 +193,22 @@
 
 
 def add_matrices(A: np.ndarray, B: np.ndarray) -> np.ndarray:
     """
     Adds two matrices even if their shapes are different.
     If B is bigger than A, A is enlarged with zeros.
     And vice versa.
+
+    :param A: The first matrix.
+    :type A: np.ndarray
+    :param B: The second matrix.
+    :type B: np.ndarray
+
+    :return: The sum of the two matrices.
+    :rtype: np.ndarray
     """
     if A.shape == B.shape:
         return A + B
     n, m = A.shape[0], B.shape[0]
     if m > n:
         res = np.zeros((m, m))
         res[:n, :n] += A
@@ -179,27 +221,36 @@
 
 
 def save_csv(
         metrics: Dict[str, List[float]],
         save_path: str
         ) -> None:
     """
-    Saves metrics in csv format for later use.
-    Columns depend on dictionary keys.
+    Saves metrics in CSV format for later use.
+
+    :param metrics: The metrics dictionary containing the data to be saved.
+    :type metrics: Dict[str, List[float]]
+    :param save_path: The file path where the CSV file will be saved.
+    :type save_path: str
     """
     metrics_df = pd.DataFrame(metrics)
     metrics_df.to_csv(save_path + '.csv', index=False)
 
 
 def save_debug_matrix(
         mat: np.ndarray,
         save_path: str
         ) -> None:
     """
-    Saves confusion matrices for debug purposes.
+    Saves a confusion matrix in CSV format for debug purposes.
+
+    :param mat: The confusion matrix to be saved.
+    :type mat: np.ndarray
+    :param save_path: The file path where the CSV file will be saved.
+    :type save_path: str
     """
     conf_mat_df = pd.DataFrame(mat)
     conf_mat_df.to_csv(save_path + '.csv')
 
 
 def _create_parser():
     parser = argparse.ArgumentParser()
```

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/config.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/config.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/dataloader/augs.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/dataloader/augs.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/dataloader/infer_loader.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/dataloader/infer_loader.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/dataloader/train_loader.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/dataloader/train_loader.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/extract_patches.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/extract_patches.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/infer/base.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/infer/base.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/infer/tile.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/infer/tile.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/infer/wsi.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/infer/wsi.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/metrics/stats_utils.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/metrics/stats_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/patch_extractor.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/patch_extractor.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/utils.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/viz_utils.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/viz_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/wsi_handler.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/misc/wsi_handler.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/opt.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/opt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/targets.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/targets.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/utils.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/models/hovernet/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_infer.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_infer.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/engine.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/engine.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/utils.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/run_utils/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/segmentation/hovernet/train.py` & `tumourkit-0.7.1/tumourkit/segmentation/hovernet/train.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/train_pipe.py` & `tumourkit-0.7.1/tumourkit/train_pipe.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,54 +16,75 @@
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Contact information: joseperez2000@hotmail.es
 """
 import argparse
 from argparse import Namespace
-from .preprocessing import geojson2pngcsv, pngcsv2graph, hovernet2geojson, pngcsv2centroids
+from .preprocessing import geojson2pngcsv_main, pngcsv2graph_main, hovernet2geojson_main, pngcsv2centroids_main
 from .segmentation import pngcsv2npy
 import os
 import logging
 from logging import Logger
 from .segmentation import hov_train, hov_infer
 from .utils.preprocessing import get_names
 import shutil
-from .postprocessing import join_graph_gt, join_hovprob_graph
+from .postprocessing import join_graph_gt_main, join_hovprob_graph_main
 from .classification import train_gnn
 
 
 def run_preproc_pipe(args: Namespace, logger: Logger) -> None:
     """
-    Converts the gson format to the rest of formats.
+    Runs the preprocessing pipeline to convert the gson format to other formats.
+
+    This function performs the following steps:
+        1. Converts the geojson files to pngcsv format.
+        2. Converts the pngcsv files to npy format.
+
+    :param args: The arguments for the preprocessing pipeline.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
     """
     for split in ['train', 'validation', 'test']:
         logger.info(f'Parsing {split} split')
         newargs = Namespace(
             gson_dir=os.path.join(args.root_dir, 'data', split, 'gson'),
             png_dir=os.path.join(args.root_dir, 'data', split, 'png'),
             csv_dir=os.path.join(args.root_dir, 'data', split, 'csv'),
             num_classes=args.num_classes,
         )
-        geojson2pngcsv(newargs)
+        geojson2pngcsv_main(newargs)
         newargs = Namespace(
             orig_dir=os.path.join(args.root_dir, 'data', 'orig'),
             png_dir=os.path.join(args.root_dir, 'data', split, 'png'),
             csv_dir=os.path.join(args.root_dir, 'data', split, 'csv'),
             out_dir=os.path.join(args.root_dir, 'data', split, 'npy'),
             save_example=False, use_labels=True, split=False,
             shape='518'
         )
         pngcsv2npy(newargs)
     return
 
 
 def run_hov_pipe(args: Namespace, logger: Logger) -> None:
     """
-    Trains hovernet and predicts cell contours on json format.
+    Trains Hovernet and predicts cell contours in json format.
+
+    This function performs the following steps:
+        1. Trains Hovernet on the training data.
+        2. Performs inference using the trained Hovernet model on the input images.
+        3. Saves the predicted cell contours in json format.
+
+    :param args: The arguments for the Hovernet pipeline.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
     """
     logger.info('Starting training.')
     newargs = Namespace(
         gpu=args.gpu, view=None, save_name=None,
         log_dir=os.path.join(args.root_dir, 'weights', 'segmentation', 'hovernet'),
         train_dir=os.path.join(args.root_dir, 'data', 'train', 'npy'),
         valid_dir=os.path.join(args.root_dir, 'data', 'validation', 'npy'),
@@ -95,15 +116,30 @@
     }
     hov_infer(newargs, newsubargs, 'tile')
     return
 
 
 def run_postproc_pipe(args: Namespace, logger: Logger) -> None:
     """
-    Converts the json format to the graph format containing GT and preds.
+    Converts the json format to the graph format containing ground truth (GT) and predictions.
+
+    This function performs the following steps:
+        1. Moves json files to their corresponding folders based on the split.
+        2. Converts the json format to geojson format.
+        3. Converts the geojson format to pngcsv format.
+        4. Converts the pngcsv format to nodes.csv format.
+        5. Extracts centroids from ground truth (GT) data.
+        6. Adds GT labels to the nodes.csv file.
+        7. Adds Hovernet predictions to the nodes.csv file.
+
+    :param args: The arguments for the post-processing pipeline.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
     """
     logger.info('Moving json files to corresponding folders.')
     tr_files = set(get_names(os.path.join(args.root_dir, 'data', 'train', 'gson'), '.geojson'))
     val_files = set(get_names(os.path.join(args.root_dir, 'data', 'validation', 'gson'), '.geojson'))
     ts_files = set(get_names(os.path.join(args.root_dir, 'data', 'test', 'gson'), '.geojson'))
     json_files = set(get_names(os.path.join(args.root_dir, 'data', 'tmp_hov', 'json'), '.json'))
     for folder_name, split_files in zip(['train', 'validation', 'test'], [tr_files, val_files, ts_files]):
@@ -116,60 +152,70 @@
         logger.info(f'Parsing {split} split')
         logger.info('   From json to geojson.')
         newargs = Namespace(
             json_dir=os.path.join(args.root_dir, 'data', split, 'json'),
             gson_dir=os.path.join(args.root_dir, 'data', split, 'gson_hov'),
             num_classes=args.num_classes
         )
-        hovernet2geojson(newargs)
+        hovernet2geojson_main(newargs)
         logger.info('   From geojson to pngcsv.')
         newargs = Namespace(
             gson_dir=os.path.join(args.root_dir, 'data', split, 'gson_hov'),
             png_dir=os.path.join(args.root_dir, 'data', split, 'png_hov'),
             csv_dir=os.path.join(args.root_dir, 'data', split, 'csv_hov'),
             num_classes=args.num_classes,
         )
-        geojson2pngcsv(newargs)
+        geojson2pngcsv_main(newargs)
         logger.info('   From pngcsv to nodes.csv.')
         newargs = Namespace(
             png_dir=os.path.join(args.root_dir, 'data', split, 'png_hov'),
             csv_dir=os.path.join(args.root_dir, 'data', split, 'csv_hov'),
             orig_dir=os.path.join(args.root_dir, 'data', 'orig'),
             output_path=os.path.join(args.root_dir, 'data', split, 'graphs', 'raw'),
             num_workers=args.num_workers
         )
-        pngcsv2graph(newargs)
+        pngcsv2graph_main(newargs)
         logger.info('   Extracting centroids from GT.')
         newargs = Namespace(
             png_dir=os.path.join(args.root_dir, 'data', split, 'png'),
             csv_dir=os.path.join(args.root_dir, 'data', split, 'csv'),
             output_path=os.path.join(args.root_dir, 'data', split, 'centroids')
         )
-        pngcsv2centroids(newargs)
+        pngcsv2centroids_main(newargs)
         logger.info('   Adding GT labels to .nodes.csv.')
         newargs = Namespace(
             graph_dir=os.path.join(args.root_dir, 'data', split, 'graphs', 'raw'),
             centroids_dir=os.path.join(args.root_dir, 'data', split, 'centroids'),
             output_dir=os.path.join(args.root_dir, 'data', split, 'graphs', 'GT')
         )
-        join_graph_gt(newargs)
+        join_graph_gt_main(newargs)
         logger.info('   Adding hovernet predictions to .nodes.csv.')
         newargs = Namespace(
             json_dir=os.path.join(args.root_dir, 'data', split, 'json'),
             graph_dir=os.path.join(args.root_dir, 'data', split, 'graphs', 'GT'),
             output_dir=os.path.join(args.root_dir, 'data', split, 'graphs', 'preds'),
             num_classes=args.num_classes,
         )
-        join_hovprob_graph(newargs, logger)
+        join_hovprob_graph_main(newargs, logger)
     return
 
 
 def run_graph_pipe(args: Namespace, logger: Logger) -> None:
     """
     Trains the graph models.
+
+    This function trains the graph models using the following steps:
+        1. Trains the GCN (Graph Convolutional Network) model.
+        2. Trains the GAT (Graph Attention Network) model.
+
+    :param args: The arguments for the graph pipeline.
+    :type args: Namespace
+
+    :param logger: The logger object used for logging messages.
+    :type logger: Logger
     """
     newargs = Namespace(
         train_node_dir=os.path.join(args.root_dir, 'data', 'train', 'graphs', 'preds'),
         validation_node_dir=os.path.join(args.root_dir, 'data', 'validation', 'graphs', 'preds'),
         test_node_dir=os.path.join(args.root_dir, 'data', 'test', 'graphs', 'preds'),
         log_dir=os.path.join(args.root_dir, 'gnn_logs'),
         early_stopping_rounds=10,
@@ -215,16 +261,14 @@
     parser.add_argument('--gpu', type=str, default='0')
     parser.add_argument('--num-workers', type=int, default=0)
     parser.add_argument('--num-classes', type=int, default=2, help='Number of classes to consider for classification (background not included).')
     return parser
 
 
 def main():
-    # TODO: Run each subpipe independently and measure time and memory requirements.
-
     parser = _create_parser()
     args = parser.parse_args()
 
     logger = logging.getLogger('train_pipe')
     logger.setLevel(logging.DEBUG)
     ch = logging.StreamHandler()
     ch.setLevel(logging.DEBUG)
```

### Comparing `tumourkit-0.7.0/tumourkit/utils/calibration_error.py` & `tumourkit-0.7.1/tumourkit/utils/calibration_error.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/utils/classification.py` & `tumourkit-0.7.1/tumourkit/utils/classification.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/utils/folder2txt.py` & `tumourkit-0.7.1/tumourkit/utils/folder2txt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/utils/nearest.py` & `tumourkit-0.7.1/tumourkit/utils/nearest.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/utils/postprocessing.py` & `tumourkit-0.7.1/tumourkit/utils/postprocessing.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/utils/preprocessing.py` & `tumourkit-0.7.1/tumourkit/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit/utils/read_nodes.py` & `tumourkit-0.7.1/tumourkit/utils/read_nodes.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit.egg-info/PKG-INFO` & `tumourkit-0.7.1/tumourkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumourkit
-Version: 0.7.0
+Version: 0.7.1
 Summary: A SDK for tumour study
 Author-email: Jose Pérez Cano <joseperez2000@hotmail.es>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `tumourkit-0.7.0/tumourkit.egg-info/SOURCES.txt` & `tumourkit-0.7.1/tumourkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit.egg-info/entry_points.txt` & `tumourkit-0.7.1/tumourkit.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `tumourkit-0.7.0/tumourkit.egg-info/requires.txt` & `tumourkit-0.7.1/tumourkit.egg-info/requires.txt`

 * *Files identical despite different names*

