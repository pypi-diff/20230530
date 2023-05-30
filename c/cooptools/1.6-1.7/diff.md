# Comparing `tmp/cooptools-1.6.tar.gz` & `tmp/cooptools-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cooptools-1.6.tar", last modified: Sat Mar 11 19:21:53 2023, max compression
+gzip compressed data, was "cooptools-1.7.tar", last modified: Tue May 30 16:59:56 2023, max compression
```

## Comparing `cooptools-1.6.tar` & `cooptools-1.7.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-03-11 19:21:53.963836 cooptools-1.6/
--rw-rw-rw-   0        0        0      770 2023-03-11 19:21:53.963836 cooptools-1.6/PKG-INFO
--rw-rw-rw-   0        0        0       59 2022-06-02 21:34:30.000000 cooptools-1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-03-11 19:21:53.765846 cooptools-1.6/cooptools/
--rw-rw-rw-   0        0        0        0 2021-08-29 04:28:10.000000 cooptools-1.6/cooptools/__init__.py
--rw-rw-rw-   0        0        0     2447 2022-11-21 16:49:49.000000 cooptools-1.6/cooptools/anchor.py
--rw-rw-rw-   0        0        0     6668 2022-08-02 18:13:17.000000 cooptools-1.6/cooptools/colors.py
-drwxrwxrwx   0        0        0        0 2023-03-11 19:21:53.814811 cooptools-1.6/cooptools/commandDesignPattern/
--rw-rw-rw-   0        0        0       66 2022-06-02 21:34:30.000000 cooptools-1.6/cooptools/commandDesignPattern/__init__.py
--rw-rw-rw-   0        0        0     3475 2022-11-10 20:52:38.000000 cooptools-1.6/cooptools/commandDesignPattern/commandController.py
--rw-rw-rw-   0        0        0      833 2022-11-10 20:53:28.000000 cooptools-1.6/cooptools/commandDesignPattern/commandProtocol.py
--rw-rw-rw-   0        0        0      410 2022-10-23 20:05:41.000000 cooptools-1.6/cooptools/commandDesignPattern/exceptions.py
--rw-rw-rw-   0        0        0     7136 2023-02-02 23:13:02.000000 cooptools-1.6/cooptools/common.py
--rw-rw-rw-   0        0        0     6403 2022-06-02 21:34:30.000000 cooptools-1.6/cooptools/config.py
--rw-rw-rw-   0        0        0     3503 2022-12-02 23:22:56.000000 cooptools-1.6/cooptools/coopEnum.py
--rw-rw-rw-   0        0        0      273 2023-02-09 23:59:03.000000 cooptools-1.6/cooptools/coopProtocols.py
--rw-rw-rw-   0        0        0     2863 2022-06-02 21:34:30.000000 cooptools-1.6/cooptools/coopthreading.py
-drwxrwxrwx   0        0        0        0 2023-03-11 19:21:53.836811 cooptools-1.6/cooptools/dataRefresher/
--rw-rw-rw-   0        0        0       70 2022-06-02 21:34:30.000000 cooptools-1.6/cooptools/dataRefresher/__init__.py
--rw-rw-rw-   0        0        0     2299 2023-02-07 17:35:24.000000 cooptools-1.6/cooptools/dataRefresher/dataHub.py
--rw-rw-rw-   0        0        0     8195 2023-02-13 23:36:35.000000 cooptools-1.6/cooptools/dataRefresher/dataRefresher.py
--rw-rw-rw-   0        0        0     4137 2023-02-02 21:58:30.000000 cooptools-1.6/cooptools/date_utils.py
--rw-rw-rw-   0        0        0     2677 2023-01-28 03:52:10.000000 cooptools-1.6/cooptools/decor.py
--rw-rw-rw-   0        0        0     2528 2022-09-19 22:09:44.000000 cooptools-1.6/cooptools/dictPolicies.py
-drwxrwxrwx   0        0        0        0 2023-03-11 19:21:53.845809 cooptools-1.6/cooptools/discreteEventSimulator/
--rw-rw-rw-   0        0        0        0 2023-01-19 21:18:55.000000 cooptools-1.6/cooptools/discreteEventSimulator/__init__.py
--rw-rw-rw-   0        0        0     5778 2023-01-23 18:26:37.000000 cooptools-1.6/cooptools/discreteEventSimulator/discreteEventSimulator.py
-drwxrwxrwx   0        0        0        0 2023-03-11 19:21:53.887814 cooptools-1.6/cooptools/geometry_utils/
--rw-rw-rw-   0        0        0        0 2023-03-07 18:24:21.000000 cooptools-1.6/cooptools/geometry_utils/__init__.py
--rw-rw-rw-   0        0        0     5481 2023-03-07 18:31:44.000000 cooptools-1.6/cooptools/geometry_utils/circle_utils.py
--rw-rw-rw-   0        0        0     8755 2023-03-07 18:29:32.000000 cooptools-1.6/cooptools/geometry_utils/curve_utils.py
--rw-rw-rw-   0        0        0     2753 2023-03-07 18:29:32.000000 cooptools-1.6/cooptools/geometry_utils/line_utils.py
--rw-rw-rw-   0        0        0     2381 2023-03-07 18:29:32.000000 cooptools-1.6/cooptools/geometry_utils/rect_utils.py
--rw-rw-rw-   0        0        0     2434 2023-03-07 18:29:32.000000 cooptools-1.6/cooptools/geometry_utils/triangle_utils.py
--rw-rw-rw-   0        0        0     7744 2023-03-07 18:31:44.000000 cooptools-1.6/cooptools/geometry_utils/vector_utils.py
--rw-rw-rw-   0        0        0     3480 2022-12-01 19:46:18.000000 cooptools-1.6/cooptools/jsonIO.py
--rw-rw-rw-   0        0        0     4137 2022-07-19 18:00:18.000000 cooptools-1.6/cooptools/marchingSquares.py
--rw-rw-rw-   0        0        0     5130 2021-08-29 04:28:10.000000 cooptools-1.6/cooptools/matrixManipulation.py
--rw-rw-rw-   0        0        0     5682 2022-06-22 22:18:21.000000 cooptools-1.6/cooptools/metrics.py
--rw-rw-rw-   0        0        0     8651 2023-02-07 17:35:24.000000 cooptools-1.6/cooptools/os_manip.py
--rw-rw-rw-   0        0        0    20839 2023-02-06 16:33:36.000000 cooptools-1.6/cooptools/pandasHelpers.py
--rw-rw-rw-   0        0        0     5928 2022-11-22 19:39:42.000000 cooptools-1.6/cooptools/plotting.py
--rw-rw-rw-   0        0        0     1421 2021-08-29 04:28:10.000000 cooptools-1.6/cooptools/printing.py
--rw-rw-rw-   0        0        0     3332 2023-02-01 19:26:21.000000 cooptools-1.6/cooptools/randoms.py
--rw-rw-rw-   0        0        0      684 2023-02-13 22:06:39.000000 cooptools-1.6/cooptools/register.py
--rw-rw-rw-   0        0        0     1695 2023-02-23 22:29:37.000000 cooptools-1.6/cooptools/retry.py
-drwxrwxrwx   0        0        0        0 2023-03-11 19:21:53.911810 cooptools-1.6/cooptools/sectors/
--rw-rw-rw-   0        0        0       20 2023-03-07 20:40:12.000000 cooptools-1.6/cooptools/sectors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 19:21:53.937810 cooptools-1.6/cooptools/sectors/grids/
--rw-rw-rw-   0        0        0       78 2023-03-07 20:35:41.000000 cooptools-1.6/cooptools/sectors/grids/__init__.py
--rw-rw-rw-   0        0        0     1253 2022-09-19 21:08:23.000000 cooptools-1.6/cooptools/sectors/grids/gridState.py
--rw-rw-rw-   0        0        0     3273 2023-03-07 20:22:53.000000 cooptools-1.6/cooptools/sectors/grids/grid_base.py
--rw-rw-rw-   0        0        0     2394 2022-11-10 19:53:54.000000 cooptools-1.6/cooptools/sectors/grids/hexGrid.py
--rw-rw-rw-   0        0        0     3024 2023-03-07 20:35:41.000000 cooptools-1.6/cooptools/sectors/grids/rectGrid.py
--rw-rw-rw-   0        0        0     7122 2022-11-12 19:13:30.000000 cooptools-1.6/cooptools/sectors/hex_utils.py
--rw-rw-rw-   0        0        0     8027 2022-11-21 15:30:38.000000 cooptools-1.6/cooptools/sectors/rect_utils.py
--rw-rw-rw-   0        0        0      337 2022-10-13 14:34:53.000000 cooptools-1.6/cooptools/sectors/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-11 19:21:53.938827 cooptools-1.6/cooptools/statistics/
--rw-rw-rw-   0        0        0       47 2021-10-05 19:39:56.000000 cooptools-1.6/cooptools/statistics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 19:21:53.955836 cooptools-1.6/cooptools/statistics/controlChart/
--rw-rw-rw-   0        0        0        0 2022-02-19 23:10:39.000000 cooptools-1.6/cooptools/statistics/controlChart/__init__.py
--rw-rw-rw-   0        0        0    13265 2022-11-10 23:04:03.000000 cooptools-1.6/cooptools/statistics/controlChart/controlChart.py
--rw-rw-rw-   0        0        0     7937 2022-11-12 19:13:30.000000 cooptools-1.6/cooptools/statistics/controlChart/plotting.py
--rw-rw-rw-   0        0        0     1677 2022-06-03 13:34:45.000000 cooptools-1.6/cooptools/timeWindow.py
--rw-rw-rw-   0        0        0     3168 2022-06-23 21:58:42.000000 cooptools-1.6/cooptools/timedDecay.py
--rw-rw-rw-   0        0        0     5204 2022-12-31 04:29:20.000000 cooptools-1.6/cooptools/toggles.py
--rw-rw-rw-   0        0        0     1553 2022-11-10 23:12:40.000000 cooptools-1.6/cooptools/trends.py
-drwxrwxrwx   0        0        0        0 2023-03-11 19:21:53.962835 cooptools-1.6/cooptools/triggerActionSystem/
--rw-rw-rw-   0        0        0        0 2023-02-09 23:42:35.000000 cooptools-1.6/cooptools/triggerActionSystem/__init__.py
--rw-rw-rw-   0        0        0      247 2023-02-10 00:02:03.000000 cooptools-1.6/cooptools/triggerActionSystem/trigger.py
--rw-rw-rw-   0        0        0     3098 2023-02-14 19:51:35.000000 cooptools-1.6/cooptools/typevalidation.py
--rw-rw-rw-   0        0        0     2375 2022-11-30 23:33:22.000000 cooptools-1.6/cooptools/version.py
-drwxrwxrwx   0        0        0        0 2023-03-11 19:21:53.790811 cooptools-1.6/cooptools.egg-info/
--rw-rw-rw-   0        0        0      770 2023-03-11 19:21:53.000000 cooptools-1.6/cooptools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2101 2023-03-11 19:21:53.000000 cooptools-1.6/cooptools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-11 19:21:53.000000 cooptools-1.6/cooptools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-08-30 22:37:58.000000 cooptools-1.6/cooptools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      171 2023-03-11 19:21:53.000000 cooptools-1.6/cooptools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-11 19:21:53.000000 cooptools-1.6/cooptools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-11 19:21:53.964810 cooptools-1.6/setup.cfg
--rw-rw-rw-   0        0        0     1197 2023-03-11 19:21:50.000000 cooptools-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:59:56.446636 cooptools-1.7/
+-rw-rw-rw-   0        0        0      770 2023-05-30 16:59:56.446636 cooptools-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2022-06-02 21:34:30.000000 cooptools-1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 16:59:56.189635 cooptools-1.7/cooptools/
+-rw-rw-rw-   0        0        0        0 2021-08-29 04:28:10.000000 cooptools-1.7/cooptools/__init__.py
+-rw-rw-rw-   0        0        0     2447 2022-11-21 16:49:49.000000 cooptools-1.7/cooptools/anchor.py
+-rw-rw-rw-   0        0        0     7443 2023-04-11 17:52:54.000000 cooptools-1.7/cooptools/colors.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:59:56.251635 cooptools-1.7/cooptools/commandDesignPattern/
+-rw-rw-rw-   0        0        0       66 2022-06-02 21:34:30.000000 cooptools-1.7/cooptools/commandDesignPattern/__init__.py
+-rw-rw-rw-   0        0        0     3475 2022-11-10 20:52:38.000000 cooptools-1.7/cooptools/commandDesignPattern/commandController.py
+-rw-rw-rw-   0        0        0      833 2022-11-10 20:53:28.000000 cooptools-1.7/cooptools/commandDesignPattern/commandProtocol.py
+-rw-rw-rw-   0        0        0      410 2022-10-23 20:05:41.000000 cooptools-1.7/cooptools/commandDesignPattern/exceptions.py
+-rw-rw-rw-   0        0        0     7136 2023-02-02 23:13:02.000000 cooptools-1.7/cooptools/common.py
+-rw-rw-rw-   0        0        0     4070 2023-05-30 16:56:37.000000 cooptools-1.7/cooptools/config.py
+-rw-rw-rw-   0        0        0     3503 2022-12-02 23:22:56.000000 cooptools-1.7/cooptools/coopEnum.py
+-rw-rw-rw-   0        0        0      273 2023-02-09 23:59:03.000000 cooptools-1.7/cooptools/coopProtocols.py
+-rw-rw-rw-   0        0        0     2863 2022-06-02 21:34:30.000000 cooptools-1.7/cooptools/coopthreading.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:59:56.276635 cooptools-1.7/cooptools/dataRefresher/
+-rw-rw-rw-   0        0        0       70 2022-06-02 21:34:30.000000 cooptools-1.7/cooptools/dataRefresher/__init__.py
+-rw-rw-rw-   0        0        0     2299 2023-02-07 17:35:24.000000 cooptools-1.7/cooptools/dataRefresher/dataHub.py
+-rw-rw-rw-   0        0        0     8195 2023-02-13 23:36:35.000000 cooptools-1.7/cooptools/dataRefresher/dataRefresher.py
+-rw-rw-rw-   0        0        0     4484 2023-05-25 14:18:36.000000 cooptools-1.7/cooptools/date_utils.py
+-rw-rw-rw-   0        0        0     2677 2023-01-28 03:52:10.000000 cooptools-1.7/cooptools/decor.py
+-rw-rw-rw-   0        0        0     2528 2022-09-19 22:09:44.000000 cooptools-1.7/cooptools/dictPolicies.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:59:56.286635 cooptools-1.7/cooptools/discreteEventSimulator/
+-rw-rw-rw-   0        0        0        0 2023-01-19 21:18:55.000000 cooptools-1.7/cooptools/discreteEventSimulator/__init__.py
+-rw-rw-rw-   0        0        0     5778 2023-01-23 18:26:37.000000 cooptools-1.7/cooptools/discreteEventSimulator/discreteEventSimulator.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:59:56.340635 cooptools-1.7/cooptools/geometry_utils/
+-rw-rw-rw-   0        0        0        0 2023-03-07 18:24:21.000000 cooptools-1.7/cooptools/geometry_utils/__init__.py
+-rw-rw-rw-   0        0        0     5532 2023-03-15 23:08:51.000000 cooptools-1.7/cooptools/geometry_utils/circle_utils.py
+-rw-rw-rw-   0        0        0     8755 2023-03-07 18:29:32.000000 cooptools-1.7/cooptools/geometry_utils/curve_utils.py
+-rw-rw-rw-   0        0        0     2753 2023-03-07 18:29:32.000000 cooptools-1.7/cooptools/geometry_utils/line_utils.py
+-rw-rw-rw-   0        0        0     2381 2023-03-07 18:29:32.000000 cooptools-1.7/cooptools/geometry_utils/rect_utils.py
+-rw-rw-rw-   0        0        0     2434 2023-03-07 18:29:32.000000 cooptools-1.7/cooptools/geometry_utils/triangle_utils.py
+-rw-rw-rw-   0        0        0     8281 2023-03-15 21:44:53.000000 cooptools-1.7/cooptools/geometry_utils/vector_utils.py
+-rw-rw-rw-   0        0        0     3480 2022-12-01 19:46:18.000000 cooptools-1.7/cooptools/jsonIO.py
+-rw-rw-rw-   0        0        0     4137 2022-07-19 18:00:18.000000 cooptools-1.7/cooptools/marchingSquares.py
+-rw-rw-rw-   0        0        0     5130 2021-08-29 04:28:10.000000 cooptools-1.7/cooptools/matrixManipulation.py
+-rw-rw-rw-   0        0        0     5682 2022-06-22 22:18:21.000000 cooptools-1.7/cooptools/metrics.py
+-rw-rw-rw-   0        0        0    11287 2023-05-30 16:47:59.000000 cooptools-1.7/cooptools/os_manip.py
+-rw-rw-rw-   0        0        0    20839 2023-02-06 16:33:36.000000 cooptools-1.7/cooptools/pandasHelpers.py
+-rw-rw-rw-   0        0        0     5928 2022-11-22 19:39:42.000000 cooptools-1.7/cooptools/plotting.py
+-rw-rw-rw-   0        0        0     1421 2021-08-29 04:28:10.000000 cooptools-1.7/cooptools/printing.py
+-rw-rw-rw-   0        0        0     3341 2023-04-11 17:19:06.000000 cooptools-1.7/cooptools/randoms.py
+-rw-rw-rw-   0        0        0      684 2023-02-13 22:06:39.000000 cooptools-1.7/cooptools/register.py
+-rw-rw-rw-   0        0        0     1695 2023-02-23 22:29:37.000000 cooptools-1.7/cooptools/retry.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:59:56.370672 cooptools-1.7/cooptools/sectors/
+-rw-rw-rw-   0        0        0       20 2023-03-07 20:40:12.000000 cooptools-1.7/cooptools/sectors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:59:56.410635 cooptools-1.7/cooptools/sectors/grids/
+-rw-rw-rw-   0        0        0       78 2023-03-07 20:35:41.000000 cooptools-1.7/cooptools/sectors/grids/__init__.py
+-rw-rw-rw-   0        0        0     1253 2022-09-19 21:08:23.000000 cooptools-1.7/cooptools/sectors/grids/gridState.py
+-rw-rw-rw-   0        0        0     3529 2023-04-12 13:39:47.000000 cooptools-1.7/cooptools/sectors/grids/grid_base.py
+-rw-rw-rw-   0        0        0     2394 2022-11-10 19:53:54.000000 cooptools-1.7/cooptools/sectors/grids/hexGrid.py
+-rw-rw-rw-   0        0        0     3024 2023-03-07 20:35:41.000000 cooptools-1.7/cooptools/sectors/grids/rectGrid.py
+-rw-rw-rw-   0        0        0     7122 2022-11-12 19:13:30.000000 cooptools-1.7/cooptools/sectors/hex_utils.py
+-rw-rw-rw-   0        0        0     8027 2022-11-21 15:30:38.000000 cooptools-1.7/cooptools/sectors/rect_utils.py
+-rw-rw-rw-   0        0        0      337 2022-10-13 14:34:53.000000 cooptools-1.7/cooptools/sectors/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:59:56.417635 cooptools-1.7/cooptools/statistics/
+-rw-rw-rw-   0        0        0       47 2021-10-05 19:39:56.000000 cooptools-1.7/cooptools/statistics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:59:56.435635 cooptools-1.7/cooptools/statistics/controlChart/
+-rw-rw-rw-   0        0        0        0 2022-02-19 23:10:39.000000 cooptools-1.7/cooptools/statistics/controlChart/__init__.py
+-rw-rw-rw-   0        0        0    13265 2022-11-10 23:04:03.000000 cooptools-1.7/cooptools/statistics/controlChart/controlChart.py
+-rw-rw-rw-   0        0        0     7937 2022-11-12 19:13:30.000000 cooptools-1.7/cooptools/statistics/controlChart/plotting.py
+-rw-rw-rw-   0        0        0     1677 2022-06-03 13:34:45.000000 cooptools-1.7/cooptools/timeWindow.py
+-rw-rw-rw-   0        0        0     3168 2022-06-23 21:58:42.000000 cooptools-1.7/cooptools/timedDecay.py
+-rw-rw-rw-   0        0        0     5204 2022-12-31 04:29:20.000000 cooptools-1.7/cooptools/toggles.py
+-rw-rw-rw-   0        0        0     1553 2022-11-10 23:12:40.000000 cooptools-1.7/cooptools/trends.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:59:56.444635 cooptools-1.7/cooptools/triggerActionSystem/
+-rw-rw-rw-   0        0        0        0 2023-02-09 23:42:35.000000 cooptools-1.7/cooptools/triggerActionSystem/__init__.py
+-rw-rw-rw-   0        0        0      247 2023-02-10 00:02:03.000000 cooptools-1.7/cooptools/triggerActionSystem/trigger.py
+-rw-rw-rw-   0        0        0     3098 2023-02-14 19:51:35.000000 cooptools-1.7/cooptools/typevalidation.py
+-rw-rw-rw-   0        0        0     2375 2022-11-30 23:33:22.000000 cooptools-1.7/cooptools/version.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:59:56.216639 cooptools-1.7/cooptools.egg-info/
+-rw-rw-rw-   0        0        0      770 2023-05-30 16:59:55.000000 cooptools-1.7/cooptools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2101 2023-05-30 16:59:55.000000 cooptools-1.7/cooptools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 16:59:55.000000 cooptools-1.7/cooptools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-08-30 22:37:58.000000 cooptools-1.7/cooptools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      171 2023-05-30 16:59:55.000000 cooptools-1.7/cooptools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 16:59:55.000000 cooptools-1.7/cooptools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 16:59:56.446636 cooptools-1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1197 2023-05-30 16:56:37.000000 cooptools-1.7/setup.py
```

### Comparing `cooptools-1.6/PKG-INFO` & `cooptools-1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cooptools
-Version: 1.6
+Version: 1.7
 Summary: Generic Tooling
 Home-page: https://github.com/tylertjburns/cooptools
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cooptools-1.6/cooptools/anchor.py` & `cooptools-1.7/cooptools/anchor.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/colors.py` & `cooptools-1.7/cooptools/colors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 from enum import Enum
-from typing import Tuple
+from typing import Tuple, List
 import random as rnd
 
