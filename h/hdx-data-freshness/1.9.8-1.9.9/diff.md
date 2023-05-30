# Comparing `tmp/hdx-data-freshness-1.9.8.tar.gz` & `tmp/hdx-data-freshness-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdx-data-freshness-1.9.8.tar", last modified: Mon Mar  6 01:43:02 2023, max compression
+gzip compressed data, was "hdx-data-freshness-1.9.9.tar", last modified: Mon Mar  6 02:52:46 2023, max compression
```

## Comparing `hdx-data-freshness-1.9.8.tar` & `hdx-data-freshness-1.9.9.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.831433 hdx-data-freshness-1.9.8/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.815433 hdx-data-freshness-1.9.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.819433 hdx-data-freshness-1.9.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/.github/workflows/run-python-tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/.readthedocs.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      428 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-03-06 01:43:02.831433 hdx-data-freshness-1.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.819433 hdx-data-freshness-1.9.8/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/doc/main.md
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      118 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1467 2023-03-06 01:43:02.831433 hdx-data-freshness-1.9.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.819433 hdx-data-freshness-1.9.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.819433 hdx-data-freshness-1.9.8/src/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.819433 hdx-data-freshness-1.9.8/src/hdx/freshness/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.819433 hdx-data-freshness-1.9.8/src/hdx/freshness/app/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/app/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5392 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-06 01:43:02.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/app/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    46015 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/app/datafreshness.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/app/project_configuration.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.823433 hdx-data-freshness-1.9.8/src/hdx/freshness/database/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/database/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3329 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/database/dbdataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1552 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/database/dbinfodataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/database/dborganization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3360 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/database/dbresource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      690 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/database/dbrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.823433 hdx-data-freshness-1.9.8/src/hdx/freshness/testdata/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/testdata/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2770 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/testdata/dbtestdataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      599 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/testdata/dbtestdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1633 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/testdata/dbtesthashresult.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1731 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/testdata/dbtestresource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1616 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/testdata/dbtestresult.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8492 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/testdata/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.823433 hdx-data-freshness-1.9.8/src/hdx/freshness/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2201 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/utils/ratelimiter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10387 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/utils/retrieval.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4644 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/src/hdx/freshness/utils/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.823433 hdx-data-freshness-1.9.8/src/hdx_data_freshness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-03-06 01:43:02.000000 hdx-data-freshness-1.9.8/src/hdx_data_freshness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-03-06 01:43:02.000000 hdx-data-freshness-1.9.8/src/hdx_data_freshness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 01:43:02.000000 hdx-data-freshness-1.9.8/src/hdx_data_freshness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-06 01:43:02.000000 hdx-data-freshness-1.9.8/src/hdx_data_freshness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-06 01:43:02.000000 hdx-data-freshness-1.9.8/src/hdx_data_freshness.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 01:43:01.000000 hdx-data-freshness-1.9.8/src/hdx_data_freshness.egg-info/zip-safe
--rwxr-xr-x   0 runner    (1001) docker     (123)       78 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.819433 hdx-data-freshness-1.9.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.823433 hdx-data-freshness-1.9.8/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.823433 hdx-data-freshness-1.9.8/tests/fixtures/CKAN/
--rwxr-xr-x   0 runner    (1001) docker     (123)      222 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/fixtures/CKAN/hdx_dataset_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)   127901 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/fixtures/datasets.pickle
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.823433 hdx-data-freshness-1.9.8/tests/fixtures/day0/
--rw-r--r--   0 runner    (1001) docker     (123)   446464 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/fixtures/day0/test_freshness.db
--rwxr-xr-x   0 runner    (1001) docker     (123)   664576 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/fixtures/day0/test_serialize.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.827433 hdx-data-freshness-1.9.8/tests/fixtures/dayN/
--rwxr-xr-x   0 runner    (1001) docker     (123)  1306624 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/fixtures/dayN/test_freshness.db
--rwxr-xr-x   0 runner    (1001) docker     (123)   657408 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/fixtures/dayN/test_serialize.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.831433 hdx-data-freshness-1.9.8/tests/fixtures/retrieve/
--rwxr-xr-x   0 runner    (1001) docker     (123)    20984 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/fixtures/retrieve/ACLED-Country-Coverage-and-ISO-Codes_8.2019.xlsx
--rwxr-xr-x   0 runner    (1001) docker     (123)   596487 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/fixtures/retrieve/COD_MOZ_Admin0.geojson
--rwxr-xr-x   0 runner    (1001) docker     (123)    26084 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/fixtures/retrieve/Dataset.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)     8461 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/fixtures/retrieve/hotosm_nic_airports_lines_shp.zip
--rwxr-xr-x   0 runner    (1001) docker     (123)  1829841 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/fixtures/retrieve/hrp_adm1_4pc.geojson
--rwxr-xr-x   0 runner    (1001) docker     (123)    81920 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/fixtures/retrieve/list_one.xls
--rwxr-xr-x   0 runner    (1001) docker     (123)     2016 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/fixtures/retrieve/response.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.819433 hdx-data-freshness-1.9.8/tests/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.831433 hdx-data-freshness-1.9.8/tests/hdx/freshness/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.831433 hdx-data-freshness-1.9.8/tests/hdx/freshness/app/
--rwxr-xr-x   0 runner    (1001) docker     (123)    15183 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/hdx/freshness/app/test_freshness_CKAN.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2473 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/hdx/freshness/app/test_freshness_by_frequency.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12865 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/hdx/freshness/app/test_freshness_day0.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16117 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/hdx/freshness/app/test_freshness_dayN.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14664 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/hdx/freshness/app/test_process_results.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1331 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/hdx/freshness/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.831433 hdx-data-freshness-1.9.8/tests/hdx/freshness/testdata/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6957 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/hdx/freshness/testdata/test_serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:02.831433 hdx-data-freshness-1.9.8/tests/hdx/freshness/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4084 2023-03-06 01:42:38.000000 hdx-data-freshness-1.9.8/tests/hdx/freshness/utils/test_retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.574087 hdx-data-freshness-1.9.9/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.558087 hdx-data-freshness-1.9.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.562087 hdx-data-freshness-1.9.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/.github/workflows/run-python-tests.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/.readthedocs.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      428 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-03-06 02:52:46.574087 hdx-data-freshness-1.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.562087 hdx-data-freshness-1.9.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/doc/main.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      118 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1467 2023-03-06 02:52:46.574087 hdx-data-freshness-1.9.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.558087 hdx-data-freshness-1.9.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.558087 hdx-data-freshness-1.9.9/src/hdx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.558087 hdx-data-freshness-1.9.9/src/hdx/freshness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.562087 hdx-data-freshness-1.9.9/src/hdx/freshness/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/app/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5392 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-06 02:52:46.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/app/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    46015 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/app/datafreshness.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/app/project_configuration.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.562087 hdx-data-freshness-1.9.9/src/hdx/freshness/database/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/database/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3499 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/database/dbdataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1613 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/database/dbinfodataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/database/dborganization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3541 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/database/dbresource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      722 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/database/dbrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.562087 hdx-data-freshness-1.9.9/src/hdx/freshness/testdata/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/testdata/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2983 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/testdata/dbtestdataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      599 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/testdata/dbtestdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1757 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/testdata/dbtesthashresult.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1731 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/testdata/dbtestresource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1740 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/testdata/dbtestresult.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8492 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/testdata/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.566087 hdx-data-freshness-1.9.9/src/hdx/freshness/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2201 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/utils/ratelimiter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10387 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/utils/retrieval.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4644 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/src/hdx/freshness/utils/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.566087 hdx-data-freshness-1.9.9/src/hdx_data_freshness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-03-06 02:52:46.000000 hdx-data-freshness-1.9.9/src/hdx_data_freshness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-03-06 02:52:46.000000 hdx-data-freshness-1.9.9/src/hdx_data_freshness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 02:52:46.000000 hdx-data-freshness-1.9.9/src/hdx_data_freshness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-06 02:52:46.000000 hdx-data-freshness-1.9.9/src/hdx_data_freshness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-06 02:52:46.000000 hdx-data-freshness-1.9.9/src/hdx_data_freshness.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 02:52:45.000000 hdx-data-freshness-1.9.9/src/hdx_data_freshness.egg-info/zip-safe
+-rwxr-xr-x   0 runner    (1001) docker     (123)       78 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.558087 hdx-data-freshness-1.9.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.566087 hdx-data-freshness-1.9.9/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.566087 hdx-data-freshness-1.9.9/tests/fixtures/CKAN/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      222 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/fixtures/CKAN/hdx_dataset_static.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)   127901 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/fixtures/datasets.pickle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.566087 hdx-data-freshness-1.9.9/tests/fixtures/day0/
+-rw-r--r--   0 runner    (1001) docker     (123)   446464 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/fixtures/day0/test_freshness.db
+-rwxr-xr-x   0 runner    (1001) docker     (123)   664576 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/fixtures/day0/test_serialize.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.570087 hdx-data-freshness-1.9.9/tests/fixtures/dayN/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1306624 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/fixtures/dayN/test_freshness.db
+-rwxr-xr-x   0 runner    (1001) docker     (123)   657408 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/fixtures/dayN/test_serialize.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.574087 hdx-data-freshness-1.9.9/tests/fixtures/retrieve/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20984 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/fixtures/retrieve/ACLED-Country-Coverage-and-ISO-Codes_8.2019.xlsx
+-rwxr-xr-x   0 runner    (1001) docker     (123)   596487 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/fixtures/retrieve/COD_MOZ_Admin0.geojson
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26084 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/fixtures/retrieve/Dataset.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8461 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/fixtures/retrieve/hotosm_nic_airports_lines_shp.zip
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1829841 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/fixtures/retrieve/hrp_adm1_4pc.geojson
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81920 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/fixtures/retrieve/list_one.xls
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2016 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/fixtures/retrieve/response.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.558087 hdx-data-freshness-1.9.9/tests/hdx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.574087 hdx-data-freshness-1.9.9/tests/hdx/freshness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.574087 hdx-data-freshness-1.9.9/tests/hdx/freshness/app/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15183 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/hdx/freshness/app/test_freshness_CKAN.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2473 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/hdx/freshness/app/test_freshness_by_frequency.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12865 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/hdx/freshness/app/test_freshness_day0.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16117 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/hdx/freshness/app/test_freshness_dayN.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14664 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/hdx/freshness/app/test_process_results.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1331 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/hdx/freshness/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.574087 hdx-data-freshness-1.9.9/tests/hdx/freshness/testdata/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6957 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/hdx/freshness/testdata/test_serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:52:46.574087 hdx-data-freshness-1.9.9/tests/hdx/freshness/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4084 2023-03-06 02:52:21.000000 hdx-data-freshness-1.9.9/tests/hdx/freshness/utils/test_retrieval.py
```

### Comparing `hdx-data-freshness-1.9.8/.dockerignore` & `hdx-data-freshness-1.9.9/.dockerignore`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/.github/workflows/build.yml` & `hdx-data-freshness-1.9.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/.github/workflows/publish.yml` & `hdx-data-freshness-1.9.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/.github/workflows/run-python-tests.yml` & `hdx-data-freshness-1.9.9/.github/workflows/run-python-tests.yml`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/.gitignore` & `hdx-data-freshness-1.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/LICENSE` & `hdx-data-freshness-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/PKG-INFO` & `hdx-data-freshness-1.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-data-freshness
-Version: 1.9.8
+Version: 1.9.9
 Summary: HDX Data Freshness analyses freshness of data on HDX
 Home-page: https://github.com/OCHA-DAP/hdx-data-freshness
 Author: Michael Rans
 Author-email: rans@email.com
 License: MIT
 Keywords: HDX,fresh,freshness,data freshness
 Platform: any
