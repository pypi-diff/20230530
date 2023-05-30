# Comparing `tmp/wellmet-0.9.5.tar.gz` & `tmp/wellmet-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wellmet-0.9.5.tar", last modified: Mon May 29 17:59:34 2023, max compression
+gzip compressed data, was "wellmet-0.9.6.tar", last modified: Tue May 30 18:18:59 2023, max compression
```

## Comparing `wellmet-0.9.5.tar` & `wellmet-0.9.6.tar`

### file list

```diff
@@ -1,75 +1,70 @@
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-29 17:59:34.130547 wellmet-0.9.5/
--rw-r--r--   0 user         (0) root         (0)     1093 2022-04-30 17:02:31.025952 wellmet-0.9.5/LICENSE
--rw-r--r--   0 user         (0) root         (0)     5007 2023-05-29 17:59:34.131072 wellmet-0.9.5/PKG-INFO
--rw-r--r--   0 user         (0) root         (0)     4337 2023-05-29 17:59:06.025952 wellmet-0.9.5/README.md
--rw-r--r--   0 user         (0) root         (0)      899 2023-05-29 13:26:34.025952 wellmet-0.9.5/pyproject.toml
--rw-r--r--   0 user         (0) root         (0)      794 2023-05-29 17:59:34.138936 wellmet-0.9.5/setup.cfg
--rw-r--r--   0 user         (0) root         (0)       54 2023-05-29 15:46:17.026214 wellmet-0.9.5/setup.py
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-29 17:59:33.855375 wellmet-0.9.5/wellmet/
--rw-r--r--   0 user         (0) root         (0)    30048 2023-05-28 14:15:30.026214 wellmet-0.9.5/wellmet/IS_stat.py
--rw-r--r--   0 user         (0) root         (0)       86 2023-05-28 15:34:51.026214 wellmet-0.9.5/wellmet/__init__.py
--rw-r--r--   0 user         (0) root         (0)       72 2022-04-30 16:53:41.026476 wellmet-0.9.5/wellmet/__main__.py
--rw-r--r--   0 user         (0) root         (0)    11243 2023-05-28 14:15:30.026476 wellmet-0.9.5/wellmet/candybox.py
--rw-r--r--   0 user         (0) root         (0)     6756 2023-05-28 14:15:30.026476 wellmet-0.9.5/wellmet/candynodes.py
--rw-r--r--   0 user         (0) root         (0)    50875 2023-05-29 17:12:11.026738 wellmet-0.9.5/wellmet/convex_hull.py
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-29 17:59:33.939524 wellmet-0.9.5/wellmet/dicebox/
--rw-r--r--   0 user         (0) root         (0)    14745 2023-05-29 17:12:04.028573 wellmet-0.9.5/wellmet/dicebox/__circumtri.py
--rw-r--r--   0 user         (0) root         (0)        6 2022-04-30 16:53:41.028573 wellmet-0.9.5/wellmet/dicebox/__init__.py
--rw-r--r--   0 user         (0) root         (0)    17010 2023-05-29 17:12:04.028835 wellmet-0.9.5/wellmet/dicebox/_circumtri.py
--rw-r--r--   0 user         (0) root         (0)     7865 2023-05-29 17:12:04.028835 wellmet-0.9.5/wellmet/dicebox/_exploration.py
--rw-r--r--   0 user         (0) root         (0)    73380 2023-01-15 11:48:48.028835 wellmet-0.9.5/wellmet/dicebox/censoring.py
--rw-r--r--   0 user         (0) root         (0)    33598 2023-05-29 17:12:04.029098 wellmet-0.9.5/wellmet/dicebox/circumtri.py
--rw-r--r--   0 user         (0) root         (0)   100174 2023-01-15 11:50:00.029098 wellmet-0.9.5/wellmet/dicebox/goal.py
--rw-r--r--   0 user         (0) root         (0)    36893 2023-01-15 11:50:38.026738 wellmet-0.9.5/wellmet/estimation.py
--rw-r--r--   0 user         (0) root         (0)    52580 2023-01-15 11:51:29.026738 wellmet-0.9.5/wellmet/f_models.py
--rw-r--r--   0 user         (0) root         (0)    42237 2023-03-12 14:45:57.027001 wellmet-0.9.5/wellmet/g_models.py
--rw-r--r--   0 user         (0) root         (0)    21042 2023-05-28 14:15:30.027001 wellmet-0.9.5/wellmet/ghull.py
--rw-r--r--   0 user         (0) root         (0)     3234 2022-05-13 19:15:46.027001 wellmet-0.9.5/wellmet/misc.py
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-29 17:59:34.009699 wellmet-0.9.5/wellmet/mplot/
--rw-r--r--   0 user         (0) root         (0)     1407 2022-04-30 16:53:41.029098 wellmet-0.9.5/wellmet/mplot/__init__.py
--rw-r--r--   0 user         (0) root         (0)     9741 2022-04-30 16:53:41.029360 wellmet-0.9.5/wellmet/mplot/_axes3d.py
--rw-r--r--   0 user         (0) root         (0)      714 2022-04-30 16:53:41.029360 wellmet-0.9.5/wellmet/mplot/_axis3d_margins_patch.py
--rw-r--r--   0 user         (0) root         (0)    23492 2023-03-30 13:18:09.029360 wellmet-0.9.5/wellmet/mplot/mart.py
--rw-r--r--   0 user         (0) root         (0)    13647 2023-01-15 11:54:22.029622 wellmet-0.9.5/wellmet/mplot/mart3d.py
--rw-r--r--   0 user         (0) root         (0)    26324 2023-05-29 17:11:54.029622 wellmet-0.9.5/wellmet/mplot/maxes.py
--rw-r--r--   0 user         (0) root         (0)     5577 2022-04-30 16:53:41.029622 wellmet-0.9.5/wellmet/mplot/maxes3d.py
--rw-r--r--   0 user         (0) root         (0)    17778 2023-05-29 17:11:54.029622 wellmet-0.9.5/wellmet/mplot/mfigs.py
--rw-r--r--   0 user         (0) root         (0)    10463 2023-02-02 13:58:18.029884 wellmet-0.9.5/wellmet/mplot/mgraph.py
--rw-r--r--   0 user         (0) root         (0)     1132 2022-04-30 16:53:41.029884 wellmet-0.9.5/wellmet/mplot/misc.py
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-29 17:59:34.087293 wellmet-0.9.5/wellmet/qt_gui/
--rw-r--r--   0 user         (0) root         (0)        6 2022-04-30 16:53:41.029884 wellmet-0.9.5/wellmet/qt_gui/__init__.py
--rw-r--r--   0 user         (0) root         (0)    44438 2023-01-15 11:54:47.030146 wellmet-0.9.5/wellmet/qt_gui/gl_plot.py
--rw-r--r--   0 user         (0) root         (0)      348 2022-10-16 03:13:28.030146 wellmet-0.9.5/wellmet/qt_gui/gui_startup.py
--rw-r--r--   0 user         (0) root         (0)     1970 2022-10-07 12:30:43.030146 wellmet-0.9.5/wellmet/qt_gui/qt_box_functions.py
--rw-r--r--   0 user         (0) root         (0)    26239 2023-05-28 15:18:02.030408 wellmet-0.9.5/wellmet/qt_gui/qt_dicebox.py
--rw-r--r--   0 user         (0) root         (0)    35342 2023-01-17 14:19:12.030408 wellmet-0.9.5/wellmet/qt_gui/qt_graph_widgets.py
--rw-r--r--   0 user         (0) root         (0)    24326 2023-05-28 14:20:54.030408 wellmet-0.9.5/wellmet/qt_gui/qt_gui.py
--rw-r--r--   0 user         (0) root         (0)    38391 2022-12-21 15:13:48.030671 wellmet-0.9.5/wellmet/qt_gui/qt_pairwise.py
--rw-r--r--   0 user         (0) root         (0)    99810 2023-05-29 17:13:09.030671 wellmet-0.9.5/wellmet/qt_gui/qt_plot.py
--rw-r--r--   0 user         (0) root         (0)     3244 2023-01-10 05:21:15.030671 wellmet-0.9.5/wellmet/qt_gui/qt_testcases.py
--rw-r--r--   0 user         (0) root         (0)    56858 2022-11-29 15:50:00.030933 wellmet-0.9.5/wellmet/qt_gui/qt_voronoi.py
--rw-r--r--   0 user         (0) root         (0)    10956 2023-01-15 11:55:28.027263 wellmet-0.9.5/wellmet/reader.py
--rw-r--r--   0 user         (0) root         (0)     4416 2023-01-15 11:56:01.027263 wellmet-0.9.5/wellmet/samplebox.py
--rw-r--r--   0 user         (0) root         (0)     6558 2022-04-30 16:53:42.027263 wellmet-0.9.5/wellmet/sball.py
--rw-r--r--   0 user         (0) root         (0)     6739 2023-05-29 17:11:42.027263 wellmet-0.9.5/wellmet/schemes.py
--rw-r--r--   0 user         (0) root         (0)     8309 2023-05-28 14:15:30.027525 wellmet-0.9.5/wellmet/shell.py
--rw-r--r--   0 user         (0) root         (0)   134283 2023-05-29 17:11:31.027525 wellmet-0.9.5/wellmet/simplex.py
--rw-r--r--   0 user         (0) root         (0)    13090 2023-05-28 14:15:30.027787 wellmet-0.9.5/wellmet/spring.py
--rw-r--r--   0 user         (0) root         (0)    10953 2022-04-30 16:53:42.027787 wellmet-0.9.5/wellmet/stm_df.py
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-29 17:59:34.123731 wellmet-0.9.5/wellmet/testcases/
--rw-r--r--   0 user         (0) root         (0)        0 2023-05-28 13:48:40.030933 wellmet-0.9.5/wellmet/testcases/__init__.py
--rw-r--r--   0 user         (0) root         (0)     8987 2023-03-12 15:00:08.030933 wellmet-0.9.5/wellmet/testcases/gaussian_2D.py
--rw-r--r--   0 user         (0) root         (0)     8183 2023-05-28 14:14:11.030933 wellmet-0.9.5/wellmet/testcases/testcases_2D.py
--rw-r--r--   0 user         (0) root         (0)     3741 2023-02-24 08:01:44.031195 wellmet-0.9.5/wellmet/testcases/testcases_2D_papers.py
--rw-r--r--   0 user         (0) root         (0)     2572 2023-01-14 08:20:10.031195 wellmet-0.9.5/wellmet/testcases/testcases_nD.py
--rw-r--r--   0 user         (0) root         (0)    11998 2023-01-30 12:29:31.031195 wellmet-0.9.5/wellmet/testcases/testcases_nD_papers.py
--rw-r--r--   0 user         (0) root         (0)    47956 2023-01-15 11:58:08.027787 wellmet-0.9.5/wellmet/voronoi.py
--rw-r--r--   0 user         (0) root         (0)     2465 2023-05-28 14:15:30.027787 wellmet-0.9.5/wellmet/welford.py
--rw-r--r--   0 user         (0) root         (0)    32101 2023-03-15 04:11:34.028049 wellmet-0.9.5/wellmet/whitebox.py
--rw-r--r--   0 user         (0) root         (0)    26468 2023-05-28 14:15:30.028049 wellmet-0.9.5/wellmet/wireframe.py
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-29 17:59:33.890241 wellmet-0.9.5/wellmet.egg-info/
--rw-r--r--   0 user         (0) root         (0)     5007 2023-05-29 17:59:33.028049 wellmet-0.9.5/wellmet.egg-info/PKG-INFO
--rw-r--r--   0 user         (0) root         (0)     1642 2023-05-29 17:59:33.028311 wellmet-0.9.5/wellmet.egg-info/SOURCES.txt
--rw-r--r--   0 user         (0) root         (0)        1 2023-05-29 17:59:33.028311 wellmet-0.9.5/wellmet.egg-info/dependency_links.txt
--rw-r--r--   0 user         (0) root         (0)       70 2023-05-29 17:59:33.028311 wellmet-0.9.5/wellmet.egg-info/requires.txt
--rw-r--r--   0 user         (0) root         (0)        8 2023-05-29 17:59:33.028573 wellmet-0.9.5/wellmet.egg-info/top_level.txt
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:18:59.725614 wellmet-0.9.6/
+-rw-r--r--   0 user         (0) root         (0)     1093 2022-04-30 17:02:31.015990 wellmet-0.9.6/LICENSE
+-rw-r--r--   0 user         (0) root         (0)     5845 2023-05-30 18:18:59.726401 wellmet-0.9.6/PKG-INFO
+-rw-r--r--   0 user         (0) root         (0)     5175 2023-05-30 18:17:45.015990 wellmet-0.9.6/README.md
+-rw-r--r--   0 user         (0) root         (0)       81 2023-05-30 15:14:52.016253 wellmet-0.9.6/pyproject.toml
+-rw-r--r--   0 user         (0) root         (0)      784 2023-05-30 18:18:59.746586 wellmet-0.9.6/setup.cfg
+-rw-r--r--   0 user         (0) root         (0)       54 2023-05-29 15:46:17.016253 wellmet-0.9.6/setup.py
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:18:59.274989 wellmet-0.9.6/wellmet/
+-rw-r--r--   0 user         (0) root         (0)    30048 2023-05-28 14:15:30.016515 wellmet-0.9.6/wellmet/IS_stat.py
+-rw-r--r--   0 user         (0) root         (0)       86 2023-05-28 15:34:51.016515 wellmet-0.9.6/wellmet/__init__.py
+-rw-r--r--   0 user         (0) root         (0)       72 2022-04-30 16:53:41.016515 wellmet-0.9.6/wellmet/__main__.py
+-rw-r--r--   0 user         (0) root         (0)    11243 2023-05-28 14:15:30.016515 wellmet-0.9.6/wellmet/candybox.py
+-rw-r--r--   0 user         (0) root         (0)     6756 2023-05-28 14:15:30.016777 wellmet-0.9.6/wellmet/candynodes.py
+-rw-r--r--   0 user         (0) root         (0)    50875 2023-05-29 17:12:11.016777 wellmet-0.9.6/wellmet/convex_hull.py
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:18:59.382730 wellmet-0.9.6/wellmet/dicebox/
+-rw-r--r--   0 user         (0) root         (0)        6 2022-04-30 16:53:41.018612 wellmet-0.9.6/wellmet/dicebox/__init__.py
+-rw-r--r--   0 user         (0) root         (0)     7865 2023-05-29 17:12:04.018874 wellmet-0.9.6/wellmet/dicebox/_exploration.py
+-rw-r--r--   0 user         (0) root         (0)    14880 2023-05-30 15:54:19.018874 wellmet-0.9.6/wellmet/dicebox/circumtri.py
+-rw-r--r--   0 user         (0) root         (0)    36893 2023-01-15 11:50:38.016777 wellmet-0.9.6/wellmet/estimation.py
+-rw-r--r--   0 user         (0) root         (0)    52580 2023-01-15 11:51:29.017039 wellmet-0.9.6/wellmet/f_models.py
+-rw-r--r--   0 user         (0) root         (0)    42237 2023-03-12 14:45:57.017039 wellmet-0.9.6/wellmet/g_models.py
+-rw-r--r--   0 user         (0) root         (0)    21042 2023-05-28 14:15:30.017039 wellmet-0.9.6/wellmet/ghull.py
+-rw-r--r--   0 user         (0) root         (0)     3234 2022-05-13 19:15:46.017301 wellmet-0.9.6/wellmet/misc.py
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:18:59.513802 wellmet-0.9.6/wellmet/mplot/
+-rw-r--r--   0 user         (0) root         (0)     1407 2022-04-30 16:53:41.018874 wellmet-0.9.6/wellmet/mplot/__init__.py
+-rw-r--r--   0 user         (0) root         (0)     9741 2022-04-30 16:53:41.019136 wellmet-0.9.6/wellmet/mplot/_axes3d.py
+-rw-r--r--   0 user         (0) root         (0)      714 2022-04-30 16:53:41.019136 wellmet-0.9.6/wellmet/mplot/_axis3d_margins_patch.py
+-rw-r--r--   0 user         (0) root         (0)    23492 2023-03-30 13:18:09.019136 wellmet-0.9.6/wellmet/mplot/mart.py
+-rw-r--r--   0 user         (0) root         (0)    13647 2023-01-15 11:54:22.019398 wellmet-0.9.6/wellmet/mplot/mart3d.py
+-rw-r--r--   0 user         (0) root         (0)    26324 2023-05-29 17:11:54.019398 wellmet-0.9.6/wellmet/mplot/maxes.py
+-rw-r--r--   0 user         (0) root         (0)     5577 2022-04-30 16:53:41.019398 wellmet-0.9.6/wellmet/mplot/maxes3d.py
+-rw-r--r--   0 user         (0) root         (0)    17778 2023-05-29 17:11:54.019660 wellmet-0.9.6/wellmet/mplot/mfigs.py
+-rw-r--r--   0 user         (0) root         (0)    10463 2023-02-02 13:58:18.019660 wellmet-0.9.6/wellmet/mplot/mgraph.py
+-rw-r--r--   0 user         (0) root         (0)     1132 2022-04-30 16:53:41.019660 wellmet-0.9.6/wellmet/mplot/misc.py
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:18:59.644087 wellmet-0.9.6/wellmet/qt_gui/
+-rw-r--r--   0 user         (0) root         (0)        6 2022-04-30 16:53:41.019660 wellmet-0.9.6/wellmet/qt_gui/__init__.py
+-rw-r--r--   0 user         (0) root         (0)    44438 2023-01-15 11:54:47.019923 wellmet-0.9.6/wellmet/qt_gui/gl_plot.py
+-rw-r--r--   0 user         (0) root         (0)      348 2022-10-16 03:13:28.019923 wellmet-0.9.6/wellmet/qt_gui/gui_startup.py
+-rw-r--r--   0 user         (0) root         (0)     1970 2022-10-07 12:30:43.019923 wellmet-0.9.6/wellmet/qt_gui/qt_box_functions.py
+-rw-r--r--   0 user         (0) root         (0)    26222 2023-05-30 16:44:01.020185 wellmet-0.9.6/wellmet/qt_gui/qt_dicebox.py
+-rw-r--r--   0 user         (0) root         (0)    35342 2023-01-17 14:19:12.020185 wellmet-0.9.6/wellmet/qt_gui/qt_graph_widgets.py
+-rw-r--r--   0 user         (0) root         (0)    24721 2023-05-30 16:56:29.020185 wellmet-0.9.6/wellmet/qt_gui/qt_gui.py
+-rw-r--r--   0 user         (0) root         (0)    99810 2023-05-29 17:13:09.020447 wellmet-0.9.6/wellmet/qt_gui/qt_plot.py
+-rw-r--r--   0 user         (0) root         (0)     3244 2023-01-10 05:21:15.020447 wellmet-0.9.6/wellmet/qt_gui/qt_testcases.py
+-rw-r--r--   0 user         (0) root         (0)    56858 2022-11-29 15:50:00.020447 wellmet-0.9.6/wellmet/qt_gui/qt_voronoi.py
+-rw-r--r--   0 user         (0) root         (0)    10978 2023-05-30 15:55:36.017301 wellmet-0.9.6/wellmet/reader.py
+-rw-r--r--   0 user         (0) root         (0)     4416 2023-01-15 11:56:01.017301 wellmet-0.9.6/wellmet/samplebox.py
+-rw-r--r--   0 user         (0) root         (0)     6558 2022-04-30 16:53:42.017563 wellmet-0.9.6/wellmet/sball.py
+-rw-r--r--   0 user         (0) root         (0)     6739 2023-05-29 17:11:42.017563 wellmet-0.9.6/wellmet/schemes.py
+-rw-r--r--   0 user         (0) root         (0)     8309 2023-05-28 14:15:30.017563 wellmet-0.9.6/wellmet/shell.py
+-rw-r--r--   0 user         (0) root         (0)   134283 2023-05-29 17:11:31.017825 wellmet-0.9.6/wellmet/simplex.py
+-rw-r--r--   0 user         (0) root         (0)    13090 2023-05-28 14:15:30.017825 wellmet-0.9.6/wellmet/spring.py
+-rw-r--r--   0 user         (0) root         (0)    10953 2022-04-30 16:53:42.017825 wellmet-0.9.6/wellmet/stm_df.py
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:18:59.712507 wellmet-0.9.6/wellmet/testcases/
+-rw-r--r--   0 user         (0) root         (0)        0 2023-05-28 13:48:40.020709 wellmet-0.9.6/wellmet/testcases/__init__.py
+-rw-r--r--   0 user         (0) root         (0)     8987 2023-03-12 15:00:08.020709 wellmet-0.9.6/wellmet/testcases/gaussian_2D.py
+-rw-r--r--   0 user         (0) root         (0)     8183 2023-05-28 14:14:11.020709 wellmet-0.9.6/wellmet/testcases/testcases_2D.py
+-rw-r--r--   0 user         (0) root         (0)     3741 2023-02-24 08:01:44.020971 wellmet-0.9.6/wellmet/testcases/testcases_2D_papers.py
+-rw-r--r--   0 user         (0) root         (0)     2572 2023-01-14 08:20:10.020971 wellmet-0.9.6/wellmet/testcases/testcases_nD.py
+-rw-r--r--   0 user         (0) root         (0)    11998 2023-01-30 12:29:31.020971 wellmet-0.9.6/wellmet/testcases/testcases_nD_papers.py
+-rw-r--r--   0 user         (0) root         (0)    47956 2023-01-15 11:58:08.018087 wellmet-0.9.6/wellmet/voronoi.py
+-rw-r--r--   0 user         (0) root         (0)     2465 2023-05-28 14:15:30.018087 wellmet-0.9.6/wellmet/welford.py
+-rw-r--r--   0 user         (0) root         (0)    32101 2023-03-15 04:11:34.018087 wellmet-0.9.6/wellmet/whitebox.py
+-rw-r--r--   0 user         (0) root         (0)    26468 2023-05-28 14:15:30.018350 wellmet-0.9.6/wellmet/wireframe.py
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:18:59.346292 wellmet-0.9.6/wellmet.egg-info/
+-rw-r--r--   0 user         (0) root         (0)     5845 2023-05-30 18:18:58.018350 wellmet-0.9.6/wellmet.egg-info/PKG-INFO
+-rw-r--r--   0 user         (0) root         (0)     1498 2023-05-30 18:18:58.018350 wellmet-0.9.6/wellmet.egg-info/SOURCES.txt
+-rw-r--r--   0 user         (0) root         (0)        1 2023-05-30 18:18:58.018350 wellmet-0.9.6/wellmet.egg-info/dependency_links.txt
+-rw-r--r--   0 user         (0) root         (0)       61 2023-05-30 18:18:58.018612 wellmet-0.9.6/wellmet.egg-info/requires.txt
+-rw-r--r--   0 user         (0) root         (0)        8 2023-05-30 18:18:58.018612 wellmet-0.9.6/wellmet.egg-info/top_level.txt
```

### Comparing `wellmet-0.9.5/LICENSE` & `wellmet-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/PKG-INFO` & `wellmet-0.9.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,51 @@
-Metadata-Version: 2.1
-Name: wellmet
-Version: 0.9.5
-Summary: a pure Python framework for spatial structural reliability analysis
-Home-page: https://rocketgit.com/iam-git/WellMet
-Author: Gerasimov Aleksei
-Author-email: ger-alex@seznam.cz
-License: MIT
-Keywords: failure probability,Monte Carlo,surrogate model,response surface
-Platform: UNKNOWN
-Classifier: Topic :: Scientific/Engineering
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 WellMet is pure Python framework for spatial structural reliability analysis. Or, more specifically, for "failure probability estimation and detection of failure surfaces by adaptive sequential decomposition of the design domain".
 