-def random_rgb():
-    r = rnd.randint(0, 255)
-    g = rnd.randint(0, 255)
-    b = rnd.randint(0, 255)
+def random_rgb(r_range: Tuple[int, int] = None,
+               g_range: Tuple[int, int] = None,
+               b_range: Tuple[int, int] = None):
+    if r_range is None:
+        r_range = (0, 255)
+
+    if g_range is None:
+        g_range = (0, 255)
+
+    if b_range is None:
+        b_range = (0, 255)
+
+    r = rnd.randint(*r_range)
+    g = rnd.randint(*g_range)
+    b = rnd.randint(*b_range)
 
     return (r, g, b)
 
 class Color(Enum):
     # LEGACY
     LIGHT_RED = 255, 204, 204
     BRIGHT_BLUE = 0, 100, 255
@@ -196,14 +207,21 @@
 
     @classmethod
     def random(cls):
         rnd_rgb = random_rgb()
         return cls.closest_color(rnd_rgb)
 
     @classmethod
+    def choice(cls,
+               excluded: List = None,
+               vibrancy_range: Tuple[int, int] = None):
+        return rnd.choice([color for color in Color if color not in (set(excluded) if excluded is not None else set())  # Color not in one of the background used colors
+                    and ((vibrancy_range[0] <= sum(color.value) <= vibrancy_range[1]) if vibrancy_range is not None else True)])  # Force towards vibrant colors
+
+    @classmethod
     def as_hex(cls, rgb):
         return '#%02x%02x%02x' % rgb
 
     @classmethod
     def from_hex(cls, hex, exact: bool = False):
         value = hex.lstrip('#')
         lv = len(value)
