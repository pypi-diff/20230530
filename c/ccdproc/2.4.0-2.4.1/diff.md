# Comparing `tmp/ccdproc-2.4.0.tar.gz` & `tmp/ccdproc-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdproc-2.4.0.tar", last modified: Wed Nov 16 23:47:48 2022, max compression
+gzip compressed data, was "ccdproc-2.4.1.tar", last modified: Tue May 30 15:58:27 2023, max compression
```

## Comparing `ccdproc-2.4.0.tar` & `ccdproc-2.4.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-11-16 23:47:48.082555 ccdproc-2.4.0/
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-11-16 23:47:48.032983 ccdproc-2.4.0/.github/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      197 2021-05-22 16:10:18.000000 ccdproc-2.4.0/.github/CONTRIBUTING.md
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      699 2016-11-01 17:27:18.000000 ccdproc-2.4.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1217 2016-11-01 17:27:18.000000 ccdproc-2.4.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-11-16 23:47:48.033333 ccdproc-2.4.0/.github/workflows/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     3302 2022-05-06 17:51:06.000000 ccdproc-2.4.0/.github/workflows/ci_tests.yml
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      771 2021-05-22 16:10:18.000000 ccdproc-2.4.0/.gitignore
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2020-07-11 15:32:50.000000 ccdproc-2.4.0/.gitmodules
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1134 2019-09-04 13:23:24.000000 ccdproc-2.4.0/.mailmap
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      143 2021-11-23 17:40:30.000000 ccdproc-2.4.0/.readthedocs.yml
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2474 2022-11-16 22:53:15.000000 ccdproc-2.4.0/AUTHORS.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    16451 2022-11-16 23:38:45.000000 ccdproc-2.4.0/CHANGES.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1822 2019-07-29 13:54:01.000000 ccdproc-2.4.0/CITATION.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      180 2019-07-29 13:54:01.000000 ccdproc-2.4.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1503 2017-04-25 20:08:02.000000 ccdproc-2.4.0/LICENSE.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      382 2020-07-11 15:32:50.000000 ccdproc-2.4.0/MANIFEST.in
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      422 2022-11-16 23:47:48.082712 ccdproc-2.4.0/PKG-INFO
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     3785 2021-05-22 16:10:18.000000 ccdproc-2.4.0/README.rst
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-11-16 23:47:48.040947 ccdproc-2.4.0/ccdproc/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1124 2021-05-22 16:10:18.000000 ccdproc-2.4.0/ccdproc/__init__.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      355 2021-05-22 16:10:18.000000 ccdproc-2.4.0/ccdproc/_astropy_init.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      408 2019-07-25 14:55:58.000000 ccdproc-2.4.0/ccdproc/ccddata.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    38231 2022-11-16 22:53:15.000000 ccdproc-2.4.0/ccdproc/combiner.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1216 2022-05-06 17:51:06.000000 ccdproc-2.4.0/ccdproc/conftest.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    76092 2022-05-06 17:51:06.000000 ccdproc-2.4.0/ccdproc/core.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-11-16 23:47:48.043461 ccdproc-2.4.0/ccdproc/extern/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       64 2017-04-25 20:08:02.000000 ccdproc-2.4.0/ccdproc/extern/__init__.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    19025 2022-05-06 17:51:06.000000 ccdproc-2.4.0/ccdproc/extern/bitfield.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    37304 2021-05-22 23:47:25.000000 ccdproc-2.4.0/ccdproc/image_collection.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5533 2021-05-22 16:10:18.000000 ccdproc-2.4.0/ccdproc/log_meta.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-11-16 23:47:48.055406 ccdproc-2.4.0/ccdproc/tests/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      121 2014-06-02 22:53:55.000000 ccdproc-2.4.0/ccdproc/tests/__init__.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-11-16 23:47:48.059298 ccdproc-2.4.0/ccdproc/tests/data/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      257 2016-07-22 02:45:08.000000 ccdproc-2.4.0/ccdproc/tests/data/README.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)   561600 2022-05-06 17:51:06.000000 ccdproc-2.4.0/ccdproc/tests/data/a8280271.fits
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      459 2019-07-29 13:54:01.000000 ccdproc-2.4.0/ccdproc/tests/data/expected_ifc_file_properties.csv
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    20160 2019-08-12 17:52:46.000000 ccdproc-2.4.0/ccdproc/tests/data/flat-mef.fits
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    20160 2019-08-12 17:52:46.000000 ccdproc-2.4.0/ccdproc/tests/data/science-mef.fits
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    23040 2017-06-06 20:45:01.000000 ccdproc-2.4.0/ccdproc/tests/data/sip-wcs.fit
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2156 2019-08-12 17:52:46.000000 ccdproc-2.4.0/ccdproc/tests/make_mef.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2297 2022-05-06 17:51:06.000000 ccdproc-2.4.0/ccdproc/tests/pytest_fixtures.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7044 2022-05-06 17:51:06.000000 ccdproc-2.4.0/ccdproc/tests/run_for_memory_profile.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7763 2019-07-27 02:34:17.000000 ccdproc-2.4.0/ccdproc/tests/run_profile.ipynb
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     9314 2021-05-22 16:10:18.000000 ccdproc-2.4.0/ccdproc/tests/run_with_file_number_limit.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2253 2022-05-06 17:51:06.000000 ccdproc-2.4.0/ccdproc/tests/test_bitfield.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    10893 2021-05-22 16:10:18.000000 ccdproc-2.4.0/ccdproc/tests/test_ccdmask.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    42879 2022-05-06 17:51:06.000000 ccdproc-2.4.0/ccdproc/tests/test_ccdproc.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4202 2021-05-22 16:10:18.000000 ccdproc-2.4.0/ccdproc/tests/test_ccdproc_logging.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2109 2019-07-25 14:59:58.000000 ccdproc-2.4.0/ccdproc/tests/test_combine_open_files.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    35523 2022-11-16 22:53:15.000000 ccdproc-2.4.0/ccdproc/tests/test_combiner.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    15231 2022-05-06 17:51:06.000000 ccdproc-2.4.0/ccdproc/tests/test_cosmicray.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2132 2021-05-22 16:10:18.000000 ccdproc-2.4.0/ccdproc/tests/test_gain.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    47232 2022-05-06 17:51:06.000000 ccdproc-2.4.0/ccdproc/tests/test_image_collection.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2170 2021-05-22 16:10:18.000000 ccdproc-2.4.0/ccdproc/tests/test_keyword.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2731 2021-05-24 15:42:21.000000 ccdproc-2.4.0/ccdproc/tests/test_memory_use.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2481 2022-05-06 17:51:06.000000 ccdproc-2.4.0/ccdproc/tests/test_rebin.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2581 2021-05-22 16:10:18.000000 ccdproc-2.4.0/ccdproc/tests/test_wrapped_external_funcs.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-11-16 23:47:48.060788 ccdproc-2.4.0/ccdproc/utils/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      199 2014-06-02 22:53:55.000000 ccdproc-2.4.0/ccdproc/utils/__init__.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2932 2019-10-05 19:18:32.000000 ccdproc-2.4.0/ccdproc/utils/sample_directory.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4170 2018-08-10 21:10:15.000000 ccdproc-2.4.0/ccdproc/utils/slices.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-11-16 23:47:48.061489 ccdproc-2.4.0/ccdproc/utils/tests/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2014-06-02 22:53:55.000000 ccdproc-2.4.0/ccdproc/utils/tests/__init__.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4340 2017-06-06 20:45:01.000000 ccdproc-2.4.0/ccdproc/utils/tests/test_slices.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      176 2022-11-16 23:47:47.000000 ccdproc-2.4.0/ccdproc/version.py
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-11-16 23:47:48.042578 ccdproc-2.4.0/ccdproc.egg-info/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      422 2022-11-16 23:47:47.000000 ccdproc-2.4.0/ccdproc.egg-info/PKG-INFO
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2513 2022-11-16 23:47:48.000000 ccdproc-2.4.0/ccdproc.egg-info/SOURCES.txt
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        1 2022-11-16 23:47:47.000000 ccdproc-2.4.0/ccdproc.egg-info/dependency_links.txt
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        1 2022-05-09 18:13:58.000000 ccdproc-2.4.0/ccdproc.egg-info/not-zip-safe
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      152 2022-11-16 23:47:47.000000 ccdproc-2.4.0/ccdproc.egg-info/requires.txt
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        8 2022-11-16 23:47:47.000000 ccdproc-2.4.0/ccdproc.egg-info/top_level.txt
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-11-16 23:47:48.070091 ccdproc-2.4.0/docs/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4724 2014-06-17 02:37:36.000000 ccdproc-2.4.0/docs/Makefile
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-11-16 23:47:48.079207 ccdproc-2.4.0/docs/_static/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)   370070 2016-07-22 02:45:08.000000 ccdproc-2.4.0/docs/_static/ccd_proc.ico
--rwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     6867 2016-07-22 02:45:08.000000 ccdproc-2.4.0/docs/_static/ccd_proc.png
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      208 2016-07-22 02:45:08.000000 ccdproc-2.4.0/docs/_static/ccdproc.css
--rwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    51513 2016-07-22 02:45:08.000000 ccdproc-2.4.0/docs/_static/ccdproc.svg
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     9342 2019-07-29 13:54:01.000000 ccdproc-2.4.0/docs/_static/ccdproc_banner.pdf
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    95067 2019-07-29 13:54:01.000000 ccdproc-2.4.0/docs/_static/ccdproc_banner.png
--rwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)   222655 2020-07-11 15:32:50.000000 ccdproc-2.4.0/docs/_static/ccdproc_banner.svg
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-11-16 23:47:48.025047 ccdproc-2.4.0/docs/_templates/
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-11-16 23:47:48.081362 ccdproc-2.4.0/docs/_templates/autosummary/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      250 2014-05-14 21:39:15.000000 ccdproc-2.4.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      251 2014-05-14 21:39:15.000000 ccdproc-2.4.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      252 2014-05-14 21:39:15.000000 ccdproc-2.4.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      222 2019-07-29 13:54:01.000000 ccdproc-2.4.0/docs/api.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       55 2016-07-22 02:45:08.000000 ccdproc-2.4.0/docs/authors_for_sphinx.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7425 2019-08-12 17:52:46.000000 ccdproc-2.4.0/docs/ccddata.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       90 2015-02-17 03:20:49.000000 ccdproc-2.4.0/docs/changelog.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       52 2019-07-29 13:54:01.000000 ccdproc-2.4.0/docs/citation.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       54 2019-07-29 13:54:01.000000 ccdproc-2.4.0/docs/conduct.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     6951 2022-05-06 17:51:06.000000 ccdproc-2.4.0/docs/conf.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1599 2019-07-29 13:54:01.000000 ccdproc-2.4.0/docs/contributing.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      280 2021-05-22 16:10:18.000000 ccdproc-2.4.0/docs/default_config.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     3839 2019-07-29 13:54:01.000000 ccdproc-2.4.0/docs/getting_started.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     9815 2022-05-06 17:51:06.000000 ccdproc-2.4.0/docs/image_combination.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     8376 2022-05-06 17:51:06.000000 ccdproc-2.4.0/docs/image_management.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1637 2021-05-22 16:10:18.000000 ccdproc-2.4.0/docs/index.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1845 2021-05-22 16:10:18.000000 ccdproc-2.4.0/docs/install.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      157 2019-07-25 14:55:58.000000 ccdproc-2.4.0/docs/license.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4513 2014-05-14 21:39:15.000000 ccdproc-2.4.0/docs/make.bat
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      892 2019-07-29 13:54:01.000000 ccdproc-2.4.0/docs/overview.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      883 2019-07-29 13:54:01.000000 ccdproc-2.4.0/docs/reduction_examples.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    21228 2020-07-11 15:32:50.000000 ccdproc-2.4.0/docs/reduction_toolbox.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       67 2019-12-12 22:09:35.000000 ccdproc-2.4.0/docs/rtd-pip-requirements
-drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-11-16 23:47:48.082197 ccdproc-2.4.0/licenses/
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1463 2017-04-25 20:08:02.000000 ccdproc-2.4.0/licenses/LICENSE_STSCI_TOOLS.txt
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      251 2017-04-25 20:08:02.000000 ccdproc-2.4.0/licenses/README.rst
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      132 2020-07-11 15:32:50.000000 ccdproc-2.4.0/pyproject.toml
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1880 2022-11-16 23:47:48.083423 ccdproc-2.4.0/setup.cfg
--rwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1609 2020-07-11 15:32:50.000000 ccdproc-2.4.0/setup.py
--rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2449 2022-05-06 17:51:06.000000 ccdproc-2.4.0/tox.ini
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.824422 ccdproc-2.4.1/
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.803008 ccdproc-2.4.1/.github/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      197 2021-03-19 20:06:38.000000 ccdproc-2.4.1/.github/CONTRIBUTING.md
+-rw-r--r--   0 mattcraig   (501) staff       (20)      699 2018-08-14 01:14:56.000000 ccdproc-2.4.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1217 2018-08-14 01:14:56.000000 ccdproc-2.4.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.803150 ccdproc-2.4.1/.github/workflows/
+-rw-r--r--   0 mattcraig   (501) staff       (20)     3302 2021-12-14 21:17:21.000000 ccdproc-2.4.1/.github/workflows/ci_tests.yml
+-rw-r--r--   0 mattcraig   (501) staff       (20)      771 2021-03-19 20:06:25.000000 ccdproc-2.4.1/.gitignore
+-rw-r--r--   0 mattcraig   (501) staff       (20)        0 2019-12-24 20:04:16.000000 ccdproc-2.4.1/.gitmodules
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1134 2019-09-02 21:23:23.000000 ccdproc-2.4.1/.mailmap
+-rw-r--r--   0 mattcraig   (501) staff       (20)      143 2021-11-24 18:20:46.000000 ccdproc-2.4.1/.readthedocs.yml
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2507 2023-05-30 15:52:39.000000 ccdproc-2.4.1/AUTHORS.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)    16811 2023-05-30 15:54:14.000000 ccdproc-2.4.1/CHANGES.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1822 2019-09-02 17:30:31.000000 ccdproc-2.4.1/CITATION.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      180 2019-09-02 17:30:31.000000 ccdproc-2.4.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1503 2018-08-18 01:06:53.000000 ccdproc-2.4.1/LICENSE.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      382 2020-11-28 20:18:08.000000 ccdproc-2.4.1/MANIFEST.in
+-rw-r--r--   0 mattcraig   (501) staff       (20)      422 2023-05-30 15:58:27.824508 ccdproc-2.4.1/PKG-INFO
+-rw-r--r--   0 mattcraig   (501) staff       (20)     3785 2021-03-19 20:06:38.000000 ccdproc-2.4.1/README.rst
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.806380 ccdproc-2.4.1/ccdproc/
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1124 2021-05-19 00:45:02.000000 ccdproc-2.4.1/ccdproc/__init__.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)      355 2021-05-19 00:45:02.000000 ccdproc-2.4.1/ccdproc/_astropy_init.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)      408 2018-08-18 01:06:53.000000 ccdproc-2.4.1/ccdproc/ccddata.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    38231 2022-11-17 14:20:04.000000 ccdproc-2.4.1/ccdproc/combiner.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1216 2022-01-19 16:10:46.000000 ccdproc-2.4.1/ccdproc/conftest.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    76092 2022-06-01 13:16:23.000000 ccdproc-2.4.1/ccdproc/core.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.807448 ccdproc-2.4.1/ccdproc/extern/
+-rw-r--r--   0 mattcraig   (501) staff       (20)       64 2018-08-18 01:06:53.000000 ccdproc-2.4.1/ccdproc/extern/__init__.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    19025 2021-12-20 17:15:43.000000 ccdproc-2.4.1/ccdproc/extern/bitfield.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    37438 2023-05-30 15:52:41.000000 ccdproc-2.4.1/ccdproc/image_collection.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     5533 2021-03-19 20:06:38.000000 ccdproc-2.4.1/ccdproc/log_meta.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.813213 ccdproc-2.4.1/ccdproc/tests/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      121 2018-08-14 01:14:56.000000 ccdproc-2.4.1/ccdproc/tests/__init__.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.815645 ccdproc-2.4.1/ccdproc/tests/data/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      257 2018-08-14 01:14:56.000000 ccdproc-2.4.1/ccdproc/tests/data/README.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)   561600 2021-12-21 15:57:22.000000 ccdproc-2.4.1/ccdproc/tests/data/a8280271.fits
+-rw-r--r--   0 mattcraig   (501) staff       (20)      459 2019-09-02 17:30:31.000000 ccdproc-2.4.1/ccdproc/tests/data/expected_ifc_file_properties.csv
+-rw-r--r--   0 mattcraig   (501) staff       (20)    20160 2019-09-02 17:30:31.000000 ccdproc-2.4.1/ccdproc/tests/data/flat-mef.fits
+-rw-r--r--   0 mattcraig   (501) staff       (20)    20160 2019-09-02 17:30:31.000000 ccdproc-2.4.1/ccdproc/tests/data/science-mef.fits
+-rw-r--r--   0 mattcraig   (501) staff       (20)    23040 2021-12-21 15:57:17.000000 ccdproc-2.4.1/ccdproc/tests/data/sip-wcs.fit
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2156 2019-09-02 17:30:31.000000 ccdproc-2.4.1/ccdproc/tests/make_mef.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2297 2022-01-19 16:10:46.000000 ccdproc-2.4.1/ccdproc/tests/pytest_fixtures.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     7044 2022-01-19 16:10:46.000000 ccdproc-2.4.1/ccdproc/tests/run_for_memory_profile.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     7763 2019-09-02 17:30:31.000000 ccdproc-2.4.1/ccdproc/tests/run_profile.ipynb
+-rw-r--r--   0 mattcraig   (501) staff       (20)     9314 2021-03-15 15:22:51.000000 ccdproc-2.4.1/ccdproc/tests/run_with_file_number_limit.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2253 2022-01-19 16:10:46.000000 ccdproc-2.4.1/ccdproc/tests/test_bitfield.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    10893 2021-03-19 20:06:38.000000 ccdproc-2.4.1/ccdproc/tests/test_ccdmask.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    42879 2022-01-19 16:10:46.000000 ccdproc-2.4.1/ccdproc/tests/test_ccdproc.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     4202 2021-03-19 20:06:38.000000 ccdproc-2.4.1/ccdproc/tests/test_ccdproc_logging.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2109 2019-03-08 20:32:20.000000 ccdproc-2.4.1/ccdproc/tests/test_combine_open_files.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    35523 2022-11-17 14:20:04.000000 ccdproc-2.4.1/ccdproc/tests/test_combiner.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    15231 2021-12-21 15:57:22.000000 ccdproc-2.4.1/ccdproc/tests/test_cosmicray.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2132 2021-03-15 15:22:51.000000 ccdproc-2.4.1/ccdproc/tests/test_gain.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    47273 2023-05-30 15:52:41.000000 ccdproc-2.4.1/ccdproc/tests/test_image_collection.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2170 2021-03-15 15:22:51.000000 ccdproc-2.4.1/ccdproc/tests/test_keyword.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2731 2021-11-19 14:38:28.000000 ccdproc-2.4.1/ccdproc/tests/test_memory_use.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2481 2022-01-19 16:10:46.000000 ccdproc-2.4.1/ccdproc/tests/test_rebin.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2581 2021-03-15 15:22:51.000000 ccdproc-2.4.1/ccdproc/tests/test_wrapped_external_funcs.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.816153 ccdproc-2.4.1/ccdproc/utils/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      199 2018-08-14 01:14:56.000000 ccdproc-2.4.1/ccdproc/utils/__init__.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2932 2019-09-06 01:45:09.000000 ccdproc-2.4.1/ccdproc/utils/sample_directory.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     4170 2018-08-18 01:06:53.000000 ccdproc-2.4.1/ccdproc/utils/slices.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.816503 ccdproc-2.4.1/ccdproc/utils/tests/
+-rw-r--r--   0 mattcraig   (501) staff       (20)        0 2018-08-14 01:14:56.000000 ccdproc-2.4.1/ccdproc/utils/tests/__init__.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     4340 2018-08-18 01:06:53.000000 ccdproc-2.4.1/ccdproc/utils/tests/test_slices.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)      160 2023-05-30 15:58:27.000000 ccdproc-2.4.1/ccdproc/version.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.807157 ccdproc-2.4.1/ccdproc.egg-info/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      422 2023-05-30 15:58:27.000000 ccdproc-2.4.1/ccdproc.egg-info/PKG-INFO
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2513 2023-05-30 15:58:27.000000 ccdproc-2.4.1/ccdproc.egg-info/SOURCES.txt
+-rw-r--r--   0 mattcraig   (501) staff       (20)        1 2023-05-30 15:58:27.000000 ccdproc-2.4.1/ccdproc.egg-info/dependency_links.txt
+-rw-r--r--   0 mattcraig   (501) staff       (20)        1 2023-05-30 15:58:27.000000 ccdproc-2.4.1/ccdproc.egg-info/not-zip-safe
+-rw-r--r--   0 mattcraig   (501) staff       (20)      162 2023-05-30 15:58:27.000000 ccdproc-2.4.1/ccdproc.egg-info/requires.txt
+-rw-r--r--   0 mattcraig   (501) staff       (20)        8 2023-05-30 15:58:27.000000 ccdproc-2.4.1/ccdproc.egg-info/top_level.txt
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.820423 ccdproc-2.4.1/docs/
+-rw-r--r--   0 mattcraig   (501) staff       (20)     4724 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/Makefile
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.822755 ccdproc-2.4.1/docs/_static/
+-rw-r--r--   0 mattcraig   (501) staff       (20)   370070 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/_static/ccd_proc.ico
+-rwxr-xr-x   0 mattcraig   (501) staff       (20)     6867 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/_static/ccd_proc.png
+-rw-r--r--   0 mattcraig   (501) staff       (20)      208 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/_static/ccdproc.css
+-rwxr-xr-x   0 mattcraig   (501) staff       (20)    51513 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/_static/ccdproc.svg
+-rw-r--r--   0 mattcraig   (501) staff       (20)     9342 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/_static/ccdproc_banner.pdf
+-rw-r--r--   0 mattcraig   (501) staff       (20)    95067 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/_static/ccdproc_banner.png
+-rwxr-xr-x   0 mattcraig   (501) staff       (20)   222655 2019-12-24 20:04:16.000000 ccdproc-2.4.1/docs/_static/ccdproc_banner.svg
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.799877 ccdproc-2.4.1/docs/_templates/
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.823881 ccdproc-2.4.1/docs/_templates/autosummary/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      250 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      251 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      252 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      222 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/api.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)       55 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/authors_for_sphinx.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     7425 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/ccddata.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)       90 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/changelog.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)       52 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/citation.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)       54 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/conduct.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     6951 2021-12-21 15:57:22.000000 ccdproc-2.4.1/docs/conf.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1599 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/contributing.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      280 2021-05-19 00:45:02.000000 ccdproc-2.4.1/docs/default_config.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     3839 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/getting_started.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     9815 2021-12-21 15:57:22.000000 ccdproc-2.4.1/docs/image_combination.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     8376 2021-12-21 15:57:22.000000 ccdproc-2.4.1/docs/image_management.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1637 2021-05-19 00:45:02.000000 ccdproc-2.4.1/docs/index.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1845 2021-03-19 20:06:38.000000 ccdproc-2.4.1/docs/install.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      157 2019-03-08 17:03:24.000000 ccdproc-2.4.1/docs/license.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     4513 2018-08-14 01:14:56.000000 ccdproc-2.4.1/docs/make.bat
+-rw-r--r--   0 mattcraig   (501) staff       (20)      892 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/overview.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      883 2019-09-02 17:30:31.000000 ccdproc-2.4.1/docs/reduction_examples.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)    21228 2019-12-24 20:04:16.000000 ccdproc-2.4.1/docs/reduction_toolbox.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)       67 2019-03-30 16:56:12.000000 ccdproc-2.4.1/docs/rtd-pip-requirements
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-05-30 15:58:27.824248 ccdproc-2.4.1/licenses/
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1463 2018-08-18 01:06:53.000000 ccdproc-2.4.1/licenses/LICENSE_STSCI_TOOLS.txt
+-rw-r--r--   0 mattcraig   (501) staff       (20)      251 2018-08-18 01:06:53.000000 ccdproc-2.4.1/licenses/README.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      132 2019-12-24 20:04:16.000000 ccdproc-2.4.1/pyproject.toml
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1890 2023-05-30 15:58:27.824947 ccdproc-2.4.1/setup.cfg
+-rwxr-xr-x   0 mattcraig   (501) staff       (20)     1609 2019-12-24 20:04:16.000000 ccdproc-2.4.1/setup.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2665 2023-05-30 15:52:39.000000 ccdproc-2.4.1/tox.ini
```

### Comparing `ccdproc-2.4.0/.github/ISSUE_TEMPLATE.md` & `ccdproc-2.4.1/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/.github/PULL_REQUEST_TEMPLATE.md` & `ccdproc-2.4.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/.github/workflows/ci_tests.yml` & `ccdproc-2.4.1/.github/workflows/ci_tests.yml`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/.gitignore` & `ccdproc-2.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/.mailmap` & `ccdproc-2.4.1/.mailmap`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/AUTHORS.rst` & `ccdproc-2.4.1/AUTHORS.rst`

 * *Files 8% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 -----------------------
 
 The people below have helped the project by opening multiple issues, suggesting
 improvements outside of GitHub, or otherwise assisted the project.
 
 * Juan Cabanela (@JuanCab)
 * @mheida
+* Aaron W Morris (@aaronwmorris)
 * Sara Ogaz (@SaOgaz)
 * Jean-Paul Ventura (@jvntra)
 * Kerry Paterson (@KerryPaterson)
 * Jane Rigby (@janerigby)
 * Kris Stern (@kakirastern)
 * Alexa Villaume (@AlexaVillaume)
 * Brian York (@york-stsci)
```