-Main dependencies are numpy+scipy, pandas, quadpy.
-Qt frontend requires pyqtgraph.
+# Installation
+## For users of conda-based distributions
+Anaconda users are encouraged to manually install WellMet's dependencies:
+```
+conda install -c anaconda scipy
+conda install -c anaconda matplotlib
+conda install -c anaconda pandas
+conda install -c anaconda mpmath
+conda install -c anaconda pyqtgraph
 
-To run graphical frontend with predefined reliability problems type in shell: python -m wellmet
+conda install -c conda-forge quadpy
+```
+pyopengl for 3D view (optionally):
+```
+conda install -c anaconda pyopengl
+```
 
-# Installation
+Finally, install WellMet from PyPI:
 ```
 pip install wellmet
 ```
 
+## For other users
+Install WellMet from PyPI:
+```
+pip install wellmet
+```
 
+WellMet relies on ```quadpy``` for simplex integration. However, quadpy became a closed source software and requires licence fee now.
+One probably could install official quadpy package and obtain a licence in order to support Nico Schloemer.
+However, WellMet has never been tested with commertial quadpy versions.
+So, we separately share the last GPL version of quadpy:
+```
+pip install quadpy-gpl
+```
 
 
 # How to use:
 ## A. To run GUI with predefined benchmark problems:
 1. Type in shell: ```python -m wellmet```
 2. Choose problem to solve, choose (optionally) filename to store samples and estimations, set up the algorithm.