```

### Comparing `cooptools-1.6/cooptools/commandDesignPattern/commandController.py` & `cooptools-1.7/cooptools/commandDesignPattern/commandController.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/commandDesignPattern/commandProtocol.py` & `cooptools-1.7/cooptools/commandDesignPattern/commandProtocol.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/common.py` & `cooptools-1.7/cooptools/common.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/coopEnum.py` & `cooptools-1.7/cooptools/coopEnum.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/coopthreading.py` & `cooptools-1.7/cooptools/coopthreading.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/dataRefresher/dataHub.py` & `cooptools-1.7/cooptools/dataRefresher/dataHub.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/dataRefresher/dataRefresher.py` & `cooptools-1.7/cooptools/dataRefresher/dataRefresher.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/date_utils.py` & `cooptools-1.7/cooptools/date_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,14 +86,23 @@
         DateIncrementType.MONTH: lambda x: x.replace(day=1, hour=0, minute=0, second=0, microsecond=0) if x is not None else None,
         DateIncrementType.YEAR: lambda x: x.replace(month=1, day=1, hour=0, minute=0, second=0, microsecond=0) if x is not None else None,
         None: lambda x: x
     }
 
     return [grouper_switch[grouping_method](datestamp_tryParse(x)) for x in date_stamps]
 
