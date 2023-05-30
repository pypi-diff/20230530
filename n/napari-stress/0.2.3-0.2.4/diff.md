# Comparing `tmp/napari_stress-0.2.3.tar.gz` & `tmp/napari_stress-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_stress-0.2.3.tar", last modified: Wed Mar 15 23:22:16 2023, max compression
+gzip compressed data, was "napari_stress-0.2.4.tar", last modified: Tue May 30 10:22:21 2023, max compression
```

## Comparing `napari_stress-0.2.3.tar` & `napari_stress-0.2.4.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:22:16.013634 napari_stress-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-03-15 23:21:59.000000 napari_stress-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-15 23:21:59.000000 napari_stress-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-03-15 23:22:16.013634 napari_stress-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-03-15 23:21:59.000000 napari_stress-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-15 23:21:59.000000 napari_stress-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-15 23:22:16.013634 napari_stress-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-15 23:21:59.000000 napari_stress-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:22:16.001634 napari_stress-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:22:16.005634 napari_stress-0.2.3/src/napari_stress/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:22:16.005634 napari_stress-0.2.3/src/napari_stress/_approximation/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_approximation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_approximation/fit_ellipsoid.py
--rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_deprecated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:22:16.009634 napari_stress-0.2.3/src/napari_stress/_measurements/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_measurements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_measurements/curvature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_measurements/deviation_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13167 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_measurements/geodesics.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_measurements/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_measurements/stresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_measurements/temporal_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_measurements/toolbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_measurements/toolbox.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_measurements/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_napari_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:22:16.009634 napari_stress-0.2.3/src/napari_stress/_plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_plotting/features_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:22:16.009634 napari_stress-0.2.3/src/napari_stress/_reconstruction/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_reconstruction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_reconstruction/reconstruct_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_reconstruction/refine_surfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_reconstruction/toolbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    13632 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_reconstruction/toolbox.ui
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:22:16.009634 napari_stress-0.2.3/src/napari_stress/_sample_data/
--rw-r--r--   0 runner    (1001) docker     (123)   354896 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_sample_data/ExampleTifSequence.tif
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_sample_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66687 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_sample_data/dropplet_point_cloud.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1808756 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_sample_data/dropplet_point_cloud_4d.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-03-15 23:21:59.000000 napari_stress-0.2.3/src/napari_stress/_sample_data/sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:22:16.013634 napari_stress-0.2.3/src/napari_stress/_spherical_harmonics/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_spherical_harmonics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_spherical_harmonics/spherical_harmonics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_spherical_harmonics/spherical_harmonics_napari.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:22:16.013634 napari_stress-0.2.3/src/napari_stress/_stress/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_stress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_stress/charts_SPB.py
--rw-r--r--   0 runner    (1001) docker     (123)    69024 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_stress/euclidian_k_form_SPB.py
--rw-r--r--   0 runner    (1001) docker     (123)    21801 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_stress/lebedev_info_SPB.py
--rw-r--r--   0 runner    (1001) docker     (123)   132687 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_stress/lebedev_write_SPB.py
--rw-r--r--   0 runner    (1001) docker     (123)    63394 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_stress/manifold_SPB.py
--rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_stress/sph_func_SPB.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_surface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:22:16.013634 napari_stress-0.2.3/src/napari_stress/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_tests/test_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_tests/test_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_tests/test_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_tests/test_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_tests/test_spherical_harmonic_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_tests/test_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:22:16.013634 napari_stress-0.2.3/src/napari_stress/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_utils/coordinate_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_utils/fit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20150 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_utils/frame_by_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-03-15 23:22:00.000000 napari_stress-0.2.3/src/napari_stress/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:22:16.005634 napari_stress-0.2.3/src/napari_stress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-03-15 23:22:15.000000 napari_stress-0.2.3/src/napari_stress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-03-15 23:22:16.000000 napari_stress-0.2.3/src/napari_stress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 23:22:15.000000 napari_stress-0.2.3/src/napari_stress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-15 23:22:15.000000 napari_stress-0.2.3/src/napari_stress.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-15 23:22:15.000000 napari_stress-0.2.3/src/napari_stress.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-15 23:22:15.000000 napari_stress-0.2.3/src/napari_stress.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.527933 napari_stress-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-30 10:22:03.000000 napari_stress-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-30 10:22:03.000000 napari_stress-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-30 10:22:21.527933 napari_stress-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-30 10:22:03.000000 napari_stress-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-30 10:22:04.000000 napari_stress-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-30 10:22:21.527933 napari_stress-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-30 10:22:04.000000 napari_stress-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.515933 napari_stress-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.519933 napari_stress-0.2.4/src/napari_stress/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.519933 napari_stress-0.2.4/src/napari_stress/_approximation/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_approximation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_approximation/fit_ellipsoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.519933 napari_stress-0.2.4/src/napari_stress/_measurements/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/curvature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/deviation_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13167 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/geodesics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/stresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/temporal_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20106 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/toolbox.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_measurements/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_napari_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.519933 napari_stress-0.2.4/src/napari_stress/_plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_plotting/features_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.519933 napari_stress-0.2.4/src/napari_stress/_reconstruction/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_reconstruction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_reconstruction/reconstruct_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_reconstruction/refine_surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_reconstruction/toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13632 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_reconstruction/toolbox.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.523933 napari_stress-0.2.4/src/napari_stress/_sample_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   354896 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_sample_data/ExampleTifSequence.tif
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_sample_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66687 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_sample_data/dropplet_point_cloud.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1808756 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_sample_data/dropplet_point_cloud_4d.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_sample_data/sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.523933 napari_stress-0.2.4/src/napari_stress/_spherical_harmonics/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_spherical_harmonics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_spherical_harmonics/spherical_harmonics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_spherical_harmonics/spherical_harmonics_napari.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.523933 napari_stress-0.2.4/src/napari_stress/_stress/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_stress/charts_SPB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69024 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_stress/euclidian_k_form_SPB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21801 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_stress/lebedev_info_SPB.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132687 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_stress/lebedev_write_SPB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63394 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_stress/manifold_SPB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_stress/sph_func_SPB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_surface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.527933 napari_stress-0.2.4/src/napari_stress/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19681 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_spherical_harmonic_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_tests/test_vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.527933 napari_stress-0.2.4/src/napari_stress/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_utils/coordinate_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_utils/fit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20150 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_utils/frame_by_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-30 10:22:04.000000 napari_stress-0.2.4/src/napari_stress/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:22:21.519933 napari_stress-0.2.4/src/napari_stress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-30 10:22:21.000000 napari_stress-0.2.4/src/napari_stress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-30 10:22:21.000000 napari_stress-0.2.4/src/napari_stress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:22:21.000000 napari_stress-0.2.4/src/napari_stress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 10:22:21.000000 napari_stress-0.2.4/src/napari_stress.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-30 10:22:21.000000 napari_stress-0.2.4/src/napari_stress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 10:22:21.000000 napari_stress-0.2.4/src/napari_stress.egg-info/top_level.txt
```

### Comparing `napari_stress-0.2.3/LICENSE` & `napari_stress-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/PKG-INFO` & `napari_stress-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_stress
-Version: 0.2.3
+Version: 0.2.4
 Summary: Interactive surface analysis in napari for measuring mechanical stresses in biological tissues
 Author: Johannes Soltwedel, Ben J. Gross, Elijah Shelton, Carlos Gomez, Otger Campas
 Author-email: johannes_richard.mueller@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/campaslab/napari-stress/issues
 Project-URL: Documentation, https://campaslab.github.io/napari-stress
 Project-URL: Source Code, https://github.com/campaslab/napari-stress
