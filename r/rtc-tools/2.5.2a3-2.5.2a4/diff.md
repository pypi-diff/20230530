# Comparing `tmp/rtc-tools-2.5.2a3.tar.gz` & `tmp/rtc-tools-2.5.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtc-tools-2.5.2a3.tar", last modified: Tue May 16 09:48:45 2023, max compression
+gzip compressed data, was "rtc-tools-2.5.2a4.tar", last modified: Tue May 30 10:06:46 2023, max compression
```

## Comparing `rtc-tools-2.5.2a3.tar` & `rtc-tools-2.5.2a4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:48:45.651263 rtc-tools-2.5.2a3/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/COPYING.LESSER
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1184 2023-05-16 09:48:45.651263 rtc-tools-2.5.2a3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      750 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      388 2023-05-16 09:48:45.652263 rtc-tools-2.5.2a3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2016 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:48:45.629262 rtc-tools-2.5.2a3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:48:45.635262 rtc-tools-2.5.2a3/src/rtc_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1184 2023-05-16 09:48:45.000000 rtc-tools-2.5.2a3/src/rtc_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2071 2023-05-16 09:48:45.000000 rtc-tools-2.5.2a3/src/rtc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 09:48:45.000000 rtc-tools-2.5.2a3/src/rtc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      151 2023-05-16 09:48:45.000000 rtc-tools-2.5.2a3/src/rtc_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-05-16 09:48:45.000000 rtc-tools-2.5.2a3/src/rtc_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-16 09:48:45.000000 rtc-tools-2.5.2a3/src/rtc_tools.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:48:45.652263 rtc-tools-2.5.2a3/src/rtctools/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:48:45.638262 rtc-tools-2.5.2a3/src/rtctools/_internal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/_internal/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5336 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/_internal/alias_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      903 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/_internal/caching.py
--rw-rw-rw-   0 root         (0) root         (0)     2243 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/_internal/casadi_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1084 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/_internal/debug_check_helpers.py
--rw-r--r--   0 root         (0) root         (0)      499 2023-05-16 09:48:45.652263 rtc-tools-2.5.2a3/src/rtctools/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:48:45.640262 rtc-tools-2.5.2a3/src/rtctools/data/
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4947 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/csv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:48:45.642263 rtc-tools-2.5.2a3/src/rtctools/data/interpolation/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/interpolation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      958 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/interpolation/bspline.py
--rw-rw-rw-   0 root         (0) root         (0)     5985 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/interpolation/bspline1d.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/interpolation/bspline2d.py
--rw-rw-rw-   0 root         (0) root         (0)    18692 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/netcdf.py
--rw-rw-rw-   0 root         (0) root         (0)    43530 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/pi.py
--rw-rw-rw-   0 root         (0) root         (0)     8853 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/rtc.py
--rw-rw-rw-   0 root         (0) root         (0)    13011 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:48:45.649263 rtc-tools-2.5.2a3/src/rtctools/optimization/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   116480 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/collocated_integrated_optimization_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     9026 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/control_tree_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    16651 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/csv_lookup_table_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11624 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/csv_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    31608 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    41999 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/goal_programming_mixin_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6782 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/homotopy_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3126 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/initial_state_estimation_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11817 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/io_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/linearization_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     8736 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/linearized_order_goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    13293 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/min_abs_goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    16198 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/modelica_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     7259 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/netcdf_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    43074 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/optimization_problem.py
--rw-rw-rw-   0 root         (0) root         (0)    10783 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/pi_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    25126 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/single_pass_goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1753 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)     4193 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/rtctoolsapp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:48:45.650263 rtc-tools-2.5.2a3/src/rtctools/simulation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/simulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6606 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/simulation/csv_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     6163 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/simulation/io_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     8922 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/simulation/pi_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    35341 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/simulation/simulation_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     7371 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/util.py
--rw-rw-rw-   0 root         (0) root         (0)    68611 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 10:06:46.452332 rtc-tools-2.5.2a4/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/COPYING.LESSER
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-05-30 10:06:46.452332 rtc-tools-2.5.2a4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      750 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      388 2023-05-30 10:06:46.453332 rtc-tools-2.5.2a4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 10:06:46.442332 rtc-tools-2.5.2a4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 10:06:46.444332 rtc-tools-2.5.2a4/src/rtc_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-05-30 10:06:46.000000 rtc-tools-2.5.2a4/src/rtc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2071 2023-05-30 10:06:46.000000 rtc-tools-2.5.2a4/src/rtc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 10:06:46.000000 rtc-tools-2.5.2a4/src/rtc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-30 10:06:46.000000 rtc-tools-2.5.2a4/src/rtc_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-05-30 10:06:46.000000 rtc-tools-2.5.2a4/src/rtc_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-30 10:06:46.000000 rtc-tools-2.5.2a4/src/rtc_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 10:06:46.453332 rtc-tools-2.5.2a4/src/rtctools/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 10:06:46.446332 rtc-tools-2.5.2a4/src/rtctools/_internal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/_internal/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5336 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/_internal/alias_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      903 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/_internal/caching.py
+-rw-rw-rw-   0 root         (0) root         (0)     2243 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/_internal/casadi_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/_internal/debug_check_helpers.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-30 10:06:46.453332 rtc-tools-2.5.2a4/src/rtctools/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 10:06:46.447332 rtc-tools-2.5.2a4/src/rtctools/data/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4947 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/csv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 10:06:46.448332 rtc-tools-2.5.2a4/src/rtctools/data/interpolation/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/interpolation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      958 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/interpolation/bspline.py
+-rw-rw-rw-   0 root         (0) root         (0)     5985 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/interpolation/bspline1d.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/interpolation/bspline2d.py
+-rw-rw-rw-   0 root         (0) root         (0)    18692 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/netcdf.py
+-rw-rw-rw-   0 root         (0) root         (0)    43530 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/pi.py
+-rw-rw-rw-   0 root         (0) root         (0)     8853 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/rtc.py
+-rw-rw-rw-   0 root         (0) root         (0)    13011 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/data/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 10:06:46.451332 rtc-tools-2.5.2a4/src/rtctools/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   117456 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/collocated_integrated_optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     9026 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/control_tree_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    16651 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/csv_lookup_table_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11624 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/csv_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    31608 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    41999 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/goal_programming_mixin_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6782 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/homotopy_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3126 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/initial_state_estimation_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    12558 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/io_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/linearization_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8736 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/linearized_order_goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    13293 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/min_abs_goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    16198 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/modelica_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     7259 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/netcdf_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    43494 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)    10783 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/pi_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    25126 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/single_pass_goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1753 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/optimization/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)     4193 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/rtctoolsapp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 10:06:46.452332 rtc-tools-2.5.2a4/src/rtctools/simulation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/simulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6606 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/simulation/csv_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6163 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/simulation/io_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8922 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/simulation/pi_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    35341 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/simulation/simulation_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     8905 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/src/rtctools/util.py
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2023-05-30 10:06:41.000000 rtc-tools-2.5.2a4/versioneer.py
```

### Comparing `rtc-tools-2.5.2a3/COPYING.LESSER` & `rtc-tools-2.5.2a4/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/PKG-INFO` & `rtc-tools-2.5.2a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtc-tools
-Version: 2.5.2a3
+Version: 2.5.2a4
 Summary: Toolbox for control and optimization of water systems.
 Home-page: https://oss.deltares.nl/web/rtc-tools/home
 Author: Deltares
 Maintainer: Deltares
 License: UNKNOWN
 Download-URL: http://gitlab.com/deltares/rtc-tools/
 Platform: Windows