+def yesterday():
+    return datestamp_tryParse(datetime.datetime.today() - datetime.timedelta(days=1), include_time=False)
+
+def today():
+    return datestamp_tryParse(datetime.datetime.today(), include_time=False)
+
+def tomorrow():
+    return datestamp_tryParse(datetime.datetime.today() + datetime.timedelta(days=1), include_time=False)
+
 if __name__ == "__main__":
     # print(bucket_datestamp([datetime.datetime.now()], grouping_method=DateIncrementType.SECOND))
     # print(bucket_datestamp(['x'], grouping_method=DateIncrementType.YEAR))
     # print(bucket_datestamp([datetime.datetime.now()], grouping_method=None))
 
     from pprint import pprint
     start = '1/1/23 5:00'
```

### Comparing `cooptools-1.6/cooptools/decor.py` & `cooptools-1.7/cooptools/decor.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/dictPolicies.py` & `cooptools-1.7/cooptools/dictPolicies.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/discreteEventSimulator/discreteEventSimulator.py` & `cooptools-1.7/cooptools/discreteEventSimulator/discreteEventSimulator.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/geometry_utils/circle_utils.py` & `cooptools-1.7/cooptools/geometry_utils/circle_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,17 @@
                   degrees: float = None) -> Tuple[float, float]:
     if rads is None and degrees is None:
         raise ValueError(f"Either radians or degress must have a value")
 
     if rads is None:
         rads = degree_to_rads(degrees)
 