### Comparing `ccdproc-2.4.0/CHANGES.rst` & `ccdproc-2.4.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+2.4.1 (2023-05-30)
+------------------
+
+New Features
+^^^^^^^^^^^^
+
+Other Changes and Additions
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Bug Fixes
+^^^^^^^^^
+
+- Fixes a crash when attempting to filter an already-empty ImageFileCollection,
+  instead simply returning an empty ImageFileCollection.  [#801]
+
+- Fixes minimum astropy version in installation requirements. [#799]
+
 2.4.0 (2022-11-16)
 ------------------
 
 New Features
 ^^^^^^^^^^^^
 
 Other Changes and Additions
```

### Comparing `ccdproc-2.4.0/CITATION.rst` & `ccdproc-2.4.1/CITATION.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/LICENSE.rst` & `ccdproc-2.4.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/README.rst` & `ccdproc-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/__init__.py` & `ccdproc-2.4.1/ccdproc/__init__.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/combiner.py` & `ccdproc-2.4.1/ccdproc/combiner.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/conftest.py` & `ccdproc-2.4.1/ccdproc/conftest.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/core.py` & `ccdproc-2.4.1/ccdproc/core.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/extern/bitfield.py` & `ccdproc-2.4.1/ccdproc/extern/bitfield.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/image_collection.py` & `ccdproc-2.4.1/ccdproc/image_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,14 +362,18 @@
             >>> collection.files_filtered(imagetyp='LIGHT', **add_filters)
 
         Notes
         -----
         Value comparison is case *insensitive* for strings, whether matching
         exactly or matching with regular expressions.
         """
+        # If the collection is empty, self.summary == None; return empty list
+        if self.summary is None:
+            return []
+
         # force a copy by explicitly converting to a list
         current_file_mask = self.summary['file'].mask.tolist()
 
         include_path = kwd.pop('include_path', False)
 
         self._find_keywords_by_values(**kwd)
         filtered_files = self.summary['file'].compressed()
```

### Comparing `ccdproc-2.4.0/ccdproc/log_meta.py` & `ccdproc-2.4.1/ccdproc/log_meta.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/data/a8280271.fits` & `ccdproc-2.4.1/ccdproc/tests/data/a8280271.fits`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/data/flat-mef.fits` & `ccdproc-2.4.1/ccdproc/tests/data/flat-mef.fits`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/data/science-mef.fits` & `ccdproc-2.4.1/ccdproc/tests/data/science-mef.fits`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/data/sip-wcs.fit` & `ccdproc-2.4.1/ccdproc/tests/data/sip-wcs.fit`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/make_mef.py` & `ccdproc-2.4.1/ccdproc/tests/make_mef.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/pytest_fixtures.py` & `ccdproc-2.4.1/ccdproc/tests/pytest_fixtures.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/run_for_memory_profile.py` & `ccdproc-2.4.1/ccdproc/tests/run_for_memory_profile.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/run_profile.ipynb` & `ccdproc-2.4.1/ccdproc/tests/run_profile.ipynb`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/run_with_file_number_limit.py` & `ccdproc-2.4.1/ccdproc/tests/run_with_file_number_limit.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/test_bitfield.py` & `ccdproc-2.4.1/ccdproc/tests/test_bitfield.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/test_ccdmask.py` & `ccdproc-2.4.1/ccdproc/tests/test_ccdmask.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/test_ccdproc.py` & `ccdproc-2.4.1/ccdproc/tests/test_ccdproc.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/test_ccdproc_logging.py` & `ccdproc-2.4.1/ccdproc/tests/test_ccdproc_logging.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/test_combine_open_files.py` & `ccdproc-2.4.1/ccdproc/tests/test_combine_open_files.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/test_combiner.py` & `ccdproc-2.4.1/ccdproc/tests/test_combiner.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/test_cosmicray.py` & `ccdproc-2.4.1/ccdproc/tests/test_cosmicray.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/test_gain.py` & `ccdproc-2.4.1/ccdproc/tests/test_gain.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/test_image_collection.py` & `ccdproc-2.4.1/ccdproc/tests/test_image_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1011,14 +1011,15 @@
             p.unlink()
 
         # Now the summary should be none
         with pytest.warns(AstropyUserWarning, match='no FITS files in the collection'):
             ic = ImageFileCollection(triage_setup.test_dir)
         assert ic.summary is None
         assert ic.keywords == []
+        assert ic.files_filtered() == []
 
     def test_regex_match_for_search(self, triage_setup):
         # Test regex matching in searches
 
         ic = ImageFileCollection(triage_setup.test_dir)
 
         files = ic.files_filtered(regex_match=True, imagetyp='b.*s')
```

### Comparing `ccdproc-2.4.0/ccdproc/tests/test_keyword.py` & `ccdproc-2.4.1/ccdproc/tests/test_keyword.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/test_memory_use.py` & `ccdproc-2.4.1/ccdproc/tests/test_memory_use.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/test_rebin.py` & `ccdproc-2.4.1/ccdproc/tests/test_rebin.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/tests/test_wrapped_external_funcs.py` & `ccdproc-2.4.1/ccdproc/tests/test_wrapped_external_funcs.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/utils/sample_directory.py` & `ccdproc-2.4.1/ccdproc/utils/sample_directory.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/utils/slices.py` & `ccdproc-2.4.1/ccdproc/utils/slices.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc/utils/tests/test_slices.py` & `ccdproc-2.4.1/ccdproc/utils/tests/test_slices.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/ccdproc.egg-info/SOURCES.txt` & `ccdproc-2.4.1/ccdproc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/docs/Makefile` & `ccdproc-2.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/docs/_static/ccd_proc.ico` & `ccdproc-2.4.1/docs/_static/ccd_proc.ico`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/docs/_static/ccd_proc.png` & `ccdproc-2.4.1/docs/_static/ccd_proc.png`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/docs/_static/ccdproc.svg` & `ccdproc-2.4.1/docs/_static/ccdproc.svg`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/docs/_static/ccdproc_banner.pdf` & `ccdproc-2.4.1/docs/_static/ccdproc_banner.pdf`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/docs/_static/ccdproc_banner.png` & `ccdproc-2.4.1/docs/_static/ccdproc_banner.png`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/docs/_static/ccdproc_banner.svg` & `ccdproc-2.4.1/docs/_static/ccdproc_banner.svg`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/docs/ccddata.rst` & `ccdproc-2.4.1/docs/ccddata.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/docs/conf.py` & `ccdproc-2.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/docs/contributing.rst` & `ccdproc-2.4.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/docs/getting_started.rst` & `ccdproc-2.4.1/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/docs/image_combination.rst` & `ccdproc-2.4.1/docs/image_combination.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/docs/image_management.rst` & `ccdproc-2.4.1/docs/image_management.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/docs/index.rst` & `ccdproc-2.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/docs/install.rst` & `ccdproc-2.4.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/docs/make.bat` & `ccdproc-2.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/docs/overview.rst` & `ccdproc-2.4.1/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/docs/reduction_examples.rst` & `ccdproc-2.4.1/docs/reduction_examples.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/docs/reduction_toolbox.rst` & `ccdproc-2.4.1/docs/reduction_toolbox.rst`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/licenses/LICENSE_STSCI_TOOLS.txt` & `ccdproc-2.4.1/licenses/LICENSE_STSCI_TOOLS.txt`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/setup.cfg` & `ccdproc-2.4.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -25,28 +25,28 @@
 edit_on_github = False
 github_project = astropy/ccdproc
 
 [options]
 packages = find:
 zip_safe = False
 setup_requires = setuptools_scm
-install_requires = numpy>=1.18
-	astropy>=4.3
+install_requires = numpy>=1.21
+	astropy>=5.0.1
 	scipy
 	astroscrappy>=1.0.8
 	reproject>=0.7
 	scikit-image
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.package_data]
 * = data/*
 
 [options.extras_require]
 test = 
-	pytest-astropy
+	pytest-astropy>=0.10.0
 	memory_profiler
 docs = 
 	sphinx-astropy
 	matplotlib
 
 [pycodestyle]
 select = E101,E111,E112,E113,E221,E222,E223,E224,E225,E241,E242,E251,E271,E272,E303,E304,E502,E703,E901,E902,W191,W291,W292,W293,W391
```

### Comparing `ccdproc-2.4.0/setup.py` & `ccdproc-2.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `ccdproc-2.4.0/tox.ini` & `ccdproc-2.4.1/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -47,25 +47,29 @@
     devdeps: git+https://github.com/astropy/astropy.git#egg=astropy
     devdeps: git+https://github.com/astropy/astroscrappy.git#egg=astroscrappy
 
     # Remember to transfer any changes here to setup.cfg also. Only listing
     # packages which are constrained in the setup.cfg
     # NOTE ABOUT NUMPY VERSION: for astroscrappy 1.0.8 have to use at least 1.20
     # for the tests to even get to the point of running.
-    oldestdeps: numpy==1.20.*
-    oldestdeps: astropy==4.0.*
+    oldestdeps: numpy==1.21.*
+    oldestdeps: astropy==5.0.*
     oldestdeps: reproject==0.7
-    oldestdeps: astroscrappy==1.0.8
+    # astroscrappy needs to install AFTER numpy so its install is done in
+    # the commands section instead of here.
+    #oldestdeps: astroscrappy==1.0.8
     oldestdeps: cython
 
 commands =
     pip freeze
     !cov-!oldestdeps: pytest --pyargs ccdproc {toxinidir}/docs {posargs}
     cov: pytest --pyargs ccdproc {toxinidir}/docs --cov ccdproc --cov-config={toxinidir}/setup.cfg {posargs}
     cov: coverage xml -o {toxinidir}/coverage.xml
+    # install astroscrappy after numpy
+    oldestdeps: python -m pip install astroscrappy==1.0.8
     # Do not care about warnings on the oldest builds
     oldestdeps: pytest --pyargs ccdproc {toxinidir}/docs -W ignore {posargs}
 
 [testenv:build_docs]
 extras = docs
 deps =
     sphinx-automodapi<=0.13
```