```

### Comparing `rtc-tools-2.5.2a3/README.md` & `rtc-tools-2.5.2a4/README.md`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/setup.py` & `rtc-tools-2.5.2a4/setup.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtc_tools.egg-info/PKG-INFO` & `rtc-tools-2.5.2a4/src/rtc_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtc-tools
-Version: 2.5.2a3
+Version: 2.5.2a4
 Summary: Toolbox for control and optimization of water systems.
 Home-page: https://oss.deltares.nl/web/rtc-tools/home
 Author: Deltares
 Maintainer: Deltares
 License: UNKNOWN
 Download-URL: http://gitlab.com/deltares/rtc-tools/
 Platform: Windows
```

### Comparing `rtc-tools-2.5.2a3/src/rtc_tools.egg-info/SOURCES.txt` & `rtc-tools-2.5.2a4/src/rtc_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/_internal/alias_tools.py` & `rtc-tools-2.5.2a4/src/rtctools/_internal/alias_tools.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/_internal/caching.py` & `rtc-tools-2.5.2a4/src/rtctools/_internal/caching.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/_internal/casadi_helpers.py` & `rtc-tools-2.5.2a4/src/rtctools/_internal/casadi_helpers.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/_internal/debug_check_helpers.py` & `rtc-tools-2.5.2a4/src/rtctools/_internal/debug_check_helpers.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/data/csv.py` & `rtc-tools-2.5.2a4/src/rtctools/data/csv.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/data/interpolation/bspline.py` & `rtc-tools-2.5.2a4/src/rtctools/data/interpolation/bspline.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/data/interpolation/bspline1d.py` & `rtc-tools-2.5.2a4/src/rtctools/data/interpolation/bspline1d.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/data/interpolation/bspline2d.py` & `rtc-tools-2.5.2a4/src/rtctools/data/interpolation/bspline2d.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/data/netcdf.py` & `rtc-tools-2.5.2a4/src/rtctools/data/netcdf.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/data/pi.py` & `rtc-tools-2.5.2a4/src/rtctools/data/pi.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/data/rtc.py` & `rtc-tools-2.5.2a4/src/rtctools/data/rtc.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/data/storage.py` & `rtc-tools-2.5.2a4/src/rtctools/data/storage.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/optimization/collocated_integrated_optimization_problem.py` & `rtc-tools-2.5.2a4/src/rtctools/optimization/collocated_integrated_optimization_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
         # Call super
         super().__init__(**kwargs)
 
     @abstractmethod
     def times(self, variable=None):
         """
-        List of time stamps for variable.
+        List of time stamps for variable (to optimize for).
 
         :param variable: Variable name.
 
         :returns: A list of time stamps for the given variable.
         """
         pass
 
