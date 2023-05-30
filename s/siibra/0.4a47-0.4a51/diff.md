# Comparing `tmp/siibra-0.4a47.tar.gz` & `tmp/siibra-0.4a51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siibra-0.4a47.tar", last modified: Wed Apr 26 11:04:32 2023, max compression
+gzip compressed data, was "siibra-0.4a51.tar", last modified: Tue May 30 15:17:41 2023, max compression
```

## Comparing `siibra-0.4a47.tar` & `siibra-0.4a51.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.645815 siibra-0.4a47/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 11:03:14.000000 siibra-0.4a47/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-26 11:03:14.000000 siibra-0.4a47/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-04-26 11:04:32.645815 siibra-0.4a47/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-04-26 11:03:14.000000 siibra-0.4a47/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 11:04:32.645815 siibra-0.4a47/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-26 11:03:14.000000 siibra-0.4a47/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.633814 siibra-0.4a47/siibra/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24325 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.633814 siibra-0.4a47/siibra/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/configuration/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.633814 siibra-0.4a47/siibra/core/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/core/atlas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/core/concept.py
--rw-r--r--   0 runner    (1001) docker     (123)    13405 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/core/parcellation.py
--rw-r--r--   0 runner    (1001) docker     (123)    24613 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/core/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/core/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.633814 siibra-0.4a47/siibra/features/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/anchor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.637815 siibra-0.4a47/siibra/features/connectivity/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/connectivity/functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/connectivity/regional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/connectivity/streamline_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/connectivity/streamline_lengths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.637815 siibra-0.4a47/siibra/features/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/dataset/ebrains.py
--rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.637815 siibra-0.4a47/siibra/features/image/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/image/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/image/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/image/volume_of_interest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.637815 siibra-0.4a47/siibra/features/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/bigbrain_intensity_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/cell_density_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/cortical_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/gene_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/layerwise_bigbrain_intensities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/layerwise_cell_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/receptor_density_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/receptor_density_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/regional_timeseries_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.637815 siibra-0.4a47/siibra/livequeries/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/livequeries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/livequeries/allen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/livequeries/bigbrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/livequeries/ebrains.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/livequeries/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.637815 siibra-0.4a47/siibra/locations/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/locations/boundingbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/locations/location.py
--rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/locations/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/locations/pointset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.641815 siibra-0.4a47/siibra/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/retrieval/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/retrieval/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.641815 siibra-0.4a47/siibra/retrieval/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/retrieval/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26309 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/retrieval/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    20940 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/retrieval/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.641815 siibra-0.4a47/siibra/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/vocabularies/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)  1647972 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/vocabularies/gene_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/vocabularies/receptor_symbols.json
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/vocabularies/region_aliases.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.641815 siibra-0.4a47/siibra/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/volumes/gifti.py
--rw-r--r--   0 runner    (1001) docker     (123)    24056 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/volumes/neuroglancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/volumes/nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)    42172 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/volumes/parcellationmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    18071 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/volumes/sparsemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/volumes/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.633814 siibra-0.4a47/siibra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-04-26 11:04:32.000000 siibra-0.4a47/siibra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-26 11:04:32.000000 siibra-0.4a47/siibra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:04:32.000000 siibra-0.4a47/siibra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-26 11:04:32.000000 siibra-0.4a47/siibra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 11:04:32.000000 siibra-0.4a47/siibra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.641815 siibra-0.4a47/test/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-26 11:03:14.000000 siibra-0.4a47/test/test_siibra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.917296 siibra-0.4a51/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 15:16:11.000000 siibra-0.4a51/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-30 15:16:11.000000 siibra-0.4a51/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-05-30 15:17:41.913296 siibra-0.4a51/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-05-30 15:16:11.000000 siibra-0.4a51/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 15:17:41.917296 siibra-0.4a51/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-30 15:16:11.000000 siibra-0.4a51/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.901295 siibra-0.4a51/siibra/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.905295 siibra-0.4a51/siibra/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/configuration/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.905295 siibra-0.4a51/siibra/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/core/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/core/concept.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13405 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/core/parcellation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24613 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/core/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/core/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.905295 siibra-0.4a51/siibra/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/anchor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.905295 siibra-0.4a51/siibra/features/connectivity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/connectivity/functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/connectivity/regional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/connectivity/streamline_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/connectivity/streamline_lengths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/connectivity/tracer_connectivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.905295 siibra-0.4a51/siibra/features/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/dataset/ebrains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16021 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.905295 siibra-0.4a51/siibra/features/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/image/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/image/volume_of_interest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.909296 siibra-0.4a51/siibra/features/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/bigbrain_intensity_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/cell_density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/cortical_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/gene_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/layerwise_bigbrain_intensities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/layerwise_cell_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/receptor_density_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/receptor_density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/regional_timeseries_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.909296 siibra-0.4a51/siibra/livequeries/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/livequeries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/livequeries/allen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/livequeries/bigbrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/livequeries/ebrains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/livequeries/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.909296 siibra-0.4a51/siibra/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/locations/boundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/locations/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/locations/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/locations/pointset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.909296 siibra-0.4a51/siibra/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/retrieval/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/retrieval/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.913296 siibra-0.4a51/siibra/retrieval/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/retrieval/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26563 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/retrieval/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21031 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/retrieval/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.913296 siibra-0.4a51/siibra/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/vocabularies/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1647972 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/vocabularies/gene_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/vocabularies/receptor_symbols.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/vocabularies/region_aliases.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.913296 siibra-0.4a51/siibra/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/volumes/gifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24056 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/volumes/neuroglancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/volumes/nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42179 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/volumes/parcellationmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21984 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/volumes/sparsemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/volumes/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.905295 siibra-0.4a51/siibra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-05-30 15:17:41.000000 siibra-0.4a51/siibra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-30 15:17:41.000000 siibra-0.4a51/siibra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:17:41.000000 siibra-0.4a51/siibra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-30 15:17:41.000000 siibra-0.4a51/siibra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 15:17:41.000000 siibra-0.4a51/siibra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.913296 siibra-0.4a51/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-30 15:16:11.000000 siibra-0.4a51/test/test_siibra.py
```

### Comparing `siibra-0.4a47/LICENSE` & `siibra-0.4a51/LICENSE`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/PKG-INFO` & `siibra-0.4a51/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siibra
-Version: 0.4a47
+Version: 0.4a51
 Summary: siibra - Software interfaces for interacting with brain atlases
 Home-page: https://github.com/FZJ-INM1-BDA/siibra-python
 Author: Big Data Analytics Group, Forschungszentrum Juelich, Institute of Neuroscience and Medicine (INM-1)
 Author-email: inm1-bda@fz-juelich.de
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-|License| |PyPI version| |Python versions| |Documentation Status|
+|License| |PyPI version| |doi| |Python versions| |Documentation Status|
 
 siibra - Software interface for interacting with brain atlases
 ==============================================================
 
 Copyright 2020-2023, Forschungszentrum Jülich GmbH
 
 *Authors: Big Data Analytics Group, Institute of Neuroscience and
@@ -131,7 +131,9 @@
    :target: https://opensource.org/licenses/Apache-2.0
 .. |PyPI version| image:: https://badge.fury.io/py/siibra.svg
    :target: https://pypi.org/project/siibra/
 .. |Python versions| image:: https://img.shields.io/pypi/pyversions/siibra.svg
    :target: https://pypi.python.org/pypi/siibra
 .. |Documentation Status| image:: https://readthedocs.org/projects/siibra-python/badge/?version=latest
    :target: https://siibra-python.readthedocs.io/en/latest/?badge=latest
+.. |doi| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7885729.svg
+   :target: https://doi.org/10.5281/zenodo.7885729
```

