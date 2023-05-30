# Comparing `tmp/hdx-data-freshness-dbclean-1.0.1.tar.gz` & `tmp/hdx-data-freshness-dbclean-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdx-data-freshness-dbclean-1.0.1.tar", last modified: Mon May  1 23:06:24 2023, max compression
+gzip compressed data, was "hdx-data-freshness-dbclean-1.0.2.tar", last modified: Tue May 30 00:34:51 2023, max compression
```

## Comparing `hdx-data-freshness-dbclean-1.0.1.tar` & `hdx-data-freshness-dbclean-1.0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:06:24.556861 hdx-data-freshness-dbclean-1.0.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)      188 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/.coveragerc
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:06:24.548861 hdx-data-freshness-dbclean-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:06:24.552861 hdx-data-freshness-dbclean-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/.github/workflows/run-python-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      174 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-01 23:06:24.556861 hdx-data-freshness-dbclean-1.0.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1678 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1397 2023-05-01 23:06:24.556861 hdx-data-freshness-dbclean-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:06:24.548861 hdx-data-freshness-dbclean-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:06:24.548861 hdx-data-freshness-dbclean-1.0.1/src/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:06:24.548861 hdx-data-freshness-dbclean-1.0.1/src/hdx/freshness/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:06:24.552861 hdx-data-freshness-dbclean-1.0.1/src/hdx/freshness/dbactions/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/src/hdx/freshness/dbactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/src/hdx/freshness/dbactions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 23:06:24.000000 hdx-data-freshness-dbclean-1.0.1/src/hdx/freshness/dbactions/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/src/hdx/freshness/dbactions/dbclean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/src/hdx/freshness/dbactions/dbclone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:06:24.552861 hdx-data-freshness-dbclean-1.0.1/src/hdx_data_freshness_dbclean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-01 23:06:24.000000 hdx-data-freshness-dbclean-1.0.1/src/hdx_data_freshness_dbclean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-01 23:06:24.000000 hdx-data-freshness-dbclean-1.0.1/src/hdx_data_freshness_dbclean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 23:06:24.000000 hdx-data-freshness-dbclean-1.0.1/src/hdx_data_freshness_dbclean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-01 23:06:24.000000 hdx-data-freshness-dbclean-1.0.1/src/hdx_data_freshness_dbclean.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-01 23:06:24.000000 hdx-data-freshness-dbclean-1.0.1/src/hdx_data_freshness_dbclean.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 23:06:23.000000 hdx-data-freshness-dbclean-1.0.1/src/hdx_data_freshness_dbclean.egg-info/zip-safe
--rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:06:24.548861 hdx-data-freshness-dbclean-1.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:06:24.556861 hdx-data-freshness-dbclean-1.0.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)    81799 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/tests/fixtures/runs.csv
--rw-r--r--   0 runner    (1001) docker     (123)    35828 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/tests/fixtures/runs2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    35789 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/tests/fixtures/runs3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    35789 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/tests/fixtures/runs4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    35710 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/tests/fixtures/runs5.csv
--rw-r--r--   0 runner    (1001) docker     (123)    81799 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/tests/fixtures/runs_broken1351.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1794048 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/tests/fixtures/test_freshness.db
--rw-r--r--   0 runner    (1001) docker     (123)  1794048 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/tests/fixtures/test_freshness_brokenrun1351.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:06:24.548861 hdx-data-freshness-dbclean-1.0.1/tests/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:06:24.548861 hdx-data-freshness-dbclean-1.0.1/tests/hdx/freshness/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:06:24.556861 hdx-data-freshness-dbclean-1.0.1/tests/hdx/freshness/dbactions/
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-01 23:06:08.000000 hdx-data-freshness-dbclean-1.0.1/tests/hdx/freshness/dbactions/test_dbactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:34:51.521256 hdx-data-freshness-dbclean-1.0.2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      188 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/.coveragerc
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:34:51.513256 hdx-data-freshness-dbclean-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:34:51.513256 hdx-data-freshness-dbclean-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/.github/workflows/run-python-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      174 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-30 00:34:51.521256 hdx-data-freshness-dbclean-1.0.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1754 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1397 2023-05-30 00:34:51.521256 hdx-data-freshness-dbclean-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:34:51.513256 hdx-data-freshness-dbclean-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:34:51.513256 hdx-data-freshness-dbclean-1.0.2/src/hdx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:34:51.513256 hdx-data-freshness-dbclean-1.0.2/src/hdx/freshness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:34:51.513256 hdx-data-freshness-dbclean-1.0.2/src/hdx/freshness/dbactions/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/src/hdx/freshness/dbactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/src/hdx/freshness/dbactions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 00:34:51.000000 hdx-data-freshness-dbclean-1.0.2/src/hdx/freshness/dbactions/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/src/hdx/freshness/dbactions/dbclean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/src/hdx/freshness/dbactions/dbclone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:34:51.517256 hdx-data-freshness-dbclean-1.0.2/src/hdx_data_freshness_dbclean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-30 00:34:51.000000 hdx-data-freshness-dbclean-1.0.2/src/hdx_data_freshness_dbclean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-30 00:34:51.000000 hdx-data-freshness-dbclean-1.0.2/src/hdx_data_freshness_dbclean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:34:51.000000 hdx-data-freshness-dbclean-1.0.2/src/hdx_data_freshness_dbclean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-30 00:34:51.000000 hdx-data-freshness-dbclean-1.0.2/src/hdx_data_freshness_dbclean.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-30 00:34:51.000000 hdx-data-freshness-dbclean-1.0.2/src/hdx_data_freshness_dbclean.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:34:50.000000 hdx-data-freshness-dbclean-1.0.2/src/hdx_data_freshness_dbclean.egg-info/zip-safe
+-rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:34:51.513256 hdx-data-freshness-dbclean-1.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:34:51.521256 hdx-data-freshness-dbclean-1.0.2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)    81799 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/tests/fixtures/runs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    35828 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/tests/fixtures/runs2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    35789 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/tests/fixtures/runs3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    35789 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/tests/fixtures/runs4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    35710 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/tests/fixtures/runs5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    81799 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/tests/fixtures/runs_broken1351.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1794048 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/tests/fixtures/test_freshness.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1794048 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/tests/fixtures/test_freshness_brokenrun1351.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:34:51.513256 hdx-data-freshness-dbclean-1.0.2/tests/hdx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:34:51.513256 hdx-data-freshness-dbclean-1.0.2/tests/hdx/freshness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:34:51.521256 hdx-data-freshness-dbclean-1.0.2/tests/hdx/freshness/dbactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-30 00:34:26.000000 hdx-data-freshness-dbclean-1.0.2/tests/hdx/freshness/dbactions/test_dbactions.py
```

### Comparing `hdx-data-freshness-dbclean-1.0.1/.dockerignore` & `hdx-data-freshness-dbclean-1.0.2/.dockerignore`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/.github/workflows/build.yml` & `hdx-data-freshness-dbclean-1.0.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/.github/workflows/publish.yml` & `hdx-data-freshness-dbclean-1.0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/.github/workflows/run-python-tests.yml` & `hdx-data-freshness-dbclean-1.0.2/.github/workflows/run-python-tests.yml`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/.gitignore` & `hdx-data-freshness-dbclean-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/LICENSE` & `hdx-data-freshness-dbclean-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/PKG-INFO` & `hdx-data-freshness-dbclean-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-data-freshness-dbclean
-Version: 1.0.1
+Version: 1.0.2
 Summary: HDX Data Freshness Database Clean
 Home-page: https://github.com/OCHA-DAP/hdx-data-freshness-dbclean
 Author: Michael Rans
 Author-email: rans@email.com
 License: MIT
 Keywords: HDX,fresh,freshness,database
 Platform: any