```

### Comparing `hdx-data-freshness-1.9.8/README.md` & `hdx-data-freshness-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/doc/main.md` & `hdx-data-freshness-1.9.9/doc/main.md`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/pyproject.toml` & `hdx-data-freshness-1.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/setup.cfg` & `hdx-data-freshness-1.9.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/src/hdx/freshness/app/__main__.py` & `hdx-data-freshness-1.9.9/src/hdx/freshness/app/__main__.py`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/src/hdx/freshness/app/datafreshness.py` & `hdx-data-freshness-1.9.9/src/hdx/freshness/app/datafreshness.py`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/src/hdx/freshness/database/dbdataset.py` & `hdx-data-freshness-1.9.9/src/hdx/freshness/database/dbdataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,44 +9,35 @@
 
 
 class DBDataset(Base):
     """
     run_number: Mapped[int] = mapped_column(
         ForeignKey("dbruns.run_number"), primary_key=True
     )
-
     id: Mapped[str] = mapped_column(
         ForeignKey("dbinfodatasets.id"), primary_key=True
     )
-
-    dataset_date: Mapped[str]
-
-    update_frequency: Mapped[int]
-
-    review_date: Mapped[datetime]
-
+    dataset_date: Mapped[str] = mapped_column(nullable=True)
+    update_frequency: Mapped[int] = mapped_column(nullable=True)
+    review_date: Mapped[datetime] = mapped_column(nullable=True)
     last_modified: Mapped[datetime] = mapped_column(nullable=False)
-
-    updated_by_script: Mapped[datetime]
-
-    metadata_modified: Mapped[datetime] = mapped_column(nullable=False
+    updated_by_script: Mapped[datetime] = mapped_column(nullable=True)
+    metadata_modified: Mapped[datetime] = mapped_column(
+        nullable=False
     )  # this field and above are CKAN fields
 
     latest_of_modifieds: Mapped[datetime] = mapped_column(nullable=False)
-
     what_updated: Mapped[str] = mapped_column(nullable=False)
-
-    last_resource_updated: Mapped[str] = mapped_column(nullable=False
+    last_resource_updated: Mapped[str] = mapped_column(
+        nullable=False
     )  # id of last resource updated
-
-    last_resource_modified: Mapped[datetime] = mapped_column(nullable=False
+    last_resource_modified: Mapped[datetime] = mapped_column(
+        nullable=False
     )  # date last resource updated
-
-    fresh: Mapped[int]
-
+    fresh: Mapped[int] = mapped_column(nullable=True)
     error: Mapped[bool] = mapped_column(nullable=False)
     """
 
     run_number: Mapped[int] = mapped_column(
         ForeignKey("dbruns.run_number"), primary_key=True
     )
     id: Mapped[str] = mapped_column(
```

