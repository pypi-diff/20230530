# Comparing `tmp/ocha-anticipy-1.0.2.tar.gz` & `tmp/ocha-anticipy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocha-anticipy-1.0.2.tar", last modified: Mon May 29 11:23:47 2023, max compression
+gzip compressed data, was "ocha-anticipy-1.1.0.tar", last modified: Tue May 30 13:13:36 2023, max compression
```

## Comparing `ocha-anticipy-1.0.2.tar` & `ocha-anticipy-1.1.0.tar`

### file list

```diff
@@ -1,119 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.999639 ocha-anticipy-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.983638 ocha-anticipy-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.987638 ocha-anticipy-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/.github/workflows/run-python-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1943 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     5246 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5371 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4133 2023-05-29 11:23:46.999639 ocha-anticipy-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3018 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.983638 ocha-anticipy-1.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.987638 ocha-anticipy-1.0.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     2394 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/config.rst
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/docs/source/datasources/
--rw-r--r--   0 runner    (1001) docker     (122)     4362 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/datasources/chirps.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3861 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/datasources/codab.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4187 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/datasources/fewsnet.rst
--rw-r--r--   0 runner    (1001) docker     (122)    12584 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/datasources/glofas.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/datasources/iri_seasonal_forecast.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6354 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/datasources/usgs_ndvi.rst
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/datasources.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/docs/source/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/utilities/raster.rst
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)    16115 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1160 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7169 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/requirements/tests.in
--rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-05-29 11:23:46.999639 ocha-anticipy-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.983638 ocha-anticipy-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/src/ocha_anticipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4133 2023-05-29 11:23:46.000000 ocha-anticipy-1.0.2/src/ocha_anticipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3166 2023-05-29 11:23:46.000000 ocha-anticipy-1.0.2/src/ocha_anticipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 11:23:46.000000 ocha-anticipy-1.0.2/src/ocha_anticipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-29 11:23:46.000000 ocha-anticipy-1.0.2/src/ocha_anticipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-29 11:23:46.000000 ocha-anticipy-1.0.2/src/ocha_anticipy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/src/ochanticipy/
--rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-29 11:23:46.000000 ocha-anticipy-1.0.2/src/ochanticipy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/src/ochanticipy/config/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/src/ochanticipy/config/countries/
--rw-r--r--   0 runner    (1001) docker     (122)      823 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/config/countries/bfa.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/config/countries/bgd.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/config/countries/cod.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1566 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/config/countries/eth.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/config/countries/mwi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/config/countries/npl.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     7912 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/config/countryconfig.py
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/config/pathconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/src/ochanticipy/datasources/
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/src/ochanticipy/datasources/chirps/
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/chirps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19881 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/chirps/chirps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/src/ochanticipy/datasources/codab/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/codab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6156 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/codab/codab.py
--rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/datasource.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.995638 ocha-anticipy-1.0.2/src/ochanticipy/datasources/fewsnet/
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/fewsnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13942 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/fewsnet/fewsnet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.995638 ocha-anticipy-1.0.2/src/ochanticipy/datasources/glofas/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/glofas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9852 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/glofas/forecast.py
--rw-r--r--   0 runner    (1001) docker     (122)    18347 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/glofas/glofas.py
--rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/glofas/reanalysis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.995638 ocha-anticipy-1.0.2/src/ochanticipy/datasources/iri/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/iri/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10406 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/iri/iri_seasonal_forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.995638 ocha-anticipy-1.0.2/src/ochanticipy/datasources/usgs/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/usgs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28079 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/usgs/ndvi_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    10009 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/usgs/ndvi_products.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.995638 ocha-anticipy-1.0.2/src/ochanticipy/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2321 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/utils/check_file_existence.py
--rw-r--r--   0 runner    (1001) docker     (122)     6071 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (122)     7202 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/utils/geoboundingbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     1874 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/utils/hdx_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1814 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (122)    25520 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/utils/raster.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.995638 ocha-anticipy-1.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.995638 ocha-anticipy-1.0.2/tests/datasources/
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      377 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/fake_config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    14174 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/test_chirps.py
--rw-r--r--   0 runner    (1001) docker     (122)     3631 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/test_codab.py
--rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/test_datasource.py
--rw-r--r--   0 runner    (1001) docker     (122)     7536 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/test_fewsnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     3582 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/test_glofas.py
--rw-r--r--   0 runner    (1001) docker     (122)     6255 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/test_glofas_download.py
--rw-r--r--   0 runner    (1001) docker     (122)     9524 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/test_glofas_process.py
--rw-r--r--   0 runner    (1001) docker     (122)     7158 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/test_iri.py
--rw-r--r--   0 runner    (1001) docker     (122)     8883 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/test_ndvi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5252 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/test_country_config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.999639 ocha-anticipy-1.0.2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     1683 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/utils/test_check_file_existence.py
--rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/utils/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2915 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/utils/test_geoboundingbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     1537 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/utils/test_hdx_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     6621 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/utils/test_raster.py
--rw-r--r--   0 runner    (1001) docker     (122)      394 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.523914 ocha-anticipy-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.471913 ocha-anticipy-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.483914 ocha-anticipy-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      342 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5855 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4455 2023-05-30 13:13:36.523914 ocha-anticipy-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3235 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.487914 ocha-anticipy-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     2438 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/config.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.487914 ocha-anticipy-1.1.0/docs/datasources/
+-rw-r--r--   0 runner    (1001) docker     (122)     4362 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/datasources/chirps.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/datasources/codab.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4187 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/datasources/fewsnet.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    12684 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/datasources/glofas.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/datasources/iri_seasonal_forecast.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5950 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/datasources/usgs_ndvi.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/datasources.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.487914 ocha-anticipy-1.1.0/docs/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/utilities/raster.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)    11353 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2149 2023-05-30 13:13:36.523914 ocha-anticipy-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.475913 ocha-anticipy-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.491914 ocha-anticipy-1.1.0/src/ocha_anticipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4455 2023-05-30 13:13:36.000000 ocha-anticipy-1.1.0/src/ocha_anticipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-05-30 13:13:36.000000 ocha-anticipy-1.1.0/src/ocha_anticipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 13:13:36.000000 ocha-anticipy-1.1.0/src/ocha_anticipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      450 2023-05-30 13:13:36.000000 ocha-anticipy-1.1.0/src/ocha_anticipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-30 13:13:36.000000 ocha-anticipy-1.1.0/src/ocha_anticipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.491914 ocha-anticipy-1.1.0/src/ochanticipy/
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-30 13:13:36.000000 ocha-anticipy-1.1.0/src/ochanticipy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.491914 ocha-anticipy-1.1.0/src/ochanticipy/config/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.503914 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/afg.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/bdi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/bfa.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/bgd.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3120 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/caf.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/cmr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/cod.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3236 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/col.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/eth.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      333 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/hti.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/irq.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/lby.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2933 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/mli.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/mmr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4181 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/moz.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/mwi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/ner.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1708 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/nga.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/npl.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/pse.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/sdn.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/som.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/ssd.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/syr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/tcd.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/ukr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/ven.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/yem.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     8920 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countryconfig.py
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/pathconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.503914 ocha-anticipy-1.1.0/src/ochanticipy/datasources/
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.503914 ocha-anticipy-1.1.0/src/ochanticipy/datasources/chirps/
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/chirps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19875 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/chirps/chirps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.507914 ocha-anticipy-1.1.0/src/ochanticipy/datasources/codab/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/codab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7182 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/codab/codab.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/datasource.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.507914 ocha-anticipy-1.1.0/src/ochanticipy/datasources/fewsnet/
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/fewsnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13942 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/fewsnet/fewsnet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.507914 ocha-anticipy-1.1.0/src/ochanticipy/datasources/glofas/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/glofas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9849 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/glofas/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19202 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/glofas/glofas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/glofas/reanalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.507914 ocha-anticipy-1.1.0/src/ochanticipy/datasources/iri/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/iri/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10404 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/iri/iri_seasonal_forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.511914 ocha-anticipy-1.1.0/src/ochanticipy/datasources/usgs/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/usgs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28079 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/usgs/ndvi_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10009 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/usgs/ndvi_products.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.511914 ocha-anticipy-1.1.0/src/ochanticipy/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      768 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/utils/check_extra_imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/utils/check_file_existence.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6071 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7202 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/utils/geoboundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/utils/hdx_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1814 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25617 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/utils/raster.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.511914 ocha-anticipy-1.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.519914 ocha-anticipy-1.1.0/tests/datasources/
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/fake_codab_multi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/fake_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    14174 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/test_chirps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5140 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/test_codab.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/test_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7536 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/test_fewsnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4790 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/test_glofas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6223 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/test_glofas_download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9524 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/test_glofas_process.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7158 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/test_iri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8882 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/test_ndvi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/test_country_config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.519914 ocha-anticipy-1.1.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/utils/test_check_extra_imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/utils/test_check_file_existence.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/utils/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2915 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/utils/test_geoboundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1547 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/utils/test_hdx_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7015 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/utils/test_raster.py
```

### Comparing `ocha-anticipy-1.0.2/.github/workflows/publish-to-pypi.yaml` & `ocha-anticipy-1.1.0/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/.github/workflows/run-python-tests.yaml` & `ocha-anticipy-1.1.0/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/.gitignore` & `ocha-anticipy-1.1.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -65,17 +65,17 @@
 instance/
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
-docs/build/
-docs/source/modules.rst
-docs/source/ochanticipy*.rst
+docs/_build/
+docs/modules.rst
+docs/ochanticipy*.rst
 
 # PyBuilder
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
```

### Comparing `ocha-anticipy-1.0.2/.pre-commit-config.yaml` & `ocha-anticipy-1.1.0/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -42,28 +42,15 @@
           - types-python-dateutil==2.8.19
         exclude: tests
   - repo: https://github.com/igorshubovych/markdownlint-cli
     rev: v0.32.0
     hooks:
       - id: markdownlint
   - repo: https://github.com/jazzband/pip-tools
-    rev: 6.12.2
+    rev: 6.13.0
     hooks:
       - id: pip-compile
         name: pip-compile requirements.txt
         files: setup.cfg
-        args: [setup.cfg, -q, -o, requirements/requirements.txt]
-      - id: pip-compile
-        name: pip-compile requirements-docs.txt
-        files: requirements/docs.in
-        args: [ requirements/docs.in, -q, -o,
-                requirements/requirements-docs.txt ]
-      - id: pip-compile
-        name: pip-compile requirements-tests.txt
-        files: requirements/tests.in
-        args: [requirements/tests.in, -q, -o,
-               requirements/requirements-tests.txt]
-      - id: pip-compile
-        name: pip-compile requirements-dev.txt
-        files: requirements/(dev.in|docs.in|tests.in|requirements.txt)
-        args: [requirements/dev.in, -q, -o,
-               requirements/requirements-dev.txt]
+        args: [setup.cfg, --resolver=backtracking,
+              --upgrade, --extra, dev, -q, -o,
+              requirements.txt]
```

### Comparing `ocha-anticipy-1.0.2/CHANGELOG.rst` & `ocha-anticipy-1.1.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,39 @@
 All notable changes to OCHA AnticiPy will be documented in this file.
 
 The format is based on `Keep a
 Changelog <https://keepachangelog.com/en/1.0.0/>`__, and this project
 adheres to `Semantic
 Versioning <https://semver.org/spec/v2.0.0.html>`__.
 
