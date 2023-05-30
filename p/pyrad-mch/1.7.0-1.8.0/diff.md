# Comparing `tmp/pyrad_mch-1.7.0.tar.gz` & `tmp/pyrad_mch-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrad_mch-1.7.0.tar", last modified: Wed Mar 29 12:57:04 2023, max compression
+gzip compressed data, was "pyrad_mch-1.8.0.tar", last modified: Tue May 30 15:41:13 2023, max compression
```

## Comparing `pyrad_mch-1.7.0.tar` & `pyrad_mch-1.8.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:57:04.228527 pyrad_mch-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-03-29 12:57:04.228527 pyrad_mch-1.7.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:57:04.208526 pyrad_mch-1.7.0/pyrad/
--rwxr-xr-x   0 runner    (1001) docker     (123)      869 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:57:04.208526 pyrad_mch-1.7.0/pyrad/flow/
--rwxr-xr-x   0 runner    (1001) docker     (123)      386 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/flow/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    57239 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/flow/flow_aux.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34809 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/flow/flow_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:57:04.208526 pyrad_mch-1.7.0/pyrad/graph/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3117 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/graph/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    54994 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/graph/plots.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8857 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/graph/plots_aux.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24477 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/graph/plots_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    52389 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/graph/plots_spectra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24330 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/graph/plots_timeseries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    70596 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/graph/plots_vol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:57:04.216527 pyrad_mch-1.7.0/pyrad/io/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7730 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/io/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9281 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/io/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   111430 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/io/io_aux.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3936 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/io/mxpol_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15513 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/io/read_data_cosmo.py
--rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/io/read_data_dem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9542 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/io/read_data_hzt.py
--rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/io/read_data_iso0_mf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37831 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/io/read_data_mxpol.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    57094 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/io/read_data_other.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   182081 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/io/read_data_radar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    78211 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/io/read_data_sensor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15042 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/io/read_data_sun.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7684 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/io/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/io/trajectory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    97871 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/io/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:57:04.220527 pyrad_mch-1.7.0/pyrad/proc/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11653 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/proc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25854 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/proc/process_Doppler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    92971 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/proc/process_aux.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    92202 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/proc/process_calib.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    38434 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/proc/process_cosmo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/proc/process_dem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    93305 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/proc/process_echoclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/proc/process_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    89471 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/proc/process_intercomp.py
--rw-r--r--   0 runner    (1001) docker     (123)    26560 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/proc/process_iq.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    62256 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/proc/process_monitoring.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43276 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/proc/process_phase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    58764 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/proc/process_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)    66245 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/proc/process_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)    47217 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/proc/process_timeseries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    72382 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/proc/process_traj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:57:04.224527 pyrad_mch-1.7.0/pyrad/prod/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2089 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/prod/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30744 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/prod/process_grid_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13183 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/prod/process_intercomp_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31042 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/prod/process_monitoring_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    56567 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/prod/process_product.py
--rw-r--r--   0 runner    (1001) docker     (123)    47103 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/prod/process_spectra_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30674 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/prod/process_timeseries_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5606 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/prod/process_traj_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   154784 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/prod/process_vol_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4392 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/prod/product_aux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:57:04.224527 pyrad_mch-1.7.0/pyrad/util/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2110 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/util/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    61246 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/util/radar_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4908 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/pyrad/util/stat_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-29 12:57:04.000000 pyrad_mch-1.7.0/pyrad/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:57:04.224527 pyrad_mch-1.7.0/pyrad_mch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-03-29 12:57:04.000000 pyrad_mch-1.7.0/pyrad_mch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-03-29 12:57:04.000000 pyrad_mch-1.7.0/pyrad_mch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 12:57:04.000000 pyrad_mch-1.7.0/pyrad_mch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 12:57:03.000000 pyrad_mch-1.7.0/pyrad_mch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-29 12:57:04.000000 pyrad_mch-1.7.0/pyrad_mch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:57:04.228527 pyrad_mch-1.7.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5799 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/scripts/common_colocated_gates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4556 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/scripts/main_precipitation_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/scripts/main_process_cosmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/scripts/main_process_cosmo_rt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6535 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/scripts/main_process_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/scripts/main_process_data_birds.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6393 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/scripts/main_process_data_period.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4434 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/scripts/main_process_data_rt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16283 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/scripts/main_process_data_trt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/scripts/main_process_euclid_data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5965 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/scripts/main_process_gecsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/scripts/movie_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/scripts/rewrite_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 12:57:04.228527 pyrad_mch-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-03-29 12:56:52.000000 pyrad_mch-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.992982 pyrad_mch-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-30 15:41:13.992982 pyrad_mch-1.8.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.980981 pyrad_mch-1.8.0/pyrad/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      869 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.980981 pyrad_mch-1.8.0/pyrad/flow/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      386 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/flow/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57500 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/flow/flow_aux.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34809 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/flow/flow_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.980981 pyrad_mch-1.8.0/pyrad/graph/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3205 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/graph/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54994 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/graph/plots.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13147 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/graph/plots_aux.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45068 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/graph/plots_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52389 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/graph/plots_spectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24330 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/graph/plots_timeseries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    70743 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/graph/plots_vol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.984981 pyrad_mch-1.8.0/pyrad/io/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7748 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9281 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   112893 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/io_aux.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3936 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/mxpol_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15513 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/read_data_cosmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/read_data_dem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9542 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/read_data_hzt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/read_data_iso0_mf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37831 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/read_data_mxpol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57335 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/read_data_other.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   185474 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/read_data_radar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    78210 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/read_data_sensor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15042 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/read_data_sun.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7684 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/trajectory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    97871 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.984981 pyrad_mch-1.8.0/pyrad/proc/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11666 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36329 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_Doppler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    93122 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_aux.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    92202 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_calib.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38434 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_cosmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_dem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    93466 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_echoclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59766 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    89471 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_intercomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26560 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_iq.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    62664 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_monitoring.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43276 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_phase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58764 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66245 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47217 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_timeseries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    72382 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_traj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.988981 pyrad_mch-1.8.0/pyrad/prod/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2089 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38966 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/process_grid_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13183 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/process_intercomp_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31042 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/process_monitoring_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    56567 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/process_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47103 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/process_spectra_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30674 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/process_timeseries_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5606 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/process_traj_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   154784 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/process_vol_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4392 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/product_aux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.988981 pyrad_mch-1.8.0/pyrad/util/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2110 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/util/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    61246 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/util/radar_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4908 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/util/stat_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-30 15:41:13.000000 pyrad_mch-1.8.0/pyrad/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.988981 pyrad_mch-1.8.0/pyrad_mch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-30 15:41:13.000000 pyrad_mch-1.8.0/pyrad_mch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-30 15:41:13.000000 pyrad_mch-1.8.0/pyrad_mch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:41:13.000000 pyrad_mch-1.8.0/pyrad_mch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:41:13.000000 pyrad_mch-1.8.0/pyrad_mch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 15:41:13.000000 pyrad_mch-1.8.0/pyrad_mch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.992982 pyrad_mch-1.8.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5799 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/common_colocated_gates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4556 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_precipitation_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_process_cosmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_process_cosmo_rt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6535 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_process_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_process_data_birds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6393 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_process_data_period.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4434 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_process_data_rt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16283 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_process_data_trt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_process_euclid_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5965 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_process_gecsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/movie_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/rewrite_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 15:41:13.992982 pyrad_mch-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/setup.py
```

### Comparing `pyrad_mch-1.7.0/PKG-INFO` & `pyrad_mch-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrad_mch
-Version: 1.7.0
+Version: 1.8.0
 Summary:  Python Radar Toolkit
 Home-page: https://github.com/MeteoSwiss/pyrad.git
 Author: MeteoSwiss Pyrad Developers
 Author-email: daniel.wolfensberger@meteoswiss.ch
 Maintainer: MeteoSwiss Pyrad Developers
 Maintainer-email: daniel.wolfensberger@meteoswiss.ch
 License: BSD
```

### Comparing `pyrad_mch-1.7.0/pyrad/__init__.py` & `pyrad_mch-1.8.0/pyrad/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/flow/flow_aux.py` & `pyrad_mch-1.8.0/pyrad/flow/flow_aux.py`

 * *Files 1% similar despite different names*

```diff
@@ -977,14 +977,16 @@
         cfg.update({'dempath': None})
     if 'smnpath' not in cfg:
         cfg.update({'smnpath': None})
     if 'disdropath' not in cfg:
         cfg.update({'disdropath': None})
     if 'solarfluxpath' not in cfg:
         cfg.update({'solarfluxpath': None})
+    if 'selfconsistencypath' not in cfg:
+        cfg.update({'selfconsistencypath': None})
     if 'loadbasepath' not in cfg:
         cfg.update({'loadbasepath': None})
     if 'loadname' not in cfg:
         cfg.update({'loadname': None})
     if 'RadarName' not in cfg:
         cfg.update({'RadarName': None})
     if 'RadarRes' not in cfg:
@@ -1300,14 +1302,15 @@
     dscfg.update({'path_convention': cfg['path_convention']})
     dscfg.update({'procname': cfg['name']})
     dscfg.update({'dsname': dataset})
     dscfg.update({'solarfluxpath': cfg['solarfluxpath']})
     dscfg.update({'colocgatespath': cfg['colocgatespath']})
     dscfg.update({'excessgatespath': cfg['excessgatespath']})
     dscfg.update({'dempath': cfg['dempath']})
+    dscfg.update({'selfconsistencypath': cfg['selfconsistencypath']})
     dscfg.update({'cosmopath': cfg['cosmopath']})
     dscfg.update({'CosmoRunFreq': cfg['CosmoRunFreq']})
     dscfg.update({'CosmoForecasted': cfg['CosmoForecasted']})
     dscfg.update({'metranet_read_lib': cfg['metranet_read_lib']})
     dscfg.update({'lastStateFile': cfg['lastStateFile']})
     dscfg.update({'timeinfo': None})
 
@@ -1396,14 +1399,16 @@
         prdcfg.update({'RadarBeamwidth': cfg['RadarBeamwidth']})
     if 'ppiImageConfig' in cfg:
         prdcfg.update({'ppiImageConfig': cfg['ppiImageConfig']})
     if 'ppiMapImageConfig' in cfg:
         prdcfg.update({'ppiMapImageConfig': cfg['ppiMapImageConfig']})
     if 'rhiImageConfig' in cfg:
         prdcfg.update({'rhiImageConfig': cfg['rhiImageConfig']})
+    if 'xsecImageConfig' in cfg:
+        prdcfg.update({'xsecImageConfig': cfg['xsecImageConfig']})
     if 'gridMapImageConfig' in cfg:
         prdcfg.update({'gridMapImageConfig': cfg['gridMapImageConfig']})
     if 'sunhitsImageConfig' in cfg:
         prdcfg.update({'sunhitsImageConfig': cfg['sunhitsImageConfig']})
     prdcfg.update({'dsname': dataset})
     prdcfg.update({'dstype': cfg[dataset]['type']})
     prdcfg.update({'prdname': product})
```

### Comparing `pyrad_mch-1.7.0/pyrad/flow/flow_control.py` & `pyrad_mch-1.8.0/pyrad/flow/flow_control.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/graph/__init__.py` & `pyrad_mch-1.8.0/pyrad/graph/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 
     plot_ray
     plot_surface_raw
     plot_surface
     plot_latitude_slice
     plot_longitude_slice
     plot_latlon_slice
+    plot_dda_map
+    plot_dda_latitude_slice
+    plot_dda_longitude_slice
     plot_ppi
     plot_ppi_contour
     plot_ppi_map
     plot_rhi
     plot_rhi_contour
     plot_bscope
     plot_fixed_rng
@@ -82,15 +85,15 @@
 from .plots_vol import plot_time_range, plot_cappi, plot_rhi_profile
 from .plots_vol import plot_along_coord, plot_field_coverage, plot_traj
 from .plots_vol import plot_rhi_contour, plot_ppi_contour, plot_ray
 from .plots_vol import plot_fixed_rng, plot_fixed_rng_span, plot_roi_contour
 from .plots_vol import plot_fixed_rng_sun
 
 from .plots_grid import plot_surface_raw, plot_surface, plot_latitude_slice
-from .plots_grid import plot_longitude_slice, plot_latlon_slice
+from .plots_grid import plot_longitude_slice, plot_latlon_slice, plot_dda_map
 
 from .plots_spectra import plot_range_Doppler, plot_complex_range_Doppler
 from .plots_spectra import plot_amp_phase_range_Doppler, plot_Doppler
 from .plots_spectra import plot_complex_Doppler, plot_amp_phase_Doppler
 from .plots_spectra import plot_time_Doppler, plot_complex_time_Doppler
 from .plots_spectra import plot_amp_phase_time_Doppler, plot_angle_Doppler
 from .plots_spectra import plot_complex_angle_Doppler
```

### Comparing `pyrad_mch-1.7.0/pyrad/graph/plots.py` & `pyrad_mch-1.8.0/pyrad/graph/plots.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/graph/plots_aux.py` & `pyrad_mch-1.8.0/pyrad/graph/plots_aux.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,14 +8,17 @@
     :toctree: generated/
 
     generate_complex_range_Doppler_title
     generate_angle_Doppler_title
     generate_complex_Doppler_title
     generate_fixed_rng_span_title
     generate_fixed_rng_title