### Comparing `hdx-data-freshness-1.9.8/src/hdx/freshness/database/dbinfodataset.py` & `hdx-data-freshness-1.9.9/src/hdx/freshness/database/dbinfodataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,26 +10,26 @@
     id: Mapped[str] = mapped_column(primary_key=True)
     name: Mapped[str] = mapped_column(nullable=False)
     title: Mapped[str] = mapped_column(nullable=False)
     private: Mapped[bool] = mapped_column(nullable=False)
     organization_id: Mapped[str] = mapped_column(
         ForeignKey("dborganizations.id"), nullable=False
     )
-    location: Mapped[str]
-    maintainer: Mapped[str]
+    location: Mapped[str] = mapped_column(nullable=True)
+    maintainer: Mapped[str] = mapped_column(nullable=True)
     """
 
     id: Mapped[str] = mapped_column(primary_key=True)
     name: Mapped[str] = mapped_column(nullable=False)
     title: Mapped[str] = mapped_column(nullable=False)
     private: Mapped[bool] = mapped_column(nullable=False)
     organization_id: Mapped[str] = mapped_column(
         ForeignKey("dborganizations.id"), nullable=False
     )
-    location: Mapped[str] = mapped_column(nullable=False)
+    location: Mapped[str] = mapped_column(nullable=True)
     maintainer: Mapped[str] = mapped_column(nullable=True)
 
     def __repr__(self) -> str:
         """String representation of DBInfoDataset row
 
         Returns:
             str: String representation of DBInfoDataset row