```

### Comparing `napari_stress-0.2.3/README.md` & `napari_stress-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/setup.cfg` & `napari_stress-0.2.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari_stress
-version = 0.2.3
+version = 0.2.4
 description = Interactive surface analysis in napari for measuring mechanical stresses in biological tissues
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Johannes Soltwedel, Ben J. Gross, Elijah Shelton, Carlos Gomez, Otger Campas
 author_email = johannes_richard.mueller@tu-dresden.de
 license = BSD-3-Clause
 license_file = LICENSE
```

### Comparing `napari_stress-0.2.3/src/napari_stress/__init__.py` & `napari_stress-0.2.4/src/napari_stress/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 
 from . import _measurements as measurements
 from . import _approximation as approximation
 from . import _reconstruction as reconstruction
 from . import _sample_data as sample_data
 
 from ._preprocess import rescale
```

### Comparing `napari_stress-0.2.3/src/napari_stress/_approximation/fit_ellipsoid.py` & `napari_stress-0.2.4/src/napari_stress/_approximation/fit_ellipsoid.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from napari.types import PointsData, VectorsData
 from .._utils.frame_by_frame import frame_by_frame
 from napari_tools_menu import register_function
-
 import numpy as np
 
+
 @register_function(menu="Points > Fit ellipsoid to pointcloud (n-STRESS)")
 @frame_by_frame
 def least_squares_ellipsoid(points: PointsData
                             ) -> VectorsData:
     """
     Fit ellipsoid to points with a last-squares approach.
 
@@ -18,29 +18,31 @@
     points : PointsData
 
     Returns
     -------
     VectorsData: Major/minor axis of the ellipsoid
     """
     from .._utils.coordinate_conversion import polynomial_to_parameters3D