+    if center is None:
+        center = (0, 0)
+
     radius = distance_between(point, center)
     pt_rads = rads_of_point_around_origin(point, center)
     rotated_rads = pt_rads + rads
 
     return point_at_angle(center=center, radius=radius, radians=rotated_rads)
```

### Comparing `cooptools-1.6/cooptools/geometry_utils/curve_utils.py` & `cooptools-1.7/cooptools/geometry_utils/curve_utils.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/geometry_utils/line_utils.py` & `cooptools-1.7/cooptools/geometry_utils/line_utils.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/geometry_utils/rect_utils.py` & `cooptools-1.7/cooptools/geometry_utils/rect_utils.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/geometry_utils/triangle_utils.py` & `cooptools-1.7/cooptools/geometry_utils/triangle_utils.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/geometry_utils/vector_utils.py` & `cooptools-1.7/cooptools/geometry_utils/vector_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,100 +1,123 @@
 from typing import Tuple, Optional, List
 import math
 import numpy as np
 from cooptools.common import verify_len, verify_len_match, divided_length
 
-def homogeneous_vector(dim: int, val: float = None) -> Tuple[float, ...]:
+FloatVec = Tuple[float, ...]
+
+def homogeneous_vector(dim: int, val: float = None) -> FloatVec:
     if val is None:
         val = 0
     return tuple([val for x in range(dim)])
 
-def identity_vector(dim: int) -> Tuple[float, ...]:
+def identity_vector(dim: int) -> FloatVec:
     return homogeneous_vector(dim, 1)
 
-def zero_vector(dim: int) -> Tuple[float, ...]:
+def zero_vector(dim: int) -> FloatVec:
     return homogeneous_vector(dim)
 
-def vector_between(start: Tuple[float, ...], end: Tuple[float, ...]) -> Tuple[float, ...]:
+def vector_between(start: FloatVec, end: FloatVec) -> FloatVec:
     verify_len_match(start, end)
 
     ret = []
     for idx in range(len(start)):
         ret.append((end[idx] - start[idx]))
 
     return tuple(ret)
 
-def add_vectors(vectors: List[Tuple[float, ...]]) -> Tuple[float, ...]:
 
-    running_sum = None
+def _add_two_vectors(a: FloatVec, b: FloatVec) -> FloatVec:
+    mx = max(len(a), len(b))
+
+    ret = []
+
+    for ii in range(mx):
+        if ii < len(a) and ii < len(b):
+            ret.append(a[ii] + b[ii])
+        elif ii < len(a):
+            ret.append(a[ii])
+        else:
+            ret.append(b[ii])
+
+    return tuple(ret)
+
 
-    add_two_vecs = lambda a, b: tuple([sum(x) for x in zip(a, b)])
+def add_vectors(vectors: List[FloatVec], allow_diff_lengths: bool = False) -> FloatVec:
+    running_sum = None
 
     for vec in vectors:
         if running_sum is None:
             running_sum = vec
         else:
-            verify_len_match(running_sum, vec)
-            running_sum = add_two_vecs(running_sum, vec)
+            if not allow_diff_lengths:
+                verify_len_match(running_sum, vec)
+
+            running_sum = _add_two_vectors(running_sum, vec)
 
     return running_sum
 
-def scale_vector_length(a: Tuple[float, ...], scale: float) -> Tuple[float, ...]:
+def subtract_vectors(a: FloatVec, b: FloatVec, allow_diff_lengths: bool = False) -> FloatVec:
+    b_calc = tuple(-1 * x for x in b)
+    return add_vectors([a, b_calc], allow_diff_lengths=allow_diff_lengths)
+
+
+def scale_vector_length(a: FloatVec, scale: float) -> FloatVec:
     scale_vector = homogeneous_vector(len(a), scale)
     return hadamard_product(a, scale_vector)
 
 
-def vector_len(a: Tuple[float, ...]) -> float:
+def vector_len(a: FloatVec) -> float:
     sum = 0
     for ii in a:
         sum += ii ** 2
     return math.sqrt(sum)
 
-def distance_between(a: Tuple[float, ...], b: Tuple[float, ...]) -> float:
+def distance_between(a: FloatVec, b: FloatVec) -> float:
     verify_len_match(a, b)
 
     vec_bet = vector_between(a, b)
     return vector_len(vec_bet)
 
-def unit_vector(a: Tuple[float, ...]) -> Optional[Tuple[float, ...]]:
+def unit_vector(a: FloatVec) -> Optional[FloatVec]:
     vec_len = vector_len(a)
     if vec_len == 0:
         return None
 
     ret = []
     for coord in a:
         ret.append(coord / vec_len)
     return tuple(ret)
 
-def scaled_to_length(a: Tuple[float, ...], desired_length: float) -> Tuple[float, ...]:
+def scaled_to_length(a: FloatVec, desired_length: float) -> FloatVec:
     u_vec = unit_vector(a)
 
     if u_vec is None:
         return homogeneous_vector(len(a))
 
     ret = []
     for ii in range(len(u_vec)):
         ret.append(u_vec[ii] * desired_length)
 
     return tuple(ret)
 
 