```

### Comparing `hdx-data-freshness-1.9.8/src/hdx/freshness/database/dborganization.py` & `hdx-data-freshness-1.9.9/src/hdx/freshness/database/dborganization.py`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/src/hdx/freshness/database/dbresource.py` & `hdx-data-freshness-1.9.9/src/hdx/freshness/database/dbresource.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,38 +17,43 @@
     name: Mapped[str] = mapped_column(nullable=False)
     dataset_id: Mapped[str] = mapped_column(
         ForeignKey("dbinfodatasets.id"), nullable=False
     )
     url: Mapped[str] = mapped_column(nullable=False)
     last_modified: Mapped[datetime] = mapped_column(nullable=False)
     metadata_modified: Mapped[datetime] = mapped_column(
-        default=None
+        default=None, nullable=True
     )  # this field and above are CKAN fields
+
     latest_of_modifieds: Mapped[datetime] = mapped_column(nullable=False)
     what_updated: Mapped[str] = mapped_column(nullable=False)
-    http_last_modified: Mapped[datetime] = mapped_column(default=None)
-    md5_hash: Mapped[str] = mapped_column(default=None)
-    hash_last_modified: Mapped[datetime] = mapped_column(default=None)
-    when_checked: Mapped[datetime] = mapped_column(default=None)
-    api: Mapped[bool]
-    error: Mapped[str]
+    http_last_modified: Mapped[datetime] = mapped_column(
+        default=None, nullable=True
+    )
+    md5_hash: Mapped[str] = mapped_column(default=None, nullable=True)
+    hash_last_modified: Mapped[datetime] = mapped_column(
+        default=None, nullable=True
+    )
+    when_checked: Mapped[datetime] = mapped_column(default=None, nullable=True)
+    api: Mapped[bool] = mapped_column(nullable=True)
+    error: Mapped[str] = mapped_column(nullable=True)
     """
 
     run_number: Mapped[int] = mapped_column(
         ForeignKey("dbruns.run_number"), primary_key=True
     )
     id: Mapped[str] = mapped_column(primary_key=True)
     name: Mapped[str] = mapped_column(nullable=False)
     dataset_id: Mapped[str] = mapped_column(
         ForeignKey("dbinfodatasets.id"), nullable=False
     )
     url: Mapped[str] = mapped_column(nullable=False)
     last_modified: Mapped[datetime] = mapped_column(nullable=False)
     metadata_modified: Mapped[datetime] = mapped_column(
-        default=None
+        default=None, nullable=True
     )  # this field and above are CKAN fields
     latest_of_modifieds: Mapped[datetime] = mapped_column(nullable=False)
     what_updated: Mapped[str] = mapped_column(nullable=False)
     http_last_modified: Mapped[datetime] = mapped_column(
         default=None, nullable=True
     )
     md5_hash: Mapped[str] = mapped_column(default=None, nullable=True)
```