-3. Choose from the main menu "Batch run" and type desired number of LSF calls.
+3. Press "Batch run..." button and type desired number of LSF calls.
 
 ## B. To test the algorithm on your own problem use the following code:
 ```
 import numpy as np
 import scipy.stats as stats
 
 from wellmet.qt_gui import qt_box_functions as gui
@@ -147,18 +152,19 @@
     next_node = box()
     # call LSF
     new_sample = my_problem(next_node)
     # put calculation result to the box
     box.add_sample(new_sample)
     
 print(box.get_pf_estimation())
+sensitivities_results = box.Tri.perform_sensitivity_analysis()
+print(sensitivities_results.sensitivities)
 ```
 
 
 
 
 
 
 
 
 This software has been developed under internal academic project no. FAST-K-21-6943  "Quality Internal Grants of BUT (KInG BUT)'' supported by  the Czech Operational Programme ``Research, Development and Education''  (CZ.02.2.69/0.0/0.0/19\_073/0016948, managed by the Czech Ministry of Education.
-
```

### Comparing `wellmet-0.9.5/README.md` & `wellmet-0.9.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,70 @@
+Metadata-Version: 2.1
+Name: wellmet
+Version: 0.9.6
+Summary: a pure Python framework for spatial structural reliability analysis
+Home-page: https://rocketgit.com/iam-git/WellMet
+Author: Gerasimov Aleksei
+Author-email: ger-alex@seznam.cz
+License: MIT
+Keywords: failure probability,Monte Carlo,surrogate model,response surface
+Platform: UNKNOWN
+Classifier: Topic :: Scientific/Engineering
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 WellMet is pure Python framework for spatial structural reliability analysis. Or, more specifically, for "failure probability estimation and detection of failure surfaces by adaptive sequential decomposition of the design domain".
 
-Main dependencies are numpy+scipy, pandas, quadpy.
-Qt frontend requires pyqtgraph.
+# Installation
+## For users of conda-based distributions
+Anaconda users are encouraged to manually install WellMet's dependencies:
+```
+conda install -c anaconda scipy
+conda install -c anaconda matplotlib
+conda install -c anaconda pandas
+conda install -c anaconda mpmath
+conda install -c anaconda pyqtgraph
 
-To run graphical frontend with predefined reliability problems type in shell: python -m wellmet
+conda install -c conda-forge quadpy
+```
+pyopengl for 3D view (optionally):
+```
+conda install -c anaconda pyopengl
+```
 