-def interpolate(a: Tuple[float, ...],
-                b: Tuple[float, ...],
-                amount: float = 0.5) -> Tuple[float, ...]:
+def interpolate(a: FloatVec,
+                b: FloatVec,
+                amount: float = 0.5) -> FloatVec:
 
     delta_v = vector_between(start=a, end=b)
     scaled_delta_v = scale_vector_length(delta_v, amount)
 
     return add_vectors([a, scaled_delta_v])
 
 def segmented_vector(inc: float,
-                   start: Tuple[float, ...],
-                   stop: Tuple[float, ...],
-                   force_to_ends: bool = False) -> List[Tuple[float, ...]]:
+                   start: FloatVec,
+                   stop: FloatVec,
+                   force_to_ends: bool = False) -> List[FloatVec]:
 
     delta = vector_between(start, stop)
     max_len = vector_len(delta)
 
     inc_vec = scaled_to_length(a=delta, desired_length=inc)
 
     ii = start
@@ -113,88 +136,99 @@
 
 
     return vals
 
 
 
 
-def absolute(a: Tuple[float, ...]) -> Tuple[float, ...]:
+def absolute(a: FloatVec) -> FloatVec:
     ret = []
     for coord in range(len(a)):
         ret.append(abs(coord))
 
     return tuple(ret)
 
-def dot(a: Tuple[float, ...],
-        b: Tuple[float, ...]) -> float:
+def dot(a: FloatVec,
+        b: FloatVec) -> float:
     return float(np.dot(a, b))
 
-def cross(a: Tuple[float, ...],
-          b: Tuple[float, ...]) -> Tuple[float, ...]:
+def cross(a: FloatVec,
+          b: FloatVec) -> FloatVec:
     return tuple(np.cross(a, b))
 
 
-def hadamard_product(a: Tuple[float, ...],
-                     b: Tuple[float, ...]) -> Tuple[float, ...]:
-    verify_len_match(a, b)
+def hadamard_product(a: FloatVec,
+                     b: FloatVec,
+                     allow_different_lengths: bool = False) -> FloatVec:
+    if not allow_different_lengths:
+        verify_len_match(a, b)
+
+    mx = max(len(a), len(b))
 
     ret = []
-    for ii in range(len(a)):
-        ret.append(a[ii] * b[ii])
+    for ii in range(mx):
+        if ii < len(a) and ii < len(b):
+            ret.append(a[ii] * b[ii])
+        elif ii < len(a):
+            ret.append(a[ii])
+        else:
+            ret.append(b[ii])
 
     return tuple(ret)
 
-def hadamard_division(a: Tuple[float, ...],
-                      b: Tuple[float, ...]) -> Tuple[float, ...]:
-    scale_vector = tuple([1/val for val in b])
-    return hadamard_product(a, scale_vector)
 
-def project_onto(a: Tuple[float, ...],
-                 b: Tuple[float, ...],
-                 origin: Tuple[float, ...] = None) -> Tuple[float, ...]:
+def hadamard_division(a: FloatVec,
+                      b: FloatVec,
+                      allow_different_lengths: bool = False) -> FloatVec:
+    scale_vector = tuple([1 / val for val in b])
+    return hadamard_product(a, scale_vector, allow_different_lengths)
+
+def project_onto(a: FloatVec,
+                 b: FloatVec,
+                 origin: FloatVec = None) -> FloatVec:
 
     verify_len_match(a, b)
 
     if origin is None:
         origin = zero_vector(len(a))
 
     e1 = vector_between(origin, end=b)
     e2 = vector_between(origin, end=a)
 
     # https://gamedev.stackexchange.com/questions/72528/how-can-i-project-a-3d-point-onto-a-3d-line
     return add_vectors([origin, scale_vector_length(e1, dot(e2, e1) / dot(e1, e1))])
 
-def pts_in_threshold(a: Tuple[float, ...],
-                     pts: List[Tuple[float, ...]],
-                     distance_threshold: float = None) -> List[Tuple[Tuple[float, ...], float]]:
+def pts_in_threshold(a: FloatVec,
+                     pts: List[FloatVec],
+                     distance_threshold: float = None) -> List[Tuple[FloatVec, float]]:
     if distance_threshold is not None and distance_threshold < 0:
         raise ValueError(f"distance_threshold must be greater than zero, but {distance_threshold} was provided")
 
     qualifiers = []
     for other in pts:
         distance = distance_between(a, other)
         if distance_threshold is None or distance < distance_threshold:
             qualifiers.append((other, distance))
 
     return qualifiers
 
-def closest_point(a: Tuple[float, ...],
-                  pts: List[Tuple[float, ...]],
-                  distance_threshold: float = None) -> Optional[Tuple[float, ...]]:
+def closest_point(a: FloatVec,
+                  pts: List[FloatVec],
+                  distance_threshold: float = None) -> Optional[FloatVec]:
 
     qualifiers = pts_in_threshold(a, pts, distance_threshold=distance_threshold)
 
     if len(qualifiers) == 0:
         return None
 
     min_dist = min([x[1] for x in qualifiers])
 
     return next(iter([x[0] for x in qualifiers if x[1] == min_dist]), None)
 
-def bounded_by(a: Tuple[float, ...], b: Tuple[float, ...], c: Tuple[float, ...]) -> bool:
+def bounded_by(a: FloatVec, b: FloatVec, c: FloatVec) -> bool:
 
     verify_len_match(a, b)
     verify_len_match(a, c)
 
     for ii in range(len(a)):
         min_val = min(b[ii], c[ii])
         max_val = max(b[ii], c[ii])
```

### Comparing `cooptools-1.6/cooptools/jsonIO.py` & `cooptools-1.7/cooptools/jsonIO.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/marchingSquares.py` & `cooptools-1.7/cooptools/marchingSquares.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/matrixManipulation.py` & `cooptools-1.7/cooptools/matrixManipulation.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/metrics.py` & `cooptools-1.7/cooptools/metrics.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/os_manip.py` & `cooptools-1.7/cooptools/os_manip.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,119 @@
 import os
 import shutil
 import logging
 import json
 from enum import Enum
-from typing import List, Tuple
+from typing import List, Tuple, Union, Callable
 import ntpath
+import struct
+import imghdr
 
 LOCALAPP_ROOT = 'LOCALAPPDATA'
-
+logger = logging.getLogger('cooptools.os_manip')
 
 class FileType(Enum):
     JSON = ".json"
     TXT = ".txt"
     CSV = ".csv"
     INI = ".ini"
 
 
