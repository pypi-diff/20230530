# Comparing `tmp/ocha-anticipy-1.1.0.tar.gz` & `tmp/ocha-anticipy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocha-anticipy-1.1.0.tar", last modified: Tue May 30 13:13:36 2023, max compression
+gzip compressed data, was "ocha-anticipy-1.1.1.tar", last modified: Tue May 30 14:08:00 2023, max compression
```

## Comparing `ocha-anticipy-1.1.0.tar` & `ocha-anticipy-1.1.1.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.523914 ocha-anticipy-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.471913 ocha-anticipy-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.483914 ocha-anticipy-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/.github/workflows/run-python-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      342 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5855 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4455 2023-05-30 13:13:36.523914 ocha-anticipy-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3235 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.487914 ocha-anticipy-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     2438 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/config.rst
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.487914 ocha-anticipy-1.1.0/docs/datasources/
--rw-r--r--   0 runner    (1001) docker     (122)     4362 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/datasources/chirps.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/datasources/codab.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4187 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/datasources/fewsnet.rst
--rw-r--r--   0 runner    (1001) docker     (122)    12684 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/datasources/glofas.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/datasources/iri_seasonal_forecast.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5950 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/datasources/usgs_ndvi.rst
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/datasources.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.487914 ocha-anticipy-1.1.0/docs/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/utilities/raster.rst
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/docs/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)    11353 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2149 2023-05-30 13:13:36.523914 ocha-anticipy-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.475913 ocha-anticipy-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.491914 ocha-anticipy-1.1.0/src/ocha_anticipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4455 2023-05-30 13:13:36.000000 ocha-anticipy-1.1.0/src/ocha_anticipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-05-30 13:13:36.000000 ocha-anticipy-1.1.0/src/ocha_anticipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 13:13:36.000000 ocha-anticipy-1.1.0/src/ocha_anticipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      450 2023-05-30 13:13:36.000000 ocha-anticipy-1.1.0/src/ocha_anticipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-30 13:13:36.000000 ocha-anticipy-1.1.0/src/ocha_anticipy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.491914 ocha-anticipy-1.1.0/src/ochanticipy/
--rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-30 13:13:36.000000 ocha-anticipy-1.1.0/src/ochanticipy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.491914 ocha-anticipy-1.1.0/src/ochanticipy/config/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.503914 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/afg.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/bdi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/bfa.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/bgd.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     3120 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/caf.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/cmr.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/cod.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     3236 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/col.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/eth.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      333 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/hti.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/irq.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/lby.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2933 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/mli.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/mmr.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4181 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/moz.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/mwi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/ner.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1708 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/nga.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/npl.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/pse.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/sdn.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/som.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      399 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/ssd.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/syr.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/tcd.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/ukr.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/ven.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countries/yem.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     8920 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/countryconfig.py
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/config/pathconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.503914 ocha-anticipy-1.1.0/src/ochanticipy/datasources/
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.503914 ocha-anticipy-1.1.0/src/ochanticipy/datasources/chirps/
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/chirps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19875 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/chirps/chirps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.507914 ocha-anticipy-1.1.0/src/ochanticipy/datasources/codab/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/codab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7182 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/codab/codab.py
--rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/datasource.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.507914 ocha-anticipy-1.1.0/src/ochanticipy/datasources/fewsnet/
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/fewsnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13942 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/fewsnet/fewsnet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.507914 ocha-anticipy-1.1.0/src/ochanticipy/datasources/glofas/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/glofas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9849 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/glofas/forecast.py
--rw-r--r--   0 runner    (1001) docker     (122)    19202 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/glofas/glofas.py
--rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/glofas/reanalysis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.507914 ocha-anticipy-1.1.0/src/ochanticipy/datasources/iri/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/iri/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10404 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/iri/iri_seasonal_forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.511914 ocha-anticipy-1.1.0/src/ochanticipy/datasources/usgs/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/usgs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28079 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/usgs/ndvi_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    10009 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/datasources/usgs/ndvi_products.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.511914 ocha-anticipy-1.1.0/src/ochanticipy/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      768 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/utils/check_extra_imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/utils/check_file_existence.py
--rw-r--r--   0 runner    (1001) docker     (122)     6071 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (122)     7202 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/utils/geoboundingbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/utils/hdx_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1814 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (122)    25617 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/src/ochanticipy/utils/raster.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.511914 ocha-anticipy-1.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.519914 ocha-anticipy-1.1.0/tests/datasources/
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/fake_codab_multi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/fake_config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    14174 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/test_chirps.py
--rw-r--r--   0 runner    (1001) docker     (122)     5140 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/test_codab.py
--rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/test_datasource.py
--rw-r--r--   0 runner    (1001) docker     (122)     7536 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/test_fewsnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     4790 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/test_glofas.py
--rw-r--r--   0 runner    (1001) docker     (122)     6223 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/test_glofas_download.py
--rw-r--r--   0 runner    (1001) docker     (122)     9524 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/test_glofas_process.py
--rw-r--r--   0 runner    (1001) docker     (122)     7158 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/test_iri.py
--rw-r--r--   0 runner    (1001) docker     (122)     8882 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/datasources/test_ndvi.py
--rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/test_country_config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:13:36.519914 ocha-anticipy-1.1.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/utils/test_check_extra_imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/utils/test_check_file_existence.py
--rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/utils/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2915 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/utils/test_geoboundingbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     1547 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/utils/test_hdx_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     7015 2023-05-30 13:13:23.000000 ocha-anticipy-1.1.0/tests/utils/test_raster.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.890235 ocha-anticipy-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.874235 ocha-anticipy-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.878235 ocha-anticipy-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     5995 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5855 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4455 2023-05-30 14:08:00.890235 ocha-anticipy-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3235 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.878235 ocha-anticipy-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     2438 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/config.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.878235 ocha-anticipy-1.1.1/docs/datasources/
+-rw-r--r--   0 runner    (1001) docker     (122)     4362 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/datasources/chirps.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/datasources/codab.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4187 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/datasources/fewsnet.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    12684 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/datasources/glofas.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/datasources/iri_seasonal_forecast.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5950 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/datasources/usgs_ndvi.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/datasources.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.878235 ocha-anticipy-1.1.1/docs/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/utilities/raster.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)    11353 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2149 2023-05-30 14:08:00.890235 ocha-anticipy-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.874235 ocha-anticipy-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.882235 ocha-anticipy-1.1.1/src/ocha_anticipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4455 2023-05-30 14:08:00.000000 ocha-anticipy-1.1.1/src/ocha_anticipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-05-30 14:08:00.000000 ocha-anticipy-1.1.1/src/ocha_anticipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 14:08:00.000000 ocha-anticipy-1.1.1/src/ocha_anticipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      450 2023-05-30 14:08:00.000000 ocha-anticipy-1.1.1/src/ocha_anticipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-30 14:08:00.000000 ocha-anticipy-1.1.1/src/ocha_anticipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.882235 ocha-anticipy-1.1.1/src/ochanticipy/
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-30 14:08:00.000000 ocha-anticipy-1.1.1/src/ochanticipy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.882235 ocha-anticipy-1.1.1/src/ochanticipy/config/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.886235 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/afg.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/bdi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/bfa.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/bgd.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3120 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/caf.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/cmr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/cod.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3236 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/col.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/eth.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      333 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/hti.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/irq.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/lby.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2933 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/mli.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/mmr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4181 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/moz.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/mwi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/ner.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1708 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/nga.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/npl.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/pse.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/sdn.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/som.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/ssd.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/syr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/tcd.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/ukr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/ven.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/yem.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     8920 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countryconfig.py
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/pathconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.886235 ocha-anticipy-1.1.1/src/ochanticipy/datasources/
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.886235 ocha-anticipy-1.1.1/src/ochanticipy/datasources/chirps/
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/chirps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19875 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/chirps/chirps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.886235 ocha-anticipy-1.1.1/src/ochanticipy/datasources/codab/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/codab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7182 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/codab/codab.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/datasource.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.886235 ocha-anticipy-1.1.1/src/ochanticipy/datasources/fewsnet/
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/fewsnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13942 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/fewsnet/fewsnet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.886235 ocha-anticipy-1.1.1/src/ochanticipy/datasources/glofas/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/glofas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9849 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/glofas/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19202 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/glofas/glofas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/glofas/reanalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.886235 ocha-anticipy-1.1.1/src/ochanticipy/datasources/iri/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/iri/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10404 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/iri/iri_seasonal_forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.886235 ocha-anticipy-1.1.1/src/ochanticipy/datasources/usgs/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/usgs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28079 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/usgs/ndvi_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10009 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/usgs/ndvi_products.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.890235 ocha-anticipy-1.1.1/src/ochanticipy/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      768 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/utils/check_extra_imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/utils/check_file_existence.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6071 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7202 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/utils/geoboundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/utils/hdx_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1814 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25617 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/utils/raster.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.890235 ocha-anticipy-1.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.890235 ocha-anticipy-1.1.1/tests/datasources/
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/fake_codab_multi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/fake_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    14174 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/test_chirps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5140 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/test_codab.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/test_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7536 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/test_fewsnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4790 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/test_glofas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6223 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/test_glofas_download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9524 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/test_glofas_process.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7158 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/test_iri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8882 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/test_ndvi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/test_country_config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.890235 ocha-anticipy-1.1.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/utils/test_check_extra_imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/utils/test_check_file_existence.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/utils/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2915 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/utils/test_geoboundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1547 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/utils/test_hdx_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7015 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/utils/test_raster.py
```

### Comparing `ocha-anticipy-1.1.0/.github/workflows/publish-to-pypi.yaml` & `ocha-anticipy-1.1.1/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/.github/workflows/run-python-tests.yaml` & `ocha-anticipy-1.1.1/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/.gitignore` & `ocha-anticipy-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/.pre-commit-config.yaml` & `ocha-anticipy-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/CHANGELOG.rst` & `ocha-anticipy-1.1.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 All notable changes to OCHA AnticiPy will be documented in this file.
 
 The format is based on `Keep a
 Changelog <https://keepachangelog.com/en/1.0.0/>`__, and this project
 adheres to `Semantic
 Versioning <https://semver.org/spec/v2.0.0.html>`__.
 