-# Installation
+Finally, install WellMet from PyPI:
 ```
 pip install wellmet
 ```
 
+## For other users
+Install WellMet from PyPI:
+```
+pip install wellmet
+```
 
+WellMet relies on ```quadpy``` for simplex integration. However, quadpy became a closed source software and requires licence fee now.
+One probably could install official quadpy package and obtain a licence in order to support Nico Schloemer.
+However, WellMet has never been tested with commertial quadpy versions.
+So, we separately share the last GPL version of quadpy:
+```
+pip install quadpy-gpl
+```
 
 
 # How to use:
 ## A. To run GUI with predefined benchmark problems:
 1. Type in shell: ```python -m wellmet```
 2. Choose problem to solve, choose (optionally) filename to store samples and estimations, set up the algorithm.
-3. Choose from the main menu "Batch run" and type desired number of LSF calls.
+3. Press "Batch run..." button and type desired number of LSF calls.
 
 ## B. To test the algorithm on your own problem use the following code:
 ```
 import numpy as np
 import scipy.stats as stats
 
 from wellmet.qt_gui import qt_box_functions as gui
@@ -128,17 +171,21 @@
     next_node = box()
     # call LSF
     new_sample = my_problem(next_node)
     # put calculation result to the box
     box.add_sample(new_sample)
     
 print(box.get_pf_estimation())
+sensitivities_results = box.Tri.perform_sensitivity_analysis()
+print(sensitivities_results.sensitivities)
 ```
 
 
 
 
 
 
 
 
-This software has been developed under internal academic project no. FAST-K-21-6943  "Quality Internal Grants of BUT (KInG BUT)'' supported by  the Czech Operational Programme ``Research, Development and Education''  (CZ.02.2.69/0.0/0.0/19\_073/0016948, managed by the Czech Ministry of Education.
+This software has been developed under internal academic project no. FAST-K-21-6943  "Quality Internal Grants of BUT (KInG BUT)'' supported by  the Czech Operational Programme ``Research, Development and Education''  (CZ.02.2.69/0.0/0.0/19\_073/0016948, managed by the Czech Ministry of Education.
+
+
```

### Comparing `wellmet-0.9.5/setup.cfg` & `wellmet-0.9.6/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wellmet
-version = 0.9.5
+version = 0.9.6
 author = Gerasimov Aleksei
 author_email = ger-alex@seznam.cz
 description = a pure Python framework for spatial structural reliability analysis
 url = https://rocketgit.com/iam-git/WellMet
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
@@ -22,17 +22,16 @@
 
 [options]
 packages = find:
 install_requires = 
 	numpy
 	scipy
 	mpmath
-	ndim<=0.1.6
-	bquadpy
 	pandas