### Comparing `hdx-data-freshness-1.9.8/src/hdx/freshness/database/dbrun.py` & `hdx-data-freshness-1.9.9/src/hdx/freshness/database/dbrun.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from hdx.database.no_timezone import Base
 from sqlalchemy.orm import Mapped, mapped_column
 
 
 class DBRun(Base):
     """
     run_number: Mapped[int] = mapped_column(primary_key=True)
-    run_date: Mapped[datetime]
+    run_date: Mapped[datetime] = mapped_column(nullable=False)
     """
 
     run_number: Mapped[int] = mapped_column(primary_key=True)
     run_date: Mapped[datetime] = mapped_column(nullable=False)
 
     def __repr__(self) -> str:
         """String representation of DBRun row
```

### Comparing `hdx-data-freshness-1.9.8/src/hdx/freshness/testdata/dbtestdataset.py` & `hdx-data-freshness-1.9.9/src/hdx/freshness/testdata/dbtestdataset.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,41 +10,41 @@
     id: Mapped[str] = mapped_column(primary_key=True)
     organization_id: Mapped[str] = mapped_column(nullable=False)
     organization_name: Mapped[str] = mapped_column(nullable=False)
     organization_title: Mapped[str] = mapped_column(nullable=False)
     dataset_name: Mapped[str] = mapped_column(nullable=False)
     dataset_title: Mapped[str] = mapped_column(nullable=False)
     dataset_private: Mapped[bool] = mapped_column(nullable=False)
-    dataset_maintainer: Mapped[str]
-    dataset_date: Mapped[str]
-    update_frequency: Mapped[str]
-    review_date: Mapped[str]
+    dataset_maintainer: Mapped[str] = mapped_column(nullable=True)
+    dataset_date: Mapped[str] = mapped_column(nullable=True)
+    update_frequency: Mapped[str] = mapped_column(nullable=True)
+    review_date: Mapped[str] = mapped_column(nullable=True)
     last_modified: Mapped[str] = mapped_column(nullable=False)
-    updated_by_script: Mapped[str]
+    updated_by_script: Mapped[str] = mapped_column(nullable=True)
     metadata_modified: Mapped[str] = mapped_column(nullable=False)
-    is_requestdata_type: Mapped[bool]
-    dataset_location: Mapped[str]
+    is_requestdata_type: Mapped[bool] = mapped_column(nullable=True)
+    dataset_location: Mapped[str] = mapped_column(nullable=True)
     """
 
     id: Mapped[str] = mapped_column(primary_key=True)
     organization_id: Mapped[str] = mapped_column(nullable=False)
     organization_name: Mapped[str] = mapped_column(nullable=False)
     organization_title: Mapped[str] = mapped_column(nullable=False)
     dataset_name: Mapped[str] = mapped_column(nullable=False)
     dataset_title: Mapped[str] = mapped_column(nullable=False)
     dataset_private: Mapped[bool] = mapped_column(nullable=False)