+def files_at_dir(directory):
+    # iterate over files in
+    # that directory
+    ret = []
+    for filename in os.scandir(directory):
+        if filename.is_file():
+            ret.append(rf"{directory}\{filename.name}")
+    return ret
+
+filePathProvider = Union[str, Callable[[], str]]
+
+def resolve_absolute_filepath(file_path: filePathProvider):
+    if file_path is None:
+        return None
+
+    if type(file_path) == str:
+        return file_path
+
+    try:
+        return file_path()
+    except Exception as e:
+        logger.error(f"Unable to resolve the file path: {e}")
+        return None
+
+def check_file_exists(file_path: filePathProvider):
+    fp = resolve_absolute_filepath(file_path)
+    return fp is not None and os.path.exists(fp)
+
+def verify_file_exists(file_path: filePathProvider):
+    # verify path exists
+    if not check_file_exists(file_path):
+        raise Exception(f"No valid file at {resolve_absolute_filepath(file_path)}")
+
+
+def path_and_file(filepath: str):
+    head, tail = ntpath.split(filepath)
+    tail = tail or ntpath.basename(head)
+    return head, tail
+
+def copy_file_from_to(filepath_to_copy: str, to_filepath: str):
+    shutil.copy2(filepath_to_copy, to_filepath)
+
+
+def write_data(data, file_path, make_dir: bool = True):
+    if make_dir:
+        check_and_make_dirs(os.path.dirname(file_path))
+
+    with open(file_path, 'w') as outfile:
+        ret = outfile.write(data)
+        return ret
+
+
+def read_data(file_path):
+    with open(file_path, 'r+') as outfile:
+        ret = outfile.read()
+        return ret
+
+
+def try_write_data(data, file_path):
+    ret = None
+    try:
+        ret = write_data(data=data, file_path=file_path)
+    except Exception as e:
+        logging.error(f"Unable to write file: {file_path}: {e}")
+
+    return ret
+
+
+def try_read_data(file_path):
+    ret = None
+    try:
+        ret = read_data(file_path)
+    except Exception as e:
+        logging.error(f"Unable to read file: {file_path}: {e}")
+    return ret
+
+def rename_files(filepaths: List[str],
+                 replace: List[Tuple[str, str]] = None,
+                 remove_spaces: bool = False):
+    for path in filepaths:
+        src = path
+        path, filename = path_and_file(path)
+
+        new = filename
+        for rep in replace or []:
+            new = new.replace(rep[0], rep[1])
+
+        if remove_spaces:
+            new = new.replace(' ', '')
+
+        os.rename(src=src, dst=fr"{path}\{new}")
+
 def check_and_make_new_proj_localapp(app_root, proj_name):
     """ Verifies that the app_root exists at LOCALAPPDATA and then verifies that a subfolder exists at that directory
     for the proj_name.
     :return the full directory path to the proj_name
     """
     root = check_and_make_localapp_application_path_dir(app_root)
     return check_and_make_proj_path_dir(root, proj_name)
@@ -152,101 +246,95 @@
     return filepath_at_check_and_make_dir(app_path, file_name, file_type)
 
 
 def filepath_at_check_and_make_app_proj_dir(app_root, proj_name, file_name, file_type: FileType = None):
     proj_path = check_and_make_new_proj_localapp(app_root, proj_name)
     return filepath_at_check_and_make_dir(proj_path, file_name, file_type)
 
-
-def copy_file_from_to(filepath_to_copy: str, to_filepath: str):
-    shutil.copy2(filepath_to_copy, to_filepath)
-
-
 def try_save_jsonable_data(my_jsonable_data, file_path, cls: json.JSONEncoder = None):
-        accepted_method_names = ['toJson', 'to_json', 'tojson']
-        to_json_method = next(iter(getattr(my_jsonable_data, x, None) for x in accepted_method_names), None)
-        if to_json_method and callable(to_json_method):
-            my_json = json.dumps(to_json_method(), indent=4, cls=cls)
-        else:
-            my_json = json.dumps(my_jsonable_data, indent=4, cls=cls)
+    accepted_method_names = ['toJson', 'to_json', 'tojson']
+    to_json_method = next(iter(getattr(my_jsonable_data, x, None) for x in accepted_method_names), None)
+    if to_json_method and callable(to_json_method):
+        data = to_json_method()
+    else:
+        data = json.dumps(my_jsonable_data, indent=4, cls=cls)
+
+    return try_write_data(data, file_path)
 
-        return try_save_json_data(my_json_data=my_json, file_path=file_path)
 
-def try_save_json_data(my_json_data, file_path):
-    check_and_make_dirs(os.path.dirname(file_path))
-    with open(file_path, 'w') as outfile:
-        try:
-            outfile.write(my_json_data)
-        except Exception as e:
-            logging.error(f"Unable to write file: {file_path}: {e}")
+def load_json_data_to_dict(file_path, cls: json.JSONEncoder = None):
+    data = read_data(file_path)
+    ret = json.loads(data, cls=cls)
+    return ret
 
-def try_load_json_data(file_path, cls: json.JSONEncoder = None):
-    ret = None
 
-    if not os.path.isfile(file_path):
-        return None
+def try_load_json_data_to_dict(file_path, cls: json.JSONEncoder = None):
+    data = try_read_data(file_path)
+    ret = None
+    if data is not None:
+        ret = json.loads(data, cls=cls)
 
-    with open(file_path, 'r+') as outfile:
-        try:
-            ret = json.load(outfile, cls=cls)
-        except Exception as e:
-            logging.error(f"Unable to read file: {file_path}: {e}")
     return ret
 
-
 def save_application_json(my_jsonable_data, app_root, filename: str):
     file_path = filepath_at_check_and_make_app_dir(app_root, filename, file_type=FileType.JSON)
     return try_save_jsonable_data(my_jsonable_data, file_path)
 
 
 def save_project_json(my_jsonable_data, app_root, project_name, filename: str):
     file_path = filepath_at_check_and_make_app_proj_dir(app_root, project_name, filename, file_type=FileType.JSON)
     return try_save_jsonable_data(my_jsonable_data, file_path)
 
 
 def load_application_json(app_root, filename):
     file_path = filepath_at_check_and_make_app_dir(app_root, filename, file_type=FileType.JSON)
-    return try_load_json_data(file_path)
+    return try_load_json_data_to_dict(file_path)
 
 
 def load_project_json(app_root, project, filename):
     proj_dir = check_and_make_new_proj_localapp(app_root, project)
     file_path = f"{proj_dir}\\{filename}.json"
-    return try_load_json_data(file_path)
+    return try_load_json_data_to_dict(file_path)
 