+	matplotlib
 	PyQt5
 	pyqtgraph>=0.13.1
 python_requires = >=3.8
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `wellmet-0.9.5/wellmet/IS_stat.py` & `wellmet-0.9.6/wellmet/IS_stat.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/candybox.py` & `wellmet-0.9.6/wellmet/candybox.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/candynodes.py` & `wellmet-0.9.6/wellmet/candynodes.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/convex_hull.py` & `wellmet-0.9.6/wellmet/convex_hull.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/dicebox/__circumtri.py` & `wellmet-0.9.6/wellmet/dicebox/circumtri.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,161 +1,50 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 
 import numpy as np
-from scipy.spatial import distance
+from scipy import stats
 
 import quadpy
 
-from .. import shell
 from .. import simplex as sx
 from .. import convex_hull as khull
 from ..reader import Store
-from ..candynodes import CandyNodes
 from .. import sball
 
 from ._exploration import _Exploration
 
 from collections import namedtuple
-from sortedcollections import ValueSortedDict
 
 
 
-
-
-def get_entropy(pf):
-    return -pf * np.log(pf) - (1 - pf) * np.log(1 - pf)
-
-
-    
-
-CircumTriEstimation = namedtuple('CircumTriEstimation', (
-    "nsim",
-    "nvar",
-    "nfacets",
-    "r","R",
-    "inner",
-    "shell",
-    "outer",
-    "FORM_outside",
-    "TwoFORM_outside",
-    "orth_outside",
-    "inside",
-    "outside",
-    "success_points",
-    "failure_points",
-    "success",
-    "failure",
-    "mix",
-    "vertex_estimation",
-    "weighted_vertex_estimation",
-    "nsimplex",
-    "tn_scheme",
-    "tn_scheme_points",
-    "newly_invalidated",
-    "newly_estimated",
-    "simplex_stats",
-    "candidates_sets",
-    "ncoplanar"
+QTriEstimation = namedtuple('QTriEstimation', (
+    *khull.QHullEstimation._fields,
+    'success_points',
+    'failure_points',
+    *sx.CubatureEstimation._fields[2:],
+    'r_safe',
+    'R_safe',
+    'r_mixed',
+    'R_mixed',
+    'r_failure',
+    'R_failure',
+    'p_sum',
+    'max_potential'
     ))
 
 
-class CircumTri(_Exploration):
-    
-    #č míží nám sampling_space: Ghull umí vzorkovat outside pouze v G prostoru
-    #č quadpy umístí integráční bodíky v prostoru triangulace.
-    def __init__(bx, sample_box, scheme, entropy_mode='weighted', 
-                    circumcenters_only=True, q=10):
-        
-        bx.sample_box = sample_box
-        bx.scheme = scheme
-        bx.entropy_mode = entropy_mode
-        bx.circumcenters_only = circumcenters_only
-        bx.q = q
-        
-        
-        bx.direct_plan = quadpy.un.mysovskikh_1(bx.nvar).points
-        bx.sball = sball.Sball(bx.nvar)
-        
-        bx.tri_space = 'G'
-        
-        #č přece ponechame složku pro uživatelské odhady
-        #č stm kód může semka něco ukladat
-        bx.estimations = []
-        
-        #č vítejte nové uložiště odhadů.
-        #č Odhady z stm kódu už ale nemají na tohle sahat
-        if hasattr(bx, 'filename'):
-            bx.box_estimations = Store.create(bx.filename + "_ctri", CircumTriEstimation)
-        else:
-            bx.box_estimations = []
-            
-        bx.CC = sx.CircumCenter(sample_box.nvar)
-            
-        # kind of interface to CandidatesWidget
-        bx.candidates_index = {}
-        bx.potential_index = ValueSortedDict()
-        
-        bx.regen()
-    
-        
-    def init_parameters(bx):
-        """
-        Returns dictionary of parameters the DiceBox was initialized with
-        """
-        return {'sample_box':bx.sample_box, 'scheme':bx.scheme.name, 
-                'entropy_mode':bx.entropy_mode, 
-                'circumcenters_only':circumcenters_only, 'q':bx.q}
-                 
+class _CircumTri(_Exploration):
     
     def __repr__(bx):
         return "%s(**%s)"%(bx.__class__.__name__,  repr(bx.init_parameters()))
         
     def __str__(bx):
         return "%s(%s)"%(bx.__class__.__name__,  str(bx.init_parameters()))
-        
-        
-        
-    def refine(bx):
-        if len(bx.candidates_index):
-            # return node with the greatest potential
-            key, value = bx.potential_index.peekitem()
-            return bx.candidates_index[key]
-        else:
-            bx._logger(msg='refine called, but triangulation does not exist yet. Fallback to random sample')
-            return bx.f_model(1)
-    
-    
-    def regen(bx):
-        """
-        regen() recreates data structures of the box. 
-        It shouldn't be called without reason, changed distribution, settings or so.
-        """
-        
-        #оӵ шайтан регенираци лэзьиз
-        bx._logger(msg='regeneration started')
-        
-        bx.candidates_index.clear()
-        bx.potential_index.clear()
-        
-        bx._regen_outside()
-        bx._regen_inside()
-        
-        if bx.nsim > 0:
-            bx.get_pf_estimation() #č updates global stats
-            bx.update_exploration_ratio()
-        else:
-            bx.exploration_ratio = 1
-        
-        bx._nsim = bx.nsim
-                 
-    
-    
-    
     
     def __len__(bx):
         return bx.sample_box.nsim
     
     def __getitem__(bx, slice):
         #č stačí vratit sample_box
         return bx.sample_box[slice]
@@ -189,256 +78,374 @@
     
         
     # přidávání vzorků musí bejt explicitní!
     def add_sample(bx, input_sample):
         bx.sample_box.add_sample(input_sample)
         bx.increment(bx.sample_box[bx._nsim:])
         bx._nsim = bx.nsim
+            
     
+    def get_exploratory_radius(bx):
+        R = bx.shell_stats.R
+        # empirical rule to get desired behavior
+        sphere_area = bx.convex_hull.nsphere_surface_area * (R + bx.q)**bx.nvar
+        p_desired = bx.shell_estimation.outside / sphere_area
+        
+        # get matematically clean radius of it
+        r = bx.sball.get_r(p_desired)
+        return r
     
+                    
+    def is_mixed(bx, simplices=None):
     
-    def update_exploration_ratio(bx):
-        if "tri" in dir(bx):
-            outside = np.sqrt(bx.global_stats['outside'])
-            mixed = np.sqrt(bx.global_stats['mix'])
-            bx.exploration_ratio = outside / (outside + mixed)
+        if simplices is None:
+            simplices = bx.tri.simplices
+        
+        in_failure = np.isin(simplices, bx.failure_points)
+        has_failure = in_failure.any(axis=1)
+        all_failure = in_failure.all(axis=1)
+        return np.logical_xor(has_failure, all_failure)
+    
+    
+    
+        
+    
+    def get_tri_radia(bx):
+        lengths = np.sum(np.square(bx.G), axis=1)
+        lengths = np.sqrt(lengths, out=lengths) #lengths of each radius-vector
+        
+        if 'Tri' in dir(bx):
+            simplices = bx.Tri.tri.simplices
+            radia = lengths[simplices]
+            r = np.min(radia, axis=1)
+            R = np.max(radia, axis=1)
+            
+            in_failure = bx.failsi[simplices]
+            
+            has_failure = in_failure.any(axis=1)
+            all_failure = in_failure.all(axis=1)
+            
+            if np.any(~has_failure):
+                r_safe = np.min(r[~has_failure])
+                R_safe = np.max(R[~has_failure])
+            else:
+                r_safe, R_safe = -1, -1
+            
+            
+            if np.any(all_failure):
+                r_failure = np.min(r[all_failure])
+                R_failure = np.max(R[all_failure])
+            else:
+                r_failure, R_failure = -1, -1
+                
+            mixed_mask = np.logical_xor(has_failure, all_failure)
+            if np.any(mixed_mask):
+                r_mixed = np.min(r[mixed_mask])
+                R_mixed = np.max(R[mixed_mask]) 
+            else:
+                r_mixed, R_mixed = -1, -1
+            
+            return r_safe, R_safe, r_mixed, R_mixed, r_failure, R_failure
+            
         else:
-            bx.exploration_ratio = 1
+            radia = [-1] * 6
+            r = np.min(lengths)
+            R = np.max(lengths)
+            
+            if np.all(bx.failsi):
+                return -1, -1, -1, -1, r, R
+            elif np.any(bx.failsi):
+                return -1, -1, r, R, -1, -1
+            else:
+                return r, R, -1, -1, -1, -1
+            
+            
+        
+    
+    def perform_topological_analysis(bx):
+        assert bx.tri_space == 'G'
+        # tn_scheme, points, simplices, neighbors, failsi, facets, normals
+        bx.ta = sx.TopologyAnalysis(bx.convex_hull.tn_scheme, bx.G, 
+                                    bx.Tri.tri.simplices, bx.Tri.tri.neighbors,
+                                     bx.failsi, bx.convex_hull.simplices, 
+                                     bx.convex_hull.A)
+        print("start integration of the convex envelope")   
+        bx.ta.integrate_convex_envelope()
+        print("start integration of the internal walls")
+        bx.ta.integrate_walls()
+        print("start topological analysis")   
+        bx.ta.perform_analysis()
         
         
     
     
     
-    #č bejvalej .estimate_simplex()
-    #č teď je to kolbek, který volá Triangulation
-    def _on_add_simplex(bx, nodes):
-        # -1=outside, 0=success, 1=failure, 2=mix
-        if nodes.event_id != 2:
-            return 
+    def get_pf_estimation(bx):
+        failsi = bx.failsi
         
+        success_points = len(failsi[~failsi])
+        failure_points = len(failsi[failsi])
         
-        indices = nodes.indices
-        failsi = bx.Tri.failsi[indices]
-        vertices_model = bx.Tri.tri.points[indices]
-        PDF = bx.Tri.PDF[indices]
+        inside = bx.shell_estimation.inside
         
-        circum_center = bx.CC.get_circumcenter(vertices_model)
-        r = distance.euclidean(circum_center, vertices_model[0])
-        circum_node = bx.f_model.new_sample(circum_center, space=bx.tri_space)
-        #č můžeme nechat numpy pole z jednoho prvku. Můžeme zredukovat na float
-        #circum_pdf = circum_node.pdf(bx.tri_space)
-        circum_pdf = float(circum_node.pdf(bx.tri_space))
-        circum_potential = r * circum_pdf**(1/bx.nvar)
-        
-        # circum rating
-        if bx.entropy_mode == 'none':
-            circum_rating = circum_potential
-        elif bx.entropy_mode == 'simple':
-            # fp like a failure points. Number of failure points
-            fp = len(failsi[failsi]) # the fastest solution
-            circum_rating = circum_potential * get_entropy(fp / len(failsi))
-        elif bx.entropy_mode == 'weighted':
-            # same as np.average(failsi, weights=pdf), but faster
-            wfr = np.sum(PDF[failsi]) / np.sum(PDF)
-            circum_rating = circum_potential * get_entropy(wfr)
-        
-        
-        if bx.circumcenters_only:
-            #č nodes příjdou zabalené do CandyNodes. Ty mají .attrs a .kwargs
-            circum_node = CandyNodes(circum_node, nodes.attrs)
-            circum_node.potential = circum_potential
-            circum_node.rating = circum_rating
-            bx.candidates_index[tuple(indices)] = circum_node
-            bx.potential_index[tuple(indices)] = circum_rating
-            
-            return
-        
-        #else:
-        
-        nodes_model = getattr(nodes, bx.tri_space)
-        dr = distance.cdist(nodes_model, [circum_center]).reshape(-1)
-        nodes_pdf = nodes.pdf(bx.tri_space)
-        node_potentials = (r - dr) * nodes_pdf**(1/bx.nvar)
-        
-        if bx.entropy_mode == 'none':
-            node_ratings = node_potentials
-        elif bx.entropy_mode == 'simple':
-            node_ratings = node_potentials * get_entropy(nodes.pfv)
-        elif bx.entropy_mode == 'weighted':
-            node_ratings = node_potentials * get_entropy(nodes.pfw)
+        if 'Tri' in dir(bx):
+            tri_estimation = bx.Tri.get_pf_estimation()
+            
+            mixed = tri_estimation.mix
+            failure = tri_estimation.failure
+            
+            if not bx.holydays:
+                success = inside - mixed - failure
+                p_sum = 1
+            else:
+                success = tri_estimation.success
+                outside = bx.shell_estimation.outside
+                p_sum = outside + failure + mixed + success
+            
+            return bx.Estimation(bx.nsim,  #č musíme sami lepit nové etikety, neboť
+                                *bx.get_outside_estimation(),
+                                success_points,
+                                failure_points,
+                                success,
+                                *tri_estimation[3:],
+                                
+                                *bx.get_tri_radia(),
+                                p_sum,
+                                bx.get_max_potential()
+                                )
             
         
+        #оӵ триангуляци ӧвӧл, иськем...
+        
+        #č může se stát, že první dvě tečky už hned májí různé barvy,
+        #č ale žádnej simplex ještě nemáme.
+        #č takže celou skříňku prostě bereme jako simplex
+        event, event_id, fr, wfr = sx.get_simplex_event(bx, weighting_space=bx.tri_space)
+        # -1=outside, 0=success, 1=failure, 2=mix
+        tri_estimation = {0:0, 1:0, 2:0}
+        tri_estimation[event_id] = inside
+        
+        success = tri_estimation[0]
+        failure = tri_estimation[1]
+        mixed = tri_estimation[2]
+        
+        return bx.Estimation(bx.nsim,  #č musíme sami lepit nové etikety, neboť
+                             *bx.get_outside_estimation(),
+                             success_points,
+                             failure_points,
+                             
+                             success,
+                             failure,
+                             mixed,
+                             inside * fr,
+                             inside * wfr, 
+                             inside * wfr,
+                             0, # nsimplex
+                             #sx.tn_scheme.name,
+                             bx.scheme.points.shape[1],
+                             0, #sx.newly_invalidated,
+                             0, #sx.newly_estimated,
+                             0, #len(sx.failure_simplices),
+                             0, #len(sx.mixed_simplices),
+                             0, #len(sx.tri.coplanar),
+                             
+                             *bx.get_tri_radia(),
+                             1,
+                             bx.get_max_potential()
+                             )
         
-        max_node = np.nanargmax(node_ratings)
-        max_node_rating = node_ratings[max_node]
-        if circum_rating > max_node_rating:
-            #č nodes příjdou zabalené do CandyNodes. Ty mají .attrs a .kwargs
-            circum_node = CandyNodes(circum_node, nodes.attrs)
-            circum_node.potential = circum_potential
-            circum_node.rating = circum_rating
-            bx.candidates_index[tuple(indices)] = circum_node
-            bx.potential_index[tuple(indices)] = circum_rating
-        else:
-            node = nodes[max_node]
-            node.potential = node_potentials[max_node]
-            node.rating = max_node_rating
-            bx.candidates_index[tuple(indices)] = node
-            bx.potential_index[tuple(indices)] = max_node_rating
-            
 
 
 
-            
-    # callback
-    #č sx.on_delete_simplex(indices=indices)
-    def _invalidate_simplex(bx, simplex):
-        bx.candidates_index.pop(simplex, None)
-        bx.potential_index.pop(simplex, None)
-    
+
+
+
+
+class CirQTri(_CircumTri):
     
+    def __init__(bx, sample_box, scheme, convex_hull_degree=5,
+                 q=1, holydays=0):
+        
+        bx.sample_box = sample_box
+        bx.convex_hull_degree = convex_hull_degree
+        bx.scheme = scheme
+        
+        bx.tri_space = 'G'
+            
+        bx.Estimation = QTriEstimation
+        bx.q = q
+        bx.holydays = holydays
+        
+        bx.sball = sball.Sball(bx.nvar)
+        
+        
+        #č přece ponechame složku pro uživatelské odhady
+        #č stm kód může semka něco ukladat
+        bx.estimations = []
+        
+        #č vítejte nové uložiště odhadů.
+        #č Odhady z stm kódu už ale nemají na tohle sahat
+        if hasattr(bx, 'filename'):
+            bx.box_estimations = Store.create(bx.filename + "_qtri", bx.Estimation)
+        else:
+            bx.box_estimations = []
+            
+        bx.CC = sx.CircumCenter(sample_box.nvar)
+        
+        bx.regen()
     
         
+    def init_parameters(bx):
+        """
+        Returns dictionary of parameters the DiceBox was initialized with
+        """
+        return {'sample_box':bx.sample_box, 'scheme':bx.scheme.name,
+                'convex_hull_degree':bx.convex_hull_degree,
+                 'q':bx.q, 'holydays':bx.holydays}
+
 
-                
     def _regen_outside(bx):
-        bx.convex_hull = khull.QHull(bx.f_model, space='G', 
-                                    incremental=True, auto_update=False)
-        bx.ghull = Ghull(bx.convex_hull)
+        facet_scheme = quadpy.tn.grundmann_moeller(bx.nvar - 1, bx.convex_hull_degree)
+        bx.convex_hull = khull.QHullCubature(bx.f_model, space='G', incremental=True, 
+                            auto_update=False, tn_scheme=facet_scheme)
+        
+        #č konečně mám pořádnou stejtful třídu
         #č pokud mám aspoň jednu tečku, tak už je mi šuma
         #č zda se konvexní obálka vytvořila, či nikoliv
         if bx.nsim > 0:
             bx.estimate_outside()
+            
+    
+    def estimate_outside(bx):
+        #č konečně mám pořádnou stejtful třídu
+        #č pokud mám aspoň jednu tečku, tak už je mi šuma
+        #č zda se konvexní obálka vytvořila, či nikoliv
         
+        #č Máme úkol: 
+        #č 1. Získat odhady a uložit je, abychom nemuseli opakovaně integrovat,
+        #č    dokud se neobjeví nějaký nový vzorek zvenku.
+        bx.shell_estimation = bx.convex_hull.get_convex_hull_estimation()
+        bx.shell_stats = bx.shell_estimation # simple trick
+    
             
+    def get_outside_estimation(bx):
+        return bx.shell_estimation[1:]
+    
+    
     def _regen_inside(bx):
         failsi = bx.failsi
         # incremental triangulation require one more point
         if (bx.nsim > bx.nvar + 1) and np.any(failsi) and not np.all(failsi):
-            #bx._logger(msg="triangulation started")
-            bx.__regen_inside()
+            try:
+                bx.Tri = sx.GaussCubatureIntegration(bx.samplebox, bx.scheme, 
+                                            incremental=True, full=bx.holydays)
+                
+                #č tri - Deloneho triangulace
+                bx.tri = bx.Tri.tri #č všichni tam očekávají QHull
+                bx._logger(msg="triangulation has been created")
+                
+            except BaseException as e:
+                #č chcu zachytit spadnuti QHull na začatku, 
+                #č kdy ještě není dostatek teček.
+                #č Jinak je třeba nechat QHull spadnout
+                if bx.nsim > 2*bx.nvar + 3: 
+                    #č no to teda ne!
+                    raise
+                else: 
+                    #č lze přípustit chybu triangulace    
+                    bx._logger(msg='triangulation failed')
         else:
             #č jíž není nutný
             bx._logger(msg="triangulation skipped")
             
-    def __regen_inside(bx):
+    
+    def get_circum_node(bx, indices):
+        vertices_model = bx.Tri.tri.points[indices]
         try:
-            bx.Tri = sx.BetterCubatureIntegration(bx.samplebox, bx.scheme,\
-                     tri_space='G', incremental=True,\
-                    on_add_simplex=bx._on_add_simplex,\
-                    on_delete_simplex=bx._invalidate_simplex)
-              
-            bx.Tri.integrate() # nic nevrácí, všecko je přes kolbeky
-            #č tri - Deloneho triangulace
-            bx.tri = bx.Tri.tri #č všichní tam očekávajou QHull
-            bx._logger(msg="triangulation has been created")
-            
+            circum_center = bx.CC.get_circumcenter(vertices_model)
         except BaseException as e:
-            #č chcu zachytit spadnuti QHull na začatku, 
-            #č kdy ještě není dostatek teček.
-            #č Jinak je třeba nechat QHull spadnout
-            if bx.nsim > 2*bx.nvar + 3: 
-                #č no to teda ne!
-                raise
-            else: 
-                #č lze přípustit chybu triangulace    
-                bx._logger(msg='triangulation failed')
+            bx._logger(repr(e), msg='CircumCenter error')
+            circum_center = np.mean(vertices_model, axis=0)
+             
+        if not np.all(np.isfinite(circum_center)):
+            raise
+             
+        length2 = np.sum(np.square(circum_center))
+        R = bx.get_exploratory_radius()
+        if length2 > R**2:
+            bx._logger(circum_center, 
+                    msg='Circumcenter lies too far away from the origin. The radial distance is reduced')
+            circum_center /= np.sqrt(length2)
+            circum_center *= R
+        
+        circum_node = bx.f_model.new_sample(circum_center, space=bx.tri_space)
+        return circum_node
     
     
+    def refine(bx):
+        if "Tri" in dir(bx):
+            # get the greatest mixed simplex
+            return bx.get_circum_node(bx.Tri.max_mixed_indices)
+        else:
+            bx._logger(msg='refine called, but triangulation does not exist yet. Fallback to a random sample')
+            return bx.f_model(1)
+    
+    
+    def holyday(bx):
+        if "Tri" in dir(bx) and (bx.Tri.max_safe > 0):
+            return bx.get_circum_node(bx.Tri.max_safe_indices)
+        else:
+            bx._logger(msg='Fallback to random sample')
+            return bx.f_model(1)
+    
+    def regen(bx):
+        """
+        regen() recreates data structures of the box. 
+        It shouldn't be called without reason, changed distribution, settings or so.
+        """
+        
+        #оӵ шайтан регенираци лэзьиз
+        bx._logger(msg='regeneration started')
+        
+        bx._regen_outside()
+        bx._regen_inside()
+        
+        bx.to_explore = 1
+        bx.to_refine = 0
+        if bx.nsim > 0:
+            bx.pf_estimation = bx.get_pf_estimation() 
+            bx.update_exploration_ratio()
+        
+        bx._nsim = bx.nsim
+
+
+
+    def get_max_potential(bx):
+        if "Tri" in dir(bx):
+             # get probability of the greatest mixed simplex
+            return bx.Tri.max_mixed
+        else:
+            return -1
+
+    def update_exploration_ratio(bx):
+        bx.to_explore = stats.norm.sf(bx.pf_estimation.r)
+        bx.to_refine = bx.get_max_potential()
+
         
     def increment(bx, input_sample):
         #č tri - Deloneho triangulace
         if "tri" in dir(bx):
             bx.Tri.update()
         else:
             bx._regen_inside()
             
-            
         if np.any(bx.convex_hull.is_outside(input_sample)):
             bx.convex_hull.update()
             bx.estimate_outside()
         
-        bx.box_estimations.append(bx.get_pf_estimation())
+        bx.pf_estimation = bx.get_pf_estimation()
+        bx.box_estimations.append(bx.pf_estimation)
         bx.update_exploration_ratio()
-    
-                
-    
-        
-        
-    
-    def estimate_outside(bx):
-        #č konečně mám pořádnou stejtful třídu
-        #č pokud mám aspoň jednu tečku, tak už je mi šuma
-        #č zda se konvexní obálka vytvořila, či nikoliv
-        
-        shell_estimation, global_stats = bx.ghull.get_shell_estimation()
-        
-        # shell_estimation  -22: inner, -3: shell, -11: outer
-        bx.shell_estimation = shell_estimation
-        
-        #č kvůli názvu neleze do namedtuple
-        global_stats['TwoFORM_outside'] = global_stats.pop('2FORM_outside')
-        #č ndim se nelibí pandas
-        global_stats['nvar'] = global_stats.pop('ndim')
-        
-        bx.global_stats = global_stats
-        
-        
-        
-        
-        
-    def get_pf_estimation(bx):
-        global_stats = bx.global_stats
-        orth_outside = global_stats['outside'] = global_stats['orth_outside']
-        pf_inside = global_stats['inside'] = 1 - orth_outside
-        
-        #č Ghull spouštíme sporadicky, 
-        #č takže musíme sami lepit nové etikety
-        global_stats['nsim'] = bx.nsim
-        
-        failsi = bx.failsi
-        
-        if 'tri' in dir(bx):
-            bx.global_stats.update(bx.Tri.get_pf_estimation())
-            failure = bx.global_stats['failure']
-            mixed = bx.global_stats['mix']
-            bx.global_stats['success_points'] = len(failsi[~failsi])
-            bx.global_stats['failure_points'] = len(failsi[failsi])
-            bx.global_stats['success'] = pf_inside - failure - mixed
-            bx.global_stats['candidates_sets'] = len(bx.candidates_index)
-            
-            return CircumTriEstimation(**bx.global_stats)
-            
-        
-        #оӵ триангуляци ӧвӧл, иськем...
-        
-        #č může se stát, že první dvě tečky už hned májí různé barvy,
-        #č ale žádnej simplex ještě nemáme.
-        #č takže celou skříňku prostě bereme jako simplex
-        event, event_id, fr, wfr = sx.get_simplex_event(bx, weighting_space=bx.tri_space)
-        # -1=outside, 0=success, 1=failure, 2=mix
-        tri_estimation = {0:0, 1:0, 2:0}
-        tri_estimation[event_id] = pf_inside
-        
-        vertex_estimation = pf_inside * fr
-        weighted_vertex_estimation = pf_inside * wfr
-        
-        global_stats = bx.global_stats
-        # outside dodá Ghull
-        global_stats['success_points'] = len(failsi[~failsi])
-        global_stats['failure_points'] = len(failsi[failsi])
-        global_stats['success'] = tri_estimation[0]
-        global_stats['failure'] = tri_estimation[1]
-        global_stats['mix'] = tri_estimation[2]
-        global_stats['vertex_estimation'] = vertex_estimation
-        global_stats['weighted_vertex_estimation'] = weighted_vertex_estimation
-        global_stats['nsimplex'] = 0
-        global_stats['tn_scheme'] = bx.scheme.name
-        global_stats['tn_scheme_points'] = bx.scheme.points.shape[1]
-        global_stats['newly_invalidated'] = 0
-        global_stats['newly_estimated'] = 0
-        global_stats['simplex_stats'] = 0
-        global_stats['candidates_sets'] = len(bx.candidates_index)
-        global_stats['ncoplanar'] = 0
-        
-        return CircumTriEstimation(**global_stats)
-        
-        
+
+
+
+
```