@@ -31,14 +31,15 @@
 
 ### Utility to clean Freshness Database
 [![Build Status](https://github.com/OCHA-DAP/hdx-data-freshness-dbclean/actions/workflows/run-python-tests.yml/badge.svg)](https://github.com/OCHA-DAP/hdx-data-freshness-dbclean/actions/workflows/run-python-tests.yml)
 [![Coverage Status](https://codecov.io/gh/OCHA-DAP/hdx-data-freshness-dbclean/branch/main/graph/badge.svg?token=JpWZc5js4y)](https://codecov.io/gh/OCHA-DAP/hdx-data-freshness-dbclean)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
+# DEPRECATED - code moved to https://github.com/OCHA-DAP/hdx-data-freshness
 
 This script cleans the freshness database.
 
 
 ### Usage
 
     python -m hdx.freshness.dbactions [-db/--db_uri=] [-dp/--db_params=] [action]
```

### Comparing `hdx-data-freshness-dbclean-1.0.1/README.md` & `hdx-data-freshness-dbclean-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ### Utility to clean Freshness Database
 [![Build Status](https://github.com/OCHA-DAP/hdx-data-freshness-dbclean/actions/workflows/run-python-tests.yml/badge.svg)](https://github.com/OCHA-DAP/hdx-data-freshness-dbclean/actions/workflows/run-python-tests.yml)
 [![Coverage Status](https://codecov.io/gh/OCHA-DAP/hdx-data-freshness-dbclean/branch/main/graph/badge.svg?token=JpWZc5js4y)](https://codecov.io/gh/OCHA-DAP/hdx-data-freshness-dbclean)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
+# DEPRECATED - code moved to https://github.com/OCHA-DAP/hdx-data-freshness
 
 This script cleans the freshness database.
 
 
 ### Usage
 
     python -m hdx.freshness.dbactions [-db/--db_uri=] [-dp/--db_params=] [action]
```

### Comparing `hdx-data-freshness-dbclean-1.0.1/pyproject.toml` & `hdx-data-freshness-dbclean-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/setup.cfg` & `hdx-data-freshness-dbclean-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/src/hdx/freshness/dbactions/__main__.py` & `hdx-data-freshness-dbclean-1.0.2/src/hdx/freshness/dbactions/__main__.py`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/src/hdx/freshness/dbactions/dbclean.py` & `hdx-data-freshness-dbclean-1.0.2/src/hdx/freshness/dbactions/dbclean.py`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/src/hdx/freshness/dbactions/dbclone.py` & `hdx-data-freshness-dbclean-1.0.2/src/hdx/freshness/dbactions/dbclone.py`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/src/hdx_data_freshness_dbclean.egg-info/PKG-INFO` & `hdx-data-freshness-dbclean-1.0.2/src/hdx_data_freshness_dbclean.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-data-freshness-dbclean
-Version: 1.0.1
+Version: 1.0.2
 Summary: HDX Data Freshness Database Clean
 Home-page: https://github.com/OCHA-DAP/hdx-data-freshness-dbclean
 Author: Michael Rans
 Author-email: rans@email.com
 License: MIT
 Keywords: HDX,fresh,freshness,database
 Platform: any
@@ -31,14 +31,15 @@
 
 ### Utility to clean Freshness Database
 [![Build Status](https://github.com/OCHA-DAP/hdx-data-freshness-dbclean/actions/workflows/run-python-tests.yml/badge.svg)](https://github.com/OCHA-DAP/hdx-data-freshness-dbclean/actions/workflows/run-python-tests.yml)
 [![Coverage Status](https://codecov.io/gh/OCHA-DAP/hdx-data-freshness-dbclean/branch/main/graph/badge.svg?token=JpWZc5js4y)](https://codecov.io/gh/OCHA-DAP/hdx-data-freshness-dbclean)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
+# DEPRECATED - code moved to https://github.com/OCHA-DAP/hdx-data-freshness
 
 This script cleans the freshness database.
 
 
 ### Usage
 
     python -m hdx.freshness.dbactions [-db/--db_uri=] [-dp/--db_params=] [action]
```

### Comparing `hdx-data-freshness-dbclean-1.0.1/src/hdx_data_freshness_dbclean.egg-info/SOURCES.txt` & `hdx-data-freshness-dbclean-1.0.2/src/hdx_data_freshness_dbclean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/tests/fixtures/runs.csv` & `hdx-data-freshness-dbclean-1.0.2/tests/fixtures/runs.csv`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/tests/fixtures/runs2.csv` & `hdx-data-freshness-dbclean-1.0.2/tests/fixtures/runs2.csv`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/tests/fixtures/runs3.csv` & `hdx-data-freshness-dbclean-1.0.2/tests/fixtures/runs3.csv`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/tests/fixtures/runs4.csv` & `hdx-data-freshness-dbclean-1.0.2/tests/fixtures/runs4.csv`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/tests/fixtures/runs5.csv` & `hdx-data-freshness-dbclean-1.0.2/tests/fixtures/runs5.csv`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/tests/fixtures/runs_broken1351.csv` & `hdx-data-freshness-dbclean-1.0.2/tests/fixtures/runs_broken1351.csv`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/tests/fixtures/test_freshness.db` & `hdx-data-freshness-dbclean-1.0.2/tests/fixtures/test_freshness.db`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/tests/fixtures/test_freshness_brokenrun1351.db` & `hdx-data-freshness-dbclean-1.0.2/tests/fixtures/test_freshness_brokenrun1351.db`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-dbclean-1.0.1/tests/hdx/freshness/dbactions/test_dbactions.py` & `hdx-data-freshness-dbclean-1.0.2/tests/hdx/freshness/dbactions/test_dbactions.py`

 * *Files identical despite different names*