+[1.1.0] - 2023-05-30
+--------------------
+
+Added
+~~~~~
+
+- Config files for 25/25 HRP countries and several non-HRP countries
+
+Changed
+~~~~~~~
+
+- Optional dependencies and documentation, testing, and development
+  reqirements moved to ``extras_require``
+- GloFAS module dependencies made optional
+- tox configuration moved to ``setup.cfg`` from ``tox.ini``
+
+Fixed
+~~~~~
+
+- Automatic raster dimension setting for `lat/lon` and `X/Y`
+  fixed to work for `rioxarray` methods
+- USGS NDVI documentation was updated to remove dead links
+  and improve users ability to use the historical data
+- GloFAS does not permit users to go above request limit of 500
+
 [1.0.2] - 2023-05-29
 --------------------
 
 Fixed
 ~~~~~
 
 - Fixed bug for loading COD AB shapefiles in Windows
```

### Comparing `ocha-anticipy-1.0.2/CONTRIBUTING.rst` & `ocha-anticipy-1.1.0/CONTRIBUTING.rst`

 * *Files 10% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 environment such as ``venv``:
 
 .. code:: shell
 
     python3.11 -m venv venv
     source venv/bin/activate
 
-In your virtual environment, please install all packages from
-``requirements/requirements-dev.txt``:
+In your virtual environment, please install all packages for
+development by running:
 
 .. code:: shell
 
-   pip install -r requirements/requirements-dev.txt
+   pip install -r requirements.txt
 
-OCHA AnticiPy makes use of
+``aa-toolbox`` makes use of
 `geopandas <https://geopandas.org/en/stable/>`__, which depends on
 `Fiona <https://github.com/Toblerity/Fiona>`__, so you will need to
 have `GDAL <https://github.com/Toblerity/Fiona#installation>`__
 installed.
 
 Installation
 ------------
 
-To install in editable mode for development, execute:
+To install ``ocha-anticipy`` in editable mode for development, execute:
 
 .. code:: shell
 
    pip install -e .
 
 Testing
 -------
@@ -99,17 +99,17 @@
 Build and view
 ^^^^^^^^^^^^^^
 
 To build the documentation and test your implementation, use the following command:
 
 .. code:: shell
 
-   sphinx-build -b html -d docs/build/doctrees docs/source docs/build/html
+   sphinx-build -b html -d docs/_build/doctrees docs docs/_build/html
 
-To view the docs, open up ``docs/build/html/index.html`` in your
+To view the docs, open up ``docs-build/html/index.html`` in your
 browser.
 
 pre-commit
 ----------
 
 All code is formatted according to
 `black <https://github.com/psf/black>`__ and
@@ -129,29 +129,49 @@
 --------
 
 `pip-tools <https://github.com/jazzband/pip-tools>`__ is used for
 package management.
 
 If you’ve introduced a new package to the source code (i.e. anywhere in
 ``src/``), please add it to the ``install_requires`` section of
-``setup.cfg`` with any known version constraints. For adding packages
-for development, documentation, or tests, add them to the relevant
-``.in`` file in the ``requirements`` directory. When you modify any of
-these lists, please try to keep them alphabetical! Any changes to the
-``requirements*.txt`` files will be generated with ``pre-commit``.
-
-To run this without commiting, execute:
+``setup.cfg`` with any known version constraints. However, in the
+case where a library is only required for a single data source,
+these should be added in the ``options.extras_require`` section
+of ``setup.cfg``, with a relevant name for the requirements list.
+For example, the GLOFAS module relies on the ``cdsapi`` and
+``cfgrib`` packages, and would look like.
+
+.. code::
+
+   [options.extras_require]
+   glofas =
+      cdsapi
+      cfgrib
+
+Also add reference to the subpackage under ``full`` using the
+``%(subpackage)s`` format.
+
+.. code::
+
+   full =
+      %(glofas)s
+
+For adding packages for testing, documentation, or development, add them to
+the relevant subpackage under ``[options.extras_require]``, ``test``,
+``doc``, and ``dev`` respectively. When you modify any of
+these lists, please try to keep them alphabetical!
+
+Any changes to the dependencies will be automatically reflected in
+``requirements.txt`` with ``pre-commit``, but you can re-generate
+the file without commiting by executing:
 
 .. code:: shell
 
    pre-commit run pip-compile --all-files
 
-For other functionality such as updating specific package versions,
-refer to the ``pip-tools`` documentation.
-
 Package Release
 ---------------
 
 Features are developed on our ``develop`` branch, with changes tracked
 in the “Unreleased” section at the top of ``CHANGELOG.md``. Upon
 release, the ``develop`` branch is merged to ``main`` and the release is
 tagged according to `semantic
```

### Comparing `ocha-anticipy-1.0.2/LICENSE` & `ocha-anticipy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/PKG-INFO` & `ocha-anticipy-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocha-anticipy
-Version: 1.0.2
+Version: 1.1.0
 Summary: Access data for anticipating humanitarian risk
 Home-page: https://github.com/OCHA-DAP/ocha-anticipy
 Author: Data Science Team, UN OCHA Centre for Humanitarian Data
 Author-email: centrehumdata@un.org
 License: GPLv3
 Project-URL: Documentation, https://ocha-anticipy.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/OCHA-DAP/ocha-anticipy/blob/main/CHANGELOG.rst