+    generate_dda_map_title
+    generate_dda_latitude_slice_title
+    generate_dda_longitude_slice_title
     get_colobar_label
     get_field_name
     get_norm
 
 """
 
 import numpy as np
@@ -26,15 +29,16 @@
 mpl.use('Agg')
 
 # Increase a bit font size
 mpl.rcParams.update({'font.size': 16})
 mpl.rcParams.update({'font.family':  "sans-serif"})
 
 
-def generate_complex_range_Doppler_title(radar, field, ray, datetime_format=None):
+def generate_complex_range_Doppler_title(radar, field, ray,
+                                         datetime_format=None):
     """
     creates the fixed range plot title
 
     Parameters
     ----------
     radar : radar
         The radar object
@@ -203,14 +207,150 @@
         time_str = begin_time.isoformat() + 'Z'
     l1 = "%s %.1f m. %s " % (pyart.graph.common.generate_radar_name(radar),
                              fixed_rng, time_str)
     field_name = pyart.graph.common.generate_field_name(radar, field)
     return l1 + '\n' + field_name
 
 
+def generate_dda_map_title(grid, field, level, datetime_format=None):
+    """
+    creates the dda map plot title
+
+    Parameters
+    ----------
+    grid : grid
+        The grid object
+    field : str
+        name of the background field
+    level : int
+        Verical level plotted.
+    datetime_format : str or None
+        The date time format to use
+
+    Returns
+    -------
+    titl : str
+        The plot title
+
+    """
+    begin_time = pyart.graph.common.generate_radar_time_begin(grid)
+    if datetime_format:
+        time_str = begin_time.strftime(datetime_format)
+    else:
+        time_str = begin_time.isoformat() + 'Z'
+    radar_names = pyart.graph.common.generate_radar_name(grid)
+
+    for mdata in grid.metadata['additional_radars']:
+        radar_names += '-' + mdata['radar_name']
+    height = grid.z["data"][level] / 1000.0
+    l1 = f"DDA: {radar_names} {height:.1f} km {time_str}"
+    field_name = "Hor. wind vectors (u,v) with " + field
+    return l1 + '\n' + field_name
+
+
+def generate_dda_latitude_slice_title(grid, field, level, datetime_format=None,
+                                      wind_vectors='hor'):
+    """
+    creates the dda latitude slice plot title
+
+    Parameters
+    ----------
+    grid : grid
+        The grid object
+    field : str
+        name of the background field
+    level : int
+        latitudinal level plotted.
+    datetime_format : str or None
+        The date time format to use
+    wind_vectors : str
+        'hor' if horizontal wind vectors are displayed (u and v) or 'ver'
+        if vertical wind vectors are displayed (v and w)
+
+    Returns
+    -------
+    titl : str
+        The plot title
+
+    """
+    begin_time = pyart.graph.common.generate_radar_time_begin(grid)
+    if datetime_format:
+        time_str = begin_time.strftime(datetime_format)
+    else:
+        time_str = begin_time.isoformat() + 'Z'
+    radar_names = pyart.graph.common.generate_radar_name(grid)
+
+    for mdata in grid.metadata['additional_radars']:
+        radar_names += '-' + mdata['radar_name']
+    disp = grid.x["data"][level] / 1000.0
+    if disp >= 0:
+        direction = "east"
+    else:
+        direction = "west"
+        disp = -disp
+
+    l1 = f"DDA: {radar_names} {disp:.1f} km {direction} of origin {time_str}"
+    if wind_vectors == 'hor':
+        field_name = "Hor. wind vectors (u,v)"
+    elif wind_vectors == 'ver':
+        field_name = "Vert. wind vectors (v,w)"
+    field_name += ' with ' + field
+    return l1 + '\n' + field_name
+
+
+def generate_dda_longitude_slice_title(grid, field, level,
+                                       datetime_format=None,
+                                       wind_vectors='hor'):
+    """
+    creates the dda longitude slice plot title
+
+    Parameters
+    ----------
+    grid : grid
+        The grid object
+    field : str
+        name of the background field
+    level : int
+        longitudinal level plotted.
+    datetime_format : str or None
+        The date time format to use
+    wind_vectors : str
+        'hor' if horizontal wind vectors are displayed (u and v) or 'ver'
+        if vertical wind vectors are displayed (v and w)
+
+    Returns
+    -------
+    titl : str
+        The plot title
+
+    """
+    begin_time = pyart.graph.common.generate_radar_time_begin(grid)
+    if datetime_format:
+        time_str = begin_time.strftime(datetime_format)
+    else:
+        time_str = begin_time.isoformat() + 'Z'
+    radar_names = pyart.graph.common.generate_radar_name(grid)
+
+    for mdata in grid.metadata['additional_radars']:
+        radar_names += '-' + mdata['radar_name']
+    disp = grid.x["data"][level] / 1000.0
+    if disp >= 0:
+        direction = "north"
+    else:
+        direction = "south"
+        disp = -disp
+    l1 = f"DDA: {radar_names} {disp:.1f} km {direction} of origin {time_str}"
+    if wind_vectors == 'hor':
+        field_name = "Hor. wind vectors (u,v)"
+    elif wind_vectors == 'ver':
+        field_name = "Vert. wind vectors (v,w)"
+    field_name += ' with ' + field
+    return l1 + '\n' + field_name
+
+
 def get_colobar_label(field_dict, field_name):
     """
     creates the colorbar label using field metadata
 
     Parameters
     ----------
     field_dict : dict
@@ -264,32 +404,33 @@
         field_name = str(field)
     field_name = field_name.replace('_', ' ')
     field_name = field_name[0].upper() + field_name[1:]
 
     return field_name
 
 
-def get_norm(field_name, field_dict={}, isxarray = False):
+def get_norm(field_name, field_dict={}, isxarray=False):
     """
     Computes the normalization of the colormap, and gets the ticks and labels
     of the colorbar from the metadata of the field. Returns None if the
     required parameters are not present in the metadata. If field dict is
     not None the metadata is obtained directly from the field. Otherwise it is
     obtained from the Py-ART config file
 
     Parameters
     ----------
     field_name : str
         name of the field
     field_dict : dict or None
         dictionary containing the field and its metadata.
     isxarray : bool
-        whether or not the norm will be used with xarray's plotting functions 
-        default is false, which means that matplotlib plotting functions will be used
-        should be set to true when plotting Grid objects which are handled as xarray by pyart
+        whether or not the norm will be used with xarray's plotting functions
+        default is false, which means that matplotlib plotting functions will
+        be used should be set to true when plotting Grid objects which are
+        handled as xarray by pyart
     Returns
     -------
     norm : list
         the colormap index
     ticks : list
         the list of ticks in the colorbar
     labels : list