@@ -209,25 +209,33 @@
 
         # Calculate nominals for the initial derivatives. We assume that the
         # history has (roughly) identical time steps for the entire ensemble.
         self.__initial_derivative_nominals = {}
         history_0 = self.history(0)
         for variable, initial_der_name in zip(self.__differentiated_states, self.__initial_derivative_names):
             times = self.times(variable)
+            default_time_step_size = 0
+            if len(times) > 1:
+                default_time_step_size = times[1] - times[0]
             try:
                 h = history_0[variable]
                 if h.times[0] == times[0] or len(h.values) == 1:
-                    dt = times[1] - times[0]
+                    dt = default_time_step_size
                 else:
                     assert h.times[-1] == times[0]
                     dt = h.times[-1] - h.times[-2]
             except KeyError:
-                dt = times[1] - times[0]
+                dt = default_time_step_size
 
-            self.__initial_derivative_nominals[initial_der_name] = self.variable_nominal(variable) / dt
+            if dt > 0:
+                self.__initial_derivative_nominals[initial_der_name] = (
+                    self.variable_nominal(variable) / dt)
+            else:
+                self.__initial_derivative_nominals[initial_der_name] = (
+                    self.variable_nominal(variable))
 
         if self.integrated_states:
             warnings.warn("Integrated states are deprecated and support will be removed in a future version.",
                           FutureWarning, stacklevel=1)
 
         # Variables that are integrated states are not yet allowed to have size > 1
         for variable in self.integrated_states:
@@ -940,30 +948,33 @@
         # Save the accumulated inputs such that can be used later in map_path_expression()
         self.__func_accumulated_inputs = (
             accumulated_X, accumulated_U,
             ca.veccat(symbolic_parameters, symbolic_extra_variables))
 
         # Use map/mapaccum to capture integration and collocation constraint generation over the
         # entire time horizon with one symbolic operation. This saves a lot of memory.
-        if len(integrated_variables) > 0:
-            accumulated = ca.Function(
-                'accumulated',
-                self.__func_accumulated_inputs,
-                [accumulated_Y[0], ca.vertcat(*accumulated_Y[1:])],
-                function_options)
-            accumulation = accumulated.mapaccum('accumulation', n_collocation_times - 1)
+        if n_collocation_times > 1:
+            if len(integrated_variables) > 0:
+                accumulated = ca.Function(
+                    'accumulated',
+                    self.__func_accumulated_inputs,
+                    [accumulated_Y[0], ca.vertcat(*accumulated_Y[1:])],
+                    function_options)
+                accumulation = accumulated.mapaccum('accumulation', n_collocation_times - 1)
+            else:
+                # Fully collocated problem. Use map(), so that we can use
+                # parallelization along the time axis.
+                accumulated = ca.Function(
+                    'accumulated',
+                    self.__func_accumulated_inputs,
+                    [ca.vertcat(*accumulated_Y)],
+                    function_options)
+                accumulation = accumulated.map(n_collocation_times - 1, 'openmp')
         else:
-            # Fully collocated problem. Use map(), so that we can use
-            # parallelization along the time axis.
-            accumulated = ca.Function(
-                'accumulated',
-                self.__func_accumulated_inputs,
-                [ca.vertcat(*accumulated_Y)],
-                function_options)
-            accumulation = accumulated.map(n_collocation_times - 1, 'openmp')
+            accumulation = None
 
         # Start collecting constraints
         f = []
         g = []
         lbg = []
         ubg = []
 
@@ -1215,21 +1226,27 @@
                  ca.repmat(ca.vertcat(parameters, extra_variables), 1, n_collocation_times - 1)))
 
             self.__func_initial_inputs.append([parameters, ca.vertcat(
                 initial_state, initial_derivatives, initial_constant_inputs, 0.0,
                 initial_path_variables, initial_extra_constant_inputs),
                 extra_variables])
 
-            integrators_and_collocation_and_path_constraints = accumulation(
-                *self.__func_mapped_inputs[ensemble_member])
+            if accumulation is not None:
+                integrators_and_collocation_and_path_constraints = accumulation(
+                    *self.__func_mapped_inputs[ensemble_member])
+            else:
+                integrators_and_collocation_and_path_constraints = None
 
-            if len(integrated_variables) > 0:
+            if accumulation is not None and len(integrated_variables) > 0:
                 integrators = integrators_and_collocation_and_path_constraints[0]
                 integrators_and_collocation_and_path_constraints = integrators_and_collocation_and_path_constraints[1]