### Comparing `wellmet-0.9.5/wellmet/dicebox/_exploration.py` & `wellmet-0.9.6/wellmet/dicebox/_exploration.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/estimation.py` & `wellmet-0.9.6/wellmet/estimation.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/f_models.py` & `wellmet-0.9.6/wellmet/f_models.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/g_models.py` & `wellmet-0.9.6/wellmet/g_models.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/ghull.py` & `wellmet-0.9.6/wellmet/ghull.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/misc.py` & `wellmet-0.9.6/wellmet/misc.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/mplot/__init__.py` & `wellmet-0.9.6/wellmet/mplot/__init__.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/mplot/_axes3d.py` & `wellmet-0.9.6/wellmet/mplot/_axes3d.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/mplot/_axis3d_margins_patch.py` & `wellmet-0.9.6/wellmet/mplot/_axis3d_margins_patch.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/mplot/mart.py` & `wellmet-0.9.6/wellmet/mplot/mart.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/mplot/mart3d.py` & `wellmet-0.9.6/wellmet/mplot/mart3d.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/mplot/maxes.py` & `wellmet-0.9.6/wellmet/mplot/maxes.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/mplot/maxes3d.py` & `wellmet-0.9.6/wellmet/mplot/maxes3d.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/mplot/mfigs.py` & `wellmet-0.9.6/wellmet/mplot/mfigs.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/mplot/mgraph.py` & `wellmet-0.9.6/wellmet/mplot/mgraph.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/mplot/misc.py` & `wellmet-0.9.6/wellmet/mplot/misc.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/qt_gui/gl_plot.py` & `wellmet-0.9.6/wellmet/qt_gui/gl_plot.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/qt_gui/qt_box_functions.py` & `wellmet-0.9.6/wellmet/qt_gui/qt_box_functions.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/qt_gui/qt_dicebox.py` & `wellmet-0.9.6/wellmet/qt_gui/qt_dicebox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import numpy as np
 from .. import schemes
 from ..candybox import CandyBox
 #from ..dicebox.goal import Goal, Razitko, DiceBox