### Comparing `siibra-0.4a47/README.rst` & `siibra-0.4a51/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-|License| |PyPI version| |Python versions| |Documentation Status|
+|License| |PyPI version| |doi| |Python versions| |Documentation Status|
 
 siibra - Software interface for interacting with brain atlases
 ==============================================================
 
 Copyright 2020-2023, Forschungszentrum Jülich GmbH
 
 *Authors: Big Data Analytics Group, Institute of Neuroscience and
@@ -113,7 +113,9 @@
    :target: https://opensource.org/licenses/Apache-2.0
 .. |PyPI version| image:: https://badge.fury.io/py/siibra.svg
    :target: https://pypi.org/project/siibra/
 .. |Python versions| image:: https://img.shields.io/pypi/pyversions/siibra.svg
    :target: https://pypi.python.org/pypi/siibra
 .. |Documentation Status| image:: https://readthedocs.org/projects/siibra-python/badge/?version=latest
    :target: https://siibra-python.readthedocs.io/en/latest/?badge=latest
+.. |doi| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7885729.svg
+   :target: https://doi.org/10.5281/zenodo.7885729
```

### Comparing `siibra-0.4a47/setup.py` & `siibra-0.4a51/setup.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/__init__.py` & `siibra-0.4a51/siibra/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 )
 
 from .core import (
     atlas as _atlas,
     parcellation as _parcellation,
     space as _space
 )
+from .volumes import parcellationmap as _parcellationmap
 from .retrieval.requests import (
     EbrainsRequest as _EbrainsRequest,
     CACHE as cache
 )
 from . import configuration
 from .configuration import factory
 from . import features, livequeries
@@ -55,14 +56,16 @@
     # lazy loading of some classes for package-level functions.
     if attr == 'atlases':
         return _atlas.Atlas.registry()
     elif attr == 'spaces':
         return _space.Space.registry()
     elif attr == 'parcellations':
         return _parcellation.Parcellation.registry()
+    elif attr == 'maps':
+        return _parcellationmap.Map.registry()
     elif attr == 'use_configuration':
         return configuration.Configuration.use_configuration
     elif attr == 'extend_configuration':
         return configuration.Configuration.extend_configuration
     else:
         raise AttributeError(f"No such attribute: {__name__}.{attr}")
```

### Comparing `siibra-0.4a47/siibra/commons.py` & `siibra-0.4a51/siibra/commons.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import os
 import re
 from enum import Enum
 from nibabel import Nifti1Image
 import logging
 from tqdm import tqdm
 import numpy as np
+import pandas as pd
 from typing import Generic, Iterable, Iterator, List, TypeVar, Union, Dict
 from skimage.filters import gaussian
 from dataclasses import dataclass
 
 logger = logging.getLogger(__name__.split(os.path.extsep)[0])
 ch = logging.StreamHandler()
 formatter = logging.Formatter("[{name}:{levelname}] {message}", style="{")
@@ -77,14 +78,15 @@
         if elements is None:
             self._elements: Dict[str, T] = {}
         else:
             assert isinstance(elements, dict)
             assert all(isinstance(k, str) for k in elements.keys())
             self._elements: Dict[str, T] = elements
         self._matchfunc = matchfunc
