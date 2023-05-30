# Comparing `tmp/cad_to_dagmc-0.2.1.tar.gz` & `tmp/cad_to_dagmc-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cad_to_dagmc-0.2.1.tar", last modified: Wed Apr  5 19:54:02 2023, max compression
+gzip compressed data, was "cad_to_dagmc-0.3.1.tar", last modified: Tue May 30 21:42:46 2023, max compression
```

## Comparing `cad_to_dagmc-0.2.1.tar` & `cad_to_dagmc-0.3.1.tar`

### file list

```diff
@@ -1,51 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:54:02.275614 cad_to_dagmc-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:54:02.267614 cad_to_dagmc-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:54:02.271614 cad_to_dagmc-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/.github/workflows/anaconda-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/.github/workflows/ci_with_install.yml
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/.github/workflows/conda-build-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-04-05 19:54:02.275614 cad_to_dagmc-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:54:02.271614 cad_to_dagmc-0.2.1/conda/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/conda/conda_build_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:54:02.271614 cad_to_dagmc-0.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/examples/cadquery_assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/examples/cadquery_compound.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/examples/cadquery_object_and_stp_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/examples/cadquery_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/examples/create_stp_files_for_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/examples/curved_cadquery_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/examples/multiple_cadquery_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/examples/multiple_stp_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/examples/single_cadquery_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/examples/single_stp_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/examples/single_stp_file_multiple_volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 19:54:02.275614 cad_to_dagmc-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:54:02.271614 cad_to_dagmc-0.2.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-05 19:54:02.000000 cad_to_dagmc-0.2.1/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:54:02.271614 cad_to_dagmc-0.2.1/src/cad_to_dagmc/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/src/cad_to_dagmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/src/cad_to_dagmc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:54:02.271614 cad_to_dagmc-0.2.1/src/cad_to_dagmc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-04-05 19:54:02.000000 cad_to_dagmc-0.2.1/src/cad_to_dagmc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-05 19:54:02.000000 cad_to_dagmc-0.2.1/src/cad_to_dagmc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 19:54:02.000000 cad_to_dagmc-0.2.1/src/cad_to_dagmc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-05 19:54:02.000000 cad_to_dagmc-0.2.1/src/cad_to_dagmc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-05 19:54:02.000000 cad_to_dagmc-0.2.1/src/cad_to_dagmc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:54:02.275614 cad_to_dagmc-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    22142 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/tests/extrude_rectangle.stp
--rw-r--r--   0 runner    (1001) docker     (123)    87541 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/tests/multi_volume_cylinders.stp
--rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/tests/single_cube.stp
--rw-r--r--   0 runner    (1001) docker     (123)   212436 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/tests/single_volume_thin.stp
--rw-r--r--   0 runner    (1001) docker     (123)  2013134 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/tests/single_volume_thin.vtk
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/tests/test_h5m_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/tests/test_h5m_in_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    33452 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/tests/two_connected_cubes.stp
--rw-r--r--   0 runner    (1001) docker     (123)    33391 2023-04-05 19:53:44.000000 cad_to_dagmc-0.2.1/tests/two_disconnected_cubes.stp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.108199 cad_to_dagmc-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.096199 cad_to_dagmc-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.096199 cad_to_dagmc-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/.github/workflows/anaconda-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/.github/workflows/ci_with_install.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-30 21:42:46.108199 cad_to_dagmc-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.096199 cad_to_dagmc-0.3.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/cadquery_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/cadquery_compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/cadquery_object_and_stp_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/cadquery_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/create_stp_files_for_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/curved_cadquery_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/multiple_cadquery_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/multiple_stp_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/single_cadquery_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/single_stp_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/single_stp_file_multiple_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:42:46.108199 cad_to_dagmc-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.096199 cad_to_dagmc-0.3.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 21:42:45.000000 cad_to_dagmc-0.3.1/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.100199 cad_to_dagmc-0.3.1/src/cad_to_dagmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc/brep_part_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc/brep_to_h5m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc/vertices_to_h5m.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.100199 cad_to_dagmc-0.3.1/src/cad_to_dagmc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-30 21:42:46.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-30 21:42:46.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:42:46.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 21:42:46.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 21:42:46.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.104199 cad_to_dagmc-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    22142 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/extrude_rectangle.stp
+-rw-r--r--   0 runner    (1001) docker     (123)    87541 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/multi_volume_cylinders.stp
+-rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/single_cube.stp
+-rw-r--r--   0 runner    (1001) docker     (123)   212436 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/single_volume_thin.stp
+-rw-r--r--   0 runner    (1001) docker     (123)  2013134 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/single_volume_thin.vtk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.104199 cad_to_dagmc-0.3.1/tests/test_brep_part_finder/
+-rw-r--r--   0 runner    (1001) docker     (123)   267095 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_part_finder/ball_reactor.brep
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_part_finder/test_get_brep_part_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_part_finder/test_get_matching_part_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_part_finder/test_get_matching_part_id_with_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_part_finder/test_get_matching_part_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_part_finder/test_loading_from_file_vs_shape_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.104199 cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/create_brep_file_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/one_cube.brep
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/test_brep_file.brep
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/test_h5m_in_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/test_python_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/test_two_joined_cubes.brep
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/test_two_sep_cubes.brep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.108199 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/
+-rw-r--r--   0 runner    (1001) docker     (123)    22142 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/extrude_rectangle.stp
+-rw-r--r--   0 runner    (1001) docker     (123)    87541 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/multi_volume_cylinders.stp
+-rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/single_cube.stp
+-rw-r--r--   0 runner    (1001) docker     (123)   212436 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/single_volume_thin.stp
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/test_h5m_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/test_h5m_in_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33452 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/two_connected_cubes.stp
+-rw-r--r--   0 runner    (1001) docker     (123)    33391 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/two_disconnected_cubes.stp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.108199 cad_to_dagmc-0.3.1/tests/test_vertices_to_h5m/
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_vertices_to_h5m/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33452 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/two_connected_cubes.stp
+-rw-r--r--   0 runner    (1001) docker     (123)    33391 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/two_disconnected_cubes.stp
```

### Comparing `cad_to_dagmc-0.2.1/.github/workflows/anaconda-publish.yml` & `cad_to_dagmc-0.3.1/.github/workflows/anaconda-publish.yml`

 * *Files 20% similar despite different names*

```diff
@@ -4,27 +4,27 @@
   workflow_dispatch:
   release:
     types: [published]
 
 jobs:
   build:
     runs-on: ubuntu-latest