-from ..dicebox.circumtri import CirQTri, CircumTri, QTri
+from ..dicebox.circumtri import CirQTri
 from ..dicebox._exploration import DumbExploration
 import pyqtgraph as pg
 from pyqtgraph.Qt import QtCore, QtWidgets
 
 spaces = ['R', 'aR', 'Rn', 'aRn', 'P', 'GK', 'G', 'aG', 'U', 'aU']
 potentials = ['q_psee', 'psee', 'fee', 'fee2', 'ksee', 'chee', 'chee2', 'dd']
```

### Comparing `wellmet-0.9.5/wellmet/qt_gui/qt_graph_widgets.py` & `wellmet-0.9.6/wellmet/qt_gui/qt_graph_widgets.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/qt_gui/qt_gui.py` & `wellmet-0.9.6/wellmet/qt_gui/qt_gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,41 +71,41 @@
         self.app.exec_()
     
     def setup_menubar(self):    
         self.bar = self.menuBar()
         self.file_menu = self.bar.addMenu("File")
         #č kontejner jen aby Python mně Cečkové objekty nevymazal
         self.file_actions = [] 
-        load_coordinates_action = QtGui.QAction("Load coordinates", self)
+        load_coordinates_action = QtGui.QAction("Load coordinates...", self)
         load_coordinates_action.triggered.connect(self.load_coordinates)
         self.file_menu.addAction(load_coordinates_action)
         self.file_actions.append(load_coordinates_action)
         
-        export_coordinates_action = QtGui.QAction("Export coordinates", self)
+        export_coordinates_action = QtGui.QAction("Export coordinates...", self)
         export_coordinates_action.triggered.connect(self.export_coordinates)
         self.file_menu.addAction(export_coordinates_action)
         self.file_actions.append(export_coordinates_action)
         
-        import_samples_action = QtGui.QAction("Import samples", self)
+        import_samples_action = QtGui.QAction("Import samples...", self)
         import_samples_action.triggered.connect(self.import_samples)
         self.file_menu.addAction(import_samples_action)
         self.file_actions.append(import_samples_action)
         
-        export_samples_action = QtGui.QAction("Export samples", self)
+        export_samples_action = QtGui.QAction("Export samples...", self)
         export_samples_action.triggered.connect(self.export_samples)
         self.file_menu.addAction(export_samples_action)
         self.file_actions.append(export_samples_action)
         
         self.view = self.bar.addMenu("View")
         
         self.graph_menu = self.bar.addMenu("Box")
-        self.add_random_points_action = QtGui.QAction("Add random points", self)
+        self.add_random_points_action = QtGui.QAction("Add random points...", self)
         self.add_random_points_action.triggered.connect(self.add_random_points)
         self.graph_menu.addAction(self.add_random_points_action)
-        self.batch_run_action = QtGui.QAction("Batch run", self)
+        self.batch_run_action = QtGui.QAction("Batch run...", self)
         self.batch_run_action.triggered.connect(self.batch_run)
         self.graph_menu.addAction(self.batch_run_action)
         #self.gen_dmatrix_action = QtGui.QAction("Matrix view...", self)
         #self.gen_dmatrix_action.triggered.connect(self.gen_dmatrix)
         #self.graph_menu.addAction(self.gen_dmatrix_action)
         
         # optional feature
@@ -195,14 +195,16 @@
         
         self.btn = QtWidgets.QPushButton('run box')
         self.btn.clicked.connect(self.run_sb)
         
 #        self.btn2 = QtWidgets.QPushButton('connect/disconnect')
 #        self.btn2.setCheckable(True)
 #        self.btn2.clicked.connect(self.bx_connect)
+        self.batch_btn = QtWidgets.QPushButton('batch run...')
+        self.batch_btn.clicked.connect(self.batch_run)
         
         self.btn3 = QtWidgets.QPushButton('redraw')
         self.btn3.clicked.connect(lambda:self.redraw_called.emit())
         
         
         ## Create a grid layout to manage the widgets size and position
         self.layout = pg.LayoutWidget()
@@ -214,17 +216,17 @@
         
         ## Add widgets to the layout in their proper positions
         #self.layout.addWidget(self.list_view, 0, 0, 2, 1) 
         self.layout.addWidget(self.combo_space, 0, 0)   
         self.layout.addWidget(self.slider, 0, 1)   
         self.layout.addWidget(self.label_nsim, 0, 2)
         self.layout.addWidget(self.btn, 0, 3) 
-        #self.layout.addWidget(self.btn2, 0, 4)
-        self.layout.addWidget(self.btn3, 0, 4) 
-        self.layout.addWidget(self.central_widget, 1, 0, 1, 5)
+        self.layout.addWidget(self.batch_btn, 0, 4)
+        self.layout.addWidget(self.btn3, 0, 5) 
+        self.layout.addWidget(self.central_widget, 1, 0, 1, 6)
         
 
 
         # status bar, mainly to observe BlackBox
         self.statusBar = QtWidgets.QStatusBar()
         self.setStatusBar(self.statusBar)
         self.btn_continue = QtWidgets.QPushButton('continue')
@@ -313,26 +315,32 @@
             
             dock = QtWidgets.QDockWidget("Error graph", self)
             dock.setWidget(gw.ErrorGraph(pf_exact, self.box_estimation_data,  dock))
             self.dockables.append(dock)
             self.tabifyDockWidget(self.dockables[0], dock)
         else:
             pf_exact = -1