-def files_at_dir(directory):
-    # iterate over files in
-    # that directory
-    ret = []
-    for filename in os.scandir(directory):
-        if filename.is_file():
-            ret.append(rf"{directory}\{filename.name}")
-    return ret
-
-def path_and_file(filepath: str):
-    head, tail = ntpath.split(filepath)
-    tail = tail or ntpath.basename(head)
-    return head, tail
-
-
-def rename_files(filepaths: List[str],
-                 replace: List[Tuple[str, str]] = None,
-                 remove_spaces: bool = False):
-    for path in filepaths:
-        src = path
-        path, filename = path_and_file(path)
 
-        new = filename
-        for rep in replace or []:
-            new = new.replace(rep[0], rep[1])
-
-        if remove_spaces:
-            new = new.replace(' ', '')
 
-        os.rename(src=src, dst=fr"{path}\{new}")
+def get_image_size(fname):
+    '''Determine the image type of fhandle and return its size.
+    from draco'''
+    with open(fname, 'rb') as fhandle:
+        head = fhandle.read(24)
+        if len(head) != 24:
+            return
+        if imghdr.what(fname) == 'png':
+            check = struct.unpack('>i', head[4:8])[0]
+            if check != 0x0d0a1a0a:
+                return
+            width, height = struct.unpack('>ii', head[16:24])
+        elif imghdr.what(fname) == 'gif':
+            width, height = struct.unpack('<HH', head[6:10])
+        elif imghdr.what(fname) == 'jpeg':
+            try:
+                fhandle.seek(0)  # Read 0xff next
+                size = 2
+                ftype = 0
+                while not 0xc0 <= ftype <= 0xcf:
+                    fhandle.seek(size, 1)
+                    byte = fhandle.read(1)
+                    while ord(byte) == 0xff:
+                        byte = fhandle.read(1)
+                    ftype = ord(byte)
+                    size = struct.unpack('>H', fhandle.read(2))[0] - 2
+                # We are at a SOFn block
+                fhandle.seek(1, 1)  # Skip `precision' byte.
+                height, width = struct.unpack('>HH', fhandle.read(4))
+            except Exception:  # IGNORE:W0703
+                return
+        else:
+            return
+        return width, height
 
 if __name__ == "__main__":
 
 
     files = files_at_dir(r'C:\Users\tburns\Downloads\zombiefiles\png\male')
     rename_files(filepaths=files, replace=[('(', '__0'),
                                            (')', ''),
```

### Comparing `cooptools-1.6/cooptools/pandasHelpers.py` & `cooptools-1.7/cooptools/pandasHelpers.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/plotting.py` & `cooptools-1.7/cooptools/plotting.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/printing.py` & `cooptools-1.7/cooptools/printing.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/randoms.py` & `cooptools-1.7/cooptools/randoms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Dict, Any, Tuple
 import numpy.random as nrnd
 import datetime
 import random as rnd
+import string
 
-LETTERS = 'abcdefghijklmnopqrstuvwxyz'
+LETTERS = string.ascii_lowercase
 NUMBERS = '1234567890'
 CHARS = '!@#$%^&*()-_=+[{]};:"/?.>,<`~'
 
 def weighted_random_choice(choices_dict: Dict[Any, float], seed: int = None):
     if seed is not None:
         rnd.seed(seed)
```

### Comparing `cooptools-1.6/cooptools/register.py` & `cooptools-1.7/cooptools/register.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/retry.py` & `cooptools-1.7/cooptools/retry.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/sectors/grids/gridState.py` & `cooptools-1.7/cooptools/sectors/grids/gridState.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/sectors/grids/grid_base.py` & `cooptools-1.7/cooptools/sectors/grids/grid_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,16 +52,22 @@
         for policy in policies:
             if policy.key not in self.grid[row][column].state.keys():
                 self._init_a_new_policy(policy)
             policy.act_on_dict(self.grid[row][column].state)
 
         return self.grid[row][column]
 
-    def state_value_as_array(self, keys: List[str]):
-        return np.array([[[self.grid[row][column].state[key] for key in keys]
+    def filtered_array_by_keys(self, keys: List[str]):
+        return np.array([[
+            {key: self.grid[row][column].state[key] for key in keys}
+                            for column in range(self.nColumns)]
+                            for row in range(self.nRows)])
+
+    def state_value_as_array(self, key: str):
+        return np.array([[self.grid[row][column].state[key]
                             for column in range(self.nColumns)]
                             for row in range(self.nRows)])
 
     def _eqls_or_in(self, val, collection):
         if type(collection) in [Set, List]:
             return val in collection
         else:
```

### Comparing `cooptools-1.6/cooptools/sectors/grids/hexGrid.py` & `cooptools-1.7/cooptools/sectors/grids/hexGrid.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/sectors/grids/rectGrid.py` & `cooptools-1.7/cooptools/sectors/grids/rectGrid.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/sectors/hex_utils.py` & `cooptools-1.7/cooptools/sectors/hex_utils.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/sectors/rect_utils.py` & `cooptools-1.7/cooptools/sectors/rect_utils.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/statistics/controlChart/controlChart.py` & `cooptools-1.7/cooptools/statistics/controlChart/controlChart.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/statistics/controlChart/plotting.py` & `cooptools-1.7/cooptools/statistics/controlChart/plotting.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/timeWindow.py` & `cooptools-1.7/cooptools/timeWindow.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/timedDecay.py` & `cooptools-1.7/cooptools/timedDecay.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/toggles.py` & `cooptools-1.7/cooptools/toggles.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/trends.py` & `cooptools-1.7/cooptools/trends.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/typevalidation.py` & `cooptools-1.7/cooptools/typevalidation.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools/version.py` & `cooptools-1.7/cooptools/version.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/cooptools.egg-info/PKG-INFO` & `cooptools-1.7/cooptools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cooptools
-Version: 1.6
+Version: 1.7
 Summary: Generic Tooling
 Home-page: https://github.com/tylertjburns/cooptools
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cooptools-1.6/cooptools.egg-info/SOURCES.txt` & `cooptools-1.7/cooptools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cooptools-1.6/setup.py` & `cooptools-1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as f:
     README = f.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(name='cooptools',
-      version='1.06',
+      version='1.07',
       description='Generic Tooling',
       url='https://github.com/tylertjburns/cooptools',
       author='tburns',
       author_email='tyler.tj.burns@gmail.com',
       license='MIT',
       packages=setuptools.find_packages(),
       python_requires=">3.5",
```