-    coefficients = solve_ellipsoid_polynomial(points)    
+    coefficients = _solve_ellipsoid_polynomial(points)    
 
     # convert results to VectorsData
-    center, axes, R, R_inverse = polynomial_to_parameters3D(coefficients=coefficients)
+    center, axes, R, R_inverse = polynomial_to_parameters3D(
+        coefficients=coefficients)
     direction = R * axes[:, None]
     origin = np.stack(3 * [center])  # cheap repeat
-    vector = np.stack([origin, direction]).transpose((1,0,2))
+    vector = np.stack([origin, direction]).transpose((1, 0, 2))
 
     return vector
 
+
 @register_function(menu="Points > Calculate normals on ellipsoid (n-STRESS)")
 @frame_by_frame
 def normals_on_ellipsoid(points: PointsData) -> VectorsData:
     """Retrieve normal vector on ellipsoid points."""
-    coefficients = solve_ellipsoid_polynomial(points)
+    coefficients = _solve_ellipsoid_polynomial(points)
 
     A = coefficients.flatten()[0]
     B = coefficients.flatten()[1]	
     C = coefficients.flatten()[2]	
     D = coefficients.flatten()[3]	
     E = coefficients.flatten()[4]	
     F = coefficients.flatten()[5]	
@@ -49,73 +51,69 @@
     I = coefficients.flatten()[8]		
 
     xx = points[:, 0][:, None]
     yy = points[:, 1][:, None]
     zz = points[:, 2][:, None]
 
     grad_F_x = 2.*A*xx + D*yy + E*zz + G
-    grad_F_y = 2.*B*yy + D*xx + F*zz + H 
+    grad_F_y = 2.*B*yy + D*xx + F*zz + H
     grad_F_z = 2.*C*zz + E*xx + F*yy + I
 
-    grad_F_X = np.hstack(( grad_F_x, grad_F_y, grad_F_z )) 
-    Vec_Norms = np.sqrt(np.sum(np.multiply(grad_F_X, grad_F_X), axis = 1)).reshape(len(xx), 1)
+    grad_F_X = np.hstack((grad_F_x, grad_F_y, grad_F_z))
+    Vec_Norms = np.sqrt(
+        np.sum(np.multiply(grad_F_X, grad_F_X), axis=1)).reshape(len(xx), 1)
     grad_F_X_normed = np.divide(grad_F_X, Vec_Norms)
-	
-    return np.stack([points, grad_F_X_normed]).transpose((1,0,2))
 
+    return np.stack([points, grad_F_X_normed]).transpose((1, 0, 2))
 
-def solve_ellipsoid_polynomial(points: PointsData) -> np.ndarray:
+
+def _solve_ellipsoid_polynomial(points: PointsData) -> np.ndarray:
     """
     Fit ellipsoid polynomial equation.
-    
-    finds best fit ellipsoid. Found at http://www.juddzone.com/ALGORITHMS/least_squares_3D_ellipsoid.html
+
+    Found at http://www.juddzone.com/ALGORITHMS/least_squares_3D_ellipsoid.html
     least squares fit to a 3D-ellipsoid
      Ax^2 + By^2 + Cz^2 +  Dxy +  Exz +  Fyz +  Gx +  Hy +  Iz  = 1
-    
+
     Note that sometimes it is expressed as a solution to
      Ax^2 + By^2 + Cz^2 + 2Dxy + 2Exz + 2Fyz + 2Gx + 2Hy + 2Iz  = 1
     where the last six terms have a factor of 2 in them
-    This is in anticipation of forming a matrix with the polynomial coefficients.
-    Those terms with factors of 2 are all off diagonal elements.  These contribute
-    two terms when multiplied out (symmetric) so would need to be divided by two
-    """    
+    This is in anticipation of forming a matrix with the polynomial
+    coefficients. Those terms with factors of 2 are all off diagonal
+    elements. These contribute two terms when multiplied out
+    (symmetric) so would need to be divided by two
+    """
 
     # change xx from vector of length N to Nx1 matrix so we can use hstack
     x = points[:, 0, np.newaxis]
     y = points[:, 1, np.newaxis]
     z = points[:, 2, np.newaxis]
 
     #  Ax^2 + By^2 + Cz^2 +  Dxy +  Exz +  Fyz +  Gx +  Hy +  Iz = 1
-    J = np.hstack((x*x,y*y,z*z,x*y,x*z,y*z, x, y, z))
-    K = np.ones_like(x) #column of ones
+    J = np.hstack((x * x, y * y, z * z, x * y, x * z, y * z, x, y, z))
+    K = np.ones_like(x)  # column of ones
 
-    #np.hstack performs a loop over all samples and creates
-    #a row in J for each x,y,z sample:
-    # J[ix,0] = x[ix]*x[ix]
-    # J[ix,1] = y[ix]*y[ix]
-    # etc.
-
-    JT=J.transpose()
-    JTJ = np.dot(JT,J)
-    InvJTJ = np.linalg.inv(JTJ);
-    ABC= np.dot(InvJTJ, np.dot(JT,K)) #!!!! LOOK AT RESIDUALS TO GET ELLIPSOID ERRORS !!!!#
+    JT = J.transpose()
+    JTJ = np.dot(JT, J)
+    InvJTJ = np.linalg.inv(JTJ)
+    ABC = np.dot(InvJTJ, np.dot(JT, K))
 
     # Rearrange, move the 1 to the other side
     #  Ax^2 + By^2 + Cz^2 +  Dxy +  Exz +  Fyz +  Gx +  Hy +  Iz - 1 = 0
     #    or
     #  Ax^2 + By^2 + Cz^2 +  Dxy +  Exz +  Fyz +  Gx +  Hy +  Iz + J = 0
     #  where J = -1
-    eansa = np.append(ABC,-1)
+    eansa = np.append(ABC, -1)
 
     return eansa
 
-    
-
 
-@register_function(menu="Points > Expand point locations on ellipsoid (n-STRESS)")
+@register_function(
+        menu="Points > Expand point locations on ellipsoid (n-STRESS)"
+        )
 @frame_by_frame
 def expand_points_on_ellipse(fitted_ellipsoid: VectorsData,
                              pointcloud: PointsData) -> PointsData:
     """
     Expand a pointcloud on the surface of a fitted ellipse.
 
     This function takes a ellipsoid (in the form of the major axes) and a