+        self._dataframe_cached = None
 
     def add(self, key: str, value: T) -> None:
         """Add a key/value pair to the registry.
 
         Args:
             key (string): Unique name or key of the object
             value (object): The registered object
@@ -93,15 +95,15 @@
             logger.error(
                 f"Key {key} already in {__class__.__name__}, existing value will be replaced."
             )
         self._elements[key] = value
 
     def __dir__(self) -> Iterable[str]:
         """List of all object keys in the registry"""
-        return self._elements.keys()
+        return ["dataframe"] + list(self._elements.keys())
 
     def __str__(self) -> str:
         if len(self) > 0:
             return f"{self.__class__.__name__}:\n - " + "\n - ".join(self._elements.keys())
         else:
             return f"Empty {self.__class__.__name__}"
 
@@ -220,14 +222,30 @@
                 closest = difflib.get_close_matches(
                     index, list(self._elements.keys()), n=3
                 )
                 if len(closest) > 0:
                     hint = f"Did you mean {' or '.join(closest)}?"
             raise AttributeError(f"Term '{index}' not in {__class__.__name__}. " + hint)
 
+    @property
+    def dataframe(self):
+        if self._dataframe_cached is None:
+            values = self._elements.values()
+            attrs = []
+            for i, val in enumerate(values):
+                attrs.append({'name': val.name, 'species': str(val.species)})
+                if hasattr(val, 'maptype'):
+                    attrs[i].update(
+                        {
+                            attribute: val.__getattribute__(attribute).name
+                            for attribute in ['parcellation', 'space', 'maptype']
+                        }
+                    )
+            self._dataframe_cached = pd.DataFrame(index=list(self._elements.keys()), data=attrs)
+        return self._dataframe_cached
 
 class LoggingContext:
     def __init__(self, level):
         self.level = level
 
     def __enter__(self):
         self.old_level = logger.level
```

### Comparing `siibra-0.4a47/siibra/configuration/__init__.py` & `siibra-0.4a51/siibra/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/configuration/configuration.py` & `siibra-0.4a51/siibra/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/configuration/factory.py` & `siibra-0.4a51/siibra/configuration/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from os import path
 import json
 import numpy as np
 from typing import List, Type
 import pandas as pd
 from io import BytesIO
 
-MIN_VOLUMES_FOR_SPARSE_MAP = 100
+MIN_VOLUMES_FOR_SPARSE_MAP = 125
 
 BUILDFUNCS = {
     "juelich/iav/atlas/v1.0.0": "build_atlas",
     "siibra/space/v0.0.1": "build_space",
     "siibra/parcellation/v0.0.1": "build_parcellation",
     "siibra/volume/v0.0.1": "build_volume",
     "siibra/map/v0.0.1": "build_map",
@@ -265,29 +265,49 @@
         # maps have no configured identifier - we require the spec filename to build one
         assert "filename" in spec
         basename = path.splitext(path.basename(spec['filename']))[0]
         name = basename.replace('-', ' ').replace('_', ' ')
         identifier = f"{spec['@type'].replace('/','-')}_{basename}"
         volumes = cls.extract_volumes(spec)
 
+        if ("sparsemap" in spec) and spec.get("sparsemap").get("is_sparsemap"):
+            Maptype = sparsemap.SparseMap
+            return Maptype(
+                identifier=spec.get("@id", identifier),
+                name=spec.get("name", name),
+                space_spec=spec.get("space", {}),
+                parcellation_spec=spec.get("parcellation", {}),
+                indices=spec.get("indices", {}),
+                volumes=volumes,
+                shortname=spec.get("shortName", ""),
+                description=spec.get("description"),
+                modality=spec.get("modality"),
+                publications=spec.get("publications", []),
+                datasets=cls.extract_datasets(spec),
+                is_cached=spec.get("sparsemap").get("cached", False),
+                cache_url=spec.get("sparsemap").get("url", "")
+            )
+
         Maptype = parcellationmap.Map
         if len(volumes) > MIN_VOLUMES_FOR_SPARSE_MAP:
             logger.debug(
-                f"Using sparse map for {spec['filename']} to code its {len(volumes)} volumes efficiently."
+                f"Using sparse map for {spec.get('filename')} to code its "
+                f"{len(volumes)} volumes efficiently."
             )
             Maptype = sparsemap.SparseMap
         else:
             max_z = max(
                 d.get('z', 0)
                 for l in spec.get("indices", {}).values()
                 for d in l
             ) + 1
             if max_z > MIN_VOLUMES_FOR_SPARSE_MAP:
                 logger.debug(
-                    f"Using sparse map for {spec['filename']} to code its {max_z} z levels efficiently."
+                    f"Using sparse map for {spec.get('filename')} to code its "
+                    f"{max_z} z levels efficiently."
                 )
                 Maptype = sparsemap.SparseMap
 
         return Maptype(
             identifier=spec.get("@id", identifier),
             name=spec.get("name", name),
             space_spec=spec.get("space", {}),
@@ -431,15 +451,15 @@
         else:
             raise ValueError(f"No method for building image section feature type {modality}.")
 
     @classmethod
     def build_connectivity_matrix(cls, spec):
         modality = spec["modality"]
         kwargs = {
-            "cohort": spec["cohort"],
+            "cohort": spec.get("cohort", ""),
             "modality": modality,
             "regions": spec["regions"],
             "connector": cls.extract_connector(spec),
             "decode_func": cls.extract_decoder(spec),
             "files": spec.get("files", {}),
             "anchor": cls.extract_anchor(spec),
             "description": spec.get("description", ""),
@@ -451,14 +471,16 @@
             return connectivity.StreamlineLengths(**kwargs)
         elif modality == "Functional":
             kwargs["paradigm"] = spec.get("paradigm")
             return connectivity.FunctionalConnectivity(**kwargs)
         elif modality == "RestingState":
             kwargs["paradigm"] = spec.get("paradigm", "RestingState")
             return connectivity.FunctionalConnectivity(**kwargs)
+        elif modality == "Tracer":
+            return connectivity.TracerConnectivity(**kwargs)
         else:
             raise ValueError(f"No method for building connectivity matrix of type {modality}.")
 
     @classmethod
     def build_activity_timeseries(cls, spec):
         modality = spec["modality"]
         kwargs = {
```

### Comparing `siibra-0.4a47/siibra/core/__init__.py` & `siibra-0.4a51/siibra/core/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/core/atlas.py` & `siibra-0.4a51/siibra/core/atlas.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/core/concept.py` & `siibra-0.4a51/siibra/core/concept.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/core/parcellation.py` & `siibra-0.4a51/siibra/core/parcellation.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/core/region.py` & `siibra-0.4a51/siibra/core/region.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/core/space.py` & `siibra-0.4a51/siibra/core/space.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,29 +77,26 @@
             publications=publications,
             datasets=datasets,
         )
         self.volumes = volumes
         for v in self.volumes:
             v.space_info = {"@id": self.id}
 
-    def get_template(self, variant: str = None, format: str = None):
+    def get_template(self, variant: str = None):
         """
         Get the volumetric reference template for this space.
 
         Parameters
         ----------
             variant: str, optional
                 Some templates are provided in different variants, e.g.
                 freesurfer is available as either white matter, pial or
                 inflated surface for left and right hemispheres (6 variants).
                 This field could be used to request a specific variant.
                 Per default, the first found variant is returned.