@@ -16,14 +16,19 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: glofas
+Provides-Extra: full
+Provides-Extra: test
+Provides-Extra: doc
+Provides-Extra: dev
 License-File: LICENSE
 
 # OCHA AnticiPy: Access data for anticipating humanitarian risk
 
 [![license](https://img.shields.io/github/license/OCHA-DAP/ocha-anticipy.svg)](https://github.com/OCHA-DAP/ocha-anticipy/blob/main/LICENSE)
 [![Test Status](https://github.com/OCHA-DAP/ocha-anticipy/workflows/tests/badge.svg)](https://github.com/OCHA-DAP/ocha-anticipy/actions?query=workflow%3Atests)
 [![PyPI Status](https://github.com/OCHA-DAP/ocha-anticipy/workflows/PyPI/badge.svg)](https://github.com/OCHA-DAP/ocha-anticipy/actions?query=workflow%3APyPI)
@@ -53,14 +58,22 @@
 
 Install and update using [pip](https://pip.pypa.io/en/stable/getting-started/):
 
 ```shell
 pip install ocha-anticipy
 ```
 
+Some modules of the toolbox have specific dependencies not installed by default.
+These are documented within each module, but all dependencies can be installed
+using.
+
+```shell
+pip install -U ocha-anticipy[full]
+```
+
 ## A Simple Example
 
 OCHA AnticiPy downloads data to the directory referenced by the
 environment variable `OAP_DATA_DIR`. Before beginning, please make
 sure that this environment variable is defined and points to where you would
 like the data to go.
```

### Comparing `ocha-anticipy-1.0.2/README.md` & `ocha-anticipy-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,22 @@
 
 Install and update using [pip](https://pip.pypa.io/en/stable/getting-started/):
 
 ```shell
 pip install ocha-anticipy
 ```
 
+Some modules of the toolbox have specific dependencies not installed by default.
+These are documented within each module, but all dependencies can be installed
+using.
+
+```shell
+pip install -U ocha-anticipy[full]
+```
+
 ## A Simple Example
 
 OCHA AnticiPy downloads data to the directory referenced by the
 environment variable `OAP_DATA_DIR`. Before beginning, please make
 sure that this environment variable is defined and points to where you would
 like the data to go.
```

### Comparing `ocha-anticipy-1.0.2/docs/source/api.rst` & `ocha-anticipy-1.1.0/docs/api.rst`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 .. automodule:: ochanticipy.datasources.fewsnet.fewsnet
 .. autoclass:: ochanticipy.FewsNet
    :members:
 
 GloFAS
 ^^^^^^
 
+.. extras-require:: glofas
+    :setup.cfg:
+
 .. automodule:: ochanticipy.datasources.glofas.glofas
 
 Reanalysis
 """"""""""
 
 .. autoclass:: ochanticipy.GlofasReanalysis
    :inherited-members:
@@ -126,17 +129,17 @@
 ^^^^^^^^^^^^^
 
 .. automodule:: ochanticipy.utils.raster
 
 Data arrays
 """""""""""
 
-.. autoclass:: ochanticipy.utils.raster.AatRasterArray
+.. autoclass:: ochanticipy.utils.raster.OapRasterArray
    :members:
    :inherited-members: RasterArray
 
 Datasets
 """"""""
 
-.. autoclass:: ochanticipy.utils.raster.AatRasterDataset
+.. autoclass:: ochanticipy.utils.raster.OapRasterDataset
    :members:
    :inherited-members: RasterDataset
```

### Comparing `ocha-anticipy-1.0.2/docs/source/conf.py` & `ocha-anticipy-1.1.0/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 
 import os
 import sys
 
-sys.path.insert(0, os.path.abspath("../.."))
+sys.path.insert(0, os.path.abspath(".."))
 
 # -- Project information -----------------------------------------------------
 
 project = "OCHA AnticiPy"
 author = "Data Science Team, UN OCHA Centre for Humanitarian Data"
 copyright = "2023, UN OCHA Centre for Humanitarian Data"
 
@@ -27,28 +27,33 @@
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.napoleon",
     "sphinx.ext.viewcode",
     "sphinxcontrib.apidoc",
+    "sphinxcontrib.extras_require",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = []  # type: list
 
 # API doc settings
-apidoc_module_dir = "../../src/ochanticipy"
+apidoc_module_dir = "../src/ochanticipy"
 apidoc_output_dir = "."
 
+# Needed to sphinxcontrib.extra_requires to work
+package_root = "ochanticipy"
+pypi_name = "ocha-anticipy"
+
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 html_theme = "alabaster"
 
 # Add any paths that contain custom static files (such as style sheets) here,
```

### Comparing `ocha-anticipy-1.0.2/docs/source/datasources/chirps.rst` & `ocha-anticipy-1.1.0/docs/datasources/chirps.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/docs/source/datasources/codab.rst` & `ocha-anticipy-1.1.0/docs/datasources/codab.rst`

 * *Files 13% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 To use this class, you first need to create a country configuration
 for the country you would like to use:
 
 .. code-block:: python
 
     from ochanticipy import create_country_config
-    country_config = create_country_config(iso3="npl")
+    country_config = create_country_config(iso3="nga")
 
 Next you need to instantiate the CodAB class with the country config:
 
 .. code-block:: python
 
     from ochanticipy import CodAB
     codab = CodAB(country_config=country_config)
@@ -41,69 +41,73 @@
     codab.download()
 
 Finally, use the load method to begin working with the data as a
 GeoPandas dataframe:
 
 .. code-block:: python
 
-    npl_admin1 = codab.load(admin_level=1)
+    nga_admin1 = codab.load(admin_level=1)
 
 Some COD AB files have additional layers that don't correspond to
-an admin level. For example, Nepal has a districts layer, which
+an admin level. For example, Nigeria has a districts layer, which
 is provided in the config file as the first custom layer:
 
 .. code-block:: python
 
-    npl_districts = codab.load_custom(custom_layer_number=0)
+    nga_districts = codab.load_custom(custom_layer_number=0)
 
 The full code snippet is below in case you would like to copy it:
 
 .. code-block:: python
 
     from ochanticipy import create_country_config, CodAB
-    country_config = create_country_config(iso3="npl")
+    country_config = create_country_config(iso3="nga")
     codab = CodAB(country_config=country_config)
     codab.download()
-    npl_admin1 = codab.load(admin_level=1)
-    npl_districts = codab.load_custom(custom_layer_number=0)
+    nga_admin1 = codab.load(admin_level=1)
+    nga_districts = codab.load_custom(custom_layer_number=0)
 
 Configuration
 -------------
 
 The COD AB portion of the configuration file
 should be setup as follows:
 
 .. code-block:: yaml
 
     codab:
-      hdx_dataset_name: npl_admbnda_nd_20201117_SHP.zip
-      layer_base_name: npl_admbnda_adm{admin_level}_nd_20201117.shp
-      admin_level_max: 2
-      admin2_name: npl_admbnda_adm2_nd.shp
-      custom_layer_names:
-        - npl_admbnda_districts_nd_20201117
+        hdx_resource_name:
+            - nga_adm_osgof_20190417.zip
+            - nga_additional.zip # contrived example for documentation
+        layer_base_name: nga_admbnda_adm{admin_level}_osgof_20190417.shp
+        admin_level_max: 3
+        adm1_name: nga_adm1.shp # contrived example for documentation
+        custom_layer_names:
+            - nga_admbnda_senDist_inec_osgof_20190417.shp
 
 Below is an explanation of the different parameters:
 
-``hdx_dataset_name``: The name of the shapefile dataset on HDX. It can be found by taking
+``hdx_resource_name``: The name of the shapefile resource on HDX. It can be found by taking
 the filename as it appears on the HDX page. For example, you can see on the
-`page for Nepal <https://data.humdata.org/dataset/cod-ab-npl>`_ that the shapefile
-(i.e. with the ``.shp``. or ``.SHP`` extension) has the name
-``npl_admbnda_nd_20201117_SHP.zip``.
+`page for Nigeria <https://data.humdata.org/dataset/cod-ab-nga>`_ that the shapefile
+(sometimes with the ``.shp``. or ``.SHP`` extension, this time not) has the name
+``nga_adm_osgof_20190417.zip``. If admin levels are stored in different resources, which is
+the case for some countries like Niger, then each individual resource should should be listed
+under ``hdx_resource_name``. The format is shown above as an example to follow.
 
 ``layer_base_name``: The baseline name of the different admin level layers, with the
 level number replaced by the variable ``{admin_level}``. To find this, you will need
 to open up the shpaefile in e.g. `QGIS <https://www.qgis.org/en/site/>`_.
-In the case of Nepal, the layers have the names ``npl_admbnda_adm0_nd_20201117.shp``,
-``npl_admbnda_adm1_nd_20201117.shp``, and ``npl_admbnda_adm2_nd_20201117.shp``
+In the case of Nigeria, the layers have the names ``nga_admbnda_adm0_osgof_20190417.shp``,
+``nga_admbnda_adm1_osgof_20190417.shp``, and ``nga_admbnda_adm2_osgof_20190417.shp``
 
-``admin_level_max``: The maximum admin level available in the layers. In the case of Nepal,
-the layer level numbers range from 0 to 2, so the maximum should be 2. In general the
-maximum admin level should not exceed 4.
+``admin_level_max``: The maximum admin level available in the layers. In the case of Nigeria,
+the layer level numbers range from 0 to 3, so the maximum should be 3. In general the
+ maximum admin level should not exceed 4.
 
 ``admin{level}_name``: An optional parameter for any admin level (``level`` can range from 0 to 4)
-whose layer names do not match the ``layer_base_name`` pattern. This example for Nepal
-is contrived, but this issue does exist for COD ABs from countries such as Ethiopia and DRC.
+whose layer names do not match the ``layer_base_name`` pattern. This example for Nigeria
+ is contrived, but this issue does exist for COD ABs from countries such as Ethiopia and DRC.
 
-``custom_layer_name``: An optional place to list any other layers that don't correspond to the
-admin level format specified above. In the case of Nepal, there is a layer for districts
-with the name ``npl_admbnda_districts_nd_20201117``.
+``custom_layer_name``: A place to list any other layers that don't correspond to the
+admin level format specified above. In the case of Nigeria, there is a layer for districts
+with the name ``nga_admbnda_senDist_inec_osgof_20190417.shp``.
```

### Comparing `ocha-anticipy-1.0.2/docs/source/datasources/fewsnet.rst` & `ocha-anticipy-1.1.0/docs/datasources/fewsnet.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/docs/source/datasources/glofas.rst` & `ocha-anticipy-1.1.0/docs/datasources/glofas.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 GloFAS
 ======
 
+.. extras-require:: glofas
+    :setup.cfg:
+
 Background
 ----------
 
 The
 `Global Flood Awareness System (GloFAS)
 <https://www.globalfloods.eu/>`_
 is part of the
@@ -181,14 +184,15 @@
 <https://github.com/ecmwf/eccodes-python#system-dependencies>_`,
 ecCodes can be installed using `brew`:
 
 .. code-block:: shell
 
     brew install eccodes
 
+
 Reporting points
 ~~~~~~~~~~~~~~~~
 
 Next, if it :ref:`doesn't already exist<list of supported countries>`,
 you need to create a country configuration
 for the country you would like to analyze.
 
@@ -332,14 +336,15 @@
 .. code-block:: python
 
     from datetime import date
 
     from ochanticipy import create_country_config, CodAB, \
         GeoBoundingBox, GlofasForecast
 
+    country_config = create_country_config(iso3="bgd")
     codab = CodAB(country_config=country_config)
     codab.download()
     admin0 = codab.load()
     geo_bounding_box = GeoBoundingBox.from_shape(admin0)
 
     glofas_forecast = GlofasForecast(
         country_config=country_config,
```

### Comparing `ocha-anticipy-1.0.2/docs/source/datasources/iri_seasonal_forecast.rst` & `ocha-anticipy-1.1.0/docs/datasources/iri_seasonal_forecast.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/docs/source/datasources/usgs_ndvi.rst` & `ocha-anticipy-1.1.0/docs/datasources/usgs_ndvi.rst`

 * *Files 22% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 ==================
 
 Warning
 -------
 
 The MODIS sensor has been reported by USGS to
 have degraded in quality since May 2022 (dekad 13), and
-updates to this data source have stopped. This module
-remains for users to have access to historic data but
+updates to this data source have stopped. Documentation of
+the product has been removed from the
+`USGS FEWS product page <https://earlywarning.usgs.gov/fews/product>`_,
+which has made methodological details and geographic links unavailable.
+
+This module remains for users to have access to historic data but
 recent data is unavailable and care should be used
 analyzing any data since dekad 13 of 2022.
 
 Background
 ----------
 
 The United States Geological Survey, `USGS <https://www.usgs.gov/>`_ provides a wide
@@ -25,46 +29,47 @@
 geographic coverage is typically comprehensive of the African continent, where
 the majority of FEWS NET's work is focused, with additional areas covered on an
 ad hoc basis. This module for now just provides access to the normalized
 difference vegetation index (`NDVI <https://en.wikipedia.org/wiki/Normalized_difference_vegetation_index>`_)
 generated from eMODIS AQUA provided by the USGS.
 
 NDVI data is generated from eMODIS AQUA and published data includes temporally smoothed NDVI, median anomaly,
-difference from the previous year, and median anomaly presented as a percentile. Full methodological
-details are available on the `Documentation page <https://earlywarning.usgs.gov/fews/product/449#documentation>`_
-for the specific coverage area. The data is made available for the following areas of coverage:
-
-- `north-africa <https://earlywarning.usgs.gov/fews/product/449>`_
-- `east-africa <https://earlywarning.usgs.gov/fews/product/448>`_
-- `southern-africa <https://earlywarning.usgs.gov/fews/product/450>`_
-- `west-africa <https://earlywarning.usgs.gov/fews/product/451>`_
-- `central-asia <https://earlywarning.usgs.gov/fews/product/493>`_
-- `yemen <https://earlywarning.usgs.gov/fews/product/502>`_
-- `central-america <https://earlywarning.usgs.gov/fews/product/445>`_
-- `hispaniola <https://earlywarning.usgs.gov/fews/product/446>`_
+difference from the previous year, and median anomaly presented as a percentile.
+The data is made available for the following areas of coverage:
+
+- north-africa
+- east-africa
+- southern-africa
+- west-africa
+- central-asia
+- yemen
+- central-america
+- hispaniola
 
 Data is published at the dekadal level, and is released soon after the end of the dekad.
 After a period of 3 dekads, data is updated with temporal smoothing and error correction
 for cloud cover. Files for a specific dekad and region can range from 30MB up to over 100MB,
 so downloading and processing can take a long time.
 
 
-USGS publishes its data through its `web portal <https://earlywarning.usgs.gov/fews/datadownloads/East%20Africa/eMODIS%20NDVI%20C6>`_,
-which allows downloading data for a single geographical area and dekad. This data
-is extracted from the `back end data explorer <https://edcintl.cr.usgs.gov/downloads/sciweb1/shared/fews/web/africa/east/dekadal/emodis/ndvi_c6/temporallysmoothedndvi/downloads/monthly/>`_.
+USGS published its data through its web portal,
+which allows downloading data for a single geographical area and dekad. However, the data
+is no longer made available there, and the data for this product are extracted
+from the `back end data explorer <https://edcintl.cr.usgs.gov/downloads/sciweb1/shared/fews/web/africa/east/dekadal/emodis/ndvi_c6/temporallysmoothedndvi/downloads/monthly/>`_.
 This module is designed to allow programmatic access to and analysis of NDVI data from the data explorer.
 
 Usage
 -----
 
 To use this class, you first need to create a country configuration
 for the country you would like to analyze. You also need to supply the area
-of coverage that the country data is contained in. You can Make sure FEWS NET covers the country
-of interest. You can find area of coverage for NDVI by searching for eMODIS NDVI C6 on
-the  `USGS search portal <https://earlywarning.usgs.gov/fews/search>`_.
+of coverage that the country data is contained in. Although the NDVI data
+are no longer available directly on the portal, you can derive the region
+name for the data using the primary
+`USGS FEWS data portal <https://earlywarning.usgs.gov/fews>`_.
 The valid values of the area names are listed above under Background.
 
 An example country config for Ethiopia is:
 
 .. code-block:: python
 
     iso3: eth
```

### Comparing `ocha-anticipy-1.0.2/docs/source/index.rst` & `ocha-anticipy-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/docs/source/introduction.rst` & `ocha-anticipy-1.1.0/docs/introduction.rst`

 * *Files 9% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 
 This is where OCHA AnticiPy comes in, providing a simple interface for downloading and
 processing a range of data relevant for anticipatory action and
 disaster risk reduction in humanitarian response.
 
 Datasets currently supported are:
 
-- CHIRPS rainfall
-- COD ABs (Common Operational Datasets administrative boundaries)
-- FEWS NET food insecurity
-- GloFAS river discharge
-- IRI seasonal rainfall forecast
-- USGS NDVI (normalized difference vegetation index)
+ - CHIRPS rainfall
+ - COD ABs (Common Operational Datasets administrative boundaries)
+ - FEWS NET food insecurity
+ - GloFAS river discharge
+ - IRI seasonal rainfall forecast
+ - USGS NDVI (normalized difference vegetation index)
 
 At the `Centre for Humanitarian Data <https://centre.humdata.org/>`_,
 we've now used OCHA Anticipy to develop
 some of our own
 `anticipatory action
 <https://www.unocha.org/our-work/humanitarian-financing/anticipatory-action>`_
 frameworks, such as for
```

### Comparing `ocha-anticipy-1.0.2/docs/source/quickstart.rst` & `ocha-anticipy-1.1.0/docs/quickstart.rst`

 * *Files 16% similar despite different names*

```diff
@@ -11,25 +11,43 @@
 
 OCHA AnticiPy downloads data to the directory referenced by the
 environment variable `OAP_DATA_DIR`. Before beginning, please make
 sure that this environment variable is defined and points to where you would
 like the data to go.
 
 Install OCHA AnticiPy
-^^^^^^^^^^^^^^^^^^
+^^^^^^^^^^^^^^^^^^^^^
 
 OCHA AnticiPy supports Python 3.8 and newer. It can be installed in your Python
 environment using the following command:
 
 .. code-block:: sh
 
     $ pip install ocha-anticipy
 
 OCHA AnticiPy should now be installed.
 
+Optional dependencies
+*********************
+
+Some modules have optional dependencies that are not installed by default. Currently,
+this is just `glofas`. Optional dependencies will be included in the install if you
+specify the module as in the below command:
+
+.. code-block:: sh
+
+    $ pip install ocha-anticipy[glofas]
+
+Alternatively, you can install all requirements for all modules by specifying
+`full`:
+
+.. code-block:: sh
+
+    $ pip install ocha-anticipy[full]
+
 Usage Examples
 --------------
 
 COD administrative boundaries
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 A simple dataset to get started with are administrative boundaries,
```

### Comparing `ocha-anticipy-1.0.2/docs/source/utilities/raster.rst` & `ocha-anticipy-1.1.0/docs/utilities/raster.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/setup.cfg` & `ocha-anticipy-1.1.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -25,16 +25,14 @@
 
 [options]
 packages = find:
 package_dir = = src
 include_package_data = true
 python_requires = >= 3.8
 install_requires = 
-	cdsapi
-	cfgrib
 	cftime
 	geopandas
 	hdx-python-api>=5.6.4
 	hdx-python-country
 	netCDF4
 	numpy
 	pydantic
@@ -55,11 +53,60 @@
 build-dir = docs/build
 
 [flake8]
 extend-ignore = SFS301 # Allow f-strings
 docstring-convention = numpy
 max-pos-args = 2
 
+[options.extras_require]
+glofas = 
+	cdsapi
+	cfgrib
+full = 
+	%(glofas)s
+test = 
+	%(full)s
+	pytest
+	pytest-cov
+	pytest-mock
+	tox
+doc = 
+	extras_require
+	sphinx
+	sphinx-rtd-theme
+	sphinxcontrib-apidoc
+dev = 
+	%(test)s
+	%(doc)s
+	pre-commit
+
+[tox:tox]
+isolated_build = true
+envlist = 
+	py38
+	py39
+	py310
+	py311
+
+[testenv]
+wheel = true
+recreate = true
+extras = test
+commands = 
+	pytest \
+	--cov=ochanticipy \
+	--no-cov-on-fail \
+	--junitxml=.tox/test-results.xml \
+	--cov-report=xml \
+	--cov-report=term-missing
+
+[gh-actions]
+python = 
+	3.8: py38
+	3.9: py39
+	3.10: py310
+	3.11: py311
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ocha-anticipy-1.0.2/src/ocha_anticipy.egg-info/PKG-INFO` & `ocha-anticipy-1.1.0/src/ocha_anticipy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocha-anticipy
-Version: 1.0.2
+Version: 1.1.0
 Summary: Access data for anticipating humanitarian risk
 Home-page: https://github.com/OCHA-DAP/ocha-anticipy
 Author: Data Science Team, UN OCHA Centre for Humanitarian Data
 Author-email: centrehumdata@un.org
 License: GPLv3
 Project-URL: Documentation, https://ocha-anticipy.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/OCHA-DAP/ocha-anticipy/blob/main/CHANGELOG.rst
@@ -16,14 +16,19 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: glofas
+Provides-Extra: full
+Provides-Extra: test
+Provides-Extra: doc
+Provides-Extra: dev
 License-File: LICENSE
 
 # OCHA AnticiPy: Access data for anticipating humanitarian risk
 
 [![license](https://img.shields.io/github/license/OCHA-DAP/ocha-anticipy.svg)](https://github.com/OCHA-DAP/ocha-anticipy/blob/main/LICENSE)
 [![Test Status](https://github.com/OCHA-DAP/ocha-anticipy/workflows/tests/badge.svg)](https://github.com/OCHA-DAP/ocha-anticipy/actions?query=workflow%3Atests)
 [![PyPI Status](https://github.com/OCHA-DAP/ocha-anticipy/workflows/PyPI/badge.svg)](https://github.com/OCHA-DAP/ocha-anticipy/actions?query=workflow%3APyPI)
@@ -53,14 +58,22 @@
 
 Install and update using [pip](https://pip.pypa.io/en/stable/getting-started/):
 
 ```shell
 pip install ocha-anticipy
 ```
 
+Some modules of the toolbox have specific dependencies not installed by default.
+These are documented within each module, but all dependencies can be installed
+using.
+
+```shell
+pip install -U ocha-anticipy[full]
+```
+
 ## A Simple Example
 
 OCHA AnticiPy downloads data to the directory referenced by the
 environment variable `OAP_DATA_DIR`. Before beginning, please make
 sure that this environment variable is defined and points to where you would
 like the data to go.
```

### Comparing `ocha-anticipy-1.0.2/src/ocha_anticipy.egg-info/SOURCES.txt` & `ocha-anticipy-1.1.0/src/ocha_anticipy.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -2,59 +2,74 @@
 .pre-commit-config.yaml
 .readthedocs.yaml
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 README.md
 pyproject.toml
+requirements.txt
 setup.cfg
-tox.ini
 .github/workflows/publish-to-pypi.yaml
 .github/workflows/run-python-tests.yaml
-docs/source/api.rst
-docs/source/changelog.rst
-docs/source/conf.py
-docs/source/config.rst
-docs/source/contributing.rst
-docs/source/datasources.rst
-docs/source/index.rst
-docs/source/introduction.rst
-docs/source/license.rst
-docs/source/quickstart.rst
-docs/source/utilities.rst
-docs/source/datasources/chirps.rst
-docs/source/datasources/codab.rst
-docs/source/datasources/fewsnet.rst
-docs/source/datasources/glofas.rst
-docs/source/datasources/iri_seasonal_forecast.rst
-docs/source/datasources/usgs_ndvi.rst
-docs/source/utilities/raster.rst
-requirements/dev.in
-requirements/docs.in
-requirements/requirements-dev.txt
-requirements/requirements-docs.txt
-requirements/requirements-tests.txt
-requirements/requirements.txt
-requirements/tests.in
+docs/api.rst
+docs/changelog.rst
+docs/conf.py
+docs/config.rst
+docs/contributing.rst
+docs/datasources.rst
+docs/index.rst
+docs/introduction.rst
+docs/license.rst
+docs/quickstart.rst
+docs/utilities.rst
+docs/datasources/chirps.rst
+docs/datasources/codab.rst
+docs/datasources/fewsnet.rst
+docs/datasources/glofas.rst
+docs/datasources/iri_seasonal_forecast.rst
+docs/datasources/usgs_ndvi.rst
+docs/utilities/raster.rst
 src/ocha_anticipy.egg-info/PKG-INFO
 src/ocha_anticipy.egg-info/SOURCES.txt
 src/ocha_anticipy.egg-info/dependency_links.txt
 src/ocha_anticipy.egg-info/requires.txt
 src/ocha_anticipy.egg-info/top_level.txt
 src/ochanticipy/__init__.py
 src/ochanticipy/_version.py
 src/ochanticipy/config/__init__.py
 src/ochanticipy/config/countryconfig.py
 src/ochanticipy/config/pathconfig.py
+src/ochanticipy/config/countries/afg.yaml
+src/ochanticipy/config/countries/bdi.yaml
 src/ochanticipy/config/countries/bfa.yaml
 src/ochanticipy/config/countries/bgd.yaml
+src/ochanticipy/config/countries/caf.yaml
+src/ochanticipy/config/countries/cmr.yaml
 src/ochanticipy/config/countries/cod.yaml
+src/ochanticipy/config/countries/col.yaml
 src/ochanticipy/config/countries/eth.yaml
+src/ochanticipy/config/countries/hti.yaml
+src/ochanticipy/config/countries/irq.yaml
+src/ochanticipy/config/countries/lby.yaml
+src/ochanticipy/config/countries/mli.yaml
+src/ochanticipy/config/countries/mmr.yaml
+src/ochanticipy/config/countries/moz.yaml
 src/ochanticipy/config/countries/mwi.yaml
+src/ochanticipy/config/countries/ner.yaml
+src/ochanticipy/config/countries/nga.yaml
 src/ochanticipy/config/countries/npl.yaml
+src/ochanticipy/config/countries/pse.yaml
+src/ochanticipy/config/countries/sdn.yaml
+src/ochanticipy/config/countries/som.yaml
+src/ochanticipy/config/countries/ssd.yaml
+src/ochanticipy/config/countries/syr.yaml
+src/ochanticipy/config/countries/tcd.yaml
+src/ochanticipy/config/countries/ukr.yaml
+src/ochanticipy/config/countries/ven.yaml
+src/ochanticipy/config/countries/yem.yaml
 src/ochanticipy/datasources/__init__.py
 src/ochanticipy/datasources/datasource.py
 src/ochanticipy/datasources/chirps/__init__.py
 src/ochanticipy/datasources/chirps/chirps.py
 src/ochanticipy/datasources/codab/__init__.py
 src/ochanticipy/datasources/codab/codab.py
 src/ochanticipy/datasources/fewsnet/__init__.py
@@ -65,30 +80,33 @@
 src/ochanticipy/datasources/glofas/reanalysis.py
 src/ochanticipy/datasources/iri/__init__.py
 src/ochanticipy/datasources/iri/iri_seasonal_forecast.py
 src/ochanticipy/datasources/usgs/__init__.py
 src/ochanticipy/datasources/usgs/ndvi_base.py
 src/ochanticipy/datasources/usgs/ndvi_products.py
 src/ochanticipy/utils/__init__.py
+src/ochanticipy/utils/check_extra_imports.py
 src/ochanticipy/utils/check_file_existence.py
 src/ochanticipy/utils/dates.py
 src/ochanticipy/utils/geoboundingbox.py
 src/ochanticipy/utils/hdx_api.py
 src/ochanticipy/utils/io.py
 src/ochanticipy/utils/raster.py
 tests/test_country_config.py
 tests/datasources/conftest.py
+tests/datasources/fake_codab_multi.yaml
 tests/datasources/fake_config.yaml
 tests/datasources/test_chirps.py
 tests/datasources/test_codab.py
 tests/datasources/test_datasource.py
 tests/datasources/test_fewsnet.py
 tests/datasources/test_glofas.py
 tests/datasources/test_glofas_download.py
 tests/datasources/test_glofas_process.py
 tests/datasources/test_iri.py
 tests/datasources/test_ndvi.py
+tests/utils/test_check_extra_imports.py
 tests/utils/test_check_file_existence.py
 tests/utils/test_dates.py
 tests/utils/test_geoboundingbox.py
 tests/utils/test_hdx_api.py
 tests/utils/test_raster.py
```

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/__init__.py` & `ocha-anticipy-1.1.0/src/ochanticipy/__init__.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/config/countries/bfa.yaml` & `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/bfa.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 iso3: bfa
 codab:
-  hdx_dataset_name: bfa_adm_igb_20200323_SHP.zip
+  hdx_resource_name: bfa_adm_igb_20200323_SHP.zip
   layer_base_name: bfa_admbnda_adm{admin_level}_igb_20200323.shp
   admin_level_max: 3
 fewsnet:
   region_name: west-africa
 glofas:
   reporting_points:
   - name: BOUGOURI-BA a DIEBOUGOU
```

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/config/countries/bgd.yaml` & `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/bgd.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 iso3: bgd
 codab:
-  hdx_dataset_name: bgd_adm_bbs_20201113_SHP.zip
+  hdx_resource_name: bgd_adm_bbs_20201113_SHP.zip
   layer_base_name: bgd_adm_bbs_20201113_SHP/bgd_admbnda_adm{admin_level}_bbs_20201113.shp
   admin_level_max: 4
 glofas:
   reporting_points:
   - name: Bahadurabad
     lon: 89.65
     lat: 25.15
```

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/config/countries/cod.yaml` & `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/cod.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 iso3: cod
 codab:
-  hdx_dataset_name: cod_admbnda_rgc_itos_20190911_SHP.zip
+  hdx_resource_name: cod_admbnda_rgc_itos_20190911_SHP.zip
   layer_base_name: cod_admbnda_adm{admin_level}_rgc_itos_20190911.shp
   admin_level_max: 1
   admin2_name: cod_admbnda_adm2_rgc_20190911.shp
 fewsnet:
   region_name: southern-africa
 glofas:
   reporting_points:
```

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/config/countries/eth.yaml` & `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/eth.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 iso3: eth
 codab:
-  hdx_dataset_name: ETH Administrative Divisions Shapefiles.zip
-  layer_base_name: eth_admbnda_adm{admin_level}_csa_bofed_20201008.shp
+  hdx_resource_name: eth_adm_csa_bofedb_2021_SHP.zip
+  layer_base_name: eth_admbnda_adm{admin_level}_csa_bofedb_2021.shp
   admin_level_max: 3
-  admin0_name: eth_admbnda_adm0_csa_bofedb_itos_2021
+  admin0_name: eth_admbnda_adm0_csa_bofedb_itos_2021.shp
 fewsnet:
   region_name: east-africa
 glofas:
   reporting_points:
   - name: Abetlti
     lon: 37.55
     lat: 8.25
```

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/config/countries/mwi.yaml` & `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/mwi.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 iso3: mwi
 codab:
-  hdx_dataset_name: mwi_adm_nso_20181016_SHP.zip
-  layer_base_name: mwi_admbnda_adm{admin_level}_nso_20181016.shp
+  hdx_resource_name: mwi_adm_nso_hotosm_20230405_SHP.zipSHP
+  layer_base_name: mwi_admbnda_adm{admin_level}_nso_hotosm_20230405.shp
   admin_level_max: 3
 fewsnet:
   region_name: southern-africa
 glofas:
   reporting_points:
   - name: Chikwawa
     lon: 34.85
```

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/config/countries/npl.yaml` & `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/npl.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 iso3: npl
 codab:
-  hdx_dataset_name: npl_admbnda_nd_20201117_SHP.zip
-  layer_base_name: npl_admbnda_adm{admin_level}_nd_20201117.shp
-  admin_level_max: 2
-  # Nepal also has districts that don't fall into a particular admin level
-  custom_layer_names:
-    - npl_admbnda_districts_nd_20201117
+  hdx_resource_name: npl_adm_nd_20190430_SHP.zip
+  layer_base_name: npl_admbnda_adm{admin_level}_nd_20190430.shp
+  admin_level_max: 3
 glofas:
   reporting_points:
   - name: After Lothar Confluence
     lon: 84.65
     lat: 27.55
   - name: Angsing
     lon: 83.75
```

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/config/countryconfig.py` & `ocha-anticipy-1.1.0/src/ochanticipy/config/countryconfig.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,40 +8,58 @@
 
 
 class CodABConfig(BaseModel):
     """COD AB configuration.
 
     Parameters
     ----------
-    hdx_dataset_name: str
-        COD AB dataset name on HDX. Can be found by taking the filename as it
-        appears on the dataset page.
+    admin_level_max: int
+         The maximum admin level available in the shapefile, cannot be
+         greater than 4. If ``hdx_resource_name`` is a list, then
+         ``admin_level_max`` must match the number of items in
+         ``hdx_resource_name``.
+    hdx_resource_name: Union[str, List[str]]
+        COD AB resource name on HDX. Can be found by taking the filename as it
+        appears on the COD AB dataset page. If individual COD AB files are
+        contained in separate resources, provide each filename in a list, where
+        the index is equivalent to admin level.
     layer_base_name: str
         The base name of the different admin layers, that presumably only
         change by a single custom_layer_number depending on the level. Should
         contain {admin_level} in place of the custom_layer_number.
-    admin_level_max: int
-         The maximum admin level available in the shapefile, cannot be
-         greater than 4
     admin{level}_name: str, optional
         The names of any admin level layers that do not conform to the
         layer_base_name pattern, where {level} ranges from 0 to 4
     custom_layer_names: list, optional
         Any additional layer names that don't fit into the admin level paradigm
     """
 
-    hdx_dataset_name: str
-    layer_base_name: str
     admin_level_max: int
+    hdx_resource_name: Union[str, List[str]]
+    layer_base_name: str
     admin0_name: Optional[str]
     admin1_name: Optional[str]
     admin2_name: Optional[str]
     admin3_name: Optional[str]
     admin4_name: Optional[str]
-    custom_layer_names: Optional[list]
+    custom_layer_names: Optional[List[str]]
+
+    @validator("hdx_resource_name")
+    def _validate_hdx_resource_name(cls, hdx_resource_name, values):
+        """Ensure hdx_resource_name is str or list for all admin areas."""
+        if isinstance(hdx_resource_name, list) and (
+            len(hdx_resource_name) != values["admin_level_max"] + 1
+        ):
+            raise ValueError(
+                "In the COD AB section of the country configuration file, "
+                "hdx_resource_name should be a string or list of length "
+                "admin_level_max, with a resource provided for each level "
+                "from 0 to admin_level_max."
+            )
+        return hdx_resource_name
 
     @validator("layer_base_name")
     def _validate_layer_base_name(cls, layer_base_name):
         """Ensure that the layer basename contains {admin_level}."""
         if "{admin_level}" not in layer_base_name:
             raise ValueError(
                 "In the COD AB section of the country configuration file, "
```

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/datasources/chirps/chirps.py` & `ocha-anticipy-1.1.0/src/ochanticipy/datasources/chirps/chirps.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,14 @@
             year=year, month=month, day=day
         )
 
     def _get_processed_path(self, raw_path: Path) -> Path:
         return self._processed_base_dir / raw_path.parts[-1]
 
     def _get_location_url(self):
-
         location_url = (
             f"X/%28{self._geobb.lon_min}%29%28{self._geobb.lon_max}"
             f"%29RANGEEDGES/"
             f"Y/%28{self._geobb.lat_max}%29%28{self._geobb.lat_min}"
             f"%29RANGEEDGES/"
         )
 
@@ -326,15 +325,14 @@
         ]
         filepath_list.sort()
 
         return filepath_list
 
     @staticmethod
     def _read_csv_from_url(url):
-
         context = ssl.create_default_context()
         context.set_ciphers("DEFAULT")
         result = urlopen(url, context=context)
 
         return pd.read_csv(result)
 
     @check_file_existence
@@ -417,15 +415,14 @@
 
     def _get_file_name(
         self,
         year: str,
         month: str,
         day: str,
     ) -> str:
-
         file_name_base = self._get_file_name_base(
             year=year,
             month=month,
         )
 
         file_name = (
             f"{file_name_base}"
@@ -451,15 +448,14 @@
             1
         ]
         datetime_object = datetime_object.replace(day=day)
 
         return datetime_object.date()
 
     def _get_url(self, year: str, month: str, day: str) -> str:
-
         # Convert month from month number (in string format) to
         # three-letter name
         month_name = calendar.month_abbr[int(month)]
 
         location_url = self._get_location_url()
 
         url = (
@@ -550,15 +546,14 @@
 
     def _get_file_name(
         self,
         year: str,
         month: str,
         day: str,
     ) -> str:
-
         file_name_base = self._get_file_name_base(
             year=year,
             month=month,
         )
 
         if len(day) == 1:
             day = f"0{day}"
@@ -585,15 +580,14 @@
         df = self._read_csv_from_url(url)
 
         datetime_object = datetime.strptime(df.values[0][0], "%d %b %Y")
 
         return datetime_object.date()
 
     def _get_url(self, year: str, month: str, day: str) -> str:
-
         # Convert month from month number (in string format) to
         # three-letter name
         month_name = calendar.month_abbr[int(month)]
 
         location_url = self._get_location_url()
 
         url = (
```

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/datasources/codab/codab.py` & `ocha-anticipy-1.1.0/src/ochanticipy/datasources/codab/codab.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Download and manipulate COD administrative boundaries."""
 import logging
 from pathlib import Path
+from typing import List, Union
 
 import geopandas as gpd
 from fiona.errors import DriverError
 
 from ochanticipy.config.countryconfig import CountryConfig
 from ochanticipy.datasources.datasource import DataSource
 from ochanticipy.utils.check_file_existence import check_file_existence
-from ochanticipy.utils.hdx_api import load_dataset_from_hdx
+from ochanticipy.utils.hdx_api import load_resource_from_hdx
 
 logger = logging.getLogger(__name__)
 
 
 class CodAB(DataSource):
     """
     Work with COD AB (administrative boundaries).
@@ -26,62 +27,81 @@
     def __init__(self, country_config: CountryConfig):
         super().__init__(
             country_config,
             datasource_base_dir="cod_ab",
             is_public=True,
             config_datasource_name="codab",
         )
-        self._raw_filepath = (
-            self._raw_base_dir / f"{self._country_config.iso3}_"
-            f"{self._datasource_base_dir}.shp.zip"
-        )
 
-    def download(self, clobber: bool = False) -> Path:
+        # account for files stored across multiple resources
+        res_name = self._datasource_config.hdx_resource_name
+        self._multiple_resources = isinstance(res_name, list)
+
+        if self._multiple_resources:
+            zip_filenames = [
+                f"{self._country_config.iso3}_adm{i}.shp.zip"
+                for i in range(len(res_name))
+            ]
+            self._hdx_resource_list = res_name
+        else:
+            zip_filenames = [f"{self._country_config.iso3}_adm.shp.zip"]
+            self._hdx_resource_list = [res_name]
+
+        # generate filepaths for all resource zipfiles
+        self._raw_filepaths = [
+            (self._raw_base_dir / fn) for fn in zip_filenames
+        ]
+
+    def download(self, clobber: bool = False) -> Union[Path, List[Path]]:
         """
         Download COD AB file from HDX.
 
         Parameters
         ----------
         clobber : bool, default = False
             If True, overwrites existing COD AB files
 
         Returns
         -------
-        The downloaded filepath
+        The downloaded filepath(s)
 
         Examples
         --------
         >>> from ochanticipy import create_country_config, CodAB
         >>> # Download COD administrative boundaries for Nepal
         >>> country_config = create_country_config(iso3="npl")
         >>> codab = CodAB(country_config=country_config)
         >>> npl_cod_shapefile = codab.download()
         """
-        return self._download(
-            filepath=self._raw_filepath,
-            hdx_address=f"cod-ab-{self._country_config.iso3}",
-            hdx_dataset_name=self._datasource_config.hdx_dataset_name,
-            clobber=clobber,
-        )
+        for filepath, hdx_resource_name in zip(
+            self._raw_filepaths, self._hdx_resource_list
+        ):
+            self._download(
+                filepath=filepath,
+                hdx_dataset=f"cod-ab-{self._country_config.iso3}",
+                hdx_resource_name=hdx_resource_name,
+                clobber=clobber,
+            )
+        return self._raw_base_dir
 
     def process(self, *args, **kwargs):
         """
         Process COD AB data.
 
         Method not implemented.
         """
         logger.info("`process()` method not implemented for CodAB.")
 
-    def load(self, admin_level: int) -> gpd.GeoDataFrame:  # type: ignore
+    def load(self, admin_level: int = 0) -> gpd.GeoDataFrame:  # type: ignore
         """
         Get the COD AB data by admin level.
 
         Parameters
         ----------
-        admin_level: int
+        admin_level: int, default = 0
             The administrative level
 
         Returns
         -------
         COD AB geodataframe with specified admin level
 
         Raises
@@ -106,15 +126,16 @@
                 f"Admin level {admin_level} requested, but maximum set to "
                 f"{admin_level_max} in {self._country_config.iso3.upper()} "
                 f"config file"
             )
         return self._load_admin_layer(
             layer_name=getattr(
                 self._datasource_config, f"admin{admin_level}_name"
-            )
+            ),
+            admin_level=admin_level,
         )
 
     def load_custom(self, custom_layer_number: int = 0) -> gpd.GeoDataFrame:
         """
         Get the COD AB data from a custom (non-level) layer.
 
         Parameters
@@ -146,41 +167,48 @@
         # TODO: possibly merge the two load methods
         try:
             # Ignore mypy for this line because custom_layer_names could be
             # None, but this is handled by the caught exceptions
             layer_name = self._datasource_config.custom_layer_names[
                 custom_layer_number
             ]  # type: ignore
+
         except (IndexError, TypeError) as err:
             raise AttributeError(
                 f"{custom_layer_number}th custom layer requested but not "
                 f"available in {self._country_config.iso3.upper()} config file"
             ) from err
-        return self._load_admin_layer(layer_name=layer_name)
+        return self._load_admin_layer(
+            layer_name=layer_name,
+            admin_level=0,  # breaks if layer in multiple resources
+        )
+
+    def _load_admin_layer(
+        self, layer_name: str, admin_level: int
+    ) -> gpd.GeoDataFrame:
+        fp_index = int(admin_level) if self._multiple_resources else 0
 
-    def _load_admin_layer(self, layer_name: str) -> gpd.GeoDataFrame:
         try:
-            return gpd.read_file(
-                f"zip://{(self._raw_filepath / layer_name).as_posix()}"
-            )
+            zip_path = self._raw_filepaths[fp_index] / layer_name
+            return gpd.read_file(f"zip://{zip_path.as_posix()}")
         except DriverError as err:
             raise FileNotFoundError(
                 f"Could not read boundary shapefile. Make sure that "
                 f"you have already called the 'download' method and "
-                f"that the file {self._raw_filepath} exists. If it does "
-                f"exist, please check the validity of the layer name: "
-                f"'{layer_name}'."
+                f"that the file {self._raw_filepaths[fp_index]} exists."
+                f"If it does exist, please check the validity of the "
+                f"layer name: '{layer_name}'."
             ) from err
 
     @check_file_existence
     def _download(
         self,
         filepath: Path,
-        hdx_address: str,
-        hdx_dataset_name: str,
+        hdx_dataset: str,
+        hdx_resource_name: str,
         clobber: bool,
     ) -> Path:
-        return load_dataset_from_hdx(
-            hdx_address=hdx_address,
-            hdx_dataset_name=hdx_dataset_name,
+        return load_resource_from_hdx(
+            hdx_dataset=hdx_dataset,
+            hdx_resource_name=hdx_resource_name,
             output_filepath=filepath,
         )
```

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/datasources/datasource.py` & `ocha-anticipy-1.1.0/src/ochanticipy/datasources/datasource.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/datasources/fewsnet/fewsnet.py` & `ocha-anticipy-1.1.0/src/ochanticipy/datasources/fewsnet/fewsnet.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/datasources/glofas/forecast.py` & `ocha-anticipy-1.1.0/src/ochanticipy/datasources/glofas/forecast.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,26 +183,26 @@
 
 
 class GlofasReforecast(_GlofasForecastBase):
     """
     Class for downloading and processing GloFAS reforecast data.
 
     The GloFAS reforecast dataset is a global raster presenting river
-    discharnge forecasted from 1999 until 2018, see
+    discharge forecasted from 1999 until 2018, see
     `this paper <https://hess.copernicus.org/preprints/hess-2020-532/>`_
     for more details.
 
     This class downloads the raw raster data
     `from CDS
     <https://cds.climate.copernicus.eu/cdsapp#!/dataset/cems-glofas-reforecast?tab=overview>`__,
     and processes it from a raster to a datasets of reporting points from the
     `GloFAS interface
     <https://www.globalfloods.eu/glofas-forecasting/>`_.
-     Due to the CDS request size limits, separate files are downloaded per
-     month (that contain all requested lead times).
+    Due to the CDS request size limits, separate files are downloaded per
+    month (that contain all requested lead times).
 
     Parameters
     ----------
     country_config : CountryConfig
         Country configuration
     geo_bounding_box: GeoBoundingBox
         The bounding coordinates of the area that should be included
```

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/datasources/glofas/glofas.py` & `ocha-anticipy-1.1.0/src/ochanticipy/datasources/glofas/glofas.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,31 +3,38 @@
 import time
 from abc import abstractmethod
 from dataclasses import dataclass
 from datetime import date
 from pathlib import Path
 from typing import List, Tuple, Union
 
-import cdsapi
 import numpy as np
 import xarray as xr
 from dateutil import rrule
 
 from ochanticipy.config.countryconfig import CountryConfig
 from ochanticipy.datasources.datasource import DataSource
+from ochanticipy.utils.check_extra_imports import check_extra_imports
 from ochanticipy.utils.dates import get_date_from_user_input
 from ochanticipy.utils.geoboundingbox import GeoBoundingBox
 
 _MODULE_BASENAME = "glofas"
 _HYDROLOGICAL_MODEL = "lisflood"
 _RIVER_DISCHARGE_VAR = "dis24"
+_CDS_MAX_REQUESTS = 500
 _REQUEST_SLEEP_TIME = 60  # seconds
 
 logger = logging.getLogger(__name__)
 
+# putting on top level to ensure easy mocking in tests
+try:
+    import cdsapi
+except ModuleNotFoundError:
+    pass
+
 
 @dataclass
 class _QueryParams:
     """
     Class to keep track of CDS query input and output.
 
     Parameters
@@ -100,14 +107,19 @@
         leadtime_max: int = None,
     ):
         super().__init__(
             country_config=country_config,
             datasource_base_dir=_MODULE_BASENAME,
             is_public=True,
         )
+        # check that extra dependencies are installed
+        check_extra_imports(
+            libraries=["cdsapi", "cfgrib"], subpackage="glofas"
+        )
+
         # The GloFAS API on CDS requires coordinates have the format x.x5
         self._geo_bounding_box = geo_bounding_box.round_coords(
             offset_val=0.05, round_val=0.1
         )
         self._start_date, self._end_date = _set_dates(
             start_date_min=start_date_min,
             end_date_max=end_date_max,
@@ -123,14 +135,23 @@
         self._leadtime_max = leadtime_max
         self._forecast_type = type(self).__name__.replace("Glofas", "").lower()
         self._date_range = rrule.rrule(
             freq=self._frequency,
             dtstart=self._start_date,
             until=self._end_date,
         )
+        if self._date_range.count() > _CDS_MAX_REQUESTS:
+            msg = (
+                f"Your parameters would result in "
+                f"{self._date_range.count()} requests, however we "
+                f"currently only support the CDS maximum of "
+                f"{_CDS_MAX_REQUESTS} at this time. Please divide your "
+                f"query into multiple instances."
+            )
+            raise RuntimeError(msg)
 
     def download(  # type: ignore
         self,
         clobber: bool = False,
     ) -> List[Path]:
         """
         Download the GloFAS data by querying CDS.
@@ -366,14 +387,15 @@
                 for query_params in query_params_list
                 if not query_params.downloaded
             ]
             # Sleep a bit before the next loop so that we're not
             # hammering on cds
             if query_params_list:
                 time.sleep(_REQUEST_SLEEP_TIME)
+                logger.info(f"Sleeping for {_REQUEST_SLEEP_TIME} s")
         return downloaded_filepaths
 
     def _get_query(
         self,
         year: int,
         month: int = None,
         day: int = None,
```

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/datasources/glofas/reanalysis.py` & `ocha-anticipy-1.1.0/src/ochanticipy/datasources/glofas/reanalysis.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/datasources/iri/iri_seasonal_forecast.py` & `ocha-anticipy-1.1.0/src/ochanticipy/datasources/iri/iri_seasonal_forecast.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,14 @@
     def _get_raw_path(self) -> Path:
         return self._raw_base_dir / self._get_file_name()
 
     def _get_processed_path(self) -> Path:
         return self._processed_base_dir / self._get_file_name()
 
     def _get_url(self) -> str:
-
         base_url = (
             "https://iridl.ldeo.columbia.edu/SOURCES/.IRI/.FD/"
             f".NMME_Seasonal_Forecast/.Precipitation_ELR/"
             f".{self._forecast_type}/"
         )
         return (
             f"{base_url}"
@@ -186,15 +185,14 @@
                 f"and that the file {self._get_raw_path()} exists. "
             ) from err
 
     @check_file_existence
     def _download(
         self, filepath: Path, url: str, iri_auth: str, clobber: bool
     ) -> Path:
-
         response = requests.get(
             url,
             # have to authenticate by using a cookie
             cookies={"__dlauth_id": iri_auth},
         )
         if response.headers["Content-Type"] != "application/x-netcdf":
             msg = (
```

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/datasources/usgs/ndvi_base.py` & `ocha-anticipy-1.1.0/src/ochanticipy/datasources/usgs/ndvi_base.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/datasources/usgs/ndvi_products.py` & `ocha-anticipy-1.1.0/src/ochanticipy/datasources/usgs/ndvi_products.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/utils/check_file_existence.py` & `ocha-anticipy-1.1.0/src/ochanticipy/utils/check_file_existence.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     # check existence
     exist_dict = {True: "exists", False: "does not exist"}
 
     # check filepath exists -> clobber
     usage_dict = {
         True: {True: "overwriting existing", False: "using existing"},
-        False: {True: "downloading new", False: "downloading new"},
+        False: {True: "creating new", False: "creating new"},
     }
     fp_exists = filepath.exists()
 
     logger.info(
         f"File {filepath} {exist_dict[fp_exists]} and clobber "
         f"set to {clobber}, {usage_dict[fp_exists][clobber]} file."
     )
```

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/utils/dates.py` & `ocha-anticipy-1.1.0/src/ochanticipy/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/utils/geoboundingbox.py` & `ocha-anticipy-1.1.0/src/ochanticipy/utils/geoboundingbox.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/utils/hdx_api.py` & `ocha-anticipy-1.1.0/src/ochanticipy/utils/hdx_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,45 +11,45 @@
 
 logger = logging.getLogger(__name__)
 Configuration.create(
     hdx_site="prod", user_agent=USER_AGENT, hdx_read_only=True
 )
 
 
-def load_dataset_from_hdx(
-    hdx_address: str, hdx_dataset_name: str, output_filepath: Path
+def load_resource_from_hdx(
+    hdx_dataset: str, hdx_resource_name: str, output_filepath: Path
 ) -> Path:
     """
     Use the HDX API to download a dataset based on the address and dataset ID.
 
     Parameters
     ----------
-    hdx_address : str
-        The page where the dataset resides on on HDX. Can be found
+    hdx_dataset : str
+        The name of the HDX dataset where the resource is located. Can be found
         by taking the portion of the url after ``data.humdata.org/dataset/``
-    hdx_dataset_name : str
-        Dataset name on HDX. Can be found by taking the filename as it
+    hdx_resource_name : str
+        Resources name on HDX. Can be found by taking the filename as it
         appears on the dataset page.
     output_filepath : Path
         Target filepath for the dataset
 
     Returns
     -------
     The full path of the downloaded dataset
 
     """
-    logger.info(f"Querying HDX API for dataset {hdx_address}")
-    resources = Dataset.read_from_hdx(hdx_address).get_resources()
+    logger.info(f"Querying HDX API for dataset {hdx_dataset}")
+    resources = Dataset.read_from_hdx(hdx_dataset).get_resources()
     logger.debug(f"Found the following resources: {resources}")
     for resource in resources:
-        if resource["name"] == hdx_dataset_name:
-            logger.info(f"Downloading dataset {hdx_dataset_name}")
+        if resource["name"] == hdx_resource_name:
+            logger.info(f"Downloading dataset {hdx_resource_name}")
             with tempfile.TemporaryDirectory() as tempdir:
                 _, downloaded_filepath = resource.download(folder=tempdir)
                 output_filepath.parent.mkdir(parents=True, exist_ok=True)
                 shutil.copy(downloaded_filepath, output_filepath)
             logger.info(f"Saved to {output_filepath}")
             return Path(output_filepath)
     raise FileNotFoundError(
-        f'Dataset with name "{hdx_dataset_name}" not found'
-        f'at HDX address "{hdx_address}".'
+        f'Dataset with name "{hdx_resource_name}" not found'
+        f'at HDX address "{hdx_dataset}".'
     )
```

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/utils/io.py` & `ocha-anticipy-1.1.0/src/ochanticipy/utils/io.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/src/ochanticipy/utils/raster.py` & `ocha-anticipy-1.1.0/src/ochanticipy/utils/raster.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,21 +50,21 @@
     _crs: CRS
 
     def __init__(self, xarray_obj):
         super().__init__(xarray_obj)
 
         # Adding lat/lon to set of default spatial dims
         if "lat" in self._obj.dims and "lon" in self._obj.dims:
-            self._x_dim = "lon"
-            self._y_dim = "lat"
+            self._x_dim = self._obj.rio._x_dim = "lon"
+            self._y_dim = self._obj.rio._y_dim = "lat"
 
         # Adding Y/X to set of default spatial dims
         if "Y" in self._obj.dims and "X" in self._obj.dims:
-            self._x_dim = "X"
-            self._y_dim = "Y"
+            self._x_dim = self._obj.rio._x_dim = "X"
+            self._y_dim = self._obj.rio._y_dim = "Y"
 
         # Managing time coordinate default dims
         self._t_dim = None
         for t in ["t", "T", "time"]:
             if t in self._obj.dims:
                 self._t_dim = t
 
@@ -529,15 +529,15 @@
                     dim=[self.x_dim, self.y_dim], **kwargs
                 ).rename(stat)
                 grid_stat_all.append(grid_stat)
 
             if percentile_list is not None:
                 grid_quant = [
                     da_clip.quantile(quant / 100, dim=[self.x_dim, self.y_dim])
-                    .drop("quantile")
+                    .drop_vars("quantile")
                     .rename(f"{quant}quant")
                     for quant in percentile_list
                 ]
                 grid_stat_all.extend(grid_quant)
 
             # if dims is 0, it throws an error when merging
             # and then converting to a df
```

### Comparing `ocha-anticipy-1.0.2/tests/datasources/conftest.py` & `ocha-anticipy-1.1.0/tests/datasources/conftest.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/tests/datasources/test_chirps.py` & `ocha-anticipy-1.1.0/tests/datasources/test_chirps.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/tests/datasources/test_codab.py` & `ocha-anticipy-1.1.0/tests/datasources/test_codab.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,67 @@
 """Test COD AB methods."""
+from unittest.mock import call
+
 import pytest
 
-from ochanticipy import CodAB
+from ochanticipy import CodAB, create_custom_country_config
 
 DATASOURCE_BASE_DIR = "cod_ab"
+MULTI_RESOURCE_CONFIG = "tests/datasources/fake_codab_multi.yaml"
+
+
+@pytest.fixture
+def mock_config_multi():
+    """Fixture for CODAB with multiple resources."""
+    return create_custom_country_config(filepath=MULTI_RESOURCE_CONFIG)
 
 
 @pytest.fixture
 def downloader(mocker):
     """Mock the HDX download function."""
     return mocker.patch(
-        "ochanticipy.datasources.codab.codab.load_dataset_from_hdx"
+        "ochanticipy.datasources.codab.codab.load_resource_from_hdx"
     )
 
 
 @pytest.fixture
 def gpd_read_file(mocker):
     """Mock GeoPandas file reading function."""
     return mocker.patch("ochanticipy.datasources.codab.codab.gpd.read_file")
 
 
 def test_codab_download(mock_aa_data_dir, mock_country_config, downloader):
     """Test that load_codab calls the HDX API to download."""
     codab = CodAB(country_config=mock_country_config)
     codab.download()
     downloader.assert_called_with(
-        hdx_address=f"cod-ab-{mock_country_config.iso3}",
-        hdx_dataset_name=mock_country_config.codab.hdx_dataset_name,
+        hdx_dataset=f"cod-ab-{mock_country_config.iso3}",
+        hdx_resource_name=mock_country_config.codab.hdx_resource_name,
         output_filepath=mock_aa_data_dir
         / f"public/raw/{mock_country_config.iso3}/"
-        f"{DATASOURCE_BASE_DIR}/{mock_country_config.iso3}_"
-        f"{DATASOURCE_BASE_DIR}.shp.zip",
+        f"{DATASOURCE_BASE_DIR}/{mock_country_config.iso3}_adm.shp.zip",
+    )
+
+
+def test_codab_download_multi(mock_aa_data_dir, mock_config_multi, downloader):
+    """Test that download calls the HDX API to download for multi resources."""
+    codab = CodAB(country_config=mock_config_multi)
+    codab.download()
+    downloader.assert_has_calls(
+        [
+            call(
+                hdx_dataset=f"cod-ab-{mock_config_multi.iso3}",
+                hdx_resource_name=mock_config_multi.codab.hdx_resource_name[i],
+                output_filepath=mock_aa_data_dir
+                / f"public/raw/{mock_config_multi.iso3}/"
+                f"{DATASOURCE_BASE_DIR}/{mock_config_multi.iso3}_"
+                f"adm{i}.shp.zip",
+            )
+            for i in range(4)
+        ]
     )
 
 
 def test_codab_load_admin_level(
     mock_aa_data_dir, mock_country_config, gpd_read_file
 ):
     """Test that load_codab retrieves expected file and layer name."""
@@ -43,61 +70,79 @@
     # First checking layer_base_name
     expected_layer_name = "fake_layer_base_name_level1"
     codab.load(admin_level=1)
 
     gpd_read_file.assert_called_with(
         f"zip://{mock_aa_data_dir}/public/raw/{mock_country_config.iso3}/"
         f"{DATASOURCE_BASE_DIR}/{mock_country_config.iso3}_"
-        f"{DATASOURCE_BASE_DIR}.shp.zip/{expected_layer_name}"
+        f"adm.shp.zip/{expected_layer_name}"
     )
 
     # Then checking custom name
     expected_layer_name = "admin2_custom_name"
     codab.load(admin_level=2)
 
     gpd_read_file.assert_called_with(
         f"zip://{mock_aa_data_dir}/public/raw/{mock_country_config.iso3}/"
         f"{DATASOURCE_BASE_DIR}/{mock_country_config.iso3}_"
-        f"{DATASOURCE_BASE_DIR}.shp.zip/{expected_layer_name}"
+        f"adm.shp.zip/{expected_layer_name}"
+    )
+
+
+def test_codab_multi_load_admin_level(
+    mock_aa_data_dir, mock_config_multi, gpd_read_file
+):
+    """Test that load_codab retrieves expected file and layer name."""
+    codab = CodAB(country_config=mock_config_multi)
+
+    # First checking layer_base_name
+    expected_layer_name = "fake_layer_base_name_level1"
+    codab.load(admin_level=1)
+
+    gpd_read_file.assert_called_with(
+        f"zip://{mock_aa_data_dir}/public/raw/{mock_config_multi.iso3}/"
+        f"{DATASOURCE_BASE_DIR}/{mock_config_multi.iso3}_"
+        f"adm1.shp.zip/{expected_layer_name}"
     )
 
 
 def test_codab_too_high_admin_level(mock_country_config):
     """Test raised error when too high admin level requested."""
     codab = CodAB(country_config=mock_country_config)
     with pytest.raises(AttributeError):
         codab.load(admin_level=10)
 
 
 def test_codab_custom(mock_aa_data_dir, mock_country_config, gpd_read_file):
     """Test that load_codab_custom retrieves expected file and layer name."""
     custom_layer_number = 1
     custom_layer_name_list = ["custom_layer_A", "custom_layer_B"]
+
     mock_country_config.codab.custom_layer_names = custom_layer_name_list
     codab = CodAB(country_config=mock_country_config)
     codab.load_custom(custom_layer_number)
     gpd_read_file.assert_called_with(
         f"zip://{mock_aa_data_dir}/public/raw/{mock_country_config.iso3}/"
         f"{DATASOURCE_BASE_DIR}/{mock_country_config.iso3}_"
-        f"{DATASOURCE_BASE_DIR}.shp.zip/"
+        f"adm.shp.zip/"
         f"{custom_layer_name_list[custom_layer_number]}"
     )
 
 
 def test_codab_custom_missing(mock_country_config, gpd_read_file):
     """Test raised error when custom COD AB missing."""
     codab = CodAB(country_config=mock_country_config)
     with pytest.raises(AttributeError):
         codab.load_custom(0)
 
 
 def test_codab_load_fail(mock_country_config):
     """Test raises file not found error when load fails."""
     codab = CodAB(country_config=mock_country_config)
-    # Remove file if it exists
-    codab._raw_filepath.unlink(missing_ok=True)
+    # Remove file for admin0 if it exists
+    codab._raw_filepaths[0].unlink(missing_ok=True)
     with pytest.raises(FileNotFoundError) as excinfo:
         codab.load(admin_level=0)
     assert (
         "Make sure that you have already called the 'download' method"
         in str(excinfo.value)
     )
```

### Comparing `ocha-anticipy-1.0.2/tests/datasources/test_datasource.py` & `ocha-anticipy-1.1.0/tests/datasources/test_datasource.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/tests/datasources/test_fewsnet.py` & `ocha-anticipy-1.1.0/tests/datasources/test_fewsnet.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/tests/datasources/test_glofas_download.py` & `ocha-anticipy-1.1.0/tests/datasources/test_glofas_download.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,17 +24,18 @@
         "ochanticipy.datasources.glofas.glofas.cdsapi.Client.retrieve"
     )
 
 
 @pytest.fixture
 def mock_result(mocker):
     """Mock the entire Result class."""
-    # This is needed because the reply is changed dynamically
-    # so very difficult to use a Mock object
+
     class MockResult:
+        """Reply changes dynamically so need mock object."""
+
         def __init__(self, *args, **kwargs):
             self.reply = {"state": "completed"}
             self.state = None
 
         def update(self):
             pass
 
@@ -57,14 +58,15 @@
 
 def test_reanalysis_download(
     mock_country_config,
     mock_aa_data_dir,
     mock_retrieve,
     mock_result,
     geo_bounding_box,
+    mocker,
 ):
     """
     Test GloFAS reanalysis download.
 
     Test that the query generated by the download method of GlofasReanlysis
     with default parameters is as expected
     """
```

### Comparing `ocha-anticipy-1.0.2/tests/datasources/test_glofas_process.py` & `ocha-anticipy-1.1.0/tests/datasources/test_glofas_process.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/tests/datasources/test_iri.py` & `ocha-anticipy-1.1.0/tests/datasources/test_iri.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/tests/datasources/test_ndvi.py` & `ocha-anticipy-1.1.0/tests/datasources/test_ndvi.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         "smoothed": UsgsNdviSmoothed,
         "pct_median": UsgsNdviPctMedian,
         "anomaly": UsgsNdviMedianAnomaly,
         "difference": UsgsNdviYearDifference,
     }
 
     def _mock_ndvi(variable: str = "smoothed"):
-
         ndvi = instantiator[variable](
             country_config=mock_country_config,
             start_date=start_date,
             end_date=end_date,
         )
         return ndvi
```

### Comparing `ocha-anticipy-1.0.2/tests/test_country_config.py` & `ocha-anticipy-1.1.0/tests/test_country_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 
 def test_codab_validate_layer_base_name(mock_parse_yaml):
     """Test that layer basename requires correct placeholder."""
     config_base = {
         "iso3": "abc",
         "codab": {
-            "hdx_dataset_name": "fake_dataset_name",
+            "hdx_resource_name": "fake_resource_name",
             "layer_base_name": "layer_base_name_",
             "admin_level_max": 1,
         },
     }
     config_correct = copy.deepcopy(config_base)
     config_correct["codab"]["layer_base_name"] += "{admin_level}"
     config_incorrect = copy.deepcopy(config_base)
@@ -95,15 +95,15 @@
 
 
 def test_codab_validate_admin_level_max(mock_parse_yaml):
     """Test that admin level can only be between 0 and 4."""
     config_base = {
         "iso3": "abc",
         "codab": {
-            "hdx_dataset_name": "fake_dataset_name",
+            "hdx_resource_name": "fake_resource_name",
             "layer_base_name": "layer_base_name_{admin_level}",
             "admin_level_max": 1,
         },
     }
     config_correct = copy.deepcopy(config_base)
     config_incorrect_a = copy.deepcopy(config_base)
     config_incorrect_a["codab"]["admin_level_max"] = -1
@@ -115,14 +115,44 @@
     # Check that correct config runs without issue
     create_country_config(iso3="abc")
     # Check that incorrect config raises error for config incorrect a
     with pytest.raises(ValueError):
         create_country_config(iso3="abc")
     # Check that incorrect config raises error for config incorrect b
     with pytest.raises(ValueError):
+        create_country_config(iso3="abc")
+
+
+def test_codab_validate_multiple_resources(mock_parse_yaml):
+    """Test that multiple resources must match admin levels."""
+    config_base = {
+        "iso3": "abc",
+        "codab": {
+            "hdx_resource_name": [f"fake_resource_name_{i}" for i in range(4)],
+            "layer_base_name": "layer_base_name_{admin_level}",
+            "admin_level_max": 3,
+        },
+    }
+    config_correct = copy.deepcopy(config_base)
+    config_incorrect_a = copy.deepcopy(config_base)
+    config_incorrect_a["codab"]["admin_level_max"] = 2
+    config_incorrect_b = copy.deepcopy(config_base)
+    config_incorrect_b["codab"]["admin_level_max"] = 4
+
+    mock_parse_yaml(
+        output_list=[config_correct, config_incorrect_a, config_incorrect_b]
+    )
+
+    # Check that correct config runs without issue
+    create_country_config(iso3="abc")
+    # Check that incorrect config raises error for config incorrect a
+    with pytest.raises(ValueError):
+        create_country_config(iso3="abc")
+    # Check that incorrect config raises error for config incorrect b
+    with pytest.raises(ValueError):
         create_country_config(iso3="abc")
 
 
 def test_fewsnet_validate_region_name(mock_parse_yaml):
     """Test that fewsnet requires correct region name."""
     config_base = {
         "iso3": "abc",
```

### Comparing `ocha-anticipy-1.0.2/tests/utils/test_check_file_existence.py` & `ocha-anticipy-1.1.0/tests/utils/test_check_file_existence.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     """Test that function returned if Path does not exist."""
     caplog.set_level(logging.INFO)
     path_new = tmp_path / "new_path"
     output_filepath = downloader(filepath=path_new, clobber=False)
     assert output_filepath == "a"
     assert (
         f"File {path_new} does not exist and clobber set to "
-        "False, downloading new file." in caplog.text
+        "False, creating new file." in caplog.text
     )
 
 
 def test_key_error(tmp_path):
     """Test that KeyError raised when filepath or clobber not a kwarg."""
     with pytest.raises(KeyError):
         downloader(filepath=tmp_path)
```

### Comparing `ocha-anticipy-1.0.2/tests/utils/test_dates.py` & `ocha-anticipy-1.1.0/tests/utils/test_dates.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/tests/utils/test_geoboundingbox.py` & `ocha-anticipy-1.1.0/tests/utils/test_geoboundingbox.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.2/tests/utils/test_hdx_api.py` & `ocha-anticipy-1.1.0/tests/utils/test_hdx_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Tests for HDX API utility."""
 from collections import UserDict
 
 import pytest
 
-from ochanticipy.utils.hdx_api import load_dataset_from_hdx
+from ochanticipy.utils.hdx_api import load_resource_from_hdx
 
 
 @pytest.fixture(autouse=True)
 def mock_resource(mocker):
     """Mock the HDX download function."""
-    # Resource is a UserDict so need to make a class to mock that
+
     class MockResource(UserDict):
+        """Resource is a UserDict so need to make a class to mock."""
         def download(self, folder):
             return "", "resource_filepath"
 
     mock_dataset = mocker.patch(
         "ochanticipy.utils.hdx_api.Dataset.read_from_hdx"
     )
     # read_from_hdx creates an instance, need to mock the instance
@@ -25,23 +26,23 @@
     # Also need to mock out shutil
     mocker.patch("ochanticipy.utils.hdx_api.shutil")
 
 
 def test_returns_filepath(tmp_path):
     """Test that querying HDX API returns expected filepath."""
     input_filepath = tmp_path / "hdx_test_path"
-    output_filepath = load_dataset_from_hdx(
-        hdx_address="hdx_address",
-        hdx_dataset_name="resource1",
+    output_filepath = load_resource_from_hdx(
+        hdx_dataset="hdx_address",
+        hdx_resource_name="resource1",
         output_filepath=input_filepath,
     )
     assert output_filepath == input_filepath
 
 
 def test_error_when_not_found(tmp_path):
     """Test that missing resource raises error."""
     with pytest.raises(FileNotFoundError):
-        load_dataset_from_hdx(
-            hdx_address="hdx_address",
-            hdx_dataset_name="some_name_not_in_fake_resrouce",
+        load_resource_from_hdx(
+            hdx_dataset="hdx_address",
+            hdx_resource_name="some_name_not_in_fake_resrouce",
             output_filepath=tmp_path / "hdx_test_error",
         )
```

### Comparing `ocha-anticipy-1.0.2/tests/utils/test_raster.py` & `ocha-anticipy-1.1.0/tests/utils/test_raster.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,16 +61,16 @@
 
 
 @pytest.fixture
 def da_2d():
     """Create 2d raster array."""
     da = xr.DataArray(
         [[1, 2, 3], [4, 5, 6]],
-        dims=("y", "x"),
-        coords={"y": [1.5, 0.5], "x": [0.5, 1.5, 2.5]},
+        dims=("Y", "X"),
+        coords={"Y": [1.5, 0.5], "X": [0.5, 1.5, 2.5]},
     ).rio.write_crs("EPSG:4326")
     return da
 
 
 @pytest.fixture
 def da_3d():
     """Create 3d raster array."""
@@ -207,7 +207,20 @@
     assert_frame_equal(result, expected_2d, check_dtype=False)
 
 
 def test_get_raster_array_crs(ds_3d):
     """Ensure dataset to array works when CRS set."""
     da = ds_3d.oap.get_raster_array("val")
     assert da.rio.crs == ds_3d.rio.crs
+
+
+def test_auto_dim_detect():
+    """Ensure lat/lon dimensions automatically set."""
+    da = xr.DataArray(
+        [[1, 2, 3], [4, 5, 6]],
+        dims=("lat", "lon"),
+        coords={"lat": [1.5, 0.5], "lon": [0.5, 1.5, 2.5]},
+    ).rio.write_crs("EPSG:4326")
+    assert da.oap.x_dim == "lon"
+    assert da.oap.y_dim == "lat"
+    assert da.rio.x_dim == "lon"
+    assert da.rio.y_dim == "lat"
```