@@ -135,39 +133,11 @@
     """
     from .._utils.coordinate_conversion import (
         cartesian_to_elliptical,
         elliptical_to_cartesian
         )
 
     U, V = cartesian_to_elliptical(fitted_ellipsoid, pointcloud)
-    points_on_fitted_ellipse =  elliptical_to_cartesian(U, V, fitted_ellipsoid)
+    points_on_fitted_ellipse = elliptical_to_cartesian(U, V, fitted_ellipsoid)
 
     return points_on_fitted_ellipse
 
-@register_function(menu="Points > Pairwise distances (n-STRESS)")
-@frame_by_frame
-def pairwise_point_distances(points: PointsData,
-                             fitted_points: PointsData) -> VectorsData:
-    """
-    Calculate pairwise distances between pointclouds.
-
-    Parameters
-    ----------
-    points : PointsData
-    fitted_points : PointsData
-
-    Raises
-    ------
-    ValueError
-        Both pointclouds must have the same number of points.
-
-    Returns
-    -------
-    VectorsData
-
-    """
-    if not len(points) == len(fitted_points):
-        raise ValueError('Both pointclouds must have same length, but had'
-                         f'{len(points)} and {len(fitted_points)}.')
-
-    delta = points - fitted_points
-    return np.stack([fitted_points, delta]).transpose((1,0,2))
```

### Comparing `napari_stress-0.2.3/src/napari_stress/_deprecated.py` & `napari_stress-0.2.4/src/napari_stress/_deprecated.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_measurements/__init__.py` & `napari_stress-0.2.4/src/napari_stress/_measurements/__init__.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_measurements/curvature.py` & `napari_stress-0.2.4/src/napari_stress/_measurements/curvature.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_measurements/deviation_analysis.py` & `napari_stress-0.2.4/src/napari_stress/_measurements/deviation_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 import napari
 
 @register_function(menu="Measurement > Measure deviation from ellipsoid (n-STRESS)")
 @frame_by_frame
 def deviation_from_ellipsoidal_mode(points: PointsData,
                                     max_degree:int=5,
                                     viewer: napari.Viewer = None) -> LayerDataTuple:
-    from napari_stress import approximation
+    from napari_stress import approximation, vectors
     from .._utils.fit_utils import Least_Squares_Harmonic_Fit
     from .._utils.coordinate_conversion import cartesian_to_elliptical
     from .._stress import sph_func_SPB as sph_f
     import numpy as np
 
     from ..types import _METADATAKEY_ELIPSOID_DEVIATION_CONTRIB
     
     # calculate errors
     ellipsoid = approximation.least_squares_ellipsoid(points)
     ellipsoid_points = approximation.expand_points_on_ellipse(ellipsoid, points)
-    errors = approximation.pairwise_point_distances(points, ellipsoid_points)[:, 1]
+    errors = vectors.pairwise_point_distances(points, ellipsoid_points)[:, 1]
     normals = approximation.normals_on_ellipsoid(ellipsoid_points)[:, 1]
     signed_errors = -1.*np.multiply(normals, errors).sum(axis=1)
 
     # least squares harmonic fit
     longitude, latitude = cartesian_to_elliptical(ellipsoid, points)
     coefficients = Least_Squares_Harmonic_Fit(
                     fit_degree=max_degree,
```

### Comparing `napari_stress-0.2.3/src/napari_stress/_measurements/geodesics.py` & `napari_stress-0.2.4/src/napari_stress/_measurements/geodesics.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_measurements/measurements.py` & `napari_stress-0.2.4/src/napari_stress/_measurements/measurements.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_measurements/stresses.py` & `napari_stress-0.2.4/src/napari_stress/_measurements/stresses.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_measurements/temporal_correlation.py` & `napari_stress-0.2.4/src/napari_stress/_measurements/temporal_correlation.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_measurements/toolbox.py` & `napari_stress-0.2.4/src/napari_stress/_measurements/toolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,15 @@
     --------
 
     [0]
     """
     from .. import approximation
     from .. import measurements
     from .. import reconstruction