-            format: str, optional
-                Volumes are typically available in multiple formats.
-                Use this to select a specific one, if needed.
 
         Returns
         -------
             Volume
                 representing the reference template, or None if not available.
         """
         tests = []
```

### Comparing `siibra-0.4a47/siibra/features/__init__.py` & `siibra-0.4a51/siibra/features/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/anchor.py` & `siibra-0.4a51/siibra/features/anchor.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/connectivity/__init__.py` & `siibra-0.4a51/siibra/features/connectivity/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,7 +12,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .functional_connectivity import FunctionalConnectivity
 from .streamline_counts import StreamlineCounts
 from .streamline_lengths import StreamlineLengths
+from .tracer_connectivity import TracerConnectivity
+
+def __dir__():
+    return [
+        "FunctionalConnectivity",
+        "StreamlineCounts",
+        "StreamlineLengths",
+        "TracerConnectivity"
+    ]
```

### Comparing `siibra-0.4a47/siibra/features/connectivity/functional_connectivity.py` & `siibra-0.4a51/siibra/features/connectivity/functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/connectivity/regional_connectivity.py` & `siibra-0.4a51/siibra/features/connectivity/regional_connectivity.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from ...locations import pointset
 from ...retrieval.repositories import RepositoryConnector
 
 from typing import Callable, Dict, Union, List
 import pandas as pd
 import numpy as np
 
-
 class RegionalConnectivity(Feature):
     """
     Parcellation-averaged connectivity, providing one or more matrices of a
     given modality for a given parcellation.
     """
 
     def __init__(
@@ -153,30 +152,36 @@
             It can only be a subset of regions of the feature.
         logscale: bool
             Display the data in log10 scale
         **kwargs:
             Can take all the arguments `nilearn.plotting.plot_matrix` can take. See the doc at
             https://nilearn.github.io/stable/modules/generated/nilearn.plotting.plot_matrix.html
         """
-        matrix = self.get_matrix(subject=subject)
+        if regions is None:
+            regions = self.regions
+        indices = [self.regions.index(r) for r in regions]
+        matrix = self.get_matrix(subject=subject).iloc[indices, indices].to_numpy()  # nilearn.plotting.plot_matrix works better with a numpy array
+        
         if logscale:
             matrix = np.log10(matrix)
-        if regions is None:
-            regions = matrix.columns.to_list()
 
         # default kwargs
         subject_title = subject or ""
         kwargs["title"] = kwargs.get(
             "title",
             f"{subject_title} - {self.modality} in {', '.join({_.name for _ in self.anchor.regions})}"
         )
         kwargs["figure"] = kwargs.get("figure", (15, 15))
 
         from nilearn import plotting