+[1.1.1] - 2023-05-30
+--------------------
+
+Fixed
+~~~~~
+
+- Typo in required extras for ReadTheDocs
+
 [1.1.0] - 2023-05-30
 --------------------
 
 Added
 ~~~~~
 
 - Config files for 25/25 HRP countries and several non-HRP countries
```

### Comparing `ocha-anticipy-1.1.0/CONTRIBUTING.rst` & `ocha-anticipy-1.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/LICENSE` & `ocha-anticipy-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/PKG-INFO` & `ocha-anticipy-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocha-anticipy
-Version: 1.1.0
+Version: 1.1.1
 Summary: Access data for anticipating humanitarian risk
 Home-page: https://github.com/OCHA-DAP/ocha-anticipy
 Author: Data Science Team, UN OCHA Centre for Humanitarian Data
 Author-email: centrehumdata@un.org
 License: GPLv3
 Project-URL: Documentation, https://ocha-anticipy.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/OCHA-DAP/ocha-anticipy/blob/main/CHANGELOG.rst
```

### Comparing `ocha-anticipy-1.1.0/README.md` & `ocha-anticipy-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/docs/api.rst` & `ocha-anticipy-1.1.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/docs/conf.py` & `ocha-anticipy-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/docs/config.rst` & `ocha-anticipy-1.1.1/docs/config.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/docs/datasources/chirps.rst` & `ocha-anticipy-1.1.1/docs/datasources/chirps.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/docs/datasources/codab.rst` & `ocha-anticipy-1.1.1/docs/datasources/codab.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/docs/datasources/fewsnet.rst` & `ocha-anticipy-1.1.1/docs/datasources/fewsnet.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/docs/datasources/glofas.rst` & `ocha-anticipy-1.1.1/docs/datasources/glofas.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/docs/datasources/iri_seasonal_forecast.rst` & `ocha-anticipy-1.1.1/docs/datasources/iri_seasonal_forecast.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/docs/datasources/usgs_ndvi.rst` & `ocha-anticipy-1.1.1/docs/datasources/usgs_ndvi.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/docs/index.rst` & `ocha-anticipy-1.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/docs/introduction.rst` & `ocha-anticipy-1.1.1/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/docs/quickstart.rst` & `ocha-anticipy-1.1.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/docs/utilities/raster.rst` & `ocha-anticipy-1.1.1/docs/utilities/raster.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/requirements.txt` & `ocha-anticipy-1.1.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/setup.cfg` & `ocha-anticipy-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ocha_anticipy.egg-info/PKG-INFO` & `ocha-anticipy-1.1.1/src/ocha_anticipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocha-anticipy
-Version: 1.1.0
+Version: 1.1.1
 Summary: Access data for anticipating humanitarian risk
 Home-page: https://github.com/OCHA-DAP/ocha-anticipy
 Author: Data Science Team, UN OCHA Centre for Humanitarian Data
 Author-email: centrehumdata@un.org
 License: GPLv3
 Project-URL: Documentation, https://ocha-anticipy.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/OCHA-DAP/ocha-anticipy/blob/main/CHANGELOG.rst