@@ -297,25 +438,28 @@
 
     """
     norm = None
     ticks = None
     ticklabs = None
 
     ref_dict = pyart.config.get_metadata(field_name)
-    cmap = mpl.cm.get_cmap(pyart.config.get_field_colormap(field_name))
-    
-    if isxarray:
-        ncolors = len(field_dict['boundaries']) - 1
-    else:
-        ncolors = cmap.N
+    cmap = mpl.colormaps[pyart.config.get_field_colormap(field_name)]
 
     if field_dict is not None and 'boundaries' in field_dict:
+        if isxarray:
+            ncolors = len(field_dict['boundaries']) - 1
+        else:
+            ncolors = cmap.N
         norm = mpl.colors.BoundaryNorm(
             boundaries=field_dict['boundaries'], ncolors=ncolors)
     elif 'boundaries' in ref_dict:
+        if isxarray:
+            ncolors = len(ref_dict['boundaries']) - 1
+        else:
+            ncolors = cmap.N
         norm = mpl.colors.BoundaryNorm(
             boundaries=ref_dict['boundaries'], ncolors=ncolors)
 
     if field_dict is not None and 'ticks' in field_dict:
         ticks = field_dict['ticks']
         if 'labels' in field_dict:
             ticklabs = field_dict['labels']
```

### Comparing `pyrad_mch-1.7.0/pyrad/graph/plots_spectra.py` & `pyrad_mch-1.8.0/pyrad/graph/plots_spectra.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/graph/plots_timeseries.py` & `pyrad_mch-1.8.0/pyrad/graph/plots_timeseries.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/graph/plots_vol.py` & `pyrad_mch-1.8.0/pyrad/graph/plots_vol.py`

 * *Files 0% similar despite different names*

```diff
@@ -490,16 +490,20 @@
             norm, ticks, ticklabs = get_norm(
                 field_name, field_dict=radar.fields[field_name])
             vmin = None
             vmax = None
 
         xsize = prdcfg['rhiImageConfig']['xsize']
         ysize = prdcfg['rhiImageConfig']['ysize']
+        if 'aspect' in prdcfg['rhiImageConfig']:
+            aspect = prdcfg['rhiImageConfig']['aspect']
+        else:
+            aspect = 'equal'
         fig = plt.figure(figsize=[xsize, ysize], dpi=dpi)
-        ax = fig.add_subplot(111, aspect='equal')
+        ax = fig.add_subplot(111, aspect=aspect)
         display = pyart.graph.RadarDisplay(radar)
         display.plot_rhi(
             field_name, title=titl, sweep=ind_az, norm=norm, ticks=ticks,
             ticklabs=ticklabs, vmin=vmin, vmax=vmax,
             colorbar_orient='horizontal',  fig=fig, ax=ax)
         display.set_limits(
             ylim=[prdcfg['rhiImageConfig']['ymin'],
```

### Comparing `pyrad_mch-1.7.0/pyrad/io/__init__.py` & `pyrad_mch-1.8.0/pyrad/io/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,15 @@
     read_histogram
     read_quantiles
     read_profile_ts
     read_histogram_ts
     read_quantiles_ts
     read_ml_ts
     read_windmills_data
+    read_windcube
 
 Writing data
 ==================
 
 .. autosummary::
     :toctree: generated/
```

### Comparing `pyrad_mch-1.7.0/pyrad/io/config.py` & `pyrad_mch-1.8.0/pyrad/io/config.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/io/io_aux.py` & `pyrad_mch-1.8.0/pyrad/io/io_aux.py`

 * *Files 1% similar despite different names*

```diff
@@ -1891,14 +1891,16 @@
         field_name = 'vol2bird_background'
     elif datatype == 'VOL2BIRD_BIOLOGY':
         field_name = 'vol2bird_biology'
 
     # wind lidar names
     elif datatype == 'wind_vel_rad':
         field_name = 'radial_wind_speed'
+    elif datatype == 'wind_vel_rad_filtered':
+        field_name = 'corrected_radial_wind_speed'
     elif datatype == 'wind_vel_rad_ci':
         field_name = 'radial_wind_speed_ci'
     elif datatype == 'wind_vel_rad_status':
         field_name = 'radial_wind_speed_status'
     elif datatype == 'WD':
         field_name = 'doppler_spectrum_width'
     elif datatype == 'WD_err':
@@ -2241,28 +2243,30 @@
     filelist = []
     for starttime, endtime in zip(starttimes, endtimes):
         startdate = starttime.replace(
             hour=0, minute=0, second=0, microsecond=0)
         enddate = endtime.replace(hour=0, minute=0, second=0, microsecond=0)
         ndays = int((enddate-startdate).days)+1
         t_filelist = []
+        pattern = None
         for i in range(ndays):
             if datagroup == 'RAINBOW':
                 if scan is None:
                     warn('Unknown scan name')
                     return []
                 daydir = (
                     starttime+datetime.timedelta(days=i)).strftime('%Y-%m-%d')
                 dayinfo = (starttime+datetime.timedelta(days=i)).strftime(
                     '%Y%m%d')
                 datapath = cfg['datapath'][ind_rad] + scan + daydir + '/'
                 if not os.path.isdir(datapath):
                     warn("WARNING: Unknown datapath '%s'" % datapath)
                     continue
-                dayfilelist = glob.glob(datapath+dayinfo+'*00'+datatype+'.*')
+                pattern = datapath+dayinfo+'*00'+datatype+'.*'
+                dayfilelist = glob.glob(pattern)
                 for filename in dayfilelist:
                     t_filelist.append(filename)
             elif datagroup == 'RAD4ALP':
                 if scan is None:
                     warn('Unknown scan name')
                     return []
 
@@ -2272,15 +2276,16 @@
                     radar_name=cfg['RadarName'][ind_rad],
                     radar_res=cfg['RadarRes'][ind_rad], scan=scan,
                     path_convention=cfg['path_convention'][ind_rad])
 
                 if not os.path.isdir(datapath):
                     warn("WARNING: Unknown datapath '%s'" % datapath)
                     continue
-                dayfilelist = glob.glob(datapath+basename+'*.'+scan+'*')
+                pattern = datapath+basename+'*.'+scan+'*'
+                dayfilelist = glob.glob(pattern)
                 for filename in dayfilelist:
                     t_filelist.append(filename)
             elif datagroup in ('RAD4ALPGRID', 'RAD4ALPGIF', 'RAD4ALPBIN'):
                 acronym, termination = get_rad4alp_prod_fname(datatype)
                 dir_day = starttime+datetime.timedelta(days=i)
                 dayinfo = dir_day.strftime('%y%j')
                 basename = acronym+dayinfo
@@ -2288,30 +2293,30 @@
                 datapath = get_rad4alp_grid_dir(
                     cfg['datapath'][ind_rad], dir_day, datatype, acronym,
                     path_convention=cfg['path_convention'][ind_rad])
 
                 if not os.path.isdir(datapath):
                     warn("WARNING: Unknown datapath '%s'" % datapath)
                     continue
-
-                dayfilelist = glob.glob(datapath+basename+'*'+termination)
+                pattern = datapath+basename+'*'+termination
+                dayfilelist = glob.glob(pattern)
                 for filename in dayfilelist:
                     t_filelist.append(filename)
             elif datagroup == 'SATGRID':
                 daydir = (
                     starttime +
                     datetime.timedelta(days=i)).strftime('%Y/%m/%d/')
                 dayinfo = (starttime+datetime.timedelta(days=i)).strftime(
                     '%Y%m%d')
                 datapath = cfg['satpath'][ind_rad] + daydir
                 if not os.path.isdir(datapath):
                     # warn("WARNING: Unknown datapath '%s'" % datapath)
                     continue
-                dayfilelist = glob.glob(
-                    datapath+'MSG?_ccs4_'+dayinfo+'*_rad_PLAX.nc')
+                pattern = datapath+'MSG?_ccs4_'+dayinfo+'*_rad_PLAX.nc'
+                dayfilelist = glob.glob(pattern)
                 for filename in dayfilelist:
                     t_filelist.append(filename)
 
             elif datagroup in ('ODIM', 'ODIMBIRDS', 'CFRADIAL', 'CFRADIAL2',
                                'CF1', 'NEXRADII', 'GAMIC', 'ODIMGRID'):
                 if scan is None:
                     warn('Unknown scan name')
@@ -2321,15 +2326,16 @@
                         '%y%j')
                     basename = ('M'+cfg['RadarRes'][ind_rad] +
                                 cfg['RadarName'][ind_rad]+dayinfo)
                     datapath = (
                         cfg['datapath'][ind_rad]+dayinfo+'/'+basename+'/')
 
                     # check that M files exist. if not search P files
-                    dayfilelist = glob.glob(datapath+basename+'*'+scan+'*')
+                    pattern = datapath+basename+'*'+scan+'*'
+                    dayfilelist = glob.glob(pattern)
                     if not dayfilelist:
                         basename = ('P'+cfg['RadarRes'][ind_rad] +
                                     cfg['RadarName'][ind_rad]+dayinfo)
                         datapath = (cfg['datapath'][ind_rad]+dayinfo+'/' +
                                     basename+'/')
                     if not os.path.isdir(datapath):
                         warn("WARNING: Unknown datapath '%s'" % datapath)
@@ -2341,27 +2347,42 @@
                     except AttributeError:
                         warn('Unknown ODIM directory and/or date ' +
                              'convention, check product config file')
                     daydir = (
                         starttime+datetime.timedelta(days=i)).strftime(
                             fpath_strf)
                     datapath = (cfg['datapath'][ind_rad]+daydir+'/')
-                    dayfilelist = glob.glob(datapath+'*'+scan+'*')
+                    pattern = datapath+'*'+scan+'*'
+                    dayfilelist = glob.glob(pattern)
+                elif cfg['path_convention'][ind_rad] == 'RADARV':
+                    try:
+                        fpath_strf = dataset[
+                            dataset.find("D")+2:dataset.find("F")-2]
+                    except AttributeError:
+                        warn('Unknown ODIM directory and/or date ' +
+                             'convention, check product config file')
+                    daydir = (
+                        starttime+datetime.timedelta(days=i)).strftime(
+                            fpath_strf)
+                    datapath = (cfg['datapath'][ind_rad]+scan+'/')
+                    pattern = datapath+'/'+daydir+'/*'
+                    dayfilelist = glob.glob(pattern)
                 else:
                     dayinfo = (starttime+datetime.timedelta(days=i)).strftime(
                         '%y%j')
                     basename = ('M'+cfg['RadarRes'][ind_rad] +
                                 cfg['RadarName'][ind_rad]+dayinfo)
                     datapath = (
                         cfg['datapath'][ind_rad]+'M' +
                         cfg['RadarRes'][ind_rad]+cfg['RadarName'][ind_rad] +
                         '/')
 
                     # check that M files exist. if not search P files
-                    dayfilelist = glob.glob(datapath+basename+'*'+scan+'*')
+                    pattern = datapath+basename+'*'+scan+'*'
+                    dayfilelist = glob.glob(pattern)
                     if not dayfilelist:
                         basename = ('P'+cfg['RadarRes'][ind_rad] +
                                     cfg['RadarName'][ind_rad]+dayinfo)
                         datapath = (
                             cfg['datapath'][ind_rad]+'P' +
                             cfg['RadarRes'][ind_rad] +
                             cfg['RadarName'][ind_rad]+'/')
@@ -2386,31 +2407,32 @@
                     '%Y%m%d')
                 datapath = (
                     cfg['loadbasepath'][ind_rad]+cfg['loadname'][ind_rad] +
                     '/'+daydir+'/'+dataset+'/'+product+'/')
                 if not os.path.isdir(datapath):
                     warn("WARNING: Unknown datapath '%s'" % datapath)
                     continue
-                dayfilelist = glob.glob(
-                    datapath+dayinfo+'*'+datatype+termination)
+                pattern = datapath+dayinfo+'*'+datatype+termination
+                dayfilelist = glob.glob(pattern)
                 for filename in dayfilelist:
                     t_filelist.append(filename)
             elif datagroup in ('MFCFRADIAL', 'MFBIN', 'MFPNG', 'MFGRIB',
                                'MFDAT', 'MFCF'):
                 try:
                     fpath_strf = dataset[
                         dataset.find("D")+2:dataset.find("F")-2]
                 except AttributeError:
                     warn('Unknown directory and/or date ' +
                          'convention, check product config file')
                 daydir = (
                     starttime+datetime.timedelta(days=i)).strftime(
                         fpath_strf)
                 datapath = (cfg['datapath'][ind_rad]+daydir+'/')
-                dayfilelist = glob.glob(datapath+'*'+scan+'*')
+                pattern = datapath+'*'+scan+'*'
+                dayfilelist = glob.glob(pattern)
 
                 for filename in dayfilelist:
                     t_filelist.append(filename)
             elif datagroup == 'MXPOL':
                 if scan is None:
                     warn('Unknown scan name')
                     return []
@@ -2420,28 +2442,29 @@
                     sub3 = starttime.strftime('%d')
                     datapath = (
                         cfg['datapath'][ind_rad]+'/'+sub1+'/'+sub2+'/'+sub3 +
                         '/')
                     basename = (
                         'MXPol-polar-'+starttime.strftime('%Y%m%d')+'-*-' +
                         scan+'*')
-                    dayfilelist = glob.glob(datapath+basename)
+                    pattern = datapath+basename
+                    dayfilelist = glob.glob(pattern)
                 else:
                     daydir = (
                         starttime+datetime.timedelta(days=i)).strftime(
                             '%Y-%m-%d')
                     dayinfo = (
                         starttime+datetime.timedelta(days=i)).strftime(
                             '%Y%m%d')
                     datapath = cfg['datapath'][ind_rad]+scan+'/'+daydir+'/'
                     if not os.path.isdir(datapath):
                         warn("WARNING: Unknown datapath '%s'" % datapath)
                         continue
-                    dayfilelist = glob.glob(
-                        datapath+'MXPol-polar-'+dayinfo+'-*-'+scan+'.nc')
+                    pattern = datapath+'MXPol-polar-'+dayinfo+'-*-'+scan+'.nc'
+                    dayfilelist = glob.glob(pattern)
                 for filename in dayfilelist:
                     t_filelist.append(filename)
             elif datagroup == 'COSMORAW':
                 daydir = (starttime+datetime.timedelta(days=i)).strftime(
                     '%Y-%m-%d')
                 dayinfo = (starttime+datetime.timedelta(days=i)).strftime(
                     '%Y%m%d')
@@ -2455,29 +2478,32 @@
                         continue
                 if cfg['path_convention'][ind_rad] == 'MCH':
                     datapath = datapath+daydir+'/'
 
                 if not os.path.isdir(datapath):
                     warn("WARNING: Unknown datapath '%s'" % datapath)
                     continue
-                dayfilelist = glob.glob(datapath+'*'+dayinfo+'*.nc')
+                pattern = datapath+'*'+dayinfo+'*.nc'
+                dayfilelist = glob.glob(pattern)
                 for filename in dayfilelist:
                     t_filelist.append(filename)
 
-        if not t_filelist:
-            continue
-
         for filename in t_filelist:
             filenamestr = str(filename)
             fdatetime = get_datetime(filenamestr, datadescriptor)
             if fdatetime is not None:
                 if starttime <= fdatetime <= endtime:
                     if filenamestr not in filelist:
                         filelist.append(filenamestr)
-
+    
+        if not filelist:
+            if pattern != None:
+                warn("WARNING: No file with pattern {:s} could be found between ".format(pattern)+\
+                    "starttime {:s} and endtime {:s}".format(str(starttime),
+                                                                str(endtime)))
     return sorted(filelist)
 
 
 def get_rad4alp_dir(basepath, voltime, radar_name='A', radar_res='L',
                     scan='001', path_convention='MCH'):
     """
     gets the directory where rad4alp data is stored
@@ -2752,15 +2778,15 @@
             datagroup = 'RAINBOW'
             datatype = descrfields[1]
             dataset = None
             product = None
         else:
             datagroup = descrfields[1]
             if datagroup in ('CFRADIALPYRAD', 'ODIMPYRAD', 'PYRADGRID',
-                             'ODIMPYRADGRID', 'NETCDFSPECTRA', 'CSV'):
+                             'ODIMPYRADGRID', 'NETCDFSPECTRA', 'CSV', 'GECSX'):
                 descrfields2 = descrfields[2].split(',')
                 datatype = descrfields2[0]
                 dataset = descrfields2[1]
                 product = descrfields2[2]
             elif datagroup == 'CFRADIALCOSMO':
                 descrfields2 = descrfields[2].split(',')
                 datatype = descrfields2[0]
```

### Comparing `pyrad_mch-1.7.0/pyrad/io/mxpol_config.py` & `pyrad_mch-1.8.0/pyrad/io/mxpol_config.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/io/read_data_cosmo.py` & `pyrad_mch-1.8.0/pyrad/io/read_data_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/io/read_data_dem.py` & `pyrad_mch-1.8.0/pyrad/io/read_data_dem.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     dem2radar_data
     read_idrisi_data
     read_idrisi_metadata
     _prepare_for_interpolation
 
 
 """
-import os
 import pathlib
 from warnings import warn
 import numpy as np
 import pandas as pd
 from scipy.interpolate import RegularGridInterpolator
 
 # check existence of gdal
@@ -119,15 +118,16 @@
     fname : str
         name of the file to read
     field_name : str
         name of the readed variable
     fill_value : float
         The fill value, if not provided will be infered from metadata
         if possible
-    projparams : projection transform as can be used by gdal either a  Proj4 
+    projparams : str or int
+        projection transform as can be used by gdal either a  Proj4 
         string, see epsg.io for a list, or a EPSG number, if not provided
         will be infered from the file, or for ASCII, LV1903 will be used
 
     Returns
     -------
     dem_data : dictionary
         dictionary with the data and metadata
@@ -135,65 +135,69 @@
     """
     extension = pathlib.Path(fname).suffix
 
     if isinstance(projparams, int): # Retrieve Wkt code from EPSG number
         proj = osr.SpatialReference()
         proj.ImportFromEPSG(projparams)
         projparams = proj.ExportToProj4()
-        
+        projparams = _proj4_str_to_dict(projparams) 
+    
     if extension in ['.tif','.tiff','.gtif']:
-        metadata, rasterarray =   read_geotiff_data(fname, fill_value)
+        dem =   read_geotiff_data(fname, fill_value)
     elif extension in ['.asc','.dem','.txt']:
-        metadata, rasterarray =  read_ascii_data(fname, fill_value)
+        dem =  read_ascii_data(fname, fill_value)
     elif extension in ['.rst']:
-        metadata, rasterarray = read_idrisi_data(fname, fill_value)
+        dem = read_idrisi_data(fname, fill_value)
     else:
-        warn('Unable to read file %s, extension must be .tif .tiff .gtif, '+
+        warn('WARNING: unable to read file %s, extension must be .tif .tiff .gtif, '+
              '.asc .dem .txt .rst'.format(fname))
         return None
 
+    if 'projparams' in dem:
+        projparams = dem['projparams']
+
     field_dict = get_metadata(field_name)
-    field_dict['data'] = rasterarray[::-1, :][None,:,:]
-    field_dict['units'] = metadata['value units']
+    field_dict['data'] = dem['data'][::-1, :][None,:,:]
+    field_dict['units'] = dem['metadata']['value units']
 
     x = get_metadata('x')
     y = get_metadata('y')
     z = get_metadata('z')
 
     orig_lat = get_metadata('origin_latitude')
     orig_lon = get_metadata('origin_longitude')
     orig_alt = get_metadata('origin_altitude')
 
     x['data'] = (
-        np.arange(metadata['columns'])*metadata['resolution'] +
-        metadata['resolution']/2.+metadata['min. X'])
+        np.arange(dem['metadata']['columns'])*dem['metadata']['resolution'] +
+        dem['metadata']['resolution']/2.+dem['metadata']['min. X'])
 
     y['data'] = (
-        np.arange(metadata['rows'])*metadata['resolution'] +
-        metadata['resolution']/2.+metadata['min. Y'])
+        np.arange(dem['metadata']['rows'])*dem['metadata']['resolution'] +
+        dem['metadata']['resolution']/2.+dem['metadata']['min. Y'])
 
     z['data'] = np.array([0])
 
     orig_lat['data'] = [y['data'][0]]
     orig_lon['data'] = [x['data'][0]]
     orig_alt['data'] = [0]
 
     if projparams is None:
+        warn('WARNING: No proj could be read from file and no projparams were provided, '+
+        'assuming the projection is CH1903.')
         projparams = _get_lv1903_proj4()
-    else:
-        projparams = _proj4_str_to_dict(projparams) 
-        
+    
     time = get_metadata('grid_time')
     time['data'] = np.array([0.0])
     time['units'] = 'seconds since 2000-01-01T00:00:00Z'
 
     # The use of CRS().to_dict() is required to use GridMapDisplay of Pyart
     # which expects a dict for the projection attribute of the grid
     dem_data = pyart.core.Grid(time, {field_name : field_dict},
-       metadata,  orig_lat, orig_lon, orig_alt, x, y, z,
+       dem['metadata'],  orig_lat, orig_lon, orig_alt, x, y, z,
        projection = projparams)
 
     return dem_data
 
 # @profile
 def read_geotiff_data(fname, fill_value = None):
 
@@ -213,27 +217,39 @@
     projparams : projection transform as can be used by pyproj, either a
         EPSG code integer (21781 for CH1903 for example), or a OGC WKT or
         Proj4 string, see epsg.io for a list,
         if not provided will be infered from the idrisi file
 
     Returns
     -------
-    dem_data : dictionary
-        dictionary with the data and metadata
-
+    dem : dict
+        A dictionary with the following keys:
+        - data : array
+            data within the DEM
+        - metadata : dict
+            a dictionary containing the metadata
+        - projparams : str
+            projection parameters in proj4 format    
     """
+
     if not _GDAL_AVAILABLE:
         warn("gdal is required to use read_geotiff_data but is not installed")
         return None
 
 
     # read the data
     try:
         raster = gdal.Open(fname)
 
+        prj = raster.GetProjection()
+        srs = osr.SpatialReference(wkt=prj)
+        projparams = _proj4_str_to_dict(srs.ExportToProj4())
+        if not len(projparams): # gdal could not read proj
+            projparams = None
+        import pdb; pdb.set_trace()
         width = raster.RasterXSize
         height = raster.RasterYSize
         gt = raster.GetGeoTransform()
         minx = gt[0]
         miny = gt[3] + width*gt[4] + height*gt[5]
 
         metadata = {}
@@ -251,16 +267,18 @@
 
         if not fill_value:
             fill_value = metadata['flag value']
 
         rasterarray = raster.ReadAsArray()
         rasterarray = np.ma.masked_equal(rasterarray, fill_value)
 
-        return metadata, rasterarray
-
+        dem = {'projparams' : projparams,
+               'metadata'   : metadata,
+               'data' : rasterarray}
+        return dem
 
     except EnvironmentError as ee:
         warn(str(ee))
         warn('Unable to read file '+fname)
         return None
 
 # @profile
@@ -282,17 +300,20 @@
         EPSG code integer (21781 for CH1903 for example), or a OGC WKT or
         Proj4 string, see epsg.io for a list,
         if not provided CH1903 (EPSG:21781) will be used
 
 
     Returns
     -------
-    dem_data : dictionary
-        dictionary with the data and metadata
-
+    dem : dict
+        A dictionary with the following keys:
+        - data : array
+            data within the DEM
+        - metadata : dict
+            a dictionary containing the metadata
     """
 
     # read the data
     try:
         asciidata = pd.read_csv(fname, header = None)
 
         metadata = {}
@@ -323,15 +344,20 @@
                                   sep = ' ')
         rasterarray = np.array(rasterarray)
         rasterarray = rasterarray[np.isfinite(rasterarray)]
         rasterarray = np.reshape(rasterarray,
                                  (metadata['rows'],metadata['columns']))
         rasterarray = np.ma.masked_equal(rasterarray, fill_value)
 
-        return metadata, rasterarray
+
+        dem = {'metadata'   : metadata,
+               'data' : rasterarray}
+
+        return dem
+
 
     except EnvironmentError as ee:
         warn(str(ee))
         warn('Unable to read file '+fname)
         return None
 
 # @profile
@@ -351,38 +377,54 @@
         EPSG code integer (21781 for CH1903 for example), or a OGC WKT or
         Proj4 string, see epsg.io for a list,
         if not provided will be infered from the idrisi file
 
 
     Returns
     -------
-    dem_data : dictionary
-        dictionary with the data and metadata
-
+    dem : dict
+        A dictionary with the following keys:
+        - data : array
+            data within the DEM
+        - metadata : dict
+            a dictionary containing the metadata
+        - projparams : str
+            projection parameters in proj4 format    
     """
+
     if not _GDAL_AVAILABLE:
         warn("gdal is required to use read_idrisi_data but is not installed")
         return None
 
 
     # read the data
     try:
         if fill_value is None:
             fill_value = -99.
 
         raster = gdal.Open(fname)
+
+        prj = raster.GetProjection()
+        srs = osr.SpatialReference(wkt=prj)
+        projparams = _proj4_str_to_dict(srs.ExportToProj4())
+        if not len(projparams): # gdal could not read proj
+            projparams = None
+
         rasterarray = raster.ReadAsArray()
         rasterarray = np.ma.masked_equal(rasterarray, fill_value)
 
         metadata = read_idrisi_metadata(fname)
 
         if metadata is None:
             return None
 
-        return metadata, rasterarray
+        dem = {'projparams' : projparams,
+               'metadata'   : metadata,
+               'data' : rasterarray}
+        return dem
 
     except EnvironmentError as ee:
         warn(str(ee))
         warn('Unable to read file '+fname)
         return None
 
 
@@ -399,16 +441,14 @@
     -------
     metadata : dictionary
         dictionary with the metadata
 
     """
     # read the data
     fname_rdc = fname.replace('.rst', '.rdc')