-        plotting.plot_matrix(matrix.loc[regions, regions], labels=regions, **kwargs)
+        plotting.plot_matrix(
+            matrix,
+            labels=regions,
+            **kwargs
+        )
 
     def __iter__(self):
         return ((sid, self.get_matrix(sid)) for sid in self._files)
 
     def get_profile(
         self,
         region: Union[str, _region.Region],
```

### Comparing `siibra-0.4a47/siibra/features/connectivity/streamline_counts.py` & `siibra-0.4a51/siibra/features/connectivity/streamline_counts.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/connectivity/streamline_lengths.py` & `siibra-0.4a51/siibra/features/connectivity/streamline_lengths.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/dataset/__init__.py` & `siibra-0.4a51/siibra/features/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/dataset/ebrains.py` & `siibra-0.4a51/siibra/features/dataset/ebrains.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/feature.py` & `siibra-0.4a51/siibra/features/feature.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,23 +80,31 @@
         return self._modality_cached
 
     @property
     def anchor(self):
         # allows subclasses to implement lazy loading of an anchor
         return self._anchor_cached
 
-    def __init_subclass__(cls, configuration_folder=None, category=None):
-        # extend the subclass lists
+    def __init_subclass__(cls, configuration_folder=None, category=None, do_not_index=False):
 
-        # Iterate over all mro, not just immediate base classes
-        for BaseCls in cls.__mro__:
-            # some base classes may not be sub class of feature, ignore these
-            if not issubclass(BaseCls, Feature):
-                continue
-            cls.SUBCLASSES[BaseCls].append(cls)
+        # Feature.SUBCLASSES serves as an index where feature class inheritance is cached. When users
+        # queries a branch on the hierarchy, all children will also be queried. There are usecases where
+        # such behavior is not desired (e.g. ProxyFeature, which wraps livequery features id to capture the
+        # query context).
+        # do_not_index flag allow the default index behavior to be toggled off.
+
+        if do_not_index == False:
+
+            # extend the subclass lists
+            # Iterate over all mro, not just immediate base classes
+            for BaseCls in cls.__mro__:
+                # some base classes may not be sub class of feature, ignore these
+                if not issubclass(BaseCls, Feature):
+                    continue
+                cls.SUBCLASSES[BaseCls].append(cls)
 
         cls._live_queries = []
         cls._preconfigured_instances = None
         cls._configuration_folder = configuration_folder
         cls.category = category
         if category is not None:
             cls.CATEGORIZED[category].add(cls.__name__, cls)
@@ -388,15 +396,15 @@
         Wrap live query features, override only the id attribute.
 
         Some features do not have setters for the id property. The ProxyFeature class
         allow the id property to be overridden without touching the underlying class.
 
         See docstring of serialize_query_context for further context.
         """
-        class ProxyFeature(feature.__class__):
+        class ProxyFeature(feature.__class__, do_not_index=True):
 
             # override __class__ property
             # some instances of features accesses inst.__class__
             @property
             def __class__(self):
                 return self.inst.__class__
```

### Comparing `siibra-0.4a47/siibra/features/image/__init__.py` & `siibra-0.4a51/siibra/features/image/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/image/image.py` & `siibra-0.4a51/siibra/features/image/image.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/image/sections.py` & `siibra-0.4a51/siibra/features/image/sections.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/image/volume_of_interest.py` & `siibra-0.4a51/siibra/features/image/volume_of_interest.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/tabular/__init__.py` & `siibra-0.4a51/siibra/features/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/tabular/bigbrain_intensity_profile.py` & `siibra-0.4a51/siibra/features/tabular/bigbrain_intensity_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/tabular/cell_density_profile.py` & `siibra-0.4a51/siibra/features/tabular/cell_density_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/tabular/cortical_profile.py` & `siibra-0.4a51/siibra/features/tabular/cortical_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/tabular/gene_expression.py` & `siibra-0.4a51/siibra/features/tabular/gene_expression.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/tabular/layerwise_bigbrain_intensities.py` & `siibra-0.4a51/siibra/features/tabular/layerwise_bigbrain_intensities.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/tabular/layerwise_cell_density.py` & `siibra-0.4a51/siibra/features/tabular/layerwise_cell_density.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/tabular/receptor_density_fingerprint.py` & `siibra-0.4a51/siibra/features/tabular/receptor_density_fingerprint.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/tabular/receptor_density_profile.py` & `siibra-0.4a51/siibra/features/tabular/receptor_density_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/features/tabular/regional_timeseries_activity.py` & `siibra-0.4a51/siibra/features/tabular/regional_timeseries_activity.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,14 +194,15 @@
                 for label, region in indexmap.items()
             }
             df = df.rename(columns=remapper)
         return df
 
     def plot(self, subject: str = None, **kwargs):
         table = self.get_table(subject)
+        table.columns = [str(r) for r in table.columns]
         return table.mean().plot(kind="bar", **kwargs)
 
 
 class RegionalBOLD(
     RegionalTimeseriesActivity,
     configuration_folder="features/tabular/activity_timeseries/bold",
     category="functional"
```

### Comparing `siibra-0.4a47/siibra/features/tabular/tabular.py` & `siibra-0.4a51/siibra/features/tabular/tabular.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/livequeries/__init__.py` & `siibra-0.4a51/siibra/livequeries/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/livequeries/allen.py` & `siibra-0.4a51/siibra/livequeries/allen.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/livequeries/bigbrain.py` & `siibra-0.4a51/siibra/livequeries/bigbrain.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/livequeries/ebrains.py` & `siibra-0.4a51/siibra/livequeries/ebrains.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/livequeries/query.py` & `siibra-0.4a51/siibra/livequeries/query.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/locations/__init__.py` & `siibra-0.4a51/siibra/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/locations/boundingbox.py` & `siibra-0.4a51/siibra/locations/boundingbox.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/locations/location.py` & `siibra-0.4a51/siibra/locations/location.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/locations/point.py` & `siibra-0.4a51/siibra/locations/point.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/locations/pointset.py` & `siibra-0.4a51/siibra/locations/pointset.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/retrieval/__init__.py` & `siibra-0.4a51/siibra/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/retrieval/cache.py` & `siibra-0.4a51/siibra/retrieval/cache.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/retrieval/datasets.py` & `siibra-0.4a51/siibra/retrieval/datasets.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/retrieval/repositories.py` & `siibra-0.4a51/siibra/retrieval/repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,15 +201,15 @@
                         f"{self.reftag} is a branch of {self.base_url}! Want last commit "
                         f"{self._want_commit_cached['short_id']} from "
                         f"{self._want_commit_cached['created_at']}"
                     )
                 self._tag_checked = True
             except Exception as e:
                 print(str(e))
-                print("Could not connect to gitlab server!")
+                logger.warning("Could not connect to gitlab server!")
         return self._want_commit_cached
 
     @property
     def branches(self):
         return self._branchloader.data
 
     def _build_url(self, folder="", filename=None, recursive=False, page=1):
@@ -315,37 +315,45 @@
             if fname.startswith(folder) and fname.endswith(suffix):
                 result.append(fname)
         return result
 
     def __eq__(self, other):
         return self.url == other.url
 
-    class FileLoader:
+    def clear_cache(self):
+        os.remove(self.zipfile)
+        self._zipfile_cached = None
+
+    class ZipFileLoader:
         """
         Loads a file from the zip archive, but mimics the behaviour
         of cached http requests used in other connectors.
         """
         def __init__(self, zipfile, filename, decode_func):
             self.zipfile = zipfile
             self.filename = filename
             self.func = decode_func
-            self.cached = True
+            self.cachefile = CACHE.build_filename(zipfile+filename)
 
         @property
+        def cached(self):
+            return os.path.isfile(self.cachefile)
+        
+        @property
         def data(self):
             container = ZipFile(self.zipfile)
             return self.func(container.open(self.filename).read())
 
     def get_loader(self, filename, folder="", decode_func=None):
         """Get a lazy loader for a file, for loading data
         only once loader.data is accessed."""
         if decode_func is None:
-            return self.FileLoader(self.zipfile, filename, lambda b: self._decode_response(b, filename))
+            return self.ZipFileLoader(self.zipfile, filename, lambda b: self._decode_response(b, filename))
         else:
-            return self.FileLoader(self.zipfile, filename, decode_func)
+            return self.ZipFileLoader(self.zipfile, filename, decode_func)
 
     def __str__(self):
         return f"{self.__class__.__name__}: {self.zipfile}"
 
 
 class OwncloudConnector(RepositoryConnector):
     def __init__(self, server: str, share: int):
```

### Comparing `siibra-0.4a47/siibra/retrieval/requests.py` & `siibra-0.4a51/siibra/retrieval/requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 DECODERS = {
     ".nii.gz": lambda b: Nifti1Image.from_bytes(gzip.decompress(b)),
     ".nii": lambda b: Nifti1Image.from_bytes(b),
     ".gii": lambda b: GiftiImage.from_bytes(b),
     ".json": lambda b: json.loads(b.decode()),
     ".tck": lambda b: streamlines.load(BytesIO(b)),
-    ".csv": lambda b: pd.read_csv(BytesIO(b), delimiter=";"),
+    ".csv": lambda b: pd.read_csv(BytesIO(b)),
     ".tsv": lambda b: pd.read_csv(BytesIO(b), delimiter="\t").dropna(axis=0, how="all"),
     ".txt": lambda b: pd.read_csv(BytesIO(b), delimiter=" ", header=None),
     ".zip": lambda b: ZipFile(BytesIO(b)),
     ".png": lambda b: io.imread(BytesIO(b)),
     ".npy": lambda b: np.load(BytesIO(b))
 }
 
@@ -175,14 +175,16 @@
             with open(temp_cachefile, "wb") as f:
                 for data in r.iter_content(block_size):
                     if size_bytes > min_bytesize_with_no_progress_info:
                         progress_bar.update(len(data))
                     f.write(data)
             if size_bytes > min_bytesize_with_no_progress_info:
                 progress_bar.close()
+            if self.refresh and os.path.isfile(self.cachefile):
+                os.remove(self.cachefile)
             self.refresh = False
             os.rename(temp_cachefile, self.cachefile)
             
 
     def get(self):
         self._retrieve()
         with open(self.cachefile, "rb") as f:
```

### Comparing `siibra-0.4a47/siibra/vocabularies/__init__.py` & `siibra-0.4a51/siibra/vocabularies/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/vocabularies/gene_names.json` & `siibra-0.4a51/siibra/vocabularies/gene_names.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/vocabularies/receptor_symbols.json` & `siibra-0.4a51/siibra/vocabularies/receptor_symbols.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/vocabularies/region_aliases.json` & `siibra-0.4a51/siibra/vocabularies/region_aliases.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'Macaca fascicularis'": "OrderedDict([('pallidum', OrderedDict([('Macaca fascicularis', "*

 * *                          "OrderedDict([('globus pallidus', 'exact')]))]))])"}*

```diff
@@ -445,9 +445,16 @@
             }
         },
         "uncinate fasciculus": {
             "Homo sapiens": {
                 "None": "exact"
             }
         }
+    },
+    "Macaca fascicularis": {
+        "pallidum": {
+            "Macaca fascicularis": {
+                "globus pallidus": "exact"
+            }
+        }
     }
 }
```

### Comparing `siibra-0.4a47/siibra/volumes/__init__.py` & `siibra-0.4a51/siibra/volumes/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/volumes/gifti.py` & `siibra-0.4a51/siibra/volumes/gifti.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/volumes/neuroglancer.py` & `siibra-0.4a51/siibra/volumes/neuroglancer.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/volumes/nifti.py` & `siibra-0.4a51/siibra/volumes/nifti.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a47/siibra/volumes/parcellationmap.py` & `siibra-0.4a51/siibra/volumes/parcellationmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -906,15 +906,15 @@
                 }
             elif isinstance(a, Assignment):
                 item_to_append = {
                     **item_to_append,
                     **{
                         "correlation": None,
                         "intersection over union": None,
-                        "map value": None,
+                        "map value": a.map_value,
                         "map weighted mean": None,
                         "map containedness": None,
                         "input weighted mean": None,
                         "input containedness": None,
                     }
                 }
             else:
```

### Comparing `siibra-0.4a47/siibra/volumes/sparsemap.py` & `siibra-0.4a51/siibra/volumes/sparsemap.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 # limitations under the License.
 """Represents lists of probabilistic brain region maps."""
 from . import parcellationmap, volume as _volume
 
 from ..commons import MapIndex, logger, iterate_connected_components, siibra_tqdm
 from ..locations import boundingbox
 from ..retrieval import cache
+from ..retrieval.repositories import ZipfileConnector, GitlabConnector
 
-from os import path
+from os import path, rename, makedirs
+from zipfile import ZipFile, ZIP_DEFLATED
 import gzip
 from typing import Dict, Union, TYPE_CHECKING, List
 from nilearn import image
 from nibabel import Nifti1Image, load
 import numpy as np
 
 if TYPE_CHECKING:
@@ -105,37 +107,37 @@
         # returns the x, y, and z coordinates of nonzero voxels for the map
         # with the given index, together with their corresponding values v.
         assert volume in range(self.num_volumes)
         x, y, z = [v.squeeze() for v in np.split(self.coords(volume), 3)]
         v = [self.probs[i][volume] for i in self.voxels[x, y, z]]
         return x, y, z, v
 
-    def to_cache(self, prefix: str):
+    def _to_local_cache(self):
         """
         Serialize this index to the cache, using the given prefix for the cache
         filenames.
         """
-        probsfile = cache.CACHE.build_filename(f"{prefix}", suffix="probs.txt.gz")
-        bboxfile = cache.CACHE.build_filename(f"{prefix}", suffix="bboxes.txt.gz")
-        voxelfile = cache.CACHE.build_filename(f"{prefix}", suffix="voxels.nii.gz")
+        probsfile = cache.CACHE.build_filename(f"{self._cache_prefix}", suffix="probs.txt.gz")
+        bboxfile = cache.CACHE.build_filename(f"{self._cache_prefix}", suffix="bboxes.txt.gz")
+        voxelfile = cache.CACHE.build_filename(f"{self._cache_prefix}", suffix="voxels.nii.gz")
         Nifti1Image(self.voxels, self.affine).to_filename(voxelfile)
         with gzip.open(probsfile, 'wt') as f:
             for D in self.probs:
                 f.write("{}\n".format(" ".join(f"{i} {p}" for i, p in D.items())))
         with gzip.open(bboxfile, "wt") as f:
             for bbox in self.bboxes:
                 f.write(
                     "{} {}\n".format(
                         " ".join(map(str, bbox["minpoint"])),
                         " ".join(map(str, bbox["maxpoint"])),
                     )
                 )
 
-    @classmethod
-    def from_cache(cls, prefix: str):
+    @staticmethod
+    def _from_local_cache(cache_name: str):
         """
         Attempts to build a sparse index from the siibra cache, looking for
         suitable cache files with the specified prefix.
 
         Parameters
         ----------
         prefix: str
@@ -143,17 +145,17 @@
 
         Returns
         -------
         SparseIndex
             None if cached files are not found or suitable.
         """
 
-        probsfile = cache.CACHE.build_filename(f"{prefix}", suffix="probs.txt.gz")
-        bboxfile = cache.CACHE.build_filename(f"{prefix}", suffix="bboxes.txt.gz")
-        voxelfile = cache.CACHE.build_filename(f"{prefix}", suffix="voxels.nii.gz")
+        probsfile = cache.CACHE.build_filename(f"{cache_name}", suffix="probs.txt.gz")
+        bboxfile = cache.CACHE.build_filename(f"{cache_name}", suffix="bboxes.txt.gz")
+        voxelfile = cache.CACHE.build_filename(f"{cache_name}", suffix="voxels.nii.gz")
         if not all(path.isfile(f) for f in [probsfile, bboxfile, voxelfile]):
             return None
 
         result = SparseIndex()
 
         voxels = load(voxelfile)
         result.voxels = np.asanyarray(voxels.dataobj)
@@ -220,14 +222,16 @@
         indices: Dict[str, MapIndex],
         volumes: list = [],
         shortname: str = "",
         description: str = "",
         modality: str = None,
         publications: list = [],
         datasets: list = [],
+        is_cached: bool = False,
+        cache_url: str = "",
     ):
         parcellationmap.Map.__init__(
             self,
             identifier=identifier,
             name=name,
             space_spec=space_spec,
             parcellation_spec=parcellation_spec,
@@ -235,22 +239,41 @@
             shortname=shortname,
             description=description,
             modality=modality,
             publications=publications,
             datasets=datasets,
             volumes=volumes,
         )
-
         self._sparse_index_cached = None
+        self._sparseindex_zip_url = cache_url if is_cached else ""
+    
+    @property
+    def _cache_prefix(self):
+        return f"{self.parcellation.id}_{self.space.id}_{self.maptype}_{self.name}_index"
 
     @property
     def sparse_index(self):
         if self._sparse_index_cached is None:
-            prefix = f"{self.parcellation.id}_{self.space.id}_{self.maptype}_{self.name}_index"
-            spind = SparseIndex.from_cache(prefix)
+            spind = SparseIndex._from_local_cache(self._cache_prefix)
+            if spind is None and len(self._sparseindex_zip_url) > 0:
+                logger.debug("Loading SparseIndex from precomputed source.")
+                try:
+                    spind = self.load_zipped_sparseindex(self._sparseindex_zip_url)
+                except Exception:
+                    logger.debug("Could not load SparseIndex from precomputed source.", exc_info=1)
+            if spind is None:
+                logger.debug("Loading SparseIndex from Gitlab.")
+                gconn = GitlabConnector(self._GITLAB_SERVER, self._GITLAB_PROJECT, "main")
+                zip_fname = f"{self.name.replace(' ', '_')}_index.zip"
+                try:
+                    assert zip_fname in gconn.search_files(), f"{zip_fname} is not in {gconn}."
+                    zipfile = gconn.get_loader(zip_fname).url
+                    spind = self.load_zipped_sparseindex(zipfile)
+                except Exception:
+                    logger.debug(f"Could not load SparseIndex from Gitlab at {gconn}", exc_info=1)
             if spind is None:
                 with _volume.SubvolumeProvider.UseCaching():
                     spind = SparseIndex()
                     for vol in siibra_tqdm(
                         range(len(self)), total=len(self), unit="maps",
                         desc=f"Fetching {len(self)} volumetric maps"
                     ):
@@ -258,27 +281,91 @@
                             index=MapIndex(volume=vol, label=None)
                         )
                         if img is None:
                             region = self.get_region(volume=vol)
                             logger.error(f"Cannot retrieve volume #{vol} for {region.name}, it will not be included in the sparse map.")
                             continue
                         spind.add_img(img)
-                    spind.to_cache(prefix)
+                    spind._to_local_cache(self._cache_prefix)
             self._sparse_index_cached = spind
         assert self._sparse_index_cached.max() == len(self._sparse_index_cached.probs) - 1
         return self._sparse_index_cached
 
     @property
     def affine(self):
         return self.sparse_index.affine
 
     @property
     def shape(self):
         return self.sparse_index.shape
 
+    def save_sparseindex(self, destination: str, filename: str = None):
+        """
+        Save SparseIndex as a .zip in destination folder from local cache. If
+        SparseIndex is not cached, siibra will firt create it first.
+
+        Parameters
+        ----------
+        destination: str
+            The path where the zip file will be created.
+        filename: str, default=None
+            Name of the zip and prefix of the SparseIndex files. If None, siibra
+            uses `name` property.
+        """
+        if filename is None:
+            filename = f"{self.name.replace(' ', '_')}_index"
+        logger.info(f"Saving SparseIndex of '{self.name}' as '{filename}.zip'")
+        if not path.isdir(destination):
+            makedirs(destination)
+        if self._sparse_index_cached is None:
+            _ = self.sparse_index
+        suffices = [".probs.txt.gz", ".bboxes.txt.gz", ".voxels.nii.gz"]
+        try:
+            with ZipFile(f"{destination}/{filename}.zip", 'w') as zipf:
+                for suffix in suffices:
+                    zipf.write(
+                        filename=cache.CACHE.build_filename(self._cache_prefix, suffix),
+                        arcname=path.basename(f"{filename}{suffix}"),
+                        compress_type=ZIP_DEFLATED
+                    )
+        except Exception as e:
+            logger.error("Could not save SparseIndex:\n")
+            raise e
+        logger.info("SparseIndex is saved.")
+
+    def load_zipped_sparseindex(self, zipfname: str):
+        """
+        Load SparseIndex from previously computed source and creates a local
+        cache.
+
+        Parameters
+        ----------
+        zipfile: str
+            A url or a path to zip file containing the SparseIndex files for
+            this SparseMap precomputed by siibra.
+
+        Returns
+        -------
+        SparseIndex
+        """
+        zconn = ZipfileConnector(zipfname)
+        with ZipFile(zconn.zipfile, 'r') as zp:
+            suffices = [".probs.txt.gz", ".bboxes.txt.gz", ".voxels.nii.gz"]
+            for suffix in suffices:
+                file = [f for f in zconn.search_files(suffix=suffix)]
+                assert len(file) == 1, f"Could not find a unique '{suffix}' file in {zipfname}."
+                zp.extract(file[0], cache.CACHE.folder)
+                rename(
+                    path.join(cache.CACHE.folder, file[0]),
+                    cache.CACHE.build_filename(self._cache_prefix, suffix=suffix)
+                )
+        zconn.clear_cache()
+
+        return SparseIndex._from_local_cache(self._cache_prefix)
+
     def fetch(
         self,
         region_or_index: Union[MapIndex, str, 'Region'] = None,
         *,
         index: MapIndex = None,
         region: Union[str, 'Region'] = None,
         **kwargs
@@ -373,15 +460,14 @@
         minsize_voxel: int, default: 1
             Minimum voxel size of image components to be taken into account.
         lower_threshold: float, default: 0
             Lower threshold on values in the statistical map. Values smaller than
             this threshold will be excluded from the assignment computation.
         """
         assignments = []
-        components = None
 
         # resample query image into this image's voxel space, if required
         if (queryimg.affine - self.affine).sum() == 0:
             queryimg = queryimg
         else:
             if issubclass(np.asanyarray(queryimg.dataobj).dtype.type, np.integer):
                 interp = "nearest"
@@ -399,15 +485,14 @@
         for mode, modeimg in iterate_connected_components(queryimg):
 
             # determine bounding box of the mode
             modemask = np.asanyarray(modeimg.dataobj)
             XYZ2 = np.array(np.where(modemask)).T
             position = np.dot(modeimg.affine, np.r_[XYZ2.mean(0), 1])[:3]
             if XYZ2.shape[0] <= minsize_voxel:
-                components[modemask] == 0
                 continue
             X2, Y2, Z2 = [v.squeeze() for v in np.split(XYZ2, 3, axis=1)]
 
             bbox2 = boundingbox.BoundingBox(XYZ2.min(0), XYZ2.max(0) + 1, space=None)
             if bbox2.volume == 0:
                 continue
```

### Comparing `siibra-0.4a47/siibra/volumes/volume.py` & `siibra-0.4a51/siibra/volumes/volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,25 +174,25 @@
         """
 
         if format is None:
             requested_formats = self.SUPPORTED_FORMATS
         elif format == 'mesh':
             requested_formats = self.MESH_FORMATS
         elif format == 'image':
-            requested_formats = set(self.SUPPORTED_FORMATS) - set(self.MESH_FORMATS)
+            requested_formats = self.IMAGE_FORMATS
         elif format in self.SUPPORTED_FORMATS:
             requested_formats = [format]
         else:
             raise ValueError(f"Invalid format requested: {format}")
 
         for fmt in requested_formats:
             if fmt in self.formats:
                 try:
                     if fmt == "gii-label":
-                        tpl = self.space.get_template(variant=kwargs.get('variant'), format=format)
+                        tpl = self.space.get_template(variant=kwargs.get('variant'))
                         mesh = tpl.fetch(**kwargs)
                         labels = self._providers[fmt].fetch(**kwargs)
                         return dict(**mesh, **labels)
                     else:
                         return self._providers[fmt].fetch(**kwargs)
                 except requests.SiibraHttpRequestError as e:
                     logger.error(f"Cannot access {self._providers[fmt]}")
```

### Comparing `siibra-0.4a47/siibra.egg-info/PKG-INFO` & `siibra-0.4a51/siibra.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siibra
-Version: 0.4a47
+Version: 0.4a51
 Summary: siibra - Software interfaces for interacting with brain atlases
 Home-page: https://github.com/FZJ-INM1-BDA/siibra-python
 Author: Big Data Analytics Group, Forschungszentrum Juelich, Institute of Neuroscience and Medicine (INM-1)
 Author-email: inm1-bda@fz-juelich.de
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-|License| |PyPI version| |Python versions| |Documentation Status|
+|License| |PyPI version| |doi| |Python versions| |Documentation Status|
 
 siibra - Software interface for interacting with brain atlases
 ==============================================================
 
 Copyright 2020-2023, Forschungszentrum Jülich GmbH
 
 *Authors: Big Data Analytics Group, Institute of Neuroscience and
@@ -131,7 +131,9 @@
    :target: https://opensource.org/licenses/Apache-2.0
 .. |PyPI version| image:: https://badge.fury.io/py/siibra.svg
    :target: https://pypi.org/project/siibra/
 .. |Python versions| image:: https://img.shields.io/pypi/pyversions/siibra.svg
    :target: https://pypi.python.org/pypi/siibra
 .. |Documentation Status| image:: https://readthedocs.org/projects/siibra-python/badge/?version=latest
    :target: https://siibra-python.readthedocs.io/en/latest/?badge=latest
+.. |doi| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7885729.svg
+   :target: https://doi.org/10.5281/zenodo.7885729
```

### Comparing `siibra-0.4a47/siibra.egg-info/SOURCES.txt` & `siibra-0.4a51/siibra.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 siibra/features/anchor.py
 siibra/features/feature.py
 siibra/features/connectivity/__init__.py
 siibra/features/connectivity/functional_connectivity.py
 siibra/features/connectivity/regional_connectivity.py
 siibra/features/connectivity/streamline_counts.py
 siibra/features/connectivity/streamline_lengths.py
+siibra/features/connectivity/tracer_connectivity.py
 siibra/features/dataset/__init__.py
 siibra/features/dataset/ebrains.py
 siibra/features/image/__init__.py
 siibra/features/image/image.py
 siibra/features/image/sections.py
 siibra/features/image/volume_of_interest.py
 siibra/features/tabular/__init__.py
```

### Comparing `siibra-0.4a47/test/test_siibra.py` & `siibra-0.4a51/test/test_siibra.py`

 * *Files identical despite different names*