-    container: continuumio/miniconda3:4.10.3
+    container: continuumio/miniconda3:4.12.0
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       - name: Set up conda
         run: |
             apt-get --allow-releaseinfo-change update
             apt install -y libgl1-mesa-glx
             conda install -y anaconda-client conda-build
             conda config --set anaconda_upload no
       - name: Build and publish to conda
         env:
           ANACONDA_API_TOKEN: ${{ secrets.ANACONDA_TOKEN }}
         run: |
-            conda build conda -c fusion-energy -c cadquery -c conda-forge --config-file conda/conda_build_config.yaml
+            conda build conda -c conda-forge --config-file conda/conda_build_config.yaml
             conda convert /opt/conda/conda-bld/linux-64/*.tar.bz2 --platform osx-64
             anaconda upload -f /opt/conda/conda-bld/*/*.tar.bz2
 
 # Note conversion to windows is not supported as MOAB is a dependency
```

### Comparing `cad_to_dagmc-0.2.1/.github/workflows/black.yml` & `cad_to_dagmc-0.3.1/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.2.1/.github/workflows/python-publish.yml` & `cad_to_dagmc-0.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.2.1/.gitignore` & `cad_to_dagmc-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.2.1/LICENSE` & `cad_to_dagmc-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.2.1/PKG-INFO` & `cad_to_dagmc-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cad_to_dagmc
-Version: 0.2.1
+Version: 0.3.1
 Summary: Converts CAD files to a DAGMC h5m file
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 Project-URL: Homepage, https://github.com/fusion-energy/cad_to_dagmc
 Project-URL: Bug Tracker, https://github.com/fusion-energy/cad_to_dagmc/issues
 Keywords: dagmc,geometry,plot,slice
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cad_to_dagmc-0.2.1/README.md` & `cad_to_dagmc-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.2.1/examples/cadquery_compound.py` & `cad_to_dagmc-0.3.1/examples/cadquery_compound.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.2.1/examples/create_stp_files_for_examples.py` & `cad_to_dagmc-0.3.1/examples/create_stp_files_for_examples.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.2.1/examples/curved_cadquery_object.py` & `cad_to_dagmc-0.3.1/examples/curved_cadquery_object.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.2.1/pyproject.toml` & `cad_to_dagmc-0.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -15,28 +15,27 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "cadquery>=2.2.0",
-    "brep_to_h5m>=0.4.2",
-    "brep_part_finder>=0.5.2",
+    "trimesh",
+    "networkx",
 ]
 dynamic = ["version"]
 
 
 [tool.setuptools_scm]
 write_to = "src/_version.py"
 
 
 [project.optional-dependencies]
 tests = [
     "pytest",
-    "dagmc_h5m_file_inspector",
     "openmc_data_downloader"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/fusion-energy/cad_to_dagmc"
 "Bug Tracker" = "https://github.com/fusion-energy/cad_to_dagmc/issues"
```

### Comparing `cad_to_dagmc-0.2.1/src/cad_to_dagmc.egg-info/PKG-INFO` & `cad_to_dagmc-0.3.1/src/cad_to_dagmc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cad-to-dagmc
-Version: 0.2.1
+Version: 0.3.1
 Summary: Converts CAD files to a DAGMC h5m file
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 Project-URL: Homepage, https://github.com/fusion-energy/cad_to_dagmc
 Project-URL: Bug Tracker, https://github.com/fusion-energy/cad_to_dagmc/issues
 Keywords: dagmc,geometry,plot,slice
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cad_to_dagmc-0.2.1/tests/extrude_rectangle.stp` & `cad_to_dagmc-0.3.1/tests/extrude_rectangle.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.2.1/tests/multi_volume_cylinders.stp` & `cad_to_dagmc-0.3.1/tests/multi_volume_cylinders.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.2.1/tests/single_cube.stp` & `cad_to_dagmc-0.3.1/tests/single_cube.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.2.1/tests/single_volume_thin.stp` & `cad_to_dagmc-0.3.1/tests/single_volume_thin.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.2.1/tests/single_volume_thin.vtk` & `cad_to_dagmc-0.3.1/tests/single_volume_thin.vtk`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.2.1/tests/test_h5m_in_simulation.py` & `cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/test_h5m_in_simulation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# import dagmc_h5m_file_inspector as di
 import openmc
 import openmc_data_downloader
 
 
 """
     - h5m files can be used a transport geometry in DAGMC with OpenMC
 """
@@ -93,45 +92,45 @@
     my_model.run()
 
 
 def test_h5m_with_single_volume_list():
     """The simplest geometry, a single 4 sided shape with lists instead of np arrays"""
 
     h5m_files = [
-        "tests/extrude_rectangle.h5m",
-        "tests/single_cube.h5m",
-        # "tests/single_volume_thin.h5m",
+        "tests/test_cad_to_dagmc/extrude_rectangle.h5m",
+        "tests/test_cad_to_dagmc/single_cube.h5m",
+        # "tests/test_cad_to_dagmc/single_volume_thin.h5m",
     ]
 
     for h5m_file in h5m_files:
         transport_particles_on_h5m_geometry(
             h5m_filename=h5m_file,
             material_tags=["mat1"],
         )
 
 
 def test_h5m_with_multi_volume_not_touching():
     material_tags = [
         ["mat1", "mat2"],
     ]
     h5m_files = [
-        "tests/two_disconnected_cubes.h5m",
+        "tests/test_cad_to_dagmc/two_disconnected_cubes.h5m",
     ]
     for mat_tags, h5m_file in zip(material_tags, h5m_files):
         transport_particles_on_h5m_geometry(
             h5m_filename=h5m_file, material_tags=mat_tags
         )
 
 
 def test_h5m_with_multi_volume_touching():
     material_tags = [
         ["mat1", "mat2", "mat3", "mat4", "mat5", "mat6"],
         ["mat1", "mat2"],
     ]
     h5m_files = [
-        "tests/multi_volume_cylinders.h5m",
-        "tests/two_connected_cubes.h5m",
+        "tests/test_cad_to_dagmc/multi_volume_cylinders.h5m",
+        "tests/test_cad_to_dagmc/two_connected_cubes.h5m",
     ]
     for mat_tags, h5m_file in zip(material_tags, h5m_files):
         transport_particles_on_h5m_geometry(
             h5m_filename=h5m_file, material_tags=mat_tags
         )
```

### Comparing `cad_to_dagmc-0.2.1/tests/test_version.py` & `cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/test_version.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.2.1/tests/two_connected_cubes.stp` & `cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/two_connected_cubes.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.2.1/tests/two_disconnected_cubes.stp` & `cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/two_disconnected_cubes.stp`

 * *Files identical despite different names*