-    dataset_maintainer: Mapped[str] = mapped_column(nullable=False)
-    dataset_date: Mapped[str] = mapped_column(nullable=False)
-    update_frequency: Mapped[str] = mapped_column(nullable=False)
+    dataset_maintainer: Mapped[str] = mapped_column(nullable=True)
+    dataset_date: Mapped[str] = mapped_column(nullable=True)
+    update_frequency: Mapped[str] = mapped_column(nullable=True)
     review_date: Mapped[str] = mapped_column(nullable=True)
     last_modified: Mapped[str] = mapped_column(nullable=False)
     updated_by_script: Mapped[str] = mapped_column(nullable=True)
     metadata_modified: Mapped[str] = mapped_column(nullable=False)
     is_requestdata_type: Mapped[bool] = mapped_column(nullable=True)
-    dataset_location: Mapped[str] = mapped_column(nullable=False)
+    dataset_location: Mapped[str] = mapped_column(nullable=True)
 
     def __repr__(self) -> str:
         """String representation of DBTestDataset row
 
         Returns:
             str: String representation of DBTestDataset row
         """
```

### Comparing `hdx-data-freshness-1.9.8/src/hdx/freshness/testdata/dbtestdate.py` & `hdx-data-freshness-1.9.9/src/hdx/freshness/testdata/dbtestdate.py`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/src/hdx/freshness/testdata/dbtesthashresult.py` & `hdx-data-freshness-1.9.9/src/hdx/freshness/testdata/dbtestresult.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """SQLAlchemy class representing DBTestResult row. Holds test data mimicking the result
-of downloading and hashing urls (second time).
+of downloading and hashing urls (first time).
 """
 from datetime import datetime
 
 from hdx.database.no_timezone import Base
 from sqlalchemy.orm import Mapped, mapped_column
 
 
-class DBTestHashResult(Base):
+class DBTestResult(Base):
     """
     id: Mapped[str] = mapped_column(primary_key=True)
     url: Mapped[str] = mapped_column(nullable=False)
     format: Mapped[str] = mapped_column(nullable=False)
-    err: Mapped[str]
-    http_last_modified: Mapped[datetime]
-    hash: Mapped[str]
-    xlsx_hash: Mapped[str]
+    err: Mapped[str] = mapped_column(nullable=True)
+    http_last_modified: Mapped[datetime] = mapped_column(nullable=True)
+    hash: Mapped[str] = mapped_column(nullable=True)
+    xlsx_hash: Mapped[str] = mapped_column(nullable=True)
     force_hash: Mapped[bool] = mapped_column(nullable=False)
     """
 
     id: Mapped[str] = mapped_column(primary_key=True)
     url: Mapped[str] = mapped_column(nullable=False)
     format: Mapped[str] = mapped_column(nullable=False)
     err: Mapped[str] = mapped_column(nullable=True)
     http_last_modified: Mapped[datetime] = mapped_column(nullable=True)
     hash: Mapped[str] = mapped_column(nullable=True)
     xlsx_hash: Mapped[str] = mapped_column(nullable=True)
     force_hash: Mapped[bool] = mapped_column(nullable=False)
 
     def __repr__(self) -> str:
-        """String representation of DBTestHashresult row
+        """String representation of DBTestResult row
 
         Returns:
-            str: String representation of DBTestHashResult row
+            str: String representation of DBTestResult row
         """
-        output = f"<TestHashResult(id={self.id}, url={self.url}, "
+        output = f"<TestResult(id={self.id}, url={self.url}, "
         output += f"format={self.format}, err={self.err}\n"
         output += f"http_last_modified={str(self.http_last_modified)}, "
         output += f"hash={self.hash}, xlsx_hash={self.xlsx_hash}, "
         output += f"force_hash={str(self.force_hash)})>"
         return output
```