-            if integrators_and_collocation_and_path_constraints.numel() > 0:
+            if (
+                accumulation is not None and
+                integrators_and_collocation_and_path_constraints.numel() > 0
+            ):
                 collocation_constraints = ca.vec(integrators_and_collocation_and_path_constraints[
                     :dae_residual_collocated_size,
                     0:n_collocation_times - 1])
                 discretized_path_objective = ca.vec(integrators_and_collocation_and_path_constraints[
                     dae_residual_collocated_size:dae_residual_collocated_size + path_objective.size1(),
                     0:n_collocation_times - 1])
                 discretized_path_constraints = ca.vec(integrators_and_collocation_and_path_constraints[
@@ -2107,18 +2124,21 @@
         x, _ = self.__states_times_in(variable, t0, tf, ensemble_member)
 
         return x
 
     def integral(self, variable, t0=None, tf=None, ensemble_member=0):
         x, t = self.__states_times_in(variable, t0, tf, ensemble_member)
 
-        # Integrate knots using trapezoid rule
-        x_avg = 0.5 * (x[:x.size1() - 1] + x[1:])
-        dt = t[1:] - t[:x.size1() - 1]
-        return ca.sum1(x_avg * dt)
+        if x.size1() > 1:
+            # Integrate knots using trapezoid rule
+            x_avg = 0.5 * (x[:x.size1() - 1] + x[1:])
+            dt = t[1:] - t[:x.size1() - 1]
+            return ca.sum1(x_avg * dt)
+        else:
+            return ca.MX(0)
 
     def der(self, variable):
         # Look up the derivative variable for the given non-derivative variable
         canonical, sign = self.alias_relation.canonical_signed(variable)
         try:
             i = self.__differentiated_states_map[canonical]
             return sign * self.dae_variables['derivatives'][i]
@@ -2187,18 +2207,22 @@
         initial_values = f(*self.__func_initial_inputs[ensemble_member])
 
         # Replace the original MX symbols with those that were mapped
         [expr_impl] = f.call(self.__func_inputs_implicit)
         f_impl = ca.Function('f_implicit', list(self.__func_accumulated_inputs), [expr_impl]).expand()
 
         # Map
-        fmap = f_impl.map(len(self.times()) - 1)
-        values = fmap(*self.__func_mapped_inputs[ensemble_member])
+        number_of_timeslots = len(self.times())
+        if number_of_timeslots > 1:
+            fmap = f_impl.map(number_of_timeslots - 1)
+            values = fmap(*self.__func_mapped_inputs[ensemble_member])
 
-        all_values = ca.horzcat(initial_values, values)
+            all_values = ca.horzcat(initial_values, values)
+        else:
+            all_values = initial_values
 
         return ca.transpose(all_values)
 
     def solver_success(self, *args, **kwargs):
         self.__debug_check_state_output_scaling()
 
         return super().solver_success(*args, **kwargs)
```

### Comparing `rtc-tools-2.5.2a3/src/rtctools/optimization/control_tree_mixin.py` & `rtc-tools-2.5.2a4/src/rtctools/optimization/control_tree_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/optimization/csv_lookup_table_mixin.py` & `rtc-tools-2.5.2a4/src/rtctools/optimization/csv_lookup_table_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/optimization/csv_mixin.py` & `rtc-tools-2.5.2a4/src/rtctools/optimization/csv_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/optimization/goal_programming_mixin.py` & `rtc-tools-2.5.2a4/src/rtctools/optimization/goal_programming_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/optimization/goal_programming_mixin_base.py` & `rtc-tools-2.5.2a4/src/rtctools/optimization/goal_programming_mixin_base.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/optimization/homotopy_mixin.py` & `rtc-tools-2.5.2a4/src/rtctools/optimization/homotopy_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/optimization/initial_state_estimation_mixin.py` & `rtc-tools-2.5.2a4/src/rtctools/optimization/initial_state_estimation_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/optimization/io_mixin.py` & `rtc-tools-2.5.2a4/src/rtctools/optimization/io_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,23 +55,42 @@
     @abstractmethod
     def write(self) -> None:
         """"
         Writes output data to files
         """
         pass
 
-    def times(self, variable=None) -> np.ndarray:
+    def times_from_input(self) -> np.ndarray:
         """
         Returns the times in seconds from the reference datetime onwards.
 
-        :param variable:
+        The times are based on the input data.
         """
         times_sec = self.io.times_sec
-        t_idx = bisect.bisect_left(times_sec, 0.0)
-        return times_sec[t_idx:]
+        time_index = bisect.bisect_left(times_sec, 0.0)
+        times = times_sec[time_index:]
+        return times
+
+    def times(self, variable=None) -> np.ndarray:
+        """
+        Returns the times in seconds from the reference datetime onwards.
+
+        The number of times is based on the number of timesteps to optimize for.
+
+        :param variable: variable name
+        """
+        all_times = self.times_from_input()
+        max_number_of_times = len(all_times)
+        if self._number_of_timesteps_to_optimize is not None:
+            number_of_times = self._number_of_timesteps_to_optimize + 1
+        else:
+            number_of_times = max_number_of_times
+        number_of_times = min(number_of_times, max_number_of_times)
+        times = all_times[:number_of_times]
+        return times
 
     @property
     def equidistant(self):
         return self.__equidistant
 
     @property
     def ensemble_size(self):
```

### Comparing `rtc-tools-2.5.2a3/src/rtctools/optimization/linearization_mixin.py` & `rtc-tools-2.5.2a4/src/rtctools/optimization/linearization_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/optimization/linearized_order_goal_programming_mixin.py` & `rtc-tools-2.5.2a4/src/rtctools/optimization/linearized_order_goal_programming_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/optimization/min_abs_goal_programming_mixin.py` & `rtc-tools-2.5.2a4/src/rtctools/optimization/min_abs_goal_programming_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/optimization/modelica_mixin.py` & `rtc-tools-2.5.2a4/src/rtctools/optimization/modelica_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/optimization/netcdf_mixin.py` & `rtc-tools-2.5.2a4/src/rtctools/optimization/netcdf_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/optimization/optimization_problem.py` & `rtc-tools-2.5.2a4/src/rtctools/optimization/optimization_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 
 
 class OptimizationProblem(DataStoreAccessor, metaclass=ABCMeta):
     """
     Base class for all optimization problems.
     """
 
+    # Number of time steps to optimize for. If None, optimize for all timesteps.
+    _number_of_timesteps_to_optimize = None
+    # Options for debug checks.
     _debug_check_level = DebugLevel.MEDIUM
     _debug_check_options = {}
 
     def __init__(self, **kwargs):
         # Call parent class first for default behaviour.
         super().__init__(**kwargs)
 
@@ -192,14 +195,21 @@
                 'Skipping Postprocessing in OptimizationProblem.optimize()')
 
         # Done
         logger.info("Done with optimize()")
 
         return success
 
+    @classmethod
+    def set_number_of_timesteps_to_optimize(cls, number_of_timesteps_to_optimize):
+        """
+        Set the number of timesteps for which to optimize.
+        """
+        cls._number_of_timesteps_to_optimize = number_of_timesteps_to_optimize
+
     def __check_bounds_control_input(self) -> None:
         # Checks if at the control inputs have bounds, log warning when a control input is not bounded.
         bounds = self.bounds()
 
         for variable in self.dae_variables['control_inputs']:
             variable = variable.name()
             if variable not in bounds:
```

### Comparing `rtc-tools-2.5.2a3/src/rtctools/optimization/pi_mixin.py` & `rtc-tools-2.5.2a4/src/rtctools/optimization/pi_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/optimization/single_pass_goal_programming_mixin.py` & `rtc-tools-2.5.2a4/src/rtctools/optimization/single_pass_goal_programming_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/optimization/timeseries.py` & `rtc-tools-2.5.2a4/src/rtctools/optimization/timeseries.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/rtctoolsapp.py` & `rtc-tools-2.5.2a4/src/rtctools/rtctoolsapp.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/simulation/csv_mixin.py` & `rtc-tools-2.5.2a4/src/rtctools/simulation/csv_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/simulation/io_mixin.py` & `rtc-tools-2.5.2a4/src/rtctools/simulation/io_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/simulation/pi_mixin.py` & `rtc-tools-2.5.2a4/src/rtctools/simulation/pi_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/simulation/simulation_problem.py` & `rtc-tools-2.5.2a4/src/rtctools/simulation/simulation_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a3/src/rtctools/util.py` & `rtc-tools-2.5.2a4/src/rtctools/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 import sys
 
 import casadi
 
 from . import __version__
 from ._internal.alias_tools import OrderedSet
 from .data import pi
+from .optimization.csv_mixin import CSVMixin as OptimizationCSVMixin
+from .optimization.io_mixin import IOMixin as OptimizationIOMixin
 from .optimization.pi_mixin import PIMixin as OptimizationPIMixin
+from .simulation.csv_mixin import CSVMixin as SimulationCSVMixin
+from .simulation.io_mixin import IOMixin as SimulationIOMixin
 from .simulation.pi_mixin import PIMixin as SimulationPIMixin
 
 
 def _resolve_folder(kwargs, base_folder, subfolder_kw, default):
     subfolder = kwargs.pop(subfolder_kw, default)
     if os.path.isabs(subfolder):
         return subfolder
@@ -40,14 +44,26 @@
     :param base_folder:                Base folder.
     :param log_level:                  The log level to use.
     :param profile:                    Whether or not to enable profiling.
 
     :returns: :class:`.OptimizationProblem` instance.
     """
 
+    # Do some checks on the problem class
+    if issubclass(optimization_problem_class, SimulationCSVMixin):
+        raise ValueError(
+            "Optimization problem class cannot be derived from simulation.csv_mixin.CSVMixin.")
+    if issubclass(optimization_problem_class, SimulationIOMixin):
+        raise ValueError(
+            "Optimization problem class cannot be derived from simulation.csv_mixin.IOMixin.")
+    if issubclass(optimization_problem_class, SimulationPIMixin):
+        raise ValueError(
+            "Optimization problem class cannot be derived from simulation.csv_mixin.PIMixin.")
+
+    # Set input/output folders
     if not os.path.isabs(base_folder):
         # Resolve base folder relative to script folder
         base_folder = os.path.join(sys.path[0], base_folder)
 
     model_folder = _resolve_folder(kwargs, base_folder, 'model_folder', 'model')
     input_folder = _resolve_folder(kwargs, base_folder, 'input_folder', 'input')
     output_folder = _resolve_folder(kwargs, base_folder, 'output_folder', 'output')
@@ -128,22 +144,34 @@
 
 def run_simulation_problem(simulation_problem_class,
                            base_folder='..', log_level=logging.INFO,
                            **kwargs):
     """
     Sets up and runs a simulation problem.
 
-    :param simulation_problem_class: Optimization problem class to solve.
+    :param simulation_problem_class: Simulation problem class to solve.
     :param base_folder:              Folder within which subfolders "input", "output", and "model" exist,
                                      containing input and output data, and the model, respectively.
     :param log_level:                The log level to use.
 
     :returns: :class:`SimulationProblem` instance.
     """
 
+    # Do some checks on the problem class
+    if issubclass(simulation_problem_class, OptimizationCSVMixin):
+        raise ValueError(
+            "Simulation problem class cannot be derived from optimization.csv_mixin.CSVMixin.")
+    if issubclass(simulation_problem_class, OptimizationIOMixin):
+        raise ValueError(
+            "Simulation problem class cannot be derived from optimization.csv_mixin.IOMixin.")
+    if issubclass(simulation_problem_class, OptimizationPIMixin):
+        raise ValueError(
+            "Simulation problem class cannot be derived from optimization.csv_mixin.PIMixin.")
+
+    # Set input/output folders
     if base_folder is None:
         # Check command line arguments
         if len(sys.argv) != 2:
             raise Exception("Usage: {} BASE_FOLDER".format(sys.argv[0]))
 
         base_folder = sys.argv[1]
     else:
```

### Comparing `rtc-tools-2.5.2a3/versioneer.py` & `rtc-tools-2.5.2a4/versioneer.py`

 * *Files identical despite different names*