+    from .. import vectors
 
     from ..types import (_METADATAKEY_MEAN_CURVATURE,
                          _METADATAKEY_MEAN_CURVATURE_DIFFERENCE,
                          _METADATAKEY_H_E123_ELLIPSOID,
                          _METADATAKEY_ANISO_STRESS_TISSUE,
                          _METADATAKEY_ANISO_STRESS_CELL,
                          _METADATAKEY_ANISO_STRESS_TOTAL,
@@ -208,21 +209,21 @@
     quadrature_points_ellipsoid = approximation.expand_points_on_ellipse(
         ellipsoid, quadrature_points)
 
     # =========================================================================
     # Evaluate fit quality
     # =========================================================================
     # Spherical harmonics
-    residue_spherical_harmonics = approximation.pairwise_point_distances(
+    residue_spherical_harmonics = vectors.pairwise_point_distances(
         pointcloud, fitted_pointcloud)
     residue_spherical_harmonics_norm = np.linalg.norm(
         residue_spherical_harmonics[:, 1], axis=1)
 
     # Ellipsoid
-    residue_ellipsoid = approximation.pairwise_point_distances(
+    residue_ellipsoid = vectors.pairwise_point_distances(
         pointcloud, ellipsoid_points)
     residue_ellipsoid_norm = np.linalg.norm(
         residue_ellipsoid[:, 1], axis=1)
 
     # =========================================================================
     # (mean) curvature on droplet and ellipsoid
     # =========================================================================
@@ -289,15 +290,15 @@
 
     GDM = None
     if GDM is None:
         GDM = measurements.geodesic_distance_matrix(surface_cell_stress,
                                                     show_progress=verbose)
 
     if maximal_distance is None:
-        maximal_distance = int(np.floor(GDM.max()))
+        maximal_distance = int(np.floor(np.nanmax(GDM[GDM != np.inf])))
 
     # Compute Overall total stress spatial correlations
     autocorrelations_total = measurements.correlation_on_surface(
         surface_total_stress,
         surface_total_stress,
         distance_matrix=GDM,
         maximal_distance=maximal_distance)
```

### Comparing `napari_stress-0.2.3/src/napari_stress/_measurements/toolbox.ui` & `napari_stress-0.2.4/src/napari_stress/_measurements/toolbox.ui`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_measurements/utils.py` & `napari_stress-0.2.4/src/napari_stress/_measurements/utils.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_plotting/features_histogram.py` & `napari_stress-0.2.4/src/napari_stress/_plotting/features_histogram.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_preprocess.py` & `napari_stress-0.2.4/src/napari_stress/_preprocess.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_reconstruction/reconstruct_surface.py` & `napari_stress-0.2.4/src/napari_stress/_reconstruction/reconstruct_surface.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_reconstruction/refine_surfaces.py` & `napari_stress-0.2.4/src/napari_stress/_reconstruction/refine_surfaces.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_reconstruction/toolbox.py` & `napari_stress-0.2.4/src/napari_stress/_reconstruction/toolbox.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_reconstruction/toolbox.ui` & `napari_stress-0.2.4/src/napari_stress/_reconstruction/toolbox.ui`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_sample_data/ExampleTifSequence.tif` & `napari_stress-0.2.4/src/napari_stress/_sample_data/ExampleTifSequence.tif`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_sample_data/dropplet_point_cloud.csv` & `napari_stress-0.2.4/src/napari_stress/_sample_data/dropplet_point_cloud.csv`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_sample_data/dropplet_point_cloud_4d.csv` & `napari_stress-0.2.4/src/napari_stress/_sample_data/dropplet_point_cloud_4d.csv`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_spherical_harmonics/spherical_harmonics.py` & `napari_stress-0.2.4/src/napari_stress/_spherical_harmonics/spherical_harmonics.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_spherical_harmonics/spherical_harmonics_napari.py` & `napari_stress-0.2.4/src/napari_stress/_spherical_harmonics/spherical_harmonics_napari.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_stress/charts_SPB.py` & `napari_stress-0.2.4/src/napari_stress/_stress/charts_SPB.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_stress/euclidian_k_form_SPB.py` & `napari_stress-0.2.4/src/napari_stress/_stress/euclidian_k_form_SPB.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_stress/lebedev_info_SPB.py` & `napari_stress-0.2.4/src/napari_stress/_stress/lebedev_info_SPB.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_stress/lebedev_write_SPB.py` & `napari_stress-0.2.4/src/napari_stress/_stress/lebedev_write_SPB.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_stress/manifold_SPB.py` & `napari_stress-0.2.4/src/napari_stress/_stress/manifold_SPB.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_stress/sph_func_SPB.py` & `napari_stress-0.2.4/src/napari_stress/_stress/sph_func_SPB.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_surface.py` & `napari_stress-0.2.4/src/napari_stress/_surface.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_tests/test_approximation.py` & `napari_stress-0.2.4/src/napari_stress/_tests/test_approximation.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,20 +81,7 @@
     results = measurements.curvature_on_ellipsoid(ellipsoid_stress,
                                                   fitted_points_stress)
 
     assert types._METADATAKEY_H_E123_ELLIPSOID in results[1]['metadata'].keys()
     assert types._METADATAKEY_H0_ELLIPSOID in results[1]['metadata'].keys()
     assert types._METADATAKEY_MEAN_CURVATURE in results[1]['features'].keys()
 
-
-def test_pairwise_distance():
-    from napari_stress import approximation, get_droplet_point_cloud
-    pointcloud = get_droplet_point_cloud()[0][0][:, 1:]
-
-    ellipsoid = approximation.least_squares_ellipsoid(pointcloud)
-    fitted_points = approximation.expand_points_on_ellipse(ellipsoid, pointcloud)
-
-    distances = approximation.pairwise_point_distances(pointcloud, fitted_points)
-
-if __name__ == '__main__':
-    import napari
-    test_ellipse_normals()
```

### Comparing `napari_stress-0.2.3/src/napari_stress/_tests/test_plotting.py` & `napari_stress-0.2.4/src/napari_stress/_tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_tests/test_processing.py` & `napari_stress-0.2.4/src/napari_stress/_tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_tests/test_reconstruction.py` & `napari_stress-0.2.4/src/napari_stress/_tests/test_reconstruction.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 # -*- coding: utf-8 -*-
 import numpy as np
 
+
 def test_reconstruction(make_napari_viewer):
     from napari_stress import reconstruction, get_droplet_4d
-    import napari_process_points_and_surfaces as nppas
-    from skimage import measure
     from napari.layers import Layer
 
-
     viewer = make_napari_viewer()
-
-
     image = get_droplet_4d()[0][0]
     viewer.add_image(image)
 
     widget = reconstruction.droplet_reconstruction_toolbox(viewer)
     viewer.window.add_dock_widget(widget)
 
     results = reconstruction.reconstruct_droplet(
@@ -32,14 +28,15 @@
         image,
         voxelsize=np.asarray([1.93, 1, 1]),
         target_voxelsize=1,
         resampling_length=1,
         use_dask=True
         )
 
+
 def test_quadrature_point_reconstuction(make_napari_viewer):
     from napari_stress import get_droplet_point_cloud, fit_spherical_harmonics
     from napari_stress import reconstruction
     from napari_stress._spherical_harmonics.spherical_harmonics_napari import perform_lebedev_quadrature
 
     pointcloud = get_droplet_point_cloud()[0]
     # Expansion
@@ -47,95 +44,109 @@
     points = fit_spherical_harmonics(pointcloud[0], max_degree=3)
     points_layer = viewer.add_points(points[0], **points[1])
 
     # quadrature
     lebedev_points = perform_lebedev_quadrature(points_layer, viewer=viewer)[0]
     reconstruction.reconstruct_surface_from_quadrature_points(lebedev_points)
 
+
 def test_vector_tools():
     from napari_stress import vectors
     import vedo
     import numpy as np
 
     sphere = vedo.Sphere(r=10, pos=(50, 50, 50))
     image = np.random.rand(100, 100, 100)
     sampling_distance = 0.25
 
     vectors.normal_vectors_on_pointcloud(sphere.points())
-    normal_vectors = vectors.normal_vectors_on_surface((sphere.points(), np.asarray(sphere.faces())))
-    df_intensity = vectors.sample_intensity_along_vector(normal_vectors, image, sampling_distance=sampling_distance)
+    normal_vectors = vectors.normal_vectors_on_surface(
+        (sphere.points(),
+         np.asarray(sphere.faces())))
+    df_intensity = vectors.sample_intensity_along_vector(
+        normal_vectors, image, sampling_distance=sampling_distance)
 
     assert df_intensity.shape[0] == normal_vectors.shape[0]
     assert df_intensity.shape[1] == 1/sampling_distance
 
+
 def test_surface_tracing():
     from napari_stress import reconstruction
-    from skimage import filters, morphology, io, measure
+    from skimage import filters, morphology
     from vedo import shapes
 
     true_radius = 30
 
     # Make a blurry sphere first
     image = np.zeros([100, 100, 100])
     image[50 - 30:50 + 31,
           50 - 30:50 + 31,
           50 - 30:50 + 31] = morphology.ball(radius=true_radius)
-    blurry_sphere = filters.gaussian(image, sigma = 5)
+    blurry_sphere = filters.gaussian(image, sigma=5)
 
     # Put surface points on a slightly larger radius and add a bit of noise
     surf_points = shapes.Sphere().points()
     surf_points += (surf_points * true_radius + 2) + 50
 
     # Test different fit methods (fancy/quick)
     fit_type = 'quick'
-    results = reconstruction.trace_refinement_of_surface(blurry_sphere, surf_points,
-                                                trace_length=20,
-                                                sampling_distance=1.0,
-                                                selected_fit_type=fit_type,
-                                                remove_outliers=False)
+    results = reconstruction.trace_refinement_of_surface(
+        blurry_sphere, surf_points,
+        trace_length=20,
+        sampling_distance=1.0,
+        selected_fit_type=fit_type,
+        interpolation_method='linear',
+        remove_outliers=False)
     traced_points = results[0][0]
 
     radial_vectors = np.array([50, 50, 50])[None, :] - traced_points
     mean_radii = np.linalg.norm(radial_vectors, axis=1).mean()
     assert np.allclose(true_radius, mean_radii, atol=1.5)
 
     fit_type = 'fancy'
-    results = reconstruction.trace_refinement_of_surface(blurry_sphere, surf_points,
-                                                trace_length=10,
-                                                selected_fit_type=fit_type,
-                                                remove_outliers=False)
+    results = reconstruction.trace_refinement_of_surface(
+        blurry_sphere, surf_points,
+        trace_length=10,
+        selected_fit_type=fit_type,
+        interpolation_method='linear',
+        remove_outliers=False)
     traced_points = results[0][0]
     radial_vectors = np.array([50, 50, 50])[None, :] - traced_points
     mean_radii = np.linalg.norm(radial_vectors, axis=1).mean()
 
     assert np.allclose(true_radius, mean_radii, atol=1)
 
     # Test outlier identification
     surf_points[0] += [0, 0, 10]
-    results= reconstruction.trace_refinement_of_surface(blurry_sphere, surf_points,
-                                                trace_length=10,
-                                                selected_fit_type=fit_type,
-                                                remove_outliers=True)
+    results = reconstruction.trace_refinement_of_surface(
+        blurry_sphere, surf_points,
+        trace_length=10,
+        selected_fit_type=fit_type,
+        interpolation_method='linear',
+        remove_outliers=True)
     traced_points = results[0][0]
     assert len(traced_points.squeeze()) < len(surf_points)
 
     # Now, let's test surface-labelled data
     blurry_ring = filters.sobel(image)
 
     surf_points = shapes.Sphere().points()
     surf_points += (surf_points * true_radius + 2) + 50
 
     fit_type = 'fancy'
-    results= reconstruction.trace_refinement_of_surface(blurry_ring, surf_points,
-                                                trace_length=10,
-                                                sampling_distance=1,
-                                                selected_fit_type=fit_type,
-                                                selected_edge='surface',
-                                                remove_outliers=False)
+    results = reconstruction.trace_refinement_of_surface(
+        blurry_ring, surf_points,
+        trace_length=10,
+        sampling_distance=1,
+        selected_fit_type=fit_type,
+        selected_edge='surface',
+        remove_outliers=False)
 
     fit_type = 'quick'
-    results = reconstruction.trace_refinement_of_surface(blurry_ring, surf_points,
-                                                trace_length=10,
-                                                sampling_distance=1,
-                                                selected_fit_type=fit_type,
-                                                selected_edge='surface',
-                                                remove_outliers=False)
+    results = reconstruction.trace_refinement_of_surface(
+        blurry_ring, surf_points,
+        trace_length=10,
+        sampling_distance=1,
+        selected_fit_type=fit_type,
+        selected_edge='surface',
+        interpolation_method='linear',
+        remove_outliers=False)
```

### Comparing `napari_stress-0.2.3/src/napari_stress/_tests/test_spherical_harmonic_fit.py` & `napari_stress-0.2.4/src/napari_stress/_tests/test_spherical_harmonic_fit.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_tests/test_surface.py` & `napari_stress-0.2.4/src/napari_stress/_tests/test_surface.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_tests/test_types.py` & `napari_stress-0.2.4/src/napari_stress/_tests/test_types.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_tests/test_utils.py` & `napari_stress-0.2.4/src/napari_stress/_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_utils/coordinate_conversion.py` & `napari_stress-0.2.4/src/napari_stress/_utils/coordinate_conversion.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_utils/fit_utils.py` & `napari_stress-0.2.4/src/napari_stress/_utils/fit_utils.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/_utils/frame_by_frame.py` & `napari_stress-0.2.4/src/napari_stress/_utils/frame_by_frame.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress/napari.yaml` & `napari_stress-0.2.4/src/napari_stress/napari.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -66,14 +66,28 @@
       python_name: napari_stress._surface:fit_ellipsoid_to_pointcloud_points
       title: Fit PCA ellipsoid to pointcloud and return points
 
     - id: napari-stress.fit_ellipsoid_vectors
       python_name: napari_stress._surface:fit_ellipsoid_to_pointcloud_vectors
       title: Fit PCA ellipsoid to pointcloud and return major axis
 
+    # Vectors
+    - id: napari-stress.normal_vectors_on_pointcloud
+      python_name: napari_stress._vectors:normal_vectors_on_pointcloud
+      title: Calculate normal vectors on pointcloud
+    - id: napari-stress.normal_vectors_on_surface
+      python_name: napari_stress._vectors:normal_vectors_on_surface
+      title: Calculate normal vectors on surface
+    - id: napari-stress.move_point_along_vector_relative
+      python_name: napari_stress._vectors:relative_move_points_along_vector
+      title: Move points along vector (relative)
+    - id: napari-stress.move_point_along_vector_absolute
+      python_name: napari_stress._vectors:absolute_move_points_along_vector
+      title: Move points along vector (absolute)
+
     # Plotting
     - id: napari-stress.features_histogram
       python_name: napari_stress:FeaturesHistogramWidget
       title: Visualize features (histogram)
 
     - id: napari-stress.fit_lsq_ellipsoid
       python_name: napari_stress.approximation:least_squares_ellipsoid
@@ -153,14 +167,28 @@
       autogenerate: true
       display_name: Pairwise point distance
 
     # Plotting
     - command: napari-stress.features_histogram
       display_name: Visualize features (histogram)
 
+    # Vectors
+    - command: napari-stress.normal_vectors_on_pointcloud
+      autogenerate: true
+      display_name: Calculate normal vectors on pointcloud
+    - command: napari-stress.normal_vectors_on_surface
+      autogenerate: true
+      display_name: Calculate normal vectors on surface
+    - command: napari-stress.move_point_along_vector_relative
+      autogenerate: true
+      display_name: Move points along vector (relative)
+    - command: napari-stress.move_point_along_vector_absolute
+      autogenerate: true
+      display_name: Move points along vector (absolute)
+
   sample_data:
     - command: napari-stress.get_pointcloud_sample_data
       display_name: Droplet pointcloud
       key: PC_1
     - command: napari-stress.get_pointcloud_sample_data_4d
       display_name: 4d Droplet pointcloud
       key: PC_2
```

### Comparing `napari_stress-0.2.3/src/napari_stress/types.py` & `napari_stress-0.2.4/src/napari_stress/types.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.2.3/src/napari_stress.egg-info/PKG-INFO` & `napari_stress-0.2.4/src/napari_stress.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-stress
-Version: 0.2.3
+Version: 0.2.4
 Summary: Interactive surface analysis in napari for measuring mechanical stresses in biological tissues
 Author: Johannes Soltwedel, Ben J. Gross, Elijah Shelton, Carlos Gomez, Otger Campas
 Author-email: johannes_richard.mueller@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/campaslab/napari-stress/issues
 Project-URL: Documentation, https://campaslab.github.io/napari-stress
 Project-URL: Source Code, https://github.com/campaslab/napari-stress
```

### Comparing `napari_stress-0.2.3/src/napari_stress.egg-info/SOURCES.txt` & `napari_stress-0.2.4/src/napari_stress.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -59,11 +59,12 @@
 src/napari_stress/_tests/test_processing.py
 src/napari_stress/_tests/test_reconstruction.py
 src/napari_stress/_tests/test_sample_data.py
 src/napari_stress/_tests/test_spherical_harmonic_fit.py
 src/napari_stress/_tests/test_surface.py
 src/napari_stress/_tests/test_types.py
 src/napari_stress/_tests/test_utils.py
+src/napari_stress/_tests/test_vectors.py
 src/napari_stress/_utils/__init__.py
 src/napari_stress/_utils/coordinate_conversion.py
 src/napari_stress/_utils/fit_utils.py
 src/napari_stress/_utils/frame_by_frame.py
```