### Comparing `hdx-data-freshness-1.9.8/src/hdx/freshness/testdata/dbtestresource.py` & `hdx-data-freshness-1.9.9/src/hdx/freshness/testdata/dbtestresource.py`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/src/hdx/freshness/testdata/serialize.py` & `hdx-data-freshness-1.9.9/src/hdx/freshness/testdata/serialize.py`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/src/hdx/freshness/utils/ratelimiter.py` & `hdx-data-freshness-1.9.9/src/hdx/freshness/utils/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/src/hdx/freshness/utils/retrieval.py` & `hdx-data-freshness-1.9.9/src/hdx/freshness/utils/retrieval.py`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/src/hdx/freshness/utils/retry.py` & `hdx-data-freshness-1.9.9/src/hdx/freshness/utils/retry.py`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/src/hdx_data_freshness.egg-info/PKG-INFO` & `hdx-data-freshness-1.9.9/src/hdx_data_freshness.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-data-freshness
-Version: 1.9.8
+Version: 1.9.9
 Summary: HDX Data Freshness analyses freshness of data on HDX
 Home-page: https://github.com/OCHA-DAP/hdx-data-freshness
 Author: Michael Rans
 Author-email: rans@email.com
 License: MIT
 Keywords: HDX,fresh,freshness,data freshness
 Platform: any
```

### Comparing `hdx-data-freshness-1.9.8/src/hdx_data_freshness.egg-info/SOURCES.txt` & `hdx-data-freshness-1.9.9/src/hdx_data_freshness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/fixtures/datasets.pickle` & `hdx-data-freshness-1.9.9/tests/fixtures/datasets.pickle`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/fixtures/day0/test_freshness.db` & `hdx-data-freshness-1.9.9/tests/fixtures/day0/test_freshness.db`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/fixtures/day0/test_serialize.db` & `hdx-data-freshness-1.9.9/tests/fixtures/day0/test_serialize.db`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/fixtures/dayN/test_freshness.db` & `hdx-data-freshness-1.9.9/tests/fixtures/dayN/test_freshness.db`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/fixtures/dayN/test_serialize.db` & `hdx-data-freshness-1.9.9/tests/fixtures/dayN/test_serialize.db`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/fixtures/retrieve/ACLED-Country-Coverage-and-ISO-Codes_8.2019.xlsx` & `hdx-data-freshness-1.9.9/tests/fixtures/retrieve/ACLED-Country-Coverage-and-ISO-Codes_8.2019.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/fixtures/retrieve/COD_MOZ_Admin0.geojson` & `hdx-data-freshness-1.9.9/tests/fixtures/retrieve/COD_MOZ_Admin0.geojson`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/fixtures/retrieve/Dataset.csv` & `hdx-data-freshness-1.9.9/tests/fixtures/retrieve/Dataset.csv`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/fixtures/retrieve/hotosm_nic_airports_lines_shp.zip` & `hdx-data-freshness-1.9.9/tests/fixtures/retrieve/hotosm_nic_airports_lines_shp.zip`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/fixtures/retrieve/hrp_adm1_4pc.geojson` & `hdx-data-freshness-1.9.9/tests/fixtures/retrieve/hrp_adm1_4pc.geojson`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/fixtures/retrieve/list_one.xls` & `hdx-data-freshness-1.9.9/tests/fixtures/retrieve/list_one.xls`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/fixtures/retrieve/response.html` & `hdx-data-freshness-1.9.9/tests/fixtures/retrieve/response.html`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/hdx/freshness/app/test_freshness_CKAN.py` & `hdx-data-freshness-1.9.9/tests/hdx/freshness/app/test_freshness_CKAN.py`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/hdx/freshness/app/test_freshness_by_frequency.py` & `hdx-data-freshness-1.9.9/tests/hdx/freshness/app/test_freshness_by_frequency.py`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/hdx/freshness/app/test_freshness_day0.py` & `hdx-data-freshness-1.9.9/tests/hdx/freshness/app/test_freshness_day0.py`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/hdx/freshness/app/test_freshness_dayN.py` & `hdx-data-freshness-1.9.9/tests/hdx/freshness/app/test_freshness_dayN.py`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/hdx/freshness/app/test_process_results.py` & `hdx-data-freshness-1.9.9/tests/hdx/freshness/app/test_process_results.py`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/hdx/freshness/conftest.py` & `hdx-data-freshness-1.9.9/tests/hdx/freshness/conftest.py`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/hdx/freshness/testdata/test_serialize.py` & `hdx-data-freshness-1.9.9/tests/hdx/freshness/testdata/test_serialize.py`

 * *Files identical despite different names*

### Comparing `hdx-data-freshness-1.9.8/tests/hdx/freshness/utils/test_retrieval.py` & `hdx-data-freshness-1.9.9/tests/hdx/freshness/utils/test_retrieval.py`

 * *Files identical despite different names*