+        
+        #dock = QtWidgets.QDockWidget("Voronoi estimation graph", self)
+        #dock.setWidget(gw.VoronoiEstimationGraph(self.sample_box, self, dock))
+        #self.dockables.append(dock)
+        #self.tabifyDockWidget(self.dockables[0], dock)
+
+        
+        dock = QtWidgets.QDockWidget("GRaph", self)
+        dock.setWidget(gw.GRaph(self, self.box_estimation_data, dock))
+        self.dockables.append(dock)
+        self.tabifyDockWidget(self.dockables[0], dock)
             
         dock = QtWidgets.QDockWidget("Estimation graph", self)
         widget = gw.EstimationGraph(pf_exact, self.box_estimation_data,  dock)
         dock.setWidget(widget)
         self.dockables.append(dock)
         self.tabifyDockWidget(self.dockables[0], dock)
         
-        
-        dock = QtWidgets.QDockWidget("GRaph", self)
-        dock.setWidget(gw.GRaph(self, self.box_estimation_data, dock))
-        self.dockables.append(dock)
-        self.tabifyDockWidget(self.dockables[0], dock)
        
     csv_filter = "CSV files (*.csv)"
     npy_filter = "NumPy binary files (*.npy)"
     txt_filter = "Text files (*.txt)"
     gz_filter = "Compressed text files (*.gz)"
        
     def load_coordinates(self):
```

### Comparing `wellmet-0.9.5/wellmet/qt_gui/qt_plot.py` & `wellmet-0.9.6/wellmet/qt_gui/qt_plot.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/qt_gui/qt_testcases.py` & `wellmet-0.9.6/wellmet/qt_gui/qt_testcases.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/qt_gui/qt_voronoi.py` & `wellmet-0.9.6/wellmet/qt_gui/qt_voronoi.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/reader.py` & `wellmet-0.9.6/wellmet/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             sb.sample_box = reader(filename, f_model)
             sb.append_allowed = True
         except FileNotFoundError:
             # Штош...
             sb.append_allowed = False
             if f_model is not None:
                 sb.sample_box = SampleBox(f_model)
-            print("Reader:", filename + '.csv', "ӧвӧл")
+            print("Reader:", filename + '.csv', "will be created") # ӧвӧл
         return sb
             
     @classmethod
     def FromSampleBox(cls, filename, sample_box):
         """
         Здесь отталкиваемся от сэмплбоксу
         """
@@ -181,15 +181,15 @@
             return self.sample_box
         except AttributeError:
             self.sample_box = reader(self.filename)
             self.append_allowed = True
             return self.sample_box
         except FileNotFoundError:
             # Штош...
-            print("Reader:", self.filename + '.csv', "opravdu ӧвӧл")
+            print("Reader:", self.filename + '.csv', "not found") # ӧвӧл
             
     def write(self):
         export(self.filename, self.sample_box)
         self.append_allowed = True
     
     # что бы эта бурда могла делать?
 #    def force_write(self):
```

### Comparing `wellmet-0.9.5/wellmet/samplebox.py` & `wellmet-0.9.6/wellmet/samplebox.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/sball.py` & `wellmet-0.9.6/wellmet/sball.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/schemes.py` & `wellmet-0.9.6/wellmet/schemes.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/shell.py` & `wellmet-0.9.6/wellmet/shell.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/simplex.py` & `wellmet-0.9.6/wellmet/simplex.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/spring.py` & `wellmet-0.9.6/wellmet/spring.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/stm_df.py` & `wellmet-0.9.6/wellmet/stm_df.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/testcases/gaussian_2D.py` & `wellmet-0.9.6/wellmet/testcases/gaussian_2D.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/testcases/testcases_2D.py` & `wellmet-0.9.6/wellmet/testcases/testcases_2D.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/testcases/testcases_2D_papers.py` & `wellmet-0.9.6/wellmet/testcases/testcases_2D_papers.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/testcases/testcases_nD.py` & `wellmet-0.9.6/wellmet/testcases/testcases_nD.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/testcases/testcases_nD_papers.py` & `wellmet-0.9.6/wellmet/testcases/testcases_nD_papers.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/voronoi.py` & `wellmet-0.9.6/wellmet/voronoi.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/welford.py` & `wellmet-0.9.6/wellmet/welford.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/whitebox.py` & `wellmet-0.9.6/wellmet/whitebox.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet/wireframe.py` & `wellmet-0.9.6/wellmet/wireframe.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.5/wellmet.egg-info/PKG-INFO` & `wellmet-0.9.6/wellmet.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wellmet
-Version: 0.9.5
+Version: 0.9.6
 Summary: a pure Python framework for spatial structural reliability analysis
 Home-page: https://rocketgit.com/iam-git/WellMet
 Author: Gerasimov Aleksei
 Author-email: ger-alex@seznam.cz
 License: MIT
 Keywords: failure probability,Monte Carlo,surrogate model,response surface
 Platform: UNKNOWN
@@ -15,32 +15,56 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 WellMet is pure Python framework for spatial structural reliability analysis. Or, more specifically, for "failure probability estimation and detection of failure surfaces by adaptive sequential decomposition of the design domain".
 
-Main dependencies are numpy+scipy, pandas, quadpy.
-Qt frontend requires pyqtgraph.
+# Installation
+## For users of conda-based distributions
+Anaconda users are encouraged to manually install WellMet's dependencies:
+```
+conda install -c anaconda scipy
+conda install -c anaconda matplotlib
+conda install -c anaconda pandas
+conda install -c anaconda mpmath
+conda install -c anaconda pyqtgraph
 
-To run graphical frontend with predefined reliability problems type in shell: python -m wellmet
+conda install -c conda-forge quadpy
+```
+pyopengl for 3D view (optionally):
+```
+conda install -c anaconda pyopengl
+```
 
-# Installation
+Finally, install WellMet from PyPI:
 ```
 pip install wellmet
 ```
 
+## For other users
+Install WellMet from PyPI:
+```
+pip install wellmet
+```
 
+WellMet relies on ```quadpy``` for simplex integration. However, quadpy became a closed source software and requires licence fee now.
+One probably could install official quadpy package and obtain a licence in order to support Nico Schloemer.
+However, WellMet has never been tested with commertial quadpy versions.
+So, we separately share the last GPL version of quadpy:
+```
+pip install quadpy-gpl
+```
 
 
 # How to use:
 ## A. To run GUI with predefined benchmark problems:
 1. Type in shell: ```python -m wellmet```
 2. Choose problem to solve, choose (optionally) filename to store samples and estimations, set up the algorithm.
-3. Choose from the main menu "Batch run" and type desired number of LSF calls.
+3. Press "Batch run..." button and type desired number of LSF calls.
 
 ## B. To test the algorithm on your own problem use the following code:
 ```
 import numpy as np
 import scipy.stats as stats
 
 from wellmet.qt_gui import qt_box_functions as gui
@@ -147,18 +171,21 @@
     next_node = box()
     # call LSF
     new_sample = my_problem(next_node)
     # put calculation result to the box
     box.add_sample(new_sample)
     
 print(box.get_pf_estimation())
+sensitivities_results = box.Tri.perform_sensitivity_analysis()
+print(sensitivities_results.sensitivities)
 ```
 
 
 
 
 
 
 
 
 This software has been developed under internal academic project no. FAST-K-21-6943  "Quality Internal Grants of BUT (KInG BUT)'' supported by  the Czech Operational Programme ``Research, Development and Education''  (CZ.02.2.69/0.0/0.0/19\_073/0016948, managed by the Czech Ministry of Education.
 
+
```

### Comparing `wellmet-0.9.5/wellmet.egg-info/SOURCES.txt` & `wellmet-0.9.6/wellmet.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -27,21 +27,17 @@
 wellmet/whitebox.py
 wellmet/wireframe.py
 wellmet.egg-info/PKG-INFO
 wellmet.egg-info/SOURCES.txt
 wellmet.egg-info/dependency_links.txt
 wellmet.egg-info/requires.txt
 wellmet.egg-info/top_level.txt
-wellmet/dicebox/__circumtri.py
 wellmet/dicebox/__init__.py
-wellmet/dicebox/_circumtri.py
 wellmet/dicebox/_exploration.py
-wellmet/dicebox/censoring.py
 wellmet/dicebox/circumtri.py
-wellmet/dicebox/goal.py
 wellmet/mplot/__init__.py
 wellmet/mplot/_axes3d.py
 wellmet/mplot/_axis3d_margins_patch.py
 wellmet/mplot/mart.py
 wellmet/mplot/mart3d.py
 wellmet/mplot/maxes.py
 wellmet/mplot/maxes3d.py
@@ -51,15 +47,14 @@
 wellmet/qt_gui/__init__.py
 wellmet/qt_gui/gl_plot.py
 wellmet/qt_gui/gui_startup.py
 wellmet/qt_gui/qt_box_functions.py
 wellmet/qt_gui/qt_dicebox.py
 wellmet/qt_gui/qt_graph_widgets.py
 wellmet/qt_gui/qt_gui.py
-wellmet/qt_gui/qt_pairwise.py
 wellmet/qt_gui/qt_plot.py
 wellmet/qt_gui/qt_testcases.py
 wellmet/qt_gui/qt_voronoi.py
 wellmet/testcases/__init__.py
 wellmet/testcases/gaussian_2D.py
 wellmet/testcases/testcases_2D.py
 wellmet/testcases/testcases_2D_papers.py
```

