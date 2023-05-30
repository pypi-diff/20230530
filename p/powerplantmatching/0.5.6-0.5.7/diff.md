# Comparing `tmp/powerplantmatching-0.5.6.tar.gz` & `tmp/powerplantmatching-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerplantmatching-0.5.6.tar", last modified: Mon Feb 13 16:37:05 2023, max compression
+gzip compressed data, was "powerplantmatching-0.5.7.tar", last modified: Tue May 30 09:22:09 2023, max compression
```

## Comparing `powerplantmatching-0.5.6.tar` & `powerplantmatching-0.5.7.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 16:37:05.153090 powerplantmatching-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (116)    35141 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      150 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     4860 2023-02-13 16:37:05.153090 powerplantmatching-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4130 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 16:37:05.149090 powerplantmatching-0.5.6/powerplantmatching/
--rw-r--r--   0 runner    (1001) docker     (116)     1453 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3213 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/accessor.py
--rw-r--r--   0 runner    (1001) docker     (116)    14912 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/cleaning.py
--rw-r--r--   0 runner    (1001) docker     (116)     9464 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/collection.py
--rw-r--r--   0 runner    (1001) docker     (116)     4557 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/core.py
--rw-r--r--   0 runner    (1001) docker     (116)    54294 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/data.py
--rw-r--r--   0 runner    (1001) docker     (116)     5426 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/duke.py
--rw-r--r--   0 runner    (1001) docker     (116)    13538 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/export.py
--rw-r--r--   0 runner    (1001) docker     (116)    21845 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/heuristics.py
--rw-r--r--   0 runner    (1001) docker     (116)    11423 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 16:37:05.153090 powerplantmatching-0.5.6/powerplantmatching/package_data/
--rw-r--r--   0 runner    (1001) docker     (116)     2731 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/package_data/Comparison.xml
--rw-r--r--   0 runner    (1001) docker     (116)     2431 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/package_data/Deleteduplicates.xml
--rw-r--r--   0 runner    (1001) docker     (116)   276266 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/package_data/PLZ_Coords_map.csv
--rw-r--r--   0 runner    (1001) docker     (116)    12063 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/package_data/config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    11150 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/package_data/country_codes.csv
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 16:37:05.153090 powerplantmatching-0.5.6/powerplantmatching/package_data/duke_binaries/
--rw-r--r--   0 runner    (1001) docker     (116)   186104 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/package_data/duke_binaries/duke-core-1.3-SNAPSHOT-tests.jar
--rw-r--r--   0 runner    (1001) docker     (116)   266706 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/package_data/duke_binaries/duke-core-1.3-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (116)    11609 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/package_data/duke_binaries/duke-es-1.3-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (116)     5646 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/package_data/duke_binaries/duke-json-1.3-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (116)    15346 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/package_data/duke_binaries/duke-lucene-1.3-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (116)     8572 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/package_data/duke_binaries/duke-mapdb-1.3-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (116)     7603 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/package_data/duke_binaries/duke-mongodb-1.3-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (116)    11877 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/package_data/duke_binaries/duke-server-1.3-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (116)      343 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/package_data/entsoe_country_codes.csv
--rw-r--r--   0 runner    (1001) docker     (116)     3484 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/package_data/manual_corrections.csv
--rw-r--r--   0 runner    (1001) docker     (116)     4540 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/package_data/manual_corrections_old.csv
--rw-r--r--   0 runner    (1001) docker     (116)    96397 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/package_data/parsed_locations.csv
--rw-r--r--   0 runner    (1001) docker     (116)    39591 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/plot.py
--rw-r--r--   0 runner    (1001) docker     (116)    19928 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/powerplantmatching/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 16:37:05.149090 powerplantmatching-0.5.6/powerplantmatching.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4860 2023-02-13 16:37:05.000000 powerplantmatching-0.5.6/powerplantmatching.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1758 2023-02-13 16:37:05.000000 powerplantmatching-0.5.6/powerplantmatching.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-13 16:37:05.000000 powerplantmatching-0.5.6/powerplantmatching.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      285 2023-02-13 16:37:05.000000 powerplantmatching-0.5.6/powerplantmatching.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       19 2023-02-13 16:37:05.000000 powerplantmatching-0.5.6/powerplantmatching.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      307 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/requirements.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       67 2023-02-13 16:37:05.153090 powerplantmatching-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1792 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 16:37:05.153090 powerplantmatching-0.5.6/test/
--rw-r--r--   0 runner    (1001) docker     (116)      567 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/test/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (116)     2026 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/test/test_cleaning.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1295 2023-02-13 16:36:56.000000 powerplantmatching-0.5.6/test/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:22:09.057524 powerplantmatching-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-30 09:22:09.057524 powerplantmatching-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:22:09.053524 powerplantmatching-0.5.7/powerplantmatching/
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14912 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68726 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/duke.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13538 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21845 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:22:09.053524 powerplantmatching-0.5.7/powerplantmatching/package_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/package_data/Comparison.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/package_data/Deleteduplicates.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   276266 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/package_data/PLZ_Coords_map.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/package_data/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/package_data/country_codes.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:22:09.057524 powerplantmatching-0.5.7/powerplantmatching/package_data/duke_binaries/
+-rw-r--r--   0 runner    (1001) docker     (123)   186104 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/package_data/duke_binaries/duke-core-1.3-SNAPSHOT-tests.jar
+-rw-r--r--   0 runner    (1001) docker     (123)   266706 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/package_data/duke_binaries/duke-core-1.3-SNAPSHOT.jar
+-rw-r--r--   0 runner    (1001) docker     (123)    11609 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/package_data/duke_binaries/duke-es-1.3-SNAPSHOT.jar
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/package_data/duke_binaries/duke-json-1.3-SNAPSHOT.jar
+-rw-r--r--   0 runner    (1001) docker     (123)    15346 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/package_data/duke_binaries/duke-lucene-1.3-SNAPSHOT.jar
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/package_data/duke_binaries/duke-mapdb-1.3-SNAPSHOT.jar
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/package_data/duke_binaries/duke-mongodb-1.3-SNAPSHOT.jar
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/package_data/duke_binaries/duke-server-1.3-SNAPSHOT.jar
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/package_data/entsoe_country_codes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/package_data/manual_corrections.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/package_data/manual_corrections_old.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    96397 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/package_data/parsed_locations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    39591 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/powerplantmatching/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:22:09.053524 powerplantmatching-0.5.7/powerplantmatching.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-30 09:22:09.000000 powerplantmatching-0.5.7/powerplantmatching.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-30 09:22:09.000000 powerplantmatching-0.5.7/powerplantmatching.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:22:09.000000 powerplantmatching-0.5.7/powerplantmatching.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-30 09:22:09.000000 powerplantmatching-0.5.7/powerplantmatching.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-30 09:22:09.000000 powerplantmatching-0.5.7/powerplantmatching.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/requirements.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 09:22:09.057524 powerplantmatching-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:22:09.057524 powerplantmatching-0.5.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/test/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/test/test_cleaning.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1295 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-30 09:22:00.000000 powerplantmatching-0.5.7/test/test_duke.py
```

### Comparing `powerplantmatching-0.5.6/LICENSE` & `powerplantmatching-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/PKG-INFO` & `powerplantmatching-0.5.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,11 @@
-Metadata-Version: 2.1
-Name: powerplantmatching
-Version: 0.5.6
-Summary: Toolset for generating and managing Power Plant Data
-Home-page: https://github.com/FRESNA/powerplantmatching
-Author: Fabian Hofmann (FIAS), Jonas Hoersch (KIT), Fabian Gotzens (FZ Jülich)
-Author-email: hofmann@fias.uni-frankfurt.de
-License: GPLv3
-Classifier: Programming Language :: Python :: 3
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: dev
-License-File: LICENSE
-
 # powerplantmatching
 
  [![pypi](https://img.shields.io/pypi/v/powerplantmatching.svg)](https://pypi.org/project/powerplantmatching/) [![conda](https://img.shields.io/conda/vn/conda-forge/powerplantmatching.svg)](https://anaconda.org/conda-forge/powerplantmatching) ![pythonversion](https://img.shields.io/pypi/pyversions/powerplantmatching) ![LICENSE](https://img.shields.io/pypi/l/powerplantmatching.svg) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3358985.svg)](https://zenodo.org/record/3358985#.XUReFPxS_MU) [![doc](https://readthedocs.org/projects/powerplantmatching/badge/?version=latest)](https://powerplantmatching.readthedocs.io/en/latest/) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/FRESNA/powerplantmatching/master.svg)](https://results.pre-commit.ci/latest/github/FRESNA/powerplantmatching/master)
+[![Stack Exchange questions](https://img.shields.io/stackexchange/stackoverflow/t/pypsa)](https://stackoverflow.com/questions/tagged/pypsa)
 
 A toolset for cleaning, standardizing and combining multiple power
 plant databases.
 
 This package provides ready-to-use power plant data for the European power system.
 Starting from openly available power plant datasets, the package cleans, standardizes
 and merges the input data to create a new combined dataset, which includes all the important information.
@@ -60,14 +42,22 @@
 
 or conda
 
 ```bash
 conda install -c conda-forge powerplantmatching
 ```
 
+# Contributing and Support
+We strongly welcome anyone interested in contributing to this project. If you have any ideas, suggestions or encounter problems, feel invited to file issues or make pull requests on GitHub.
+-   In case of code-related **questions**, please post on [stack overflow](https://stackoverflow.com/questions/tagged/pypsa).
+-   For non-programming related and more general questions please refer to the [PyPSA mailing list](https://groups.google.com/group/pypsa).
+-   To **discuss** with other PyPSA & technology-data users, organise projects, share news, and get in touch with the community you can use the [discord server](https://discord.gg/JTdvaEBb).
+-   For **bugs and feature requests**, please use the [powerplantmatching Github Issues page](https://github.com/PyPSA/powerplantmatching/issues).
+
+
 ## Citing powerplantmatching
 
 If you want to cite powerplantmatching, use the following paper
 
 - F. Gotzens, H. Heinrichs, J. Hörsch, and F. Hofmann, [Performing energy modelling exercises in a transparent way - The issue of data quality in power plant databases](https://www.sciencedirect.com/science/article/pii/S2211467X18301056?dgcid=author), Energy Strategy Reviews, vol. 23, pp. 1–12, Jan. 2019.
 
 with bibtex
```

### Comparing `powerplantmatching-0.5.6/powerplantmatching/__init__.py` & `powerplantmatching-0.5.7/powerplantmatching/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 A set of tools for cleaning, standardising and combining multiple
 power plant databases.
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.5.6"
+__version__ = "0.5.7"
 __author__ = "Fabian Hofmann"
 __copyright__ = "Copyright 2017-2022 Technical University of Berlin"
 # The rough hierarchy of this package is
 # core, utils, heuristics, cleaning, matching, collection, data
 
 # from . import cleaning
 # from . import matching
```

### Comparing `powerplantmatching-0.5.6/powerplantmatching/accessor.py` & `powerplantmatching-0.5.7/powerplantmatching/accessor.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/cleaning.py` & `powerplantmatching-0.5.7/powerplantmatching/cleaning.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/collection.py` & `powerplantmatching-0.5.7/powerplantmatching/collection.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/core.py` & `powerplantmatching-0.5.7/powerplantmatching/core.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/data.py` & `powerplantmatching-0.5.7/powerplantmatching/data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1578,14 +1578,373 @@
 
     l = list(set(df.columns).difference(set(["Capacity"])))
     df = df.groupby(l, as_index=False, dropna=True).sum()
 
     return df
 
 
+def GBPT(raw=False, update=False, config=None):
+    """
+    Importer for the global bioenergy powerplant tracker from global energy monitor.
+
+    Parameters
+    ----------
+    raw : boolean, default False
+        Whether to return the original dataset
+    update: bool, default False
+        Whether to update the data from the url.
+    config : dict, default None
+        Add custom specific configuration,
+        e.g. powerplantmatching.config.get_config(target_countries='Italy'),
+        defaults to powerplantmatching.config.get_config()
+    """
+    config = get_config() if config is None else config
+    fn = get_raw_file("GBPT", update=update, config=config)
+    df = pd.read_csv(fn, thousands=",")
+
+    if raw:
+        return df
+
+    RENAME_COLUMNS = {
+        "Project Name": "Name",
+        "Capacity (MW)": "Capacity",
+        "Operating Status": "Status",
+        "Latitude": "lat",
+        "Longitude": "lon",
+        "Start year": "DateIn",
+        "Retired year": "DateOut",
+        "GEM phase ID": "projectID",
+    }
+
+    df = df.rename(columns=RENAME_COLUMNS)
+    df_final = (
+        df.pipe(clean_name)
+        .pipe(set_column_name, "GBPT")
+        .pipe(convert_to_short_name)
+        .dropna(subset="Capacity")
+        .assign(
+            DateIn=df["DateIn"].apply(pd.to_numeric, errors="coerce"),
+            DateOut=df["DateOut"].apply(pd.to_numeric, errors="coerce"),
+            lat=df["lat"].apply(pd.to_numeric, errors="coerce"),
+            lon=df["lon"].apply(pd.to_numeric, errors="coerce"),
+        )
+        .query("Status in ['operating','mothballed','construction']")
+        .pipe(lambda x: x[df.columns.intersection(config.get("target_columns"))])
+        .assign(Fueltype="Bioenergy")
+        .assign(Technology="Steam Turbine")
+        .assign(Set="PP")
+        .pipe(config_filter, config)
+    )
+    return df_final
+
+
+def GNPT(raw=False, update=False, config=None):
+    """
+    Importer for the global nuclear energy powerplant tracker from global energy monitor.
+
+    Parameters
+    ----------
+    raw : boolean, default False
+        Whether to return the original dataset
+    update: bool, default False
+        Whether to update the data from the url.
+    config : dict, default None
+        Add custom specific configuration,
+        e.g. powerplantmatching.config.get_config(target_countries='Italy'),
+        defaults to powerplantmatching.config.get_config()
+    """
+    config = get_config() if config is None else config
+    fn = get_raw_file("GNPT", update=update, config=config)
+    df = pd.read_csv(fn, thousands=",")
+
+    if raw:
+        return df
+
+    RENAME_COLUMNS = {
+        "Project Name": "Name",
+        "Capacity (MW)": "Capacity",
+        "Latitude": "lat",
+        "Longitude": "lon",
+        "Start Year": "DateIn",
+        "Retired Year": "DateOut",
+        "GEM unit ID": "projectID",
+    }
+
+    df = df.rename(columns=RENAME_COLUMNS)
+    df_final = (
+        df.pipe(clean_name)
+        .pipe(set_column_name, "GNPT")
+        .pipe(convert_to_short_name)
+        .dropna(subset="Capacity")
+        .assign(
+            DateIn=df["DateIn"].apply(pd.to_numeric, errors="coerce"),
+            DateOut=df["DateOut"].apply(pd.to_numeric, errors="coerce"),
+            lat=df["lat"].apply(pd.to_numeric, errors="coerce"),
+            lon=df["lon"].apply(pd.to_numeric, errors="coerce"),
+        )
+        .query("Status in ['operating','mothballed','construction']")
+        .pipe(lambda x: x[df.columns.intersection(config.get("target_columns"))])
+        .assign(Fueltype="Nuclear")
+        .assign(Technology="Steam Turbine")
+        .assign(Set="PP")
+        .pipe(config_filter, config)
+    )
+    return df_final
+
+
+def GCPT(raw=False, update=False, config=None):
+    """
+    Importer for the global coal powerplant tracker from global energy monitor.
+
+    Parameters
+    ----------
+    raw : boolean, default False
+        Whether to return the original dataset
+    update: bool, default False
+        Whether to update the data from the url.
+    config : dict, default None
+        Add custom specific configuration,
+        e.g. powerplantmatching.config.get_config(target_countries='Italy'),
+        defaults to powerplantmatching.config.get_config()
+    """
+
+    config = get_config() if config is None else config
+    fn = get_raw_file("GCPT", update=update, config=config)
+    df = pd.read_csv(fn)
+
+    if raw:
+        return df
+
+    RENAME_COLUMNS = {
+        "Plant": "Name",
+        "Combustion technology": "Technology",
+        "Coal type": "Fueltype",
+        "Capacity (MW)": "Capacity",
+        "Latitude": "lat",
+        "Longitude": "lon",
+        "Year": "DateIn",
+        "RETIRED": "DateOut",
+        "Tracker ID": "projectID",
+    }
+    fueltype_dict = {
+        "bituminous": "Hard Coal",
+        "lignite": "Lignite",
+        "unknown": "Hard Coal",
+        "sub-bit": "Hard Coal",
+        "bituminous/sub-bit": "Hard Coal",
+        "wstbituminous": "Hard Coal",
+        "unknown(ccs90)": "Hard Coal",
+        "hard": "Hard Coal",
+        "anth": "Hard Coal",
+        "lignite(ccs90)": "Lignite",
+        "sub-bit(ccs90)": "Hard Coal",
+        "lignite/sub-bit": "Lignite",
+        "wstcoal": "Hard Coal",
+        "bituminous(ccs90)": "Hard Coal",
+        "bituminous(ccs30)": "Hard Coal",
+        "lignite/bituminous": "Lignite",
+        "anth/bituminous": "Hard Coal",
+        "anth/culm": "Hard Coal",
+        "bituminous/wstbituminous": "Hard Coal",
+    }
+    df = df.rename(columns=RENAME_COLUMNS)
+    df_final = (
+        df.pipe(clean_name)
+        .pipe(set_column_name, "GCPT")
+        .pipe(convert_to_short_name)
+        .dropna(subset="Capacity")
+        .pipe(lambda x: x.replace({"Fueltype": fueltype_dict}))
+        .pipe(lambda x: x.assign(Technology="Steam Turbine"))
+        .pipe(lambda x: x.assign(Set="PP"))
+        .assign(
+            DateIn=df["DateIn"].apply(pd.to_numeric, errors="coerce"),
+            DateOut=df["DateOut"].apply(pd.to_numeric, errors="coerce"),
+            lat=df["lat"].apply(pd.to_numeric, errors="coerce"),
+            lon=df["lon"].apply(pd.to_numeric, errors="coerce"),
+        )
+        .pipe(lambda x: x[df.columns.intersection(config.get("target_columns"))])
+        .pipe(config_filter, config)
+    )
+
+    return df_final
+
+
+def GGTPT(raw=False, update=False, config=None):
+    """
+    Importer for the global geothermal powerplant tracker from global energy monitor.
+
+    Parameters
+    ----------
+    raw : boolean, default False
+        Whether to return the original dataset
+    update: bool, default False
+        Whether to update the data from the url.
+    config : dict, default None
+        Add custom specific configuration,
+        e.g. powerplantmatching.config.get_config(target_countries='Italy'),
+        defaults to powerplantmatching.config.get_config()
+    """
+    config = get_config() if config is None else config
+    fn = get_raw_file("GGTPT", update=update, config=config)
+    df = pd.read_csv(fn)
+
+    if raw:
+        return df
+
+    RENAME_COLUMNS = {
+        "Project Name": "Name",
+        "Unit Capacity (MW)": "Capacity",
+        "Latitude": "lat",
+        "Longitude": "lon",
+        "Start year": "DateIn",
+        "Retired year": "DateOut",
+        "GEM unit ID": "projectID",
+    }
+
+    df = df.rename(columns=RENAME_COLUMNS)
+    df_final = (
+        df.pipe(clean_name)
+        .pipe(set_column_name, "GGTPT")
+        .pipe(convert_to_short_name)
+        .dropna(subset="Capacity")
+        .assign(
+            DateIn=df["DateIn"].apply(pd.to_numeric, errors="coerce"),
+            DateOut=df["DateOut"].apply(pd.to_numeric, errors="coerce"),
+            lat=df["lat"].apply(pd.to_numeric, errors="coerce"),
+            lon=df["lon"].apply(pd.to_numeric, errors="coerce"),
+        )
+        .query("Status in ['operating','mothballed','construction']")
+        .pipe(lambda x: x[df.columns.intersection(config.get("target_columns"))])
+        .assign(Fueltype="Geothermal")
+        .assign(Technology="Steam Turbine")
+        .assign(Set="PP")
+        .pipe(config_filter, config)
+    )
+    return df_final
+
+
+def GWPT(raw=False, update=False, config=None):
+    """
+    Importer for the global wind powerplant tracker from global energy monitor.
+
+    Parameters
+    ----------
+    raw : boolean, default False
+        Whether to return the original dataset
+    update: bool, default False
+        Whether to update the data from the url.
+    config : dict, default None
+        Add custom specific configuration,
+        e.g. powerplantmatching.config.get_config(target_countries='Italy'),
+        defaults to powerplantmatching.config.get_config()
+    """
+    config = get_config() if config is None else config
+    fn = get_raw_file("GWPT", update=update, config=config)
+    df = pd.read_csv(fn)
+
+    RENAME_COLUMNS = {
+        "Project Name": "Name",
+        "Capacity (MW)": "Capacity",
+        "Latitude": "lat",
+        "Longitude": "lon",
+        "Start year": "DateIn",
+        "Retired year": "DateOut",
+        "GEM phase ID": "projectID",
+        "Installation Type": "Technology",
+    }
+
+    technology_dict = {
+        "onshore": "Onshore",
+        "offshore hard mount": "Offshore",
+        "offshore floating": "Offshore",
+        "offshore mount unknown": "Offshore",
+    }
+
+    df = df.rename(columns=RENAME_COLUMNS)
+    df_final = (
+        df.pipe(clean_name)
+        .pipe(set_column_name, "GWPT")
+        .pipe(convert_to_short_name)
+        .dropna(subset="Capacity")
+        .assign(
+            DateIn=df["DateIn"].apply(pd.to_numeric, errors="coerce"),
+            DateOut=df["DateOut"].apply(pd.to_numeric, errors="coerce"),
+            lat=df["lat"].apply(pd.to_numeric, errors="coerce"),
+            lon=df["lon"].apply(pd.to_numeric, errors="coerce"),
+        )
+        .query("Status in ['operating','mothballed','construction']")
+        .pipe(lambda x: x[df.columns.intersection(config.get("target_columns"))])
+        .assign(Fueltype="Wind")
+        .assign(Set="PP")
+        .pipe(config_filter, config)
+    )
+    return df_final
+
+
+def GSPT(raw=False, update=False, config=None):
+    """
+    Importer for the global solar powerplant tracker from global energy monitor.
+
+    Parameters
+    ----------
+    raw : boolean, default False
+        Whether to return the original dataset
+    update: bool, default False
+        Whether to update the data from the url.
+    config : dict, default None
+        Add custom specific configuration,
+        e.g. powerplantmatching.config.get_config(target_countries='Italy'),
+        defaults to powerplantmatching.config.get_config()
+    """
+
+    config = get_config() if config is None else config
+    fn = get_raw_file("GSPT", update=update, config=config)
+    df = pd.read_csv(fn)
+
+    if raw:
+        return df
+
+    RENAME_COLUMNS = {
+        "Project Name": "Name",
+        "Capacity (MW)": "Capacity",
+        "Latitude": "lat",
+        "Longitude": "lon",
+        "Start year": "DateIn",
+        "Retired year": "DateOut",
+        "Technology Type": "Technology",
+        "GEM phase ID": "projectID",
+    }
+
+    technology_dict = {
+        "PV": "PV",
+        "Solar Thermal": "CSP",
+        "Assumed PV": "PV",
+    }
+    df = df.rename(columns=RENAME_COLUMNS)
+    df_final = (
+        df.pipe(clean_name)
+        .pipe(set_column_name, "GSPT")
+        .pipe(convert_to_short_name)
+        .dropna(subset="Capacity")
+        .pipe(lambda x: x.replace({"Technology": technology_dict}))
+        .assign(
+            DateIn=df["DateIn"].apply(pd.to_numeric, errors="coerce"),
+            DateOut=df["DateOut"].apply(pd.to_numeric, errors="coerce"),
+            lat=df["lat"].apply(pd.to_numeric, errors="coerce"),
+            lon=df["lon"].apply(pd.to_numeric, errors="coerce"),
+        )
+        .query("Status in ['operating','mothballed','construction']")
+        .pipe(lambda x: x[df.columns.intersection(config.get("target_columns"))])
+        .assign(Fueltype="Solar")
+        .assign(Set="PP")
+        .pipe(config_filter, config)
+    )
+    return df_final
+
+
 def GGPT(raw=False, update=False, config=None):
     """
     Importer for the global gas powerplant tracker from global energy monitor.
 
     Parameters
     ----------
     raw : boolean, default False
@@ -1595,29 +1954,29 @@
     config : dict, default None
         Add custom specific configuration,
         e.g. powerplantmatching.config.get_config(target_countries='Italy'),
         defaults to powerplantmatching.config.get_config()
     """
     config = get_config() if config is None else config
     fn = get_raw_file("GGPT", update=update, config=config)
-    df = pd.read_excel(fn, sheet_name="Gas plants - data")
+    df = pd.read_csv(fn)
 
     if raw:
         return df
 
     RENAME_COLUMNS = {
         "Plant name": "Name",
         "Fuel": "Fueltype",
         "Capacity elec. (MW)": "Capacity",
         "Latitude": "lat",
         "Longitude": "lon",
         "Start year": "DateIn",
         "Retired year": "DateOut",
         "CHP": "Set",
-        "GEM unit ID": "projectID",
+        "GEM location ID": "projectID",
     }
 
     technology_dict = {
         "GT": "Steam Turbine",
         "CC": "CCGT",
         "GT/IC": "Steam Turbine",
         "ICCC": "CCGT",
@@ -1627,33 +1986,98 @@
 
     set_dict = {
         "Y": "CHP",
         "N": "PP",
         "not found": "PP",
     }
 
-    df = (
-        df.rename(columns=RENAME_COLUMNS)
-        .pipe(clean_name)
+    df = df.rename(columns=RENAME_COLUMNS)
+    df_final = (
+        df.pipe(clean_name)
         .pipe(set_column_name, "GGPT")
         .pipe(convert_to_short_name)
         .dropna(subset="Capacity")
-        .assign(Fueltype="Natural Gas")[
-            lambda df: df.Status.isin(["operating", "mothballed", "construction"])
-        ]
-    )
-    df["DateIn"] = pd.to_numeric(df.DateIn, errors="coerce")
-    df["lat"] = pd.to_numeric(df.lat, errors="coerce")
-    df["lon"] = pd.to_numeric(df.lon, errors="coerce")
-    df.Technology.replace(technology_dict, inplace=True)
-    df.Set.replace(set_dict, inplace=True)
-    df = df[df.columns.intersection(config.get("target_columns"))]
-    df = df.pipe(config_filter, config)
+        .pipe(lambda x: x.query("Capacity != 'not found'"))
+        .assign(
+            DateIn=df["DateIn"].apply(pd.to_numeric, errors="coerce"),
+            DateOut=df["DateOut"].apply(pd.to_numeric, errors="coerce"),
+            lat=df["lat"].apply(pd.to_numeric, errors="coerce"),
+            lon=df["lon"].apply(pd.to_numeric, errors="coerce"),
+            Capacity=lambda df: pd.to_numeric(df.Capacity, "coerce"),
+        )
+        .pipe(lambda x: x.replace({"Technology": technology_dict}))
+        .pipe(lambda x: x.replace({"Set": set_dict}))
+        .query("Status in ['operating','mothballed','construction']")
+        .pipe(lambda x: x[df.columns.intersection(config.get("target_columns"))])
+        .assign(Fueltype="Natural Gas")
+        .pipe(config_filter, config)
+    )
+    return df_final
 
-    return df
+
+def GHPT(raw=False, update=False, config=None):
+    """
+    Importer for the global gas powerplant tracker from global energy monitor.
+
+    Parameters
+    ----------
+    raw : boolean, default False
+        Whether to return the original dataset
+    update: bool, default False
+        Whether to update the data from the url.
+    config : dict, default None
+        Add custom specific configuration,
+        e.g. powerplantmatching.config.get_config(target_countries='Italy'),
+        defaults to powerplantmatching.config.get_config()
+    """
+    config = get_config() if config is None else config
+    fn = get_raw_file("GHPT", update=update, config=config)
+    df = pd.read_csv(fn)
+
+    if raw:
+        return df
+
+    RENAME_COLUMNS = {
+        "Project Name": "Name",
+        "Capacity (MW)": "Capacity",
+        "Latitude": "lat",
+        "Longitude": "lon",
+        "Start Year": "DateIn",
+        "Retired Year": "DateOut",
+        "GEM unit ID": "projectID",
+        "Country 1": "Country",
+        "Technology Type": "Technology",
+    }
+    technology_dict = {
+        "conventional storage": "Reservoir",
+        "pumped storage": "Pumped Storage",
+        "run-of-river": "Run-Of-River",
+        "conventional and pumped storage": "Pumped Storage",
+        "conventional and run-of-river": "Run-Of-River",
+    }
+    df = df.rename(columns=RENAME_COLUMNS)
+    df_final = (
+        df.pipe(clean_name)
+        .pipe(set_column_name, "GHPT")
+        .pipe(convert_to_short_name)
+        .dropna(subset="Capacity")
+        .assign(
+            DateIn=df["DateIn"].apply(pd.to_numeric, errors="coerce"),
+            DateOut=df["DateOut"].apply(pd.to_numeric, errors="coerce"),
+            lat=df["lat"].apply(pd.to_numeric, errors="coerce"),
+            lon=df["lon"].apply(pd.to_numeric, errors="coerce"),
+        )
+        .query("Status in ['operating','construction']")
+        .pipe(lambda x: x.replace({"Technology": technology_dict}))
+        .pipe(lambda x: x[df.columns.intersection(config.get("target_columns"))])
+        .assign(Fueltype="Hydro")
+        .assign(Set="PP")
+        .pipe(config_filter, config)
+    )
+    return df_final
 
 
 # deprecated alias for GGPT
 @deprecated(
     deprecated_in="0.5.5",
     removed_in="0.6",
     details="Use `GGPT` instead.",
```

### Comparing `powerplantmatching-0.5.6/powerplantmatching/duke.py` & `powerplantmatching-0.5.7/powerplantmatching/duke.py`

 * *Files 10% similar despite different names*

```diff
@@ -73,14 +73,21 @@
         Only in Record Linkage Mode. Only report the best match for each entry
         of the first named dataset. This does not guarantee a unique match in
         the second named dataset.
     keepfiles : boolean, default False
         If true, do not delete temporary files
     """
 
+    try:
+        sub.run(["java", "-version"], check=True, stderr=sub.PIPE, stdout=sub.PIPE)
+    except sub.CalledProcessError:
+        err = "Java is not installed or not in the system's PATH. Please install Java and ensure it is in your system's PATH, then try again."
+        logger.error(err)
+        raise FileNotFoundError(err)
+
     dedup = isinstance(datasets, pd.DataFrame)
     if dedup:
         # Deduplication mode
         duke_config = "Deleteduplicates.xml"
         datasets = [datasets]
     else:
         duke_config = "Comparison.xml"
@@ -122,27 +129,21 @@
         if showmatches:
             args.append("--showmatches")
             stdout = sub.PIPE
         else:
             stdout = None
         args.append("config.xml")
 
-        try:
-            run = sub.Popen(
-                args,
-                stderr=sub.PIPE,
-                cwd=tmpdir,
-                stdout=stdout,
-                universal_newlines=True,
-            )
-        except FileNotFoundError:
-            err = "Java was not found on your system."
-            logger.error(err)
-            raise FileNotFoundError(err)
-
+        run = sub.Popen(
+            args,
+            stderr=sub.PIPE,
+            cwd=tmpdir,
+            stdout=stdout,
+            universal_newlines=True,
+        )
         _, stderr = run.communicate()
 
         if showmatches:
             print(_)
 
         logger.debug("Stderr: {}".format(stderr))
         if any(word in stderr.lower() for word in ["error", "fehler"]):
```

### Comparing `powerplantmatching-0.5.6/powerplantmatching/export.py` & `powerplantmatching-0.5.7/powerplantmatching/export.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/heuristics.py` & `powerplantmatching-0.5.7/powerplantmatching/heuristics.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/matching.py` & `powerplantmatching-0.5.7/powerplantmatching/matching.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
     if matches.empty:
         logger.warn("No matches found")
         return pd.DataFrame(columns=labels)
 
     if matches.isnull().all().any():
         cols = ", ".join(matches.columns[matches.isnull().all()])
-        raise ValueError(f"No matches found for data source {cols}")
+        logger.warn(f"No matches found for data source {cols}")
 
     matches = matches.drop_duplicates().reset_index(drop=True)
     for i in labels:
         matches = pd.concat(
             [
                 matches.groupby(i, as_index=False, sort=False).apply(
                     lambda x: x.loc[x.isnull().sum(axis=1).idxmin()]
```

### Comparing `powerplantmatching-0.5.6/powerplantmatching/package_data/Comparison.xml` & `powerplantmatching-0.5.7/powerplantmatching/package_data/Comparison.xml`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/package_data/Deleteduplicates.xml` & `powerplantmatching-0.5.7/powerplantmatching/package_data/Deleteduplicates.xml`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/package_data/PLZ_Coords_map.csv` & `powerplantmatching-0.5.7/powerplantmatching/package_data/PLZ_Coords_map.csv`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/package_data/config.yaml` & `powerplantmatching-0.5.7/powerplantmatching/package_data/config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -8,35 +8,51 @@
 #                                Matching Config                               #
 # ---------------------------------------------------------------------------- #
 
 # This query is applied to all input data
 # Note: querying "key == key" filters out nan values
 main_query: "Name != '' and (DateOut >= 2020 or DateOut != DateOut) and (lat >= 30 or lat != lat)"
 
+# matching_sources, only the matched powerplants are added to the final dataset
 matching_sources:
   # Make individual queries for the datasets as done in `fully_included_sources`
   # Queries are combined with `main_query` with an `and` operator
   - ENTSOE
   - GEO
   - GPD
   - JRC
   - OPSD: Country != "Spain" and Fueltype != 'Hard Coal'
   - BEYONDCOAL
   - WIKIPEDIA
+  - GBPT
   - GGPT
+  - GCPT
+  - GGTPT
+  - GNPT
+  - GSPT
+  - GWPT
+  - GHPT
 
+# fully_included_sources, these sources are included even without match to the final dataset
 fully_included_sources:
   # Make individual queries for the datasets
-  - BEYONDCOAL
-  - GGPT
-  - OPSD: Country not in ['Switzerland', 'Italy', 'Spain', 'Norway', 'Austria']
-  - JRC: Country not in ['Switzerland', 'Albania', 'United Kingdom', 'Norway']
   - ENTSOE: (Country not in ['Switzerland', 'Ireland', 'Albania', 'Greece', 'Czech Republic', 'Bulgaria', 'United Kingdom', 'Italy', 'Serbia'] and not (Country == 'Spain' and Fueltype == 'Hydro')) or (Fueltype == 'Geothermal')
-  - GPD: Country in ['Finland', 'Spain']
   - GEO: (Country == 'Spain' and Fueltype == 'Natural Gas')
+  - GPD: Country in ['Finland', 'Spain']
+  - JRC: Country not in ['Switzerland', 'Albania', 'United Kingdom', 'Norway']
+  - OPSD: Country not in ['Switzerland', 'Italy', 'Spain', 'Norway', 'Austria']
+  - BEYONDCOAL
+  - GBPT
+  - GGPT
+  - GCPT
+  - GGTPT
+  - GNPT
+  - GSPT
+  - GWPT
+  - GHPT
 
 parallel_duke_processes: false
 process_limit: 4
 matched_data_url: https://raw.githubusercontent.com/FRESNA/powerplantmatching/{tag}/powerplants.csv
 
 # ---------------------------------------------------------------------------- #
 #                                  Data Source Config                          #
@@ -58,58 +74,58 @@
   net_capacity: true
   aggregated_units: true
   fn: IRENASTAT_capacities_2000-2020.csv
   url: https://zenodo.org/record/6412255/files/IRENASTAT_capacities_2000-2020.csv
 CARMA:
   net_capacity: false
   reliability_score: 1
-  url: https://vfs.fias.science/f/e1d9d9d587/?raw=1
+  url: https://raw.githubusercontent.com/pypsa-meets-earth/ppm-data-backup/main/Full_CARMA_2009_Dataset_1.csv
   fn: Full_CARMA_2009_Dataset_1.csv
 ENTSOE:
   reliability_score: 5
-  url: https://vfs.fias.science/f/ebbdf6ba8c/?raw=1
+  url: https://raw.githubusercontent.com/pypsa-meets-earth/ppm-data-backup/main/entsoe_powerplants.csv
   fn: entsoe_powerplants.csv
 ENTSOE-EIC:
   url: https://eepublicdownloads.entsoe.eu/eic-codes-csv/W_eiccodes.csv
   fn: entsoe_eic_codes.csv
 JRC:
   reliability_score: 4
   fn: jrc-hydro-power-database-10.zip
   url: https://github.com/energy-modelling-toolkit/hydro-power-database/archive/refs/tags/v10.zip
 GEO:
   net_capacity: false
   reliability_score: 3
-  url: https://vfs.fias.science/f/b4607c76b4/?raw=1
+  url: https://raw.githubusercontent.com/pypsa-meets-earth/ppm-data-backup/main/global_energy_observatory_power_plants.csv
   fn: global_energy_observatory_power_plants.csv
 GEO_units:
   net_capacity: false
   reliability_score: 3
-  url: https://vfs.fias.science/f/3f4cc3876f/?raw=1
+  url: https://raw.githubusercontent.com/pypsa-meets-earth/ppm-data-backup/main/global_energy_observatory_ppl_units.csv
   fn: global_energy_observatory_ppl_units.csv
 GPD:
   reliability_score: 3
   fn: globalpowerplantdatabasev120.zip
   #if outdated, look at http://datasets.wri.org/dataset/globalpowerplantdatabase
   url: https://wri-dataportal-prod.s3.amazonaws.com/manual/global_power_plant_database_v_1_3.zip
 WIKIPEDIA:
   reliability_score: 4
-  url: https://vfs.fias.science/f/c49203915f/?raw=1
+  url: https://raw.githubusercontent.com/pypsa-meets-earth/ppm-data-backup/main/nuclear_plants_from_wikipedia.csv
   fn: nuclear_plants_from_wikipedia.csv
 IWPDCY:
   aggregated_units: true
   reliability_score: 3
   fn: IWPDCY.csv
 OPSD_DE:
   reliability_score: 5
   fn: conventional_power_plants_DE.csv
-  url: https://data.open-power-system-data.org/conventional_power_plants/2020-10-01/conventional_power_plants_DE.csv
+  url: https://raw.githubusercontent.com/pypsa-meets-earth/ppm-data-backup/main/conventional_power_plants_DE.csv
 OPSD_EU:
   reliability_score: 5
   fn: conventional_power_plants_EU.csv
-  url: https://data.open-power-system-data.org/conventional_power_plants/2020-10-01/conventional_power_plants_EU.csv
+  url: https://raw.githubusercontent.com/pypsa-meets-earth/ppm-data-backup/main/conventional_power_plants_EU.csv
 OPSD_VRE:
   url: https://data.open-power-system-data.org/renewable_power_plants/2020-08-25/renewable_power_plants_EU.csv
   fn: renewable_power_plants_EU.csv
 OPSD_VRE_DE:
   url: https://data.open-power-system-data.org/renewable_power_plants/2020-08-25/renewable_power_plants_DE.csv
   fn: renewable_power_plants_DE.csv
 OPSD_VRE_FR:
@@ -146,17 +162,52 @@
 WEPP:
   net_capacity: false
   reliability_score: 4
   fn: platts_wepp.csv
 GGPT:
   net_capacity: false
   reliability_score: 4
-  fn: Global-Gas-Plant-Tracker-Aug-2022.xlsx
-  url: https://github.com/pz-max/gem-powerplant-data/raw/main/Global-Gas-Plant-Tracker-Aug-2022.xlsx
+  fn: Global-Gas-Plant-Tracker-GGPT-February-2023-v2.csv
+  url: https://raw.githubusercontent.com/pz-max/gem-powerplant-data/main/Global-Gas-Plant-Tracker-GGPT-February-2023-v2.csv
+GCPT:
+  net_capacity: false
+  reliability_score: 5
+  fn: Global-Coal-Plant-Tracker-January-2023.csv
+  url: https://raw.githubusercontent.com/pz-max/gem-powerplant-data/main/Global-Coal-Plant-Tracker-January-2023.csv
+GGTPT:
+  net_capacity: false
+  reliability_score: 4
+  fn: Global-Geothermal-Power-Tracker-January-2023.csv
+  url: https://raw.githubusercontent.com/pz-max/gem-powerplant-data/main/Global-Geothermal-Power-Tracker-January-2023.csv
+GWPT:
+  net_capacity: false
+  reliability_score: 4
+  fn: Global-Wind-Power-Tracker-January-2023.csv
+  url: https://raw.githubusercontent.com/pz-max/gem-powerplant-data/main/Global-Wind-Power-Tracker-January-2023.csv
+GSPT:
+  net_capacity: false
+  reliability_score: 4
+  fn: Global-Solar-Power-Tracker-January-2023.csv
+  url: https://raw.githubusercontent.com/pz-max/gem-powerplant-data/main/Global-Solar-Power-Tracker-January-2023.csv
+GBPT:
+  net_capacity: false
+  reliability_score: 4
+  fn: Global-Bioenergy-Power-Tracker-January-2023.csv
+  url: https://raw.githubusercontent.com/pz-max/gem-powerplant-data/main/Global-Bioenergy-Power-Tracker-January-2023.csv
+GNPT:
+  net_capacity: false
+  reliability_score: 4
+  fn: Global-Nuclear-Power-Tracker-January-2023.csv
+  url: https://raw.githubusercontent.com/pz-max/gem-powerplant-data/main/Global-Nuclear-Power-Tracker-January-2023.csv
 
+GHPT:
+  net_capacity: false
+  reliability_score: 4
+  fn: Global-Hydropower-Tracker-May-2023.csv
+  url: https://raw.githubusercontent.com/pz-max/gem-powerplant-data/main/Global-Hydropower-Tracker-May-2023.csv
 # ---------------------------------------------------------------------------- #
 #                             Data Structure Config                            #
 # ---------------------------------------------------------------------------- #
 
 display_net_caps: true
 target_columns:
   - Name
```

### Comparing `powerplantmatching-0.5.6/powerplantmatching/package_data/country_codes.csv` & `powerplantmatching-0.5.7/powerplantmatching/package_data/country_codes.csv`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/package_data/duke_binaries/duke-core-1.3-SNAPSHOT-tests.jar` & `powerplantmatching-0.5.7/powerplantmatching/package_data/duke_binaries/duke-core-1.3-SNAPSHOT-tests.jar`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/package_data/duke_binaries/duke-core-1.3-SNAPSHOT.jar` & `powerplantmatching-0.5.7/powerplantmatching/package_data/duke_binaries/duke-core-1.3-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/package_data/duke_binaries/duke-es-1.3-SNAPSHOT.jar` & `powerplantmatching-0.5.7/powerplantmatching/package_data/duke_binaries/duke-es-1.3-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/package_data/duke_binaries/duke-json-1.3-SNAPSHOT.jar` & `powerplantmatching-0.5.7/powerplantmatching/package_data/duke_binaries/duke-json-1.3-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/package_data/duke_binaries/duke-lucene-1.3-SNAPSHOT.jar` & `powerplantmatching-0.5.7/powerplantmatching/package_data/duke_binaries/duke-lucene-1.3-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/package_data/duke_binaries/duke-mapdb-1.3-SNAPSHOT.jar` & `powerplantmatching-0.5.7/powerplantmatching/package_data/duke_binaries/duke-mapdb-1.3-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/package_data/duke_binaries/duke-mongodb-1.3-SNAPSHOT.jar` & `powerplantmatching-0.5.7/powerplantmatching/package_data/duke_binaries/duke-mongodb-1.3-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/package_data/duke_binaries/duke-server-1.3-SNAPSHOT.jar` & `powerplantmatching-0.5.7/powerplantmatching/package_data/duke_binaries/duke-server-1.3-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/package_data/manual_corrections.csv` & `powerplantmatching-0.5.7/powerplantmatching/package_data/manual_corrections.csv`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/package_data/manual_corrections_old.csv` & `powerplantmatching-0.5.7/powerplantmatching/package_data/manual_corrections_old.csv`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/package_data/parsed_locations.csv` & `powerplantmatching-0.5.7/powerplantmatching/package_data/parsed_locations.csv`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/plot.py` & `powerplantmatching-0.5.7/powerplantmatching/plot.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching/utils.py` & `powerplantmatching-0.5.7/powerplantmatching/utils.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/powerplantmatching.egg-info/PKG-INFO` & `powerplantmatching-0.5.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerplantmatching
-Version: 0.5.6
+Version: 0.5.7
 Summary: Toolset for generating and managing Power Plant Data
 Home-page: https://github.com/FRESNA/powerplantmatching
 Author: Fabian Hofmann (FIAS), Jonas Hoersch (KIT), Fabian Gotzens (FZ Jülich)
 Author-email: hofmann@fias.uni-frankfurt.de
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
@@ -16,14 +16,15 @@
 Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 # powerplantmatching
 
  [![pypi](https://img.shields.io/pypi/v/powerplantmatching.svg)](https://pypi.org/project/powerplantmatching/) [![conda](https://img.shields.io/conda/vn/conda-forge/powerplantmatching.svg)](https://anaconda.org/conda-forge/powerplantmatching) ![pythonversion](https://img.shields.io/pypi/pyversions/powerplantmatching) ![LICENSE](https://img.shields.io/pypi/l/powerplantmatching.svg) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3358985.svg)](https://zenodo.org/record/3358985#.XUReFPxS_MU) [![doc](https://readthedocs.org/projects/powerplantmatching/badge/?version=latest)](https://powerplantmatching.readthedocs.io/en/latest/) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/FRESNA/powerplantmatching/master.svg)](https://results.pre-commit.ci/latest/github/FRESNA/powerplantmatching/master)
+[![Stack Exchange questions](https://img.shields.io/stackexchange/stackoverflow/t/pypsa)](https://stackoverflow.com/questions/tagged/pypsa)
 
 A toolset for cleaning, standardizing and combining multiple power
 plant databases.
 
 This package provides ready-to-use power plant data for the European power system.
 Starting from openly available power plant datasets, the package cleans, standardizes
 and merges the input data to create a new combined dataset, which includes all the important information.
@@ -60,14 +61,22 @@
 
 or conda
 
 ```bash
 conda install -c conda-forge powerplantmatching
 ```
 
+# Contributing and Support
+We strongly welcome anyone interested in contributing to this project. If you have any ideas, suggestions or encounter problems, feel invited to file issues or make pull requests on GitHub.
+-   In case of code-related **questions**, please post on [stack overflow](https://stackoverflow.com/questions/tagged/pypsa).
+-   For non-programming related and more general questions please refer to the [PyPSA mailing list](https://groups.google.com/group/pypsa).
+-   To **discuss** with other PyPSA & technology-data users, organise projects, share news, and get in touch with the community you can use the [discord server](https://discord.gg/JTdvaEBb).
+-   For **bugs and feature requests**, please use the [powerplantmatching Github Issues page](https://github.com/PyPSA/powerplantmatching/issues).
+
+
 ## Citing powerplantmatching
 
 If you want to cite powerplantmatching, use the following paper
 
 - F. Gotzens, H. Heinrichs, J. Hörsch, and F. Hofmann, [Performing energy modelling exercises in a transparent way - The issue of data quality in power plant databases](https://www.sciencedirect.com/science/article/pii/S2211467X18301056?dgcid=author), Energy Strategy Reviews, vol. 23, pp. 1–12, Jan. 2019.
 
 with bibtex
```

### Comparing `powerplantmatching-0.5.6/powerplantmatching.egg-info/SOURCES.txt` & `powerplantmatching-0.5.7/powerplantmatching.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,8 +36,9 @@
 powerplantmatching/package_data/duke_binaries/duke-json-1.3-SNAPSHOT.jar
 powerplantmatching/package_data/duke_binaries/duke-lucene-1.3-SNAPSHOT.jar
 powerplantmatching/package_data/duke_binaries/duke-mapdb-1.3-SNAPSHOT.jar
 powerplantmatching/package_data/duke_binaries/duke-mongodb-1.3-SNAPSHOT.jar
 powerplantmatching/package_data/duke_binaries/duke-server-1.3-SNAPSHOT.jar
 test/test_aggregate.py
 test/test_cleaning.py
-test/test_data.py
+test/test_data.py
+test/test_duke.py
```

### Comparing `powerplantmatching-0.5.6/setup.py` & `powerplantmatching-0.5.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="powerplantmatching",
-    version="0.5.6",
+    version="0.5.7",
     author="Fabian Hofmann (FIAS), Jonas Hoersch (KIT), Fabian Gotzens (FZ Jülich)",
     author_email="hofmann@fias.uni-frankfurt.de",
     description="Toolset for generating and managing Power Plant Data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FRESNA/powerplantmatching",
     license="GPLv3",
```

### Comparing `powerplantmatching-0.5.6/test/test_aggregate.py` & `powerplantmatching-0.5.7/test/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/test/test_cleaning.py` & `powerplantmatching-0.5.7/test/test_cleaning.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.6/test/test_data.py` & `powerplantmatching-0.5.7/test/test_data.py`

 * *Files identical despite different names*