```

### Comparing `ocha-anticipy-1.1.0/src/ocha_anticipy.egg-info/SOURCES.txt` & `ocha-anticipy-1.1.1/src/ocha_anticipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/__init__.py` & `ocha-anticipy-1.1.1/src/ochanticipy/__init__.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/bfa.yaml` & `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/bfa.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/bgd.yaml` & `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/bgd.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/caf.yaml` & `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/caf.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/cmr.yaml` & `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/cmr.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/cod.yaml` & `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/cod.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/col.yaml` & `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/col.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/eth.yaml` & `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/eth.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/mli.yaml` & `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/mli.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/mmr.yaml` & `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/mmr.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/moz.yaml` & `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/moz.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/mwi.yaml` & `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/mwi.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/ner.yaml` & `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/ner.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/nga.yaml` & `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/nga.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/npl.yaml` & `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/npl.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/sdn.yaml` & `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/sdn.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/som.yaml` & `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/som.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/tcd.yaml` & `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/tcd.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/config/countries/ven.yaml` & `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/ven.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/config/countryconfig.py` & `ocha-anticipy-1.1.1/src/ochanticipy/config/countryconfig.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/datasources/chirps/chirps.py` & `ocha-anticipy-1.1.1/src/ochanticipy/datasources/chirps/chirps.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/datasources/codab/codab.py` & `ocha-anticipy-1.1.1/src/ochanticipy/datasources/codab/codab.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/datasources/datasource.py` & `ocha-anticipy-1.1.1/src/ochanticipy/datasources/datasource.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/datasources/fewsnet/fewsnet.py` & `ocha-anticipy-1.1.1/src/ochanticipy/datasources/fewsnet/fewsnet.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/datasources/glofas/forecast.py` & `ocha-anticipy-1.1.1/src/ochanticipy/datasources/glofas/forecast.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/datasources/glofas/glofas.py` & `ocha-anticipy-1.1.1/src/ochanticipy/datasources/glofas/glofas.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/datasources/glofas/reanalysis.py` & `ocha-anticipy-1.1.1/src/ochanticipy/datasources/glofas/reanalysis.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/datasources/iri/iri_seasonal_forecast.py` & `ocha-anticipy-1.1.1/src/ochanticipy/datasources/iri/iri_seasonal_forecast.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/datasources/usgs/ndvi_base.py` & `ocha-anticipy-1.1.1/src/ochanticipy/datasources/usgs/ndvi_base.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/datasources/usgs/ndvi_products.py` & `ocha-anticipy-1.1.1/src/ochanticipy/datasources/usgs/ndvi_products.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/utils/check_extra_imports.py` & `ocha-anticipy-1.1.1/src/ochanticipy/utils/check_extra_imports.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/utils/check_file_existence.py` & `ocha-anticipy-1.1.1/src/ochanticipy/utils/check_file_existence.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/utils/dates.py` & `ocha-anticipy-1.1.1/src/ochanticipy/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/utils/geoboundingbox.py` & `ocha-anticipy-1.1.1/src/ochanticipy/utils/geoboundingbox.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/utils/hdx_api.py` & `ocha-anticipy-1.1.1/src/ochanticipy/utils/hdx_api.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/utils/io.py` & `ocha-anticipy-1.1.1/src/ochanticipy/utils/io.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/src/ochanticipy/utils/raster.py` & `ocha-anticipy-1.1.1/src/ochanticipy/utils/raster.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/tests/datasources/conftest.py` & `ocha-anticipy-1.1.1/tests/datasources/conftest.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/tests/datasources/test_chirps.py` & `ocha-anticipy-1.1.1/tests/datasources/test_chirps.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/tests/datasources/test_codab.py` & `ocha-anticipy-1.1.1/tests/datasources/test_codab.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/tests/datasources/test_datasource.py` & `ocha-anticipy-1.1.1/tests/datasources/test_datasource.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/tests/datasources/test_fewsnet.py` & `ocha-anticipy-1.1.1/tests/datasources/test_fewsnet.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/tests/datasources/test_glofas.py` & `ocha-anticipy-1.1.1/tests/datasources/test_glofas.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/tests/datasources/test_glofas_download.py` & `ocha-anticipy-1.1.1/tests/datasources/test_glofas_download.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/tests/datasources/test_glofas_process.py` & `ocha-anticipy-1.1.1/tests/datasources/test_glofas_process.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/tests/datasources/test_iri.py` & `ocha-anticipy-1.1.1/tests/datasources/test_iri.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/tests/datasources/test_ndvi.py` & `ocha-anticipy-1.1.1/tests/datasources/test_ndvi.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/tests/test_country_config.py` & `ocha-anticipy-1.1.1/tests/test_country_config.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/tests/utils/test_check_file_existence.py` & `ocha-anticipy-1.1.1/tests/utils/test_check_file_existence.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/tests/utils/test_dates.py` & `ocha-anticipy-1.1.1/tests/utils/test_dates.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/tests/utils/test_geoboundingbox.py` & `ocha-anticipy-1.1.1/tests/utils/test_geoboundingbox.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/tests/utils/test_hdx_api.py` & `ocha-anticipy-1.1.1/tests/utils/test_hdx_api.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.0/tests/utils/test_raster.py` & `ocha-anticipy-1.1.1/tests/utils/test_raster.py`

 * *Files identical despite different names*