-    if not os.path.exists(fname_rdc):
-        fname_rdc = fname.replace('.rst', '.RDC')
 
     try:
         metadata = dict()
         with open(fname_rdc, 'r', newline='') as txtfile:
             for line in txtfile:
                 strs = line.split(':')
                 metadata.update({
```

### Comparing `pyrad_mch-1.7.0/pyrad/io/read_data_hzt.py` & `pyrad_mch-1.8.0/pyrad/io/read_data_hzt.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/io/read_data_iso0_mf.py` & `pyrad_mch-1.8.0/pyrad/io/read_data_iso0_mf.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/io/read_data_mxpol.py` & `pyrad_mch-1.8.0/pyrad/io/read_data_mxpol.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/io/read_data_other.py` & `pyrad_mch-1.8.0/pyrad/io/read_data_other.py`

 * *Files 1% similar despite different names*

```diff
@@ -1194,18 +1194,22 @@
     try:
         with open(fname, 'r', newline='') as csvfile:
             while True:
                 try:
                     fcntl.flock(csvfile, fcntl.LOCK_EX | fcntl.LOCK_NB)
                     break
                 except OSError as e:
-                    if e.errno != errno.EAGAIN:
-                        raise
-                    else:
+                    if e.errno == errno.EAGAIN:
                         time.sleep(0.1)
+                    elif e.errno == errno.EBADF:
+                        warn("WARNING: No file locking is possible (NFS mount?), "+
+                             "expect strange issues with multiprocessing...")
+                        break
+                    else:
+                        raise
 
             # first count the lines
             reader = csv.DictReader(
                 row for row in csvfile if not row.startswith('#'))
             nrows = sum(1 for row in reader)
             np_t = np.zeros(nrows, dtype=int)
             central_quantile = np.ma.empty(nrows, dtype=float)
```

### Comparing `pyrad_mch-1.7.0/pyrad/io/read_data_radar.py` & `pyrad_mch-1.8.0/pyrad/io/read_data_radar.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
                 Doppler spectral
 
             'RAD4ALPIQ': Format used to store rad4alp IQ data
 
         'RAINBOW', 'RAD4ALP', 'ODIM' 'ODIMBIRDS' CFRADIAL2', 'CF1' 'MFCFRADIAL'
         'GAMIC' and 'MXPOL' are primary data file sources and they cannot be
         mixed for the same radar. It is also the case for their complementary
-        data files, i.e. 'COSMO' and 'RAD4ALPCOSMO', etc. 'CFRADIAL' and
+        data files, i.e. 'COSMO' and 'RAD4ALPCOSMO', etc. 'CFRADIALPYRAD' and
         'ODIMPYRAD' are secondary data file sources and they can be combined
         with any other datagroup type.
         For a list of accepted datatypes and how they map to the Py-ART name
         convention check function 'get_field_name_pyart' in pyrad/io/io_aux.py
     cfg: dictionary of dictionaries
         configuration info to figure out where the data is
 
@@ -247,14 +247,17 @@
     dataset_gamic = list()
     datatype_odimbirds = list()
     dataset_odimbirds = list()
     datatype_mfcfradial = list()
     dataset_mfcfradial = list()
     datatype_nexrad2 = list()
     dataset_nexrad2 = list()
+    datatype_gecsx = list()
+    dataset_gecsx = list()
+    product_gecsx = list()
     datatype_cfradialpyrad = list()
     dataset_cfradialpyrad = list()
     product_cfradialpyrad = list()
     datatype_cfradial = list()
     dataset_cfradial = list()
     datatype_cfradial2 = list()
     dataset_cfradial2 = list()
@@ -319,14 +322,18 @@
             dataset_gamic.append(dataset)
         elif datagroup == 'MFCFRADIAL':
             datatype_mfcfradial.append(datatype)
             dataset_mfcfradial.append(dataset)
         elif datagroup == 'NEXRADII':
             datatype_nexrad2.append(datatype)
             dataset_nexrad2.append(dataset)
+        elif datagroup == 'GECSX':
+            datatype_gecsx.append(datatype)
+            dataset_gecsx.append(dataset)
+            product_gecsx.append(product)
         elif datagroup == 'CFRADIALPYRAD':
             datatype_cfradialpyrad.append(datatype)
             dataset_cfradialpyrad.append(dataset)
             product_cfradialpyrad.append(product)
         elif datagroup == 'CFRADIAL':
             datatype_cfradial.append(datatype)
             dataset_cfradial.append(dataset)
@@ -397,15 +404,15 @@
             datatype_psr.append(datatype)
         elif datagroup == 'PSRSPECTRA':
             datatype_psrspectra.append(datatype)
         elif datagroup == 'NETCDFSPECTRA':
             datatype_netcdfspectra.append(datatype)
             dataset_netcdfspectra.append(dataset)
             product_netcdfspectra.append(product)
-
+  
     ind_rad = int(radarnr[5:8])-1
 
     ndatatypes_rainbow = len(datatype_rainbow)
     ndatatypes_rad4alp = len(datatype_rad4alp)
     ndatatypes_odim = len(datatype_odim)
     ndatatypes_odimbirds = len(datatype_odimbirds)
     ndatatypes_gamic = len(datatype_gamic)
@@ -436,14 +443,15 @@
     ndatatypes_rad4alpIQ = len(datatype_rad4alpIQ)
     ndatatypes_pyradgrid = len(datatype_pyradgrid)
     ndatatypes_odimpyradgrid = len(datatype_odimpyradgrid)
     ndatatypes_odimgrid = len(datatype_odimgrid)
     ndatatypes_psr = len(datatype_psr)
     ndatatypes_psrspectra = len(datatype_psrspectra)
     ndatatypes_netcdfspectra = len(datatype_netcdfspectra)
+    ndatatypes_gecsx = len(datatype_gecsx)
 
     rmin = None
     rmax = None
     elmin = None
     elmax = None
     azmin = None
     azmax = None
@@ -588,23 +596,31 @@
     if ndatatypes_cfradialpyrad > 0:
         radar_aux = merge_fields_pyrad(
             cfg['loadbasepath'][ind_rad], cfg['loadname'][ind_rad], voltime,
             datatype_cfradialpyrad, dataset_cfradialpyrad,
             product_cfradialpyrad, rng_min=rmin, rng_max=rmax, ele_min=elmin,
             ele_max=elmax, azi_min=azmin, azi_max=azmax)
         radar = add_field(radar, radar_aux)
-
+    
     if ndatatypes_odimpyrad > 0:
         radar_aux = merge_fields_pyrad(
             cfg['loadbasepath'][ind_rad], cfg['loadname'][ind_rad], voltime,
             datatype_odimpyrad, dataset_odimpyrad, product_odimpyrad,
             rng_min=rmin, rng_max=rmax, ele_min=elmin, ele_max=elmax,
             azi_min=azmin, azi_max=azmax, termination='.h*')
         radar = add_field(radar, radar_aux)
 
+    if ndatatypes_gecsx > 0:
+        radar_aux = merge_fields_gecsx(
+            cfg['loadbasepath'][ind_rad], cfg['loadname'][ind_rad],
+            datatype_gecsx, dataset_gecsx, product_gecsx,
+            rng_min=rmin, rng_max=rmax, ele_min=elmin, ele_max=elmax,
+            azi_min=azmin, azi_max=azmax)
+        radar = add_field(radar, radar_aux)
+        
     if ndatatypes_cfradialcosmo > 0:
         radar_aux = merge_fields_pyradcosmo(
             cfg['cosmopath'][ind_rad], voltime,
             datatype_cfradialcosmo, dataset_cfradialcosmo, cfg,
             rng_min=rmin, rng_max=rmax, ele_min=elmin, ele_max=elmax,
             azi_min=azmin, azi_max=azmax, termination='.nc')
         radar = add_field(radar, radar_aux)
@@ -644,15 +660,15 @@
             else:
                 radar = radar_aux
 
     if ndatatypes_pyradgrid > 0:
         radar_aux = merge_fields_pyradgrid(
             cfg['loadbasepath'][ind_rad], cfg['loadname'][ind_rad], voltime,
             datatype_pyradgrid, dataset_pyradgrid, product_pyradgrid, cfg,
-            termination='nc')
+            termination='.nc')
         if radar_aux is not None:
             if radar is not None:
                 radar = merge_grids(radar, radar_aux)
             else:
                 radar = radar_aux
 
     if ndatatypes_odimpyradgrid > 0:
@@ -1186,15 +1202,14 @@
             datadescriptor = radarnr+':RAINBOW:dBZ'
         else:
             datadescriptor = radarnr+':RAINBOW:'+datatype_list[0]
         endtime = voltime+datetime.timedelta(minutes=scan_period)
         for scan in scan_list[1:]:
             filelist = get_file_list(datadescriptor, [voltime], [endtime],
                                      cfg, scan=scan)
-
             if not filelist:
                 warn("ERROR: No data file found for scan '%s' "
                      "between %s and %s" % (scan, voltime, endtime))
                 continue
             scantime = get_datetime(filelist[0], datadescriptor)
 
             radar_aux = merge_fields_rainbow(
@@ -2484,14 +2499,27 @@
         filenames = glob.glob(datapath+'*'+scan_list[0]+'*')
         filename = []
         for filename_aux in filenames:
             fdatetime = find_date_in_file_name(
                 filename_aux, date_format=fdate_strf)
             if fdatetime == voltime:
                 filename = [filename_aux]
+    elif cfg['path_convention'][ind_rad] == 'RADARV':
+        fpath_strf = (
+            dataset_list[0][
+                dataset_list[0].find("D")+2:dataset_list[0].find("F")-2])
+        fdate_strf = dataset_list[0][dataset_list[0].find("F")+2:-1]
+        datapath = (basepath+scan_list[0]+'/')
+        filenames = glob.glob(datapath+'/'+voltime.strftime(fpath_strf)+'/*')
+        filename = []
+        for filename_aux in filenames:
+            fdatetime = find_date_in_file_name(
+                filename_aux, date_format=fdate_strf)
+            if fdatetime == voltime:
+                filename = [filename_aux]
     else:
         datapath = basepath+'M'+radar_res+radar_name+'/'
         filename = glob.glob(
             datapath+basename+timeinfo+'*'+scan_list[0] + '*')
         if not filename:
             basename = 'P'+radar_res+radar_name+dayinfo
             datapath = basepath+'P'+radar_res+radar_name+'/'
@@ -3756,15 +3784,15 @@
     scan_list : list
         list of scans
     cfg : dict
         configuration dictionary
     ind_rad : int
         radar index
     ftype : str
-        File type. Can be 'png', 'bin' or 'grib'
+        File type. Can be 'png', 'bin', 'grib', 'dat' or 'nc'
 
     Returns
     -------
     radar : Radar
         radar object
 
     """
@@ -3933,14 +3961,81 @@
     if radar is None:
         return radar
 
     return pyart.util.subset_radar(
         radar, radar.fields.keys(), rng_min=rng_min, rng_max=rng_max,
         ele_min=ele_min, ele_max=ele_max, azi_min=azi_min, azi_max=azi_max)
 
+def merge_fields_gecsx(basepath, loadname, datatype_list,
+                       dataset_list, product_list, rng_min=None, rng_max=None,
+                       azi_min=None, azi_max=None, ele_min=None, ele_max=None):
+    """
+    merge fields from GECSX Pyrad-generated files into a single radar object.
+    Accepted file types are CFRadial.
+
+    Parameters
+    ----------
+    basepath : str
+        name of the base path where to find the data
+    loadname: str
+        name of the saving directory
+    datatype_list : list
+        list of data types to get
+    dataset_list : list
+        list of datasets that produced the data type to get.
+        Used to get path.
+    product_list : list
+        list of products. Used to get path
+    rng_min, rng_max : float
+        The range limits [m]. If None the entire coverage of the radar is
+        going to be used
+    ele_min, ele_max, azi_min, azi_max : float or None
+        The limits of the grid [deg]. If None the limits will be the limits
+        of the radar volume
+    Returns
+    -------
+    radar : Radar
+        radar object
+
+    """
+    radar = None
+    for i, dataset in enumerate(dataset_list):
+        datapath = (
+            basepath+loadname+'/' +
+            dataset+'/'+product_list[i]+'/')
+        filename = glob.glob(
+            datapath+'*'+datatype_list[i]+'.nc')
+        if not filename:
+            warn('No file found in '+datapath+'*' +
+                 datatype_list[i]+'.nc')
+            continue
+
+        try:
+            radar_aux = pyart.io.read_cfradial(filename[0])
+        except (OSError, KeyError) as ee:
+            warn(str(ee))
+            warn('Unable to read file '+filename[0])
+            radar_aux = None
+
+        if radar_aux is None:
+            continue
+
+        if radar is None:
+            radar = radar_aux
+            continue
+
+        radar = add_field(radar, radar_aux)
+
+    if radar is None:
+        return radar
+
+    return pyart.util.subset_radar(
+        radar, radar.fields.keys(), rng_min=rng_min, rng_max=rng_max,
+        ele_min=ele_min, ele_max=ele_max, azi_min=azi_min, azi_max=azi_max)
+
 
 def merge_fields_pyradcosmo(basepath, voltime, datatype_list, dataset_list,
                             cfg, rng_min=None, rng_max=None, azi_min=None,
                             azi_max=None, ele_min=None, ele_max=None,
                             termination='.nc'):
     """
     merge fields from Pyrad-generated files into a single radar object.
@@ -4264,15 +4359,14 @@
 
         for field_name in radar_aux.fields.keys():
             break
         radar.add_field(field_name, radar_aux.fields[field_name])
 
     return radar
 
-
 def get_data_rainbow(filename, datatype):
     """
     gets rainbow radar data
 
     Parameters
     ----------
     filename : str
```

### Comparing `pyrad_mch-1.7.0/pyrad/io/read_data_sensor.py` & `pyrad_mch-1.8.0/pyrad/io/read_data_sensor.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2057,8 +2057,8 @@
             np.ma.set_fill_value(variable, get_fillvalue())
             csvfile.close()
 
             return (date, preciptype, variable, scatt_temp)
     except EnvironmentError as ee:
         warn(str(ee))
         warn('Unable to read file '+fname)
-        return (None, None, None, None)
+        return (None, None, None, None)
```

### Comparing `pyrad_mch-1.7.0/pyrad/io/read_data_sun.py` & `pyrad_mch-1.8.0/pyrad/io/read_data_sun.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/io/timeseries.py` & `pyrad_mch-1.8.0/pyrad/io/timeseries.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/io/trajectory.py` & `pyrad_mch-1.8.0/pyrad/io/trajectory.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/io/write_data.py` & `pyrad_mch-1.8.0/pyrad/io/write_data.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/proc/__init__.py` & `pyrad_mch-1.8.0/pyrad/proc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
 from .process_retrieve import process_radial_noise_hs, process_vpr
 from .process_retrieve import process_radial_noise_ivic
 
 from .process_Doppler import process_wind_vel, process_windshear
 from .process_Doppler import process_radial_velocity, process_dealias_fourdd
 from .process_Doppler import process_dealias_region_based
 from .process_Doppler import process_dealias_unwrap_phase
-from .process_Doppler import process_vad, process_turbulence
+from .process_Doppler import process_vad, process_turbulence, process_dda
 
 from .process_cosmo import process_cosmo, process_cosmo_lookup_table
 from .process_cosmo import process_cosmo_coord, process_hzt, process_iso0_mf
 from .process_cosmo import process_hzt_lookup_table, process_hzt_coord
 from .process_cosmo import process_cosmo_to_radar, process_iso0_grib
 
 from .process_dem import process_dem, process_visibility, process_gecsx
```

### Comparing `pyrad_mch-1.7.0/pyrad/proc/process_Doppler.py` & `pyrad_mch-1.8.0/pyrad/proc/process_Doppler.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,32 +11,38 @@
     process_dealias_fourdd
     process_dealias_region_based
     process_dealias_unwrap_phase
     process_radial_velocity
     process_wind_vel
     process_windshear
     process_vad
+    process_dda
 
 """
 
 from copy import deepcopy
 from warnings import warn
-
 import numpy as np
 
 import pyart
 
 try:
     import pytda
     _PYTDA_AVAILABLE = True
 except ImportError:
     _PYTDA_AVAILABLE = False
 
-from ..io.io_aux import get_datatype_fields, get_fieldname_pyart
+try:
+    import pydda
+    _PYDDA_AVAILABLE = True
+except ImportError:
+    _PYDDA_AVAILABLE = False
 
+from ..io.io_aux import get_datatype_fields, get_fieldname_pyart
+from .process_grid import process_grid
 
 def process_turbulence(procstatus, dscfg, radar_list=None):
     """
     Computes turbulence from the Doppler spectrum width and reflectivity using
     the PyTDA package
 
     Parameters
@@ -308,14 +314,19 @@
             between and along a ray. Set these parameters to 0 to disable
             unfolding across filtered gates.
         centered : bool, optional
             True to apply centering to each sweep after the dealiasing
             algorithm so that the average number of unfolding is near 0. False
             does not apply centering which may results in individual sweeps
             under or over folded by the nyquist interval.
+        nyquist_vel : float, optional
+            Nyquist velocity of the aquired radar velocity.
+            Usually this parameter is provided in the
+            Radar object intrument_parameters. If it is not available it can 
+            be provided as a keyword here.
     radar_list : list of Radar objects
         Optional. list of radar objects
 
     Returns
     -------
     new_dataset : dict
         dictionary containing the output
@@ -342,28 +353,29 @@
     corr_vel_field = 'dealiased_'+vel_field
 
     # get user parameters
     interval_splits = dscfg.get('interval_splits', 3)
     skip_between_rays = dscfg.get('skip_between_rays', 100)
     skip_along_ray = dscfg.get('skip_along_ray', 100)
     centered = dscfg.get('centered', True)
+    nyquist_vel = dscfg.get('nyquist_vel', None)
 
     corr_vel_dict = pyart.correct.dealias_region_based(
         radar, ref_vel_field=None, interval_splits=interval_splits,
         interval_limits=None, skip_between_rays=skip_between_rays,
         skip_along_ray=skip_along_ray, centered=centered,
-        nyquist_vel=None, check_nyquist_uniform=True, gatefilter=False,
+        nyquist_vel=nyquist_vel, check_nyquist_uniform=True, gatefilter=False,
         rays_wrap_around=None, keep_original=False, set_limits=False,
         vel_field=vel_field, corr_vel_field=corr_vel_field)
 
     # prepare for exit
     new_dataset = {'radar_out': deepcopy(radar)}
     new_dataset['radar_out'].fields = dict()
     new_dataset['radar_out'].add_field(corr_vel_field, corr_vel_dict)
-
+    
     return new_dataset, ind_rad
 
 
 def process_dealias_unwrap_phase(procstatus, dscfg, radar_list=None):
     """
     Dealiases the Doppler velocity field using multi-dimensional phase
     unwrapping
@@ -747,7 +759,245 @@
     new_dataset['radar_out'].add_field('northward_wind_component', v_vel_dict)
     new_dataset['radar_out'].add_field('vertical_wind_component', w_vel_dict)
     new_dataset['radar_out'].add_field('retrieved_velocity', vel_est_dict)
     new_dataset['radar_out'].add_field('retrieved_velocity_std', vel_std_dict)
     new_dataset['radar_out'].add_field('velocity_difference', vel_diff_dict)
 
     return new_dataset, ind_rad
+
+def process_dda(procstatus, dscfg, radar_list=None):
+    """
+    Estimates horizontal wind speed and direction with a multi-doppler approach
+    This method uses the python package pyDDA
+
+    Parameters
+    ----------
+    procstatus : int
+        Processing status: 0 initializing, 1 processing volume,
+        2 post-processing
+    dscfg : dictionary of dictionaries
+        data set configuration. Accepted Configuration Keywords::
+
+        datatype : string. Dataset keyword
+            The input data type
+
+        gridding  parameters:
+            gridconfig : dictionary. Dataset keyword
+                Dictionary containing some or all of this keywords:
+                xmin, xmax, ymin, ymax, zmin, zmax : floats
+                    minimum and maximum horizontal distance from grid origin [km]
+                    and minimum and maximum vertical distance from grid origin [m]
+                    Defaults -40, 40, -40, 40, 0., 10000.
+                latmin, latmax, lonmin, lonmax : floats
+                    minimum and maximum latitude and longitude [deg], if specified
+                    xmin, xmax, ymin, ymax will be ignored
+                hres, vres : floats
+                    horizontal and vertical grid resolution [m]
+                    Defaults 1000., 500.
+                latorig, lonorig, altorig : floats
+                    latitude and longitude of grid origin [deg] and altitude of
+                    grid origin [m MSL]
+                    Defaults the latitude, longitude and altitude of the radar
+            wfunc : str. Dataset keyword
+                the weighting function used to combine the radar gates close to a
+                grid point. Possible values BARNES, BARNES2, CRESSMAN, NEAREST
+                Default NEAREST
+            roif_func : str. Dataset keyword
+                the function used to compute the region of interest.
+                Possible values: dist_beam, constant
+            roi : float. Dataset keyword
+                the (minimum) radius of the region of interest in m. Default half
+                the largest resolution
+            beamwidth : float. Dataset keyword
+                the radar antenna beamwidth [deg]. If None that of the key
+                radar_beam_width_h in attribute instrument_parameters of the radar
+                object will be used. If the key or the attribute are not present
+                a default 1 deg value will be used
+            beam_spacing : float. Dataset keyword
+                the beam spacing, i.e. the ray angle resolution [deg]. If None,
+                that of the attribute ray_angle_res of the radar object will be
+                used. If the attribute is None a default 1 deg value will be used
+        dda parameters:
+            signs : list of integers
+                The sign of the velocity field for every radar object.  
+                A value of 1 represents when
+                positive values velocities are towards the radar, -1 represents
+                when negative velocities are towards the radar.
+            Co : float
+                Weight for cost function related to observed radial velocities.
+                Default: 1. 
+            Cm : float
+                Weight for cost function related to the mass continuity equation.
+                Default: 1500. 
+
+    radar_list : list of Radar objects
+        Optional. list of radar objects
+
+    Returns
+    -------
+    new_dataset : dict
+        dictionary containing the output
+    ind_rad : int
+        radar index
+
+    """
+    if not _PYDDA_AVAILABLE:
+        warn('PyDDA package not available. Unable to compute wind fields')
+        return None, None
+
+    if procstatus != 1:
+        return None, None
+    
+    if len(radar_list) < 2:
+        warn('DDA requires data from at least two different radars')
+        return None, None
+
+    # check how many radars have to be compared and which datatype to use
+    ind_radar_list = []
+    field_name_list = []
+    datatype_list = []
+    for datatypedescr in dscfg['datatype']:
+        radarnr, _, datatype, _, _ = get_datatype_fields(datatypedescr)
+        field_name = get_fieldname_pyart(datatype)
+        ind_radar_list.append(int(radarnr[5:8])-1)
+        datatype_list.append(datatype)
+        field_name_list.append(field_name)
+    ind_radar_list = np.array(ind_radar_list)
+    datatype_list = np.array(datatype_list)
+    field_name_list = np.array(field_name_list)
+    
+    # Get DDA numerical parameters
+    Co = dscfg.get('Co', 1.)
+    Cm = dscfg.get('Cm', 1500.)
+
+    # Compute VAD for every radar to initialize DDA
+    # z-vector for vad
+    z_want = np.arange(dscfg['gridConfig']['zmin'],
+        dscfg['gridConfig']['zmax'] + dscfg['gridConfig']['vres'],
+        dscfg['gridConfig']['vres'])
+    
+    all_vad = []
+    distances_to_center = []
+    vel_fields = []
+    refl_fields = []
+    for i, radar in enumerate(radar_list):
+        # Find vel and refl fields
+        field_names_rad = field_name_list[ind_radar_list == i]
+        vel_field = field_names_rad[['velocity' in vname 
+                    for vname in field_name_list[ind_radar_list == i]]][0]
+        vel_fields.append(vel_field)
+        refl_field = field_names_rad[['reflectivity' in vname 
+                    for vname in field_name_list[ind_radar_list == i]]][0]
+        refl_fields.append(refl_field)
+
+        # Compute VAD
+        all_vad.append(pyart.retrieve.vad_browning(radar, vel_field, 
+            z_want = z_want, sign = dscfg['signs'][i]))
+        dist = np.sqrt((radar.latitude['data'][0] 
+                                - dscfg['gridConfig']['latorig'])**2 + 
+                        (radar.longitude['data'][0] 
+                                - dscfg['gridConfig']['lonorig'])**2)
+        distances_to_center.append(dist)
+
+    # Compute VAD weights
+    distances_to_center = np.array(distances_to_center)
+    weights = 1/distances_to_center
+    weights /= np.sum(weights)
+
+    # Now average the VADs
+    u_avg = []
+    v_avg = []
+    for i, vad in enumerate(all_vad):
+        u_avg.append(weights[i] * np.ma.filled(vad.u_wind, np.nan))
+        v_avg.append(weights[i] * np.ma.filled(vad.v_wind, np.nan))
+    u_avg = np.nansum(u_avg, axis = 0)
+    v_avg = np.nansum(v_avg, axis = 0)
+
+    vad_avg = pyart.core.HorizontalWindProfile.from_u_and_v(z_want, 
+                    np.ma.array(u_avg, mask = np.isnan(u_avg)),
+                    np.ma.array(v_avg,  mask = np.isnan(v_avg)))
+
+    grids = []
+    for i, radar in enumerate(radar_list):
+        # Now we grid
+        dscfg_grid = deepcopy(dscfg)
+        dscfg_grid['datatype'] = np.array(dscfg['datatype'])[ind_radar_list == i]
+        grids.append(process_grid(1, dscfg_grid, radar_list)[0]['radar_out'])
+
+    # Harmonize variables
+    for i, grid in enumerate(grids):
+        grid.fields['velocity'] = grid.fields.pop(vel_fields[i])
+        if dscfg['signs'][i] == 1:
+            grid.fields['velocity']['data'] *= -1
+        grid.fields['reflectivity'] = grid.fields.pop(refl_fields[i])
+
+    # DDA initialization
+    u_init, v_init, w_init = pydda.initialization.make_wind_field_from_profile(grids[0], 
+                                vad_avg, vel_field='velocity')
+
+    # Actual DDA computation
+    new_grids = pydda.retrieval.get_dd_wind_field(grids,
+                                u_init, v_init, w_init,
+                                vel_name='velocity', refl_field='reflectivity', 
+                                mask_outside_opt=True, wind_tol=0.01,
+                                engine='scipy', Co = Co, Cm = Cm)
+
+    # pyDDA returns as many grid objects as input radars
+    # the idea here is to merge these grid objects into one
+    # and to replace the homogeneized vel and refl fields by the
+    # original ones
+
+    # create merged grid from first dda grid
+    # First radar will have normal field names
+    # Additional radars will have _radar1, radar_2, ..., radar_N
+    # appended to their field names 
+    merged_grid = deepcopy(new_grids[0])
+    for var in list(merged_grid.fields):
+        if var in grids[0].fields:
+            if var == 'velocity':
+                new_key = vel_fields[0]
+            elif var == 'reflectivity':
+                new_key = refl_fields[0]
+            else:
+                new_key = var
+            merged_grid.fields[new_key] = merged_grid.fields.pop(var)
+
+    # add the other dda grids
+    radar_metadata = []
+    for i, additional_grid in enumerate(new_grids[1:]):
+        for var in list(additional_grid.fields):
+            if var in grids[i+1].fields:
+                if var == 'velocity':
+                    new_key = vel_fields[i+1]
+                elif var == 'reflectivity':
+                    new_key = refl_fields[i+1]
+                else:
+                    new_key = var
+                new_key += '_radar{:d}'.format(i+1)
+                merged_grid.fields[new_key] = additional_grid.fields[var]
+                
+        # Get additional radar metadata
+        mdata = {}
+        mdata['radar_longitude'] =  additional_grid.radar_longitude['data']
+        mdata['radar_latitude'] =  additional_grid.radar_latitude['data']
+        # Try to find name of radar
+        if additional_grid.radar_name['data'] != '':
+            mdata['radar_name'] =  additional_grid.radar_name['data'][0]
+        elif dscfg['RadarName'][i+1] != '':
+            mdata['radar_name'] =  dscfg['RadarName'][i+1]
+        else:
+            mdata['radar_name'] =  'Unknown'
+
+        radar_metadata.append(mdata)
+    
+    # Rename DDA u, v, w fields to pyart names
+    merged_grid.fields['eastward_wind_component'] = merged_grid.fields.pop('u')
+    merged_grid.fields['northward_wind_component'] = merged_grid.fields.pop('v')
+    merged_grid.fields['vertical_wind_component'] = merged_grid.fields.pop('w')
+
+    # Add coordinates of additional radars in metadata
+    merged_grid.metadata['additional_radars'] = radar_metadata
+
+    new_dataset = {}
+    new_dataset['radar_out'] = merged_grid
+
+    return new_dataset, ind_radar_list
```

### Comparing `pyrad_mch-1.7.0/pyrad/proc/process_aux.py` & `pyrad_mch-1.8.0/pyrad/proc/process_aux.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,15 @@
                 'GRID': process_grid
                 'GRID_FIELDS_DIFF': process_grid_fields_diff
                 'GRID_MASK': process_grid_mask
                 'GRID_TEXTURE': process_grid_texture
                 'NORMALIZE_LUMINOSITY': process_normalize_luminosity
                 'PIXEL_FILTER': process_pixel_filter
                 'VOL2GRID': process_vol_to_grid
+                'DDA': process_dda
             'GRID_TIMEAVG' format output:
                 'GRID_TIME_STATS': process_grid_time_stats
                 'GRID_TIME_STATS2': process_grid_time_stats2
                 'GRID_RAIN_ACCU': process_grid_rainfall_accumulation
             'INTERCOMP' format output:
                 'INTERCOMP': process_intercomp
                 'INTERCOMP_FIELDS': process_intercomp_fields
@@ -213,15 +214,14 @@
                 'SVP': process_svp
                 'TIME_HEIGHT': process_time_height
                 'TIME_ALONG_COORD': process_ts_along_coord
             'SPARSE_GRID' format output:
                 'ZDR_COLUMN': process_zdr_column
             'SUN_HITS' format output:
                 'SUN_HITS': process_sun_hits
-            'SUNSCAN' format output:
                 'SUNSCAN': process_sunscan
             'TIMEAVG' format output:
                 'FLAG_TIME_AVG': process_time_avg_flag
                 'TIME_AVG': process_time_avg
                 'WEIGHTED_TIME_AVG': process_weighted_time_avg
                 'TIME_STATS': process_time_stats
                 'TIME_STATS2': process_time_stats2
@@ -258,14 +258,17 @@
     elif dataset_type == 'RADAR_RESAMPLING':
         func_name = 'process_radar_resampling'
     elif dataset_type == 'CCOR':
         func_name = 'process_ccor'
     elif dataset_type == 'GECSX':
         func_name = 'process_gecsx'
         dsformat = ['GRID', 'VOL']
+    elif dataset_type == 'DDA':
+        func_name = 'process_dda'
+        dsformat = 'GRID'
     elif dataset_type == 'GRID':
         func_name = 'process_grid'
         dsformat = 'GRID'
     elif dataset_type == 'RAW_GRID':
         func_name = 'process_raw_grid'
         dsformat = 'GRID'
     elif dataset_type == 'VOL2GRID':
@@ -765,15 +768,15 @@
     ymin = dscfg.get('ymin', -20000.)
     ymax = dscfg.get('ymax', 20000.)
     zmin = dscfg.get('zmin', 1000.)
     zmax = dscfg.get('zmax', 1000.)
     hres = dscfg.get('hres', 1000.)
     vres = dscfg.get('vres', 500.)
     lat = dscfg.get('lat0', float(radar_list_aux[0].latitude['data']))
-    lon = dscfg.get('lon0', float(radar_list_aux[0].latitude['data']))
+    lon = dscfg.get('lon0', float(radar_list_aux[0].longitude['data']))
     alt = dscfg.get('alt0', 0.)
 
     wfunc = dscfg.get('wfunc', 'NEAREST')
 
     # number of grid points
     ny = int((ymax-ymin)/hres)+1
     nx = int((xmax-xmin)/hres)+1
@@ -1421,20 +1424,20 @@
         inds, is_roi = belongs_roi_indices(
             y, x, roi_dict, use_latlon=use_latlon)
 
     if is_roi == 'None':
         warn('No values within ROI')
         return None, None
 
-    inds_ray = inds_ray[inds]
-    inds_rng = inds_rng[inds]
+    inds_ray = np.squeeze(inds_ray[inds])
+    inds_rng = np.squeeze(inds_rng[inds])
 
-    lat = lat[inds]
-    lon = lon[inds]
-    alt = radar.gate_altitude['data'][inds_ray, inds_rng]
+    lat = np.squeeze(lat[inds])
+    lon = np.squeeze(lon[inds])
+    alt = np.squeeze(radar.gate_altitude['data'][inds_ray, inds_rng])
 
     # prepare new radar object output
     new_dataset = {
         'radar_out': deepcopy(radar),
         'rng_res': radar.range['data'][1]-radar.range['data'][0]
     }
```

### Comparing `pyrad_mch-1.7.0/pyrad/proc/process_calib.py` & `pyrad_mch-1.8.0/pyrad/proc/process_calib.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/proc/process_cosmo.py` & `pyrad_mch-1.8.0/pyrad/proc/process_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/proc/process_dem.py` & `pyrad_mch-1.8.0/pyrad/proc/process_dem.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/proc/process_echoclass.py` & `pyrad_mch-1.8.0/pyrad/proc/process_echoclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -547,15 +547,14 @@
     ind_rad : int
         radar index
 
     """
 
     if procstatus != 1:
         return None, None
-
     echoid_field = None
     hydro_field = None
     vis_field = None
     for datatypedescr in dscfg['datatype']:
         radarnr, _, datatype, _, _ = get_datatype_fields(datatypedescr)
         if datatype == 'echoID':
             echoid_field = get_fieldname_pyart(datatype)
@@ -632,15 +631,15 @@
     """
 
     if procstatus != 1:
         return None, None
 
     for datatypedescr in dscfg['datatype']:
         radarnr, _, datatype, _, _ = get_datatype_fields(datatypedescr)
-        if datatype in ('SNRh', 'SNRv', 'SNR'):
+        if datatype in ('SNRh', 'SNRv', 'SNR','CNR'):
             snr_field = get_fieldname_pyart(datatype)
             break
 
     ind_rad = int(radarnr[5:8])-1
     if radar_list[ind_rad] is None:
         warn('No valid radar')
         return None, None
@@ -820,14 +819,16 @@
         return None, None
 
     for datatypedescr in dscfg['datatype']:
         radarnr, _, datatype, _, _ = get_datatype_fields(datatypedescr)
         if datatype == 'VIS':
             vis_field = get_fieldname_pyart(datatype)
             break
+        elif 'visibility_polar' in datatype: # from GECSX
+            vis_field = get_fieldname_pyart('visibility_polar')
 
     ind_rad = int(radarnr[5:8])-1
     if radar_list[ind_rad] is None:
         warn('No valid radar')
         return None, None
     radar = radar_list[ind_rad]
 
@@ -843,15 +844,15 @@
         radar, vis_field=vis_field, min_vis=dscfg['VISmin'])
     is_lowVIS = gatefilter.gate_excluded == 1
 
     for datatypedescr in dscfg['datatype']:
         _, _, datatype, _, _ = get_datatype_fields(
             datatypedescr)
 
-        if datatype == 'VIS':
+        if datatype == 'VIS' or 'visibility_polar' in datatype:
             continue
         field_name = get_fieldname_pyart(datatype)
         if field_name not in radar.fields:
             warn('Unable to filter '+field_name +
                  ' according to visibility. No valid input fields')
             continue
```

### Comparing `pyrad_mch-1.7.0/pyrad/proc/process_grid.py` & `pyrad_mch-1.8.0/pyrad/proc/process_grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             Dictionary containing some or all of this keywords:
             xmin, xmax, ymin, ymax, zmin, zmax : floats
                 minimum and maximum horizontal distance from grid origin [km]
                 and minimum and maximum vertical distance from grid origin [m]
                 Defaults -40, 40, -40, 40, 0., 10000.
             latmin, latmax, lonmin, lonmax : floats
                 minimum and maximum latitude and longitude [deg], if specified
-                xmin, xmax, ymin, ymax will be ignored
+                xmin, xmax, ymin, ymax, latorig, lonorig will be ignored
             hres, vres : floats
                 horizontal and vertical grid resolution [m]
                 Defaults 1000., 500.
             latorig, lonorig, altorig : floats
                 latitude and longitude of grid origin [deg] and altitude of
                 grid origin [m MSL]
                 Defaults the latitude, longitude and altitude of the radar
@@ -202,34 +202,38 @@
             zmin = dscfg['gridConfig']['zmin']
         if 'zmax' in dscfg['gridConfig']:
             zmax = dscfg['gridConfig']['zmax']
         if 'hres' in dscfg['gridConfig']:
             hres = dscfg['gridConfig']['hres']
         if 'vres' in dscfg['gridConfig']:
             vres = dscfg['gridConfig']['vres']
-        if 'latorig' in dscfg['gridConfig']:
-            lat = dscfg['gridConfig']['latorig']
-        if 'lonorig' in dscfg['gridConfig']:
-            lon = dscfg['gridConfig']['lonorig']
         if 'altorig' in dscfg['gridConfig']:
             alt = dscfg['gridConfig']['altorig']
-
+            
     if (latmin is not None and latmax is not None and 
         lonmin is not None and lonmax is not None):
+        warn('Specified lat/lon limits')
+        warn('xmin, xmax, ymin, ymax, latorig and lonorig parameters\n' +
+            'will be ignored') 
         # get xmin, xmax, ymin, ymax from lon/lat
         gatelat = radar.gate_latitude['data']
         gatelon = radar.gate_longitude['data']
         mask1 = np.logical_and(gatelat > latmin, gatelat <= latmax)
         mask2 = np.logical_and(gatelon > lonmin, gatelon <= lonmax)
         mask = np.logical_and(mask1, mask2)
         xmin = np.min(radar.gate_x['data'][mask]) / 1000.
         xmax = np.max(radar.gate_x['data'][mask]) / 1000.
         ymin = np.min(radar.gate_y['data'][mask]) / 1000.
         ymax = np.max(radar.gate_y['data'][mask]) / 1000.
-
+    else:
+        if 'latorig' in dscfg['gridConfig']:
+            lat = dscfg['gridConfig']['latorig']
+        if 'lonorig' in dscfg['gridConfig']:
+            lon = dscfg['gridConfig']['lonorig']
+       
     wfunc = dscfg.get('wfunc', 'NEAREST')
     roi_func = dscfg.get('roi_func', 'dist_beam')
 
     # number of grid points in cappi
     nz = int((zmax-zmin)/vres)+1
     ny = int((ymax-ymin)*1000./hres)+1
     nx = int((xmax-xmin)*1000./hres)+1
```

### Comparing `pyrad_mch-1.7.0/pyrad/proc/process_intercomp.py` & `pyrad_mch-1.8.0/pyrad/proc/process_intercomp.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/proc/process_iq.py` & `pyrad_mch-1.8.0/pyrad/proc/process_iq.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/proc/process_monitoring.py` & `pyrad_mch-1.8.0/pyrad/proc/process_monitoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,28 +179,32 @@
         if parametrization == 'None':
             # find unique elevations
             el_vec = np.unique(
                 (10.*np.round(radar.elevation['data'], decimals=1)).astype(int))
             zdr_kdpzh_list = list()
             el_list = list()
             for el in el_vec:
+                if 'selfconsistencypath' in dscfg:
+                    selfcons_dir = dscfg['selfconsistencypath']
+                else:
+                    selfcons_dir = dscfg['configpath'] + 'selfconsistency/'
                 fname = (
-                    dscfg['configpath'] + 'selfconsistency/' +
+                    selfcons_dir +
                     'selfconsistency_zdr_zhkdp_'+freq_band+'band_temp10_elev' +
                     '{:03d}'.format(el)+'_mu05.txt')
                 zdr_kdpzh_table = read_selfconsistency(fname)
                 if zdr_kdpzh_table is not None:
                     zdr_kdpzh_list.append(zdr_kdpzh_table)
                     el_list.append((el/10.).astype(int))
             if not el_list:
                 warn('Unable to retrieve PhiDP and KDP using self-consistency. ' +
                      'No selfconsistency files for the radar elevations.')
 
                 return None, None
-
+            import pdb; pdb.set_trace()
             zdr_kdpzh_dict = {'zdr_kdpzh': zdr_kdpzh_list,
                               'elev': el_list,
                               'freq_band': freq_band}
         else:
             zdr_kdpzh_dict = {'zdr_kdpzh': None,
                               'elev': None,
                               'freq_band': freq_band}
@@ -427,28 +431,31 @@
         if parametrization == 'None':
             # find unique elevations
             el_vec = np.unique(
                 (10.*np.round(radar.elevation['data'], decimals=1)).astype(int))
             zdr_kdpzh_list = list()
             el_list = list()
             for el in el_vec:
+                if 'selfconsistencypath' in dscfg:
+                    selfcons_dir = dscfg['selfconsistencypath']
+                else:
+                    selfcons_dir = dscfg['configpath'] + 'selfconsistency/'
                 fname = (
-                    dscfg['configpath'] + 'selfconsistency/' +
+                    selfcons_dir +
                     'selfconsistency_zdr_zhkdp_'+freq_band+'band_temp10_elev' +
                     '{:03d}'.format(el)+'_mu05.txt')
                 zdr_kdpzh_table = read_selfconsistency(fname)
                 if zdr_kdpzh_table is not None:
                     zdr_kdpzh_list.append(zdr_kdpzh_table)
                     el_list.append((el/10.).astype(int))
             if not el_list:
                 warn('Unable to retrieve Zh bias using self-consistency. ' +
                      'No selfconsistency files for the radar elevations.')
 
                 return None, None
-
             zdr_kdpzh_dict = {'zdr_kdpzh': zdr_kdpzh_list,
                               'elev': el_list,
                               'freq_band': freq_band}
         else:
             zdr_kdpzh_dict = {'zdr_kdpzh': None,
                               'elev': None,
                               'freq_band': freq_band}
```

### Comparing `pyrad_mch-1.7.0/pyrad/proc/process_phase.py` & `pyrad_mch-1.8.0/pyrad/proc/process_phase.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/proc/process_retrieve.py` & `pyrad_mch-1.8.0/pyrad/proc/process_retrieve.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/proc/process_spectra.py` & `pyrad_mch-1.8.0/pyrad/proc/process_spectra.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/proc/process_timeseries.py` & `pyrad_mch-1.8.0/pyrad/proc/process_timeseries.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/proc/process_traj.py` & `pyrad_mch-1.8.0/pyrad/proc/process_traj.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/prod/__init__.py` & `pyrad_mch-1.8.0/pyrad/prod/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/prod/process_grid_products.py` & `pyrad_mch-1.8.0/pyrad/prod/process_grid_products.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,20 +23,24 @@
 from ..io.io_aux import get_fieldname_pyart
 from ..io.io_aux import get_save_dir, make_filename
 from ..io.write_data import write_histogram, write_ts_stats
 
 from ..graph.plots_grid import plot_surface, plot_surface_raw
 from ..graph.plots_grid import plot_longitude_slice, plot_latitude_slice
 from ..graph.plots_grid import plot_latlon_slice, plot_surface_contour
+from ..graph.plots_grid import plot_dda_map, plot_dda_slice
+
 from ..graph.plots_aux import get_colobar_label, get_field_name
+from ..graph.plots_aux import generate_dda_map_title
+from ..graph.plots_aux import generate_dda_latitude_slice_title
+from ..graph.plots_aux import generate_dda_longitude_slice_title
 from ..graph.plots import plot_histogram, plot_pos
 
 from ..util.radar_utils import compute_histogram
 
-
 def generate_grid_time_avg_products(dataset, prdcfg):
     """
     generates time average products. Accepted product types:
         All the products of the 'VOL' dataset group
 
     Parameters
     ----------
@@ -136,15 +140,15 @@
     """
     generates grid products. Accepted product types:
         'CROSS_SECTION': Plots a cross-section of gridded data
             User defined parameters:
                 coord1, coord2: dict
                     The two lat-lon coordinates marking the limits. They have
                     the keywords 'lat' and 'lon' [degree]. The altitude limits
-                    are defined by the parameters in 'rhiImageConfig' in the
+                    are defined by the parameters in 'xsecImageConfig' in the
                     'loc' configuration file
         'HISTOGRAM': Computes a histogram of the radar volum data
             User defined parameters:
                 step: float or None
                     the data quantization step. If none it will be obtained
                     from the Py-ART configuration file
                 vmin, vmax: float or None
@@ -155,22 +159,22 @@
                 write_data: Bool
                     If true the histogram data is written in a csv file
         'LATITUDE_SLICE': Plots a cross-section of gridded data over a
             constant latitude.
             User defined parameters:
                 lon, lat: floats
                     The starting point of the cross-section. The ending point
-                    is defined by the parameters in 'rhiImageConfig' in the
+                    is defined by the parameters in 'xsecImageConfig' in the
                     'loc' configuration file
         'LONGITUDE_SLICE': Plots a cross-ection of gridded data over a
             constant longitude.
             User defined parameters:
                 lon, lat: floats
                     The starting point of the cross-section. The ending point
-                    is defined by the parameters in 'rhiImageConfig' in the
+                    is defined by the parameters in 'xsecImageConfig' in the
                     'loc' configuration file
         'SAVEALL': Saves a gridded data object including all or a list of
             user-defined fields in a netcdf file
             User defined parameters:
                 datatypes: list of str or None
                     The list of data types to save. If it is None, all fields
                     in the radar object will be saved
@@ -255,15 +259,49 @@
                     'ppiMapImageConfig' in the 'loc' configuration file
                 contour_values : float array or None
                     The contour values. If None the values are taken from the
                     'boundaries' keyword in the field description in the
                     Py-ART config file. If 'boundaries' is not set the
                     countours are 10 values linearly distributed from vmin to
                     vmax
-
+        DDA_MAP:
+            Plots wind vectors obtained from a DDA analysis. The pyDDA package is
+            required
+            User defined parameters:
+                level: int
+                    The altitude level to plot. The rest of the parameters are
+                    defined by the parameters in 'ppiImageConfig' and
+                    'ppiMapImageConfig' in the 'loc' configuration file
+                display_type: str
+                    Display method for the wind vectors, can be either
+                    'streamline', 'quiver' or 'barbs'
+                bg_ref_rad: int
+                    Which radar to use as reference to display the background
+                    voltype.
+                u_vel_contours: list of int
+                    The contours to use for plotting contours of u. Set to None to not
+                    display such contours.
+                v_vel_contours: list of int
+                    The contours to use for plotting contours of v. Set to None to not
+                    display such contours.
+                w_vel_contours: list of int
+                    The contours to use for plotting contours of w. Set to None to not
+                    display such contours.
+                vector_spacing_km: float
+                    Spacing in km between wind vectors in x and y axis
+                    (only used for barbs and quiver plots)
+                quiver_len: float
+                    Length to use for the quiver key in m/s.
+                    (only used for quiver plots)
+                streamline_arrowsize: float
+                    Factor scale arrow size for streamlines.
+                    (only used for streamline plots)
+                linewidth: float
+                    Linewidths for streamlines.
+                    (only used for streamline plots)
     Parameters
     ----------
     dataset : grid
         grid object
 
     prdcfg : dictionary of dictionaries
         product configuration dictionary of dictionaries
@@ -799,9 +837,168 @@
 
         pyart.io.write_grid(fname, new_dataset, write_point_x_y_z=True,
                             write_point_lon_lat_alt=True)
         print('saved file: '+fname)
 
         return fname
 
-    warn(' Unsupported product type: ' + prdcfg['type'])
-    return None
+    if prdcfg['type'] == 'DDA_MAP':
+
+        display_type = prdcfg.get('display_type', 'quiver')
+        if display_type not in ['quiver', 'barbs', 'streamline']:
+            warn(
+                'Invalid display_type, must be ' +
+                '"streamline", "quiver" or "barbs"'
+            )
+            return None
+
+        bg_field_name = get_fieldname_pyart(prdcfg['voltype'])
+        bg_ref_rad = prdcfg.get('bg_ref_rad', 0)
+        # get bg field name given which radar serves as reference
+        if bg_ref_rad != 0:
+            bg_field_name += '_radar{:d}'.format(bg_ref_rad)
+
+        if bg_field_name not in dataset['radar_out'].fields:
+            warn(
+                ' Field type ' + field_name +
+                ' not available in data set. Skipping product ' +
+                prdcfg['type'])
+            return None
+
+        # user defined values
+        level = prdcfg.get('level', 0)
+        alpha = prdcfg.get('alpha', 1)
+
+        savedir = get_save_dir(
+            prdcfg['basepath'], prdcfg['procname'], dssavedir,
+            prdcfg['prdname'], timeinfo=prdcfg['timeinfo'])
+
+        fname_list = make_filename(
+            'dda_map', prdcfg['dstype'], prdcfg['voltype'],
+            prdcfg['imgformat'], prdcfginfo='l'+str(level),
+            timeinfo=prdcfg['timeinfo'], runinfo=prdcfg['runinfo'])
+
+        for i, fname in enumerate(fname_list):
+            fname_list[i] = savedir+fname
+
+        titl = generate_dda_map_title(dataset['radar_out'], bg_field_name, level)
+
+        plot_dda_map(
+            dataset['radar_out'], bg_field_name, level, prdcfg, fname_list,
+            alpha = alpha, display_type = display_type, titl = titl)
+
+        print('----- save to '+' '.join(fname_list))
+
+    if prdcfg['type'] == 'DDA_LONGITUDE_SLICE':
+
+        display_type = prdcfg.get('display_type', 'quiver')
+        if display_type not in ['quiver', 'barbs', 'streamline']:
+            warn(
+                'Invalid display_type, must be ' +
+                '"streamline", "quiver" or "barbs"'
+            )
+            return None
+
+        bg_field_name = get_fieldname_pyart(prdcfg['voltype'])
+        bg_ref_rad = prdcfg.get('bg_ref_rad', 0)
+        # get bg field name given which radar serves as reference
+        if bg_ref_rad != 0:
+            bg_field_name += '_radar{:d}'.format(bg_ref_rad)
+
+        if bg_field_name not in dataset['radar_out'].fields:
+            warn(
+                ' Field type ' + field_name +
+                ' not available in data set. Skipping product ' +
+                prdcfg['type'])
+            return None
+
+        # user defined values
+        lon = prdcfg.get(
+            'lon', dataset['radar_out'].origin_longitude['data'][0])
+        lat = prdcfg.get(
+            'lat', dataset['radar_out'].origin_latitude['data'][0])
+        alpha = prdcfg.get('alpha', 1)
+        wind_vectors = prdcfg.get('wind_vectors', 'hor')
+
+        # Find indexes where to slice with a pyart display object
+        # this is a bit clumsy
+        display = pyart.graph.GridMapDisplay(dataset['radar_out'])
+        level, _ = display._find_nearest_grid_indices(lon, lat)
+
+        savedir = get_save_dir(
+            prdcfg['basepath'], prdcfg['procname'], dssavedir,
+            prdcfg['prdname'], timeinfo=prdcfg['timeinfo'])
+
+        fname_list = make_filename(
+            'dda_lon_slice', prdcfg['dstype'], prdcfg['voltype'],
+            prdcfg['imgformat'], prdcfginfo='l'+str(level),
+            timeinfo=prdcfg['timeinfo'], runinfo=prdcfg['runinfo'])
+
+        for i, fname in enumerate(fname_list):
+            fname_list[i] = savedir+fname
+
+        titl = generate_dda_longitude_slice_title(dataset['radar_out'], bg_field_name, level)
+
+        plot_dda_slice(
+            dataset['radar_out'], bg_field_name, 'longitude', level, prdcfg, fname_list,
+            alpha = alpha, display_type = display_type, titl = titl, wind_vectors = wind_vectors)
+
+        print('----- save to '+' '.join(fname_list))
+
+    if prdcfg['type'] == 'DDA_LATITUDE_SLICE':
+
+        display_type = prdcfg.get('display_type', 'quiver')
+        if display_type not in ['quiver', 'barbs', 'streamline']:
+            warn(
+                'Invalid display_type, must be ' +
+                '"streamline", "quiver" or "barbs"'
+            )
+            return None
+
+        bg_field_name = get_fieldname_pyart(prdcfg['voltype'])
+        bg_ref_rad = prdcfg.get('bg_ref_rad', 0)
+        # get bg field name given which radar serves as reference
+        if bg_ref_rad != 0:
+            bg_field_name += '_radar{:d}'.format(bg_ref_rad)
+
+        if bg_field_name not in dataset['radar_out'].fields:
+            warn(
+                ' Field type ' + field_name +
+                ' not available in data set. Skipping product ' +
+                prdcfg['type'])
+            return None
+
+        # user defined values
+        lon = prdcfg.get(
+            'lon', dataset['radar_out'].origin_longitude['data'][0])
+        lat = prdcfg.get(
+            'lat', dataset['radar_out'].origin_latitude['data'][0])
+        alpha = prdcfg.get('alpha', 1)
+        wind_vectors = prdcfg.get('wind_vectors', 'hor')
+
+        # Find indexes where to slice with a pyart display object
+        # this is a bit clumsy
+        display = pyart.graph.GridMapDisplay(dataset['radar_out'])
+        _, level = display._find_nearest_grid_indices(lon, lat)
+
+        savedir = get_save_dir(
+            prdcfg['basepath'], prdcfg['procname'], dssavedir,
+            prdcfg['prdname'], timeinfo=prdcfg['timeinfo'])
+
+        fname_list = make_filename(
+            'dda_lat_slice', prdcfg['dstype'], prdcfg['voltype'],
+            prdcfg['imgformat'], prdcfginfo='l'+str(level),
+            timeinfo=prdcfg['timeinfo'], runinfo=prdcfg['runinfo'])
+
+        for i, fname in enumerate(fname_list):
+            fname_list[i] = savedir+fname
+
+        titl = generate_dda_latitude_slice_title(dataset['radar_out'], bg_field_name, level)
+
+        plot_dda_slice(
+            dataset['radar_out'], bg_field_name, 'latitude', level, prdcfg, fname_list,
+            alpha = alpha, display_type = display_type, titl = titl, wind_vectors = wind_vectors)
+
+        print('----- save to '+' '.join(fname_list))
+
+    else:
+        return None
```

### Comparing `pyrad_mch-1.7.0/pyrad/prod/process_intercomp_products.py` & `pyrad_mch-1.8.0/pyrad/prod/process_intercomp_products.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/prod/process_monitoring_products.py` & `pyrad_mch-1.8.0/pyrad/prod/process_monitoring_products.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/prod/process_product.py` & `pyrad_mch-1.8.0/pyrad/prod/process_product.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/prod/process_spectra_products.py` & `pyrad_mch-1.8.0/pyrad/prod/process_spectra_products.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/prod/process_timeseries_products.py` & `pyrad_mch-1.8.0/pyrad/prod/process_timeseries_products.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/prod/process_traj_products.py` & `pyrad_mch-1.8.0/pyrad/prod/process_traj_products.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/prod/process_vol_products.py` & `pyrad_mch-1.8.0/pyrad/prod/process_vol_products.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/prod/product_aux.py` & `pyrad_mch-1.8.0/pyrad/prod/product_aux.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/util/__init__.py` & `pyrad_mch-1.8.0/pyrad/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/util/radar_utils.py` & `pyrad_mch-1.8.0/pyrad/util/radar_utils.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad/util/stat_utils.py` & `pyrad_mch-1.8.0/pyrad/util/stat_utils.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/pyrad_mch.egg-info/PKG-INFO` & `pyrad_mch-1.8.0/pyrad_mch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrad-mch
-Version: 1.7.0
+Version: 1.8.0
 Summary:  Python Radar Toolkit
 Home-page: https://github.com/MeteoSwiss/pyrad.git
 Author: MeteoSwiss Pyrad Developers
 Author-email: daniel.wolfensberger@meteoswiss.ch
 Maintainer: MeteoSwiss Pyrad Developers
 Maintainer-email: daniel.wolfensberger@meteoswiss.ch
 License: BSD
```

### Comparing `pyrad_mch-1.7.0/pyrad_mch.egg-info/SOURCES.txt` & `pyrad_mch-1.8.0/pyrad_mch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/scripts/common_colocated_gates.py` & `pyrad_mch-1.8.0/scripts/common_colocated_gates.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/scripts/main_precipitation_comparison.py` & `pyrad_mch-1.8.0/scripts/main_precipitation_comparison.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/scripts/main_process_cosmo.py` & `pyrad_mch-1.8.0/scripts/main_process_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/scripts/main_process_cosmo_rt.py` & `pyrad_mch-1.8.0/scripts/main_process_cosmo_rt.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/scripts/main_process_data.py` & `pyrad_mch-1.8.0/scripts/main_process_data.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/scripts/main_process_data_birds.py` & `pyrad_mch-1.8.0/scripts/main_process_data_birds.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/scripts/main_process_data_period.py` & `pyrad_mch-1.8.0/scripts/main_process_data_period.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/scripts/main_process_data_rt.py` & `pyrad_mch-1.8.0/scripts/main_process_data_rt.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/scripts/main_process_data_trt.py` & `pyrad_mch-1.8.0/scripts/main_process_data_trt.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/scripts/main_process_euclid_data.py` & `pyrad_mch-1.8.0/scripts/main_process_euclid_data.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/scripts/main_process_gecsx.py` & `pyrad_mch-1.8.0/scripts/main_process_gecsx.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/scripts/movie_maker.py` & `pyrad_mch-1.8.0/scripts/movie_maker.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/scripts/rewrite_monitoring.py` & `pyrad_mch-1.8.0/scripts/rewrite_monitoring.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.7.0/setup.py` & `pyrad_mch-1.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 LONG_DESCRIPTION = "\n".join(DOCLINES[2:])
 URL = "https://github.com/MeteoSwiss/pyrad.git"
 DOWNLOAD_URL = "https://github.com/MeteoSwiss/pyrad.git"
 LICENSE = 'BSD'
 CLASSIFIERS = list(filter(None, CLASSIFIERS.split('\n')))
 PLATFORMS = ["Linux"]
 MAJOR = 1
-MINOR = 7
+MINOR = 8
 MICRO = 0
 ISRELEASED = True
 VERSION = '%d.%d.%d' % (MAJOR, MINOR, MICRO)
 SCRIPTS = glob.glob('scripts/*')
 COMPILE_DATE_TIME = datetime.utcnow().strftime("%Y-%m-%d %H:%M")
 USERNAME = getpass.getuser()
```

