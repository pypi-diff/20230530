# Comparing `tmp/romanisim-0.2.0.tar.gz` & `tmp/romanisim-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "romanisim-0.2.0.tar", last modified: Tue Apr  4 19:55:14 2023, max compression
+gzip compressed data, was "romanisim-0.2.2.tar", last modified: Tue May 30 16:46:11 2023, max compression
```

## Comparing `romanisim-0.2.0.tar` & `romanisim-0.2.2.tar`

### file list

```diff
@@ -1,83 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:55:14.133917 romanisim-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-04 19:55:02.000000 romanisim-0.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:55:14.125917 romanisim-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-04 19:55:02.000000 romanisim-0.2.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:55:14.125917 romanisim-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-04 19:55:02.000000 romanisim-0.2.0/.github/workflows/cancel_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-04 19:55:02.000000 romanisim-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-04 19:55:02.000000 romanisim-0.2.0/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-04 19:55:02.000000 romanisim-0.2.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-04 19:55:02.000000 romanisim-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-04 19:55:02.000000 romanisim-0.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-04 19:55:02.000000 romanisim-0.2.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-04 19:55:02.000000 romanisim-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-04 19:55:02.000000 romanisim-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-04-04 19:55:14.133917 romanisim-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-04 19:55:02.000000 romanisim-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:55:14.125917 romanisim-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-04 19:55:02.000000 romanisim-0.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-04 19:55:02.000000 romanisim-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-04 19:55:02.000000 romanisim-0.2.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:55:14.129917 romanisim-0.2.0/docs/romanisim/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-04 19:55:02.000000 romanisim-0.2.0/docs/romanisim/apt.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-04 19:55:02.000000 romanisim-0.2.0/docs/romanisim/bandpass.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-04 19:55:02.000000 romanisim-0.2.0/docs/romanisim/catalog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-04 19:55:02.000000 romanisim-0.2.0/docs/romanisim/image.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-04 19:55:02.000000 romanisim-0.2.0/docs/romanisim/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-04-04 19:55:02.000000 romanisim-0.2.0/docs/romanisim/l1.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-04 19:55:02.000000 romanisim-0.2.0/docs/romanisim/l2.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-04 19:55:02.000000 romanisim-0.2.0/docs/romanisim/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-04 19:55:02.000000 romanisim-0.2.0/docs/romanisim/parameters.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-04 19:55:02.000000 romanisim-0.2.0/docs/romanisim/psf.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-04 19:55:02.000000 romanisim-0.2.0/docs/romanisim/refs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-04 19:55:02.000000 romanisim-0.2.0/docs/romanisim/running.rst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-04 19:55:02.000000 romanisim-0.2.0/docs/romanisim/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-04 19:55:02.000000 romanisim-0.2.0/docs/romanisim/wcs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-04 19:55:02.000000 romanisim-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:55:14.129917 romanisim-0.2.0/regtest/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-04 19:55:02.000000 romanisim-0.2.0/regtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-04 19:55:02.000000 romanisim-0.2.0/regtest/test_l1.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-04 19:55:02.000000 romanisim-0.2.0/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:55:14.129917 romanisim-0.2.0/romanisim/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/apt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/bandpass.py
--rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/cr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:55:14.133917 romanisim-0.2.0/romanisim/data/
--rw-r--r--   0 runner    (1001) docker     (123)    20073 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/data/Roman_effarea_20201130.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/gaia.py
--rw-r--r--   0 runner    (1001) docker     (123)    30203 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    22127 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/l1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/nonlinearity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/psf.py
--rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/ramp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:55:14.133917 romanisim-0.2.0/romanisim/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/tests/test_bandpass.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/tests/test_cr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/tests/test_gaia.py
--rw-r--r--   0 runner    (1001) docker     (123)    21781 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/tests/test_l1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/tests/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/tests/test_psf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/tests/test_ramp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/tests/test_wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10041 2023-04-04 19:55:02.000000 romanisim-0.2.0/romanisim/wcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:55:14.133917 romanisim-0.2.0/romanisim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-04-04 19:55:14.000000 romanisim-0.2.0/romanisim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-04 19:55:14.000000 romanisim-0.2.0/romanisim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 19:55:14.000000 romanisim-0.2.0/romanisim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 19:55:13.000000 romanisim-0.2.0/romanisim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-04 19:55:14.000000 romanisim-0.2.0/romanisim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-04 19:55:14.000000 romanisim-0.2.0/romanisim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:55:14.133917 romanisim-0.2.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4628 2023-04-04 19:55:02.000000 romanisim-0.2.0/scripts/romanisim-make-image
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 19:55:14.133917 romanisim-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-04 19:55:02.000000 romanisim-0.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-04 19:55:02.000000 romanisim-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:46:11.933564 romanisim-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-30 16:45:57.000000 romanisim-0.2.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:46:11.925564 romanisim-0.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-30 16:45:57.000000 romanisim-0.2.2/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:46:11.925564 romanisim-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-30 16:45:57.000000 romanisim-0.2.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-30 16:45:57.000000 romanisim-0.2.2/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-30 16:45:57.000000 romanisim-0.2.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-30 16:45:57.000000 romanisim-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-30 16:45:57.000000 romanisim-0.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-30 16:45:57.000000 romanisim-0.2.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-30 16:45:57.000000 romanisim-0.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-30 16:45:57.000000 romanisim-0.2.2/JenkinsfileRT_dev
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-30 16:45:57.000000 romanisim-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-05-30 16:46:11.933564 romanisim-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-30 16:45:57.000000 romanisim-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:46:11.925564 romanisim-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-30 16:45:57.000000 romanisim-0.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-30 16:45:57.000000 romanisim-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-30 16:45:57.000000 romanisim-0.2.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:46:11.925564 romanisim-0.2.2/docs/romanisim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-30 16:45:57.000000 romanisim-0.2.2/docs/romanisim/apt.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-30 16:45:57.000000 romanisim-0.2.2/docs/romanisim/bandpass.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-30 16:45:57.000000 romanisim-0.2.2/docs/romanisim/catalog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-30 16:45:57.000000 romanisim-0.2.2/docs/romanisim/image.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-30 16:45:57.000000 romanisim-0.2.2/docs/romanisim/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-05-30 16:45:57.000000 romanisim-0.2.2/docs/romanisim/l1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-30 16:45:57.000000 romanisim-0.2.2/docs/romanisim/l2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-30 16:45:57.000000 romanisim-0.2.2/docs/romanisim/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-30 16:45:57.000000 romanisim-0.2.2/docs/romanisim/parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-30 16:45:57.000000 romanisim-0.2.2/docs/romanisim/psf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-30 16:45:57.000000 romanisim-0.2.2/docs/romanisim/refs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-05-30 16:45:57.000000 romanisim-0.2.2/docs/romanisim/running.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-30 16:45:57.000000 romanisim-0.2.2/docs/romanisim/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-30 16:45:57.000000 romanisim-0.2.2/docs/romanisim/wcs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-30 16:45:57.000000 romanisim-0.2.2/docs/rtd_environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-30 16:45:57.000000 romanisim-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-30 16:45:57.000000 romanisim-0.2.2/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:46:11.929564 romanisim-0.2.2/romanisim/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/apt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/bandpass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/cr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:46:11.929564 romanisim-0.2.2/romanisim/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20073 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/data/Roman_effarea_20201130.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31438 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22927 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/l1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/nonlinearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/psf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25215 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   405518 2023-05-30 16:46:11.000000 romanisim-0.2.2/romanisim/ramp_fit_casertano.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/ramp_fit_casertano.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:46:11.929564 romanisim-0.2.2/romanisim/regtest/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/regtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/regtest/test_l1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:46:11.933564 romanisim-0.2.2/romanisim/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/tests/test_bandpass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/tests/test_cr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/tests/test_gaia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23028 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/tests/test_l1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/tests/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/tests/test_psf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/tests/test_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/tests/test_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-30 16:45:57.000000 romanisim-0.2.2/romanisim/wcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:46:11.929564 romanisim-0.2.2/romanisim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-05-30 16:46:11.000000 romanisim-0.2.2/romanisim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-30 16:46:11.000000 romanisim-0.2.2/romanisim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:46:11.000000 romanisim-0.2.2/romanisim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:46:11.000000 romanisim-0.2.2/romanisim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-30 16:46:11.000000 romanisim-0.2.2/romanisim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-30 16:46:11.000000 romanisim-0.2.2/romanisim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:46:11.933564 romanisim-0.2.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4603 2023-05-30 16:45:57.000000 romanisim-0.2.2/scripts/romanisim-make-image
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 16:46:11.933564 romanisim-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-30 16:45:57.000000 romanisim-0.2.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-30 16:45:57.000000 romanisim-0.2.2/tox.ini
```

### Comparing `romanisim-0.2.0/.github/workflows/ci.yml` & `romanisim-0.2.2/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,18 @@
     branches:
       - main
   schedule:
     # Weekly Monday 9AM build
     # * is a special character in YAML so you have to quote this string
     - cron: '0 9 * * 0'
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+
 jobs:
   check:
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@v1
     with:
       envs: |
         - linux: check-style
         - linux: build-dist
@@ -65,17 +69,15 @@
       setenv: |
         WEBBPSF_PATH: ${{ needs.data.outputs.webbpsf_path }}
         GALSIM_CAT_PATH: ${{ needs.data.outputs.galsim_cat_path }}
       cache-path: ${{ needs.data.outputs.path }}
       cache-key: data-${{ needs.data.outputs.hash }}
       envs: |
         - linux: test-oldestdeps-cov-xdist
-          python-version: 3.8
-        - linux: test-xdist
-          python-version: 3.8
+          python-version: 3.9
         - linux: test-xdist
           python-version: 3.9
         - linux: test-xdist
           python-version: 3.10
         - linux: test-xdist
           python-version: 3.11
         - macos: test-xdist
```

### Comparing `romanisim-0.2.0/.github/workflows/ci_cron.yml` & `romanisim-0.2.2/.github/workflows/ci_cron.yml`

 * *Files 4% similar despite different names*

```diff
@@ -50,12 +50,11 @@
       setenv: |
         WEBBPSF_PATH: ${{ needs.data.outputs.webbpsf_path }}
         GALSIM_CAT_PATH: ${{ needs.data.outputs.galsim_cat_path }}
       cache-path: ${{ needs.data.outputs.path }}
       cache-key: data-${{ needs.data.outputs.hash }}
       envs: |
         - macos: test-xdist
-          python-version: 3.8
-        - macos: test-xdist
           python-version: 3.9
         - macos: test-xdist
           python-version: 3.10
+        - linux: test-devdeps-xdist
```

### Comparing `romanisim-0.2.0/.github/workflows/publish-to-pypi.yml` & `romanisim-0.2.2/.github/workflows/publish-to-pypi.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,12 +5,12 @@
     types: [released]
 
 jobs:
   publish:
     uses: spacetelescope/action-publish_to_pypi/.github/workflows/workflow.yml@master
     with:
       test: false
-      build_platform_wheels: false # Set to true if your package contains a C extension
+      build_platform_wheels: true # Set to true if your package contains a C extension
     secrets:
       user: ${{ secrets.PYPI_USERNAME_STSCI_MAINTAINER }}
       password: ${{ secrets.PYPI_PASSWORD_STSCI_MAINTAINER }} # WARNING: Do not hardcode secret values here! If you want to use a different user or password, you can override this secret by creating one with the same name in your Github repository settings.
       test_password: ${{ secrets.PYPI_PASSWORD_STSCI_MAINTAINER_TEST }}
```

### Comparing `romanisim-0.2.0/.gitignore` & `romanisim-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/.readthedocs.yaml` & `romanisim-0.2.2/.readthedocs.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,23 @@
   fail_on_warning: true
 
 # Optionally build your docs in additional formats such as PDF and ePub
 formats:
   - htmlzip
   - pdf
 
+build:
+  os: ubuntu-22.04
+  tools:
+    python: mambaforge-4.10
+
+conda:
+  environment: docs/rtd_environment.yaml
+
 # Optionally set the version of Python and requirements required to build your docs
 python:
-  version: 3.8
+  system_packages: false
   install:
     - method: pip
       path: .
       extra_requirements:
         - docs
```

### Comparing `romanisim-0.2.0/CODE_OF_CONDUCT.md` & `romanisim-0.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/LICENSE` & `romanisim-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/PKG-INFO` & `romanisim-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romanisim
-Version: 0.2.0
+Version: 0.2.2
 Summary: Nancy Grace Roman Space Telescope WFI Simulator
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2022 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -38,17 +38,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 [![CI](https://github.com/spacetelescope/romanisim/actions/workflows/ci.yml/badge.svg)](https://github.com/spacetelescope/romanisim/actions/workflows/ci.yml) [![codecov](https://codecov.io/gh/spacetelescope/romanisim/branch/main/graph/badge.svg?token=pkoLtQOa2v)](https://codecov.io/gh/spacetelescope/romanisim)
```

### Comparing `romanisim-0.2.0/README.md` & `romanisim-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/docs/Makefile` & `romanisim-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/docs/conf.py` & `romanisim-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/docs/romanisim/apt.rst` & `romanisim-0.2.2/docs/romanisim/apt.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/docs/romanisim/bandpass.rst` & `romanisim-0.2.2/docs/romanisim/bandpass.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/docs/romanisim/catalog.rst` & `romanisim-0.2.2/docs/romanisim/catalog.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/docs/romanisim/image.rst` & `romanisim-0.2.2/docs/romanisim/image.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/docs/romanisim/l1.rst` & `romanisim-0.2.2/docs/romanisim/l1.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/docs/romanisim/l2.rst` & `romanisim-0.2.2/docs/romanisim/l2.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 L2 images
 =========
 
 L2 images are constructed from :doc:`L1 </romanisim/l1>` images, which are in turn constructed from idealized :doc:`count </romanisim/image>` images.  This means that even when constructing L2 images, one must go through the process of simulating how counts get apportioned among the various reads.  It is challenging to realistically model the statistics in the noise of L2 images without going through this process.
 
 L2 images are constructed by doing "ramp fitting" on the level 1 images.  Each pixel of a level 1 image is a series of "resultants", giving the measured value of that pixel averaged over a series on non-destructive reads as the exposure is being observed.  A simple model for a pixel is that its flux as a function of time is simply two numbers: a pedestal and a linear ramp representing the rate at which photons are detected by the pixel.  Ramp fitting turns these one-dimensional series of resultants into a "slope" image that is of interest astronomically.  Due to details of the H4RG detectors, the pedestals of the ramp vary widely from exposure to exposure, and so current fitting completely throws away as non-astronomical any information in the ramp that is sensitive to the pedestal.
 
-Ramps are currently fit using "optimal" weighting, considering the full covariance matrix between each of the resultants stemming from read \& Poisson noise from the sources.  The covariance is inverted and combined with the design matrix in the usual least-squares approach to solve for the optimal slope and pedestal measurements for each pixel.  This approach is naively expensive, but because the covariance matrices for each pixel for a one-dimensional family depending only on the ratio of the flux in the pixel to the read variance, the relevant matrices can be precomputed.  These are then interpolated between for each pixel and summed over to get the parameters and variances for each pixel.
+The package contains two algorithms for ramp fitting.  The first uses "optimal" weighting, considering the full covariance matrix between each of the resultants stemming from read \& Poisson noise from the sources.  The covariance is inverted and combined with the design matrix in the usual least-squares approach to solve for the optimal slope and pedestal measurements for each pixel.  This approach is naively expensive, but because the covariance matrices for each pixel for a one-dimensional family depending only on the ratio of the flux in the pixel to the read variance, the relevant matrices can be precomputed.  These are then interpolated between for each pixel and summed over to get the parameters and variances for each pixel.
 
 This approach does not handle cosmic rays or saturated pixels well, though for modest sized sets of resultants introducing an additional series of fits for the roughly :math:`2 n_\mathrm{resultant}` sub-ramps would be straightforward.  That approach would also naturally handle saturated ramps.  Even explicitly computing every possible :math:`n_\mathrm{resultant} (n_\mathrm{resultant} - 1) / 2` subramp would likely still be quite inexpensive for modestly sized ramps.
 
-This is a fairly faithful representation of how level two image construction works, so there are not many additional effects to add here.
+The second approach follows `Casertano+2022 <https://webbpsf.readthedocs.io/en/latest/installation.html#installing-the-required-data-files>`_.  In this approach, a diagonal set of weights is used in place of the full covariance matrix.  The choice of weights depend on the particular pattern of reads assigned to each resultant and the amount of flux in the ramp, allowing them to interpolate from simply differencing the first and last resultants when the flux is very large to weighting the resultants by the number of reads when the flux is zero.  This approach more efficiently handles dealing with ramps that have been split by cosmic rays, and obtaining uncertainties within a few percent of the "optimal" weighting approach.  For these cases, we report final ramp slopes and variances derived from the inverse variance weighted subramp slopes and variances, using the read-noise derived variances.
 
-* We are ignoring saturation both here and at the L1 stage.
+This is a fairly faithful representation of how level two image construction works, so there are not many additional effects to add here.  But mentioning some limitations:
+
+* We have a simplistic saturation treatment, just clipping resultants that exceed
+  the saturation level to the saturation level and throwing a flag.
+* We do not include dark counts as part of the Poisson noise term in the ramp fitting.
 
 .. automodapi:: romanisim.ramp
```

### Comparing `romanisim-0.2.0/docs/romanisim/overview.rst` & `romanisim-0.2.2/docs/romanisim/overview.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 Overview
 ==================
 
 romanisim simulates Roman Wide-Field Imager images of astronomical scenes
 described by catalogs of sources.  The simulation includes:
 
-* convolution of the sources by the appropriate PSF for each detector
-* realistic world coordinate system
+* convolution of the sources by the Roman point spread function
+* optical distortion
 * sky background
 * level 1 image support (3D image stack of up-the-ramp samples)
 * level 2 image support (2D image after calibration & ramp fitting)
 * point sources and analytic galaxy profiles
 * expected system throughput
 * dark current
 * read noise
 * inter-pixel capacitance
 * non-linearity
-* reciprocity failure
+* saturation
+* ramp fitting
+* source injection
 
 The simulator is based on galsim and most of these features directly invoke the
 equivalents in the galsim.roman package.  The chief additions of this package
-on top of the galsim.roman implementation are using "official" PSF, WCS, and
-reference files from the Roman CRDS (not yet public!) and webbpsf.  This
+on top of the galsim.roman implementation are using "official" webbpsf
+PSF, and distortion and reference files from the Roman CRDS (not yet
+public!).  This
 package also implements WFI up-the-ramp sampled and averaged images like those
 that will be downlinked from the telescope, and the official Roman WFI file
 format (asdf).
 
+Future expected features include:
+
+* frame zero effects
+* L3 image simulations
+* "image-based" simulation inputs (i.e., provide an input image based
+  on a galaxy hydro sim; romanisim applies the Roman PSF &
+  instrumental effects on top to produce a detailed instrumental simulation)
+
 The best way to interact with romanisim is to make an image.  Running ::
 
     romanisim-make-image out.asdf
 
 will make a test image in the file ``out.asdf``.  Naturally, usually one has a
 particular astronomical scene in mind, and one can't really simulate a scene
 without knowing where the telescope is pointing and when the observation is
```

### Comparing `romanisim-0.2.0/docs/romanisim/psf.rst` & `romanisim-0.2.2/docs/romanisim/psf.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/docs/romanisim/refs.rst` & `romanisim-0.2.2/docs/romanisim/refs.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/docs/romanisim/running.rst` & `romanisim-0.2.2/docs/romanisim/running.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/docs/romanisim/wcs.rst` & `romanisim-0.2.2/docs/romanisim/wcs.rst`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/pyproject.toml` & `romanisim-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 [project]
 name = 'romanisim'
 description = 'Nancy Grace Roman Space Telescope WFI Simulator'
 readme = 'README.md'
-requires-python = '>=3.8'
+requires-python = '>=3.9'
 license = { file = 'LICENSE' }
 authors = [{ name = 'STScI', email = 'help@stsci.edu' }]
 classifiers = [
     'Intended Audience :: Science/Research',
     'Topic :: Scientific/Engineering :: Astronomy',
     'License :: OSI Approved :: BSD License',
     'Operating System :: MacOS :: MacOS X',
     'Operating System :: POSIX',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3 :: Only',
-    'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
 ]
 dependencies = [
     'asdf >=2.14.2',
     'astropy >=5.2',
     'crds >=10.3.1',
     'defusedxml >=0.5',
     'galsim >=2.3',
+    'rad >=0.15',
+    'roman_datamodels >=0.15',
     'gwcs >=0.18.1',
     'jsonschema >=4.0.1',
     'webbpsf >=1.0.0',
-    'roman_datamodels >=0.14.1',
+    'Cython >=0.29.21',
 ]
 dynamic = ['version']
 
 [project.optional-dependencies]
 docs = [
     'sphinx',
     'sphinx-automodapi',
@@ -43,28 +44,29 @@
     'ci-watson >=0.3.0',
     'colorama >=0.4.1',
     'getch >=1.0.0',
     'pytest >=4.6.0',
     'pytest-openfiles >=0.5.0',
     'pytest-doctestplus >=0.10.0',
     'pytest-cov >=2.9.0',
-    'codecov >=1.6.0',
     'flake8 >=3.6.0',
 ]
 
 [project.urls]
 'Tracker' = 'https://github.com/spacetelescope/romanisim/issues'
 'Documentation' = 'https://romanisim.readthedocs.io/en/stable/'
 'Source Code' = 'https://github.com/spacetelescope/romanisim'
 
 [build-system]
 requires = [
     'setuptools >=61',
     'setuptools_scm[toml] >=3.4',
     'wheel',
+    'Cython >=0.29.21',
+    'numpy >=1.18',
 ]
 build-backend = 'setuptools.build_meta'
 
 [tool.setuptools_scm]
 
 [tool.setuptools]
 zip-safe = false
```

### Comparing `romanisim-0.2.0/romanisim/__init__.py` & `romanisim-0.2.2/romanisim/__init__.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/romanisim/apt.py` & `romanisim-0.2.2/romanisim/apt.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/romanisim/bandpass.py` & `romanisim-0.2.2/romanisim/bandpass.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/romanisim/catalog.py` & `romanisim-0.2.2/romanisim/catalog.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/romanisim/cr.py` & `romanisim-0.2.2/romanisim/cr.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/romanisim/data/Roman_effarea_20201130.csv` & `romanisim-0.2.2/romanisim/data/Roman_effarea_20201130.csv`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/romanisim/gaia.py` & `romanisim-0.2.2/romanisim/gaia.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/romanisim/image.py` & `romanisim-0.2.2/romanisim/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,30 +10,34 @@
 import astropy.time
 from astropy import units as u
 from astropy import coordinates
 from astropy import table
 import asdf
 import galsim
 from galsim import roman
-try:
-    import roman_datamodels.testing.utils as maker_utils
-except ImportError:
-    import roman_datamodels.maker_utils as maker_utils
+
+
 from . import wcs
 from . import catalog
 from . import parameters
 from . import util
 from . import nonlinearity
 import romanisim.l1
 import romanisim.bandpass
 import romanisim.psf
 import romanisim.persistence
 from romanisim import log
 import crds
-from roman_datamodels import units as ru
+
+import roman_datamodels
+try:
+    import roman_datamodels.maker_utils as maker_utils
+except ImportError:
+    import roman_datamodels.testing.utils as maker_utils
+
 
 # galsim fluxes are in photons / cm^2 / s
 # we need to specify the area and exposure time in drawImage if
 # specifying fluxes in physical units.
 # presently we're behaving a bit badly in that the fluxes are given in
 # physical units, but the galsim objects with SEDs are already scaled
 # for Roman's collecting area and exposure time.
@@ -57,15 +61,15 @@
 # should we let people specify reference files?
 # what reference files do we use?
 # distortion, read noise, dark, gain, flat
 # these would each be optional arguments that would override
 
 
 def make_l2(resultants, ma_table, read_noise=None, gain=None, flat=None,
-            linearity=None, dark=None):
+            linearity=None, dark=None, dq=None):
     """
     Simulate an image in a filter given resultants.
 
     This routine does idealized ramp fitting on a set of resultants.
 
     Parameters
     ----------
@@ -77,14 +81,16 @@
         read_noise image to use.  If None, use galsim.roman.read_noise.
     flat : np.ndarray[nx, ny] (float)
         flat field to use
     linearity : romanisim.nonlinearity.NL object or None
         non-linearity correction to use.
     dark : np.ndarray[nresultants, nx, ny] (float)
         dark image to subtract from ramps (DN)
+    dq : np.ndarray[nresultants, nx, ny] (int)
+        DQ image corresponding to resultants
 
     Returns
     -------
     im : galsim.Image
         best fitting slopes
     var_rnoise : galsim.Image
         variance in slopes from read noise
@@ -103,29 +109,41 @@
         # no error propagation
 
     if dark is not None:
         resultants = resultants - dark
 
     from . import ramp
     log.info('Fitting ramps.')
-    rampfitter = ramp.RampFitInterpolator(ma_table)
-    ramppar, rampvar = rampfitter.fit_ramps(resultants * gain,
-                                            read_noise * gain)
+
+    # commented out code below is inverse-covariance ramp fitting
+    # which doesn't presently support DQ information
+    # rampfitter = ramp.RampFitInterpolator(ma_table)
+    # ramppar, rampvar = rampfitter.fit_ramps(resultants * gain,
+    #                                         read_noise * gain)
+
+    if dq is None:
+        dq = np.zeros(resultants.shape, dtype='i4')
+    ramppar, rampvar = ramp.fit_ramps_casertano(resultants * gain, dq,
+                                                read_noise * gain, ma_table)
+
+    log.warning('The ramp fitter is unaware of noise from dark current because '
+                'it runs on dark-subtracted images.  We could consider adding '
+                'a separate dark rate term to fit ramps.')
     # could iterate if we wanted to improve the flux estimates
 
     # The ramp fitter is not presently unit-aware; fix up the units by hand.
     # To do this right the ramp fitter should be made unit aware.
     # It takes a bit of work to get this right because we use the fact
     # that the variance of a Poisson distribution is equal to its mean,
     # which isn't true as soon as things start having units and requires
     # special handling.  And we use read_time without units a lot throughout
     # the code base.
     slopes = ramppar[..., 1] / u.s
-    readvar = rampvar[..., 0, 1, 1] * (ru.electron / u.s)**2
-    poissonvar = rampvar[..., 1, 1, 1] * (ru.electron / u.s)**2
+    readvar = rampvar[..., 0, 1, 1] * (u.electron / u.s)**2
+    poissonvar = rampvar[..., 1, 1, 1] * (u.electron / u.s)**2
 
     if flat is not None:
         flat = np.clip(flat, 1e-9, np.inf)
         slopes /= flat
         readvar /= flat**2
         poissonvar /= flat**2
 
@@ -480,28 +498,30 @@
     image : galsim.Image
         idealized image of scene as seen by Roman, giving total electron counts
         from rate sources (astronomical objects; backgrounds; dark current) in
         each pixel.
     simcatobj : np.ndarray
         catalog of simulated objects in image
     """
+
     ma_table = parameters.ma_table[
-        metadata['roman.meta.exposure.ma_table_number']]
-    sca = int(metadata['roman.meta.instrument.detector'][3:])
+        metadata['exposure']['ma_table_number']]
+
+    sca = int(metadata['instrument']['detector'][3:])
     exptime = parameters.read_time * (ma_table[-1][0] + ma_table[-1][1] - 1)
     if rng is None and seed is None:
         seed = 43
         log.warning(
             'No RNG set, constructing a new default RNG from default seed.')
     if rng is None:
         rng = galsim.UniformDeviate(seed)
 
-    filter_name = metadata['roman.meta.instrument.optical_element']
+    filter_name = metadata['instrument']['optical_element']
 
-    date = metadata['roman.meta.exposure.start_time']
+    date = metadata['exposure']['start_time']
     if not isinstance(date, astropy.time.Time):
         date = astropy.time.Time(date, format='isot')
 
     galsim_filter_name = romanisim.bandpass.roman2galsim_bandpass[filter_name]
     bandpass = roman.getBandpasses(AB_zeropoint=True)[galsim_filter_name]
     imwcs = wcs.get_wcs(metadata, usecrds=usecrds)
     chromatic = False
@@ -570,133 +590,160 @@
     Returns
     -------
     image : roman_datamodels model
         simulated image
     simcatobj : np.ndarray
         image positions and fluxes of simulated objects
     """
-    all_metadata = copy.deepcopy(parameters.default_parameters_dictionary)
-    flatmetadata = util.flatten_dictionary(metadata)
-    util.add_more_metadata(metadata)
-    flatmetadata = {'roman.meta' + k if k.find('roman.meta') != 0 else k: v
-                    for k, v in flatmetadata.items()}
-    all_metadata.update(**util.flatten_dictionary(metadata))
-    ma_table_number = all_metadata['roman.meta.exposure.ma_table_number']
-    filter_name = all_metadata['roman.meta.instrument.optical_element']
+    meta = maker_utils.mk_common_meta()
+    meta["photometry"] = maker_utils.mk_photometry()
+
+    for key in parameters.default_parameters_dictionary.keys():
+        meta[key].update(parameters.default_parameters_dictionary[key])
+
+    util.add_more_metadata(meta)
+
+    for key in metadata.keys():
+        meta[key].update(metadata[key])
+
+    # Create Image model to track validation
+    image_node = maker_utils.mk_level2_image()
+    image_node['meta'] = meta
+    image_mod = roman_datamodels.datamodels.ImageModel(image_node)
+
+    ma_table_number = image_mod.meta.exposure.ma_table_number
+    filter_name = image_mod.meta.instrument.optical_element
 
     ma_table = parameters.ma_table[ma_table_number]
     exptime_tau = ((ma_table[-1][0] + (ma_table[-1][1] / 2))
                    * parameters.read_time)
 
     # TODO: replace this stanza with a function that looks at the metadata
     # and keywords and returns a dictionary with all of the relevant reference
     # data in numpy arrays.
     # should query CRDS for any reference files not specified on the command
     # line.
     if usecrds:
+        refnames_lst = ['readnoise', 'dark', 'gain', 'linearity', 'saturation']
         reffiles = crds.getreferences(
-            all_metadata, observatory='roman',
-            reftypes=['readnoise', 'dark', 'gain', 'linearity'])
-        read_noise = asdf.open(reffiles['readnoise'])['roman']['data']
-        dark = asdf.open(reffiles['dark'])['roman']['data']
-        gain = asdf.open(reffiles['gain'])['roman']['data']
-        linearity = asdf.open(reffiles['linearity'])['roman']['coeffs']
+            image_mod.get_crds_parameters(), reftypes=refnames_lst,
+            observatory='roman')
+
+        read_noise_model = roman_datamodels.datamodels.ReadnoiseRefModel(
+            reffiles['readnoise'])
+        dark_model = roman_datamodels.datamodels.DarkRefModel(
+            reffiles['dark'])
+        gain_model = roman_datamodels.datamodels.GainRefModel(
+            reffiles['gain'])
+        linearity_model = roman_datamodels.datamodels.LinearityRefModel(
+            reffiles['linearity'])
+        saturation_model = roman_datamodels.datamodels.SaturationRefModel(
+            reffiles['saturation'])
+
         try:
-            reffiles = crds.getreferences(
-                all_metadata, observatory='roman',
-                reftypes=['flat'])
-            flat = asdf.open(reffiles['flat'])['roman']['data']
+            flatfile = crds.getreferences(
+                image_mod.get_crds_parameters(),
+                reftypes=['flat'], observatory='roman')['flat']
+
+            flat_model = roman_datamodels.datamodels.FlatRefModel(flatfile)
+            flat = flat_model.data
+
         except crds.core.exceptions.CrdsLookupError:
             log.warning('Could not find flat; using 1')
             flat = 1
 
         # convert the last dark resultant into a dark rate by dividing by the
         # mean time in that resultant.
-        darkrate = dark[-1] / exptime_tau
         nborder = parameters.nborder
-        read_noise = read_noise[nborder:-nborder, nborder:-nborder]
-        darkrate = darkrate[nborder:-nborder, nborder:-nborder]
-        dark = dark[:, nborder:-nborder, nborder:-nborder]
-        gain = gain[nborder:-nborder, nborder:-nborder]
-        linearity = linearity[:, nborder:-nborder, nborder:-nborder]
-        linearity = nonlinearity.NL(linearity)
+        read_noise = read_noise_model.data[nborder:-nborder, nborder:-nborder]
+        darkrate = dark_model.data[-1, nborder:-nborder, nborder:-nborder] / exptime_tau
+        dark = dark_model.data[:, nborder:-nborder, nborder:-nborder]
+        gain = gain_model.data[nborder:-nborder, nborder:-nborder]
+        linearity = nonlinearity.NL(
+            linearity_model.coeffs[:, nborder:-nborder, nborder:-nborder])
         darkrate *= gain
+        image_mod.meta.ref_file.crds.sw_version = crds.__version__
+        image_mod.meta.ref_file.crds.context_used = crds.get_context_name(
+            observatory=image_mod.crds_observatory
+        )
+        saturation = saturation_model.data[nborder:-nborder, nborder:-nborder]
     else:
         read_noise = galsim.roman.read_noise
         darkrate = galsim.roman.dark_current
         dark = None
         gain = None
         flat = 1
         linearity = None
+        saturation = None
 
     if rng is None and seed is None:
         seed = 43
         log.warning(
             'No RNG set, constructing a new default RNG from default seed.')
     if rng is None:
         rng = galsim.UniformDeviate(seed)
 
     if persistence is None:
         persistence = romanisim.persistence.Persistence()
 
     log.info('Simulating filter {0}...'.format(filter_name))
     counts, simcatobj = simulate_counts(
-        all_metadata, objlist, rng=rng,
-        usecrds=usecrds, darkrate=darkrate,
+        image_mod.meta, objlist, rng=rng, usecrds=usecrds, darkrate=darkrate,
         webbpsf=webbpsf, flat=flat)
     if level == 0:
         im = dict(data=counts.array)
     else:
-        l1 = romanisim.l1.make_l1(
+        l1, l1dq = romanisim.l1.make_l1(
             counts, ma_table_number, read_noise=read_noise, rng=rng, gain=gain,
             crparam=crparam,
-            linearity=linearity, tstart=astropy.time.Time(
-                all_metadata['roman.meta.exposure.start_time']),
-            persistence=persistence,
+            linearity=linearity, tstart=image_mod.meta.exposure.start_time,
+            persistence=persistence, saturation=saturation,
             **kwargs)
     if level == 1:
-        im = romanisim.l1.make_asdf(l1, metadata=all_metadata,
+        im = romanisim.l1.make_asdf(l1, dq=l1dq, metadata=image_mod.meta,
                                     persistence=persistence)
+
     elif level == 2:
         slopeinfo = make_l2(l1, ma_table, read_noise=read_noise,
                             gain=gain, flat=flat, linearity=linearity,
-                            dark=dark)
-        im = make_asdf(*slopeinfo, metadata=all_metadata,
-                       persistence=persistence)
+                            dark=dark, dq=l1dq)
+        l2dq = np.bitwise_or.reduce(l1dq, axis=0)
+        im = make_asdf(*slopeinfo, metadata=image_mod.meta,
+                       persistence=persistence, dq=l2dq)
     log.info('Simulation complete.')
     return im, simcatobj
 
 
 def make_test_catalog_and_images(
-        seed=12345, sca=7, filters=None, nobj=1000, return_variance=False,
+        seed=12345, sca=7, filters=None, nobj=1000, 
         usecrds=True, webbpsf=True, galaxy_sample_file_name=None, **kwargs):
     """This routine kicks the tires on everything in this module."""
     log.info('Making catalog...')
     if filters is None:
         filters = ['Y106', 'J129', 'H158']
     metadata = copy.deepcopy(parameters.default_parameters_dictionary)
-    metadata['roman.meta.instrument.detector'] = 'WFI%02d' % sca
+    metadata['instrument']['detector'] = 'WFI%02d' % sca
     imwcs = wcs.get_wcs(metadata, usecrds=usecrds)
     rd_sca = imwcs.toWorld(galsim.PositionD(
         roman.n_pix / 2 + 0.5, roman.n_pix / 2 + 0.5))
     cat = catalog.make_dummy_catalog(
         rd_sca, seed=seed, nobj=nobj,
         galaxy_sample_file_name=galaxy_sample_file_name)
     rng = galsim.UniformDeviate(0)
     out = dict()
     for filter_name in filters:
-        metadata['roman.meta.instrument.optical_element'] = filter_name
+        metadata['instrument']['optical_element'] = 'F' + filter_name[1:]
         im = simulate(metadata, objlist=cat, rng=rng, usecrds=usecrds,
                       webbpsf=webbpsf, **kwargs)
         out[filter_name] = im
     return out
 
 
 def make_asdf(slope, slopevar_rn, slopevar_poisson, metadata=None,
-              filepath=None, persistence=None):
+              filepath=None, persistence=None, dq=None):
     """Wrap a galsim simulated image with ASDF/roman_datamodel metadata.
 
     Eventually this needs to get enough info to reconstruct a refit WCS.
     """
 
     out = maker_utils.mk_level2_image()
     # fill this output with as much real information as possible.
@@ -743,23 +790,20 @@
     #     the "right" thing is probably
     #     sqrt(noisless image + read_noise**2)
     #     i.e., Gaussian approximation of Poisson noise + read noise.
     #     this is just sqrt(var_poisson + var_rnoise + var_flat)?
     # var_rnoise: okay
     # var_flat: currently zero
     if metadata is not None:
-        # ugly mess of flattening & unflattening to make sure that deeply
-        # nested keywords all get propagated into the metadata structure.
-        tmpmeta = util.flatten_dictionary(out['meta'])
-        tmpmeta.update(util.flatten_dictionary(
-            util.unflatten_dictionary(metadata)['roman']['meta']))
-        out['meta'].update(util.unflatten_dictionary(tmpmeta))
+        out['meta'].update(metadata)
 
     out['data'] = slope
     out['dq'] = np.zeros(slope.shape, dtype='u4')
+    if dq is not None:
+        out['dq'][:, :] = dq
     out['var_poisson'] = slopevar_poisson
     out['var_rnoise'] = slopevar_rn
     out['var_flat'] = slopevar_rn * 0
     out['err'] = np.sqrt(out['var_poisson'] + out['var_rnoise'] + out['var_flat'])
     if persistence is not None:
         out['meta']['persistence'] = persistence.to_dict()
     if filepath:
```

### Comparing `romanisim-0.2.0/romanisim/l1.py` & `romanisim-0.2.2/romanisim/l1.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,17 +108,15 @@
 
 import numpy as np
 import asdf
 import galsim
 from scipy import ndimage
 from . import parameters
 from . import log
-from . import util
 from astropy import units as u
-from roman_datamodels import units as ru
 from . import cr
 
 
 def validate_times(tij):
     """Verify that a set of times tij for a valid resultant.
 
     Parameters
@@ -230,16 +228,19 @@
     rng : galsim.BaseDeviate
         random number generator
     seed : int
         seed to use for random number generator
 
     Returns
     -------
-    np.ndarray[n_resultant, nx, ny]
+    resultants, dq
+    resultants : np.ndarray[n_resultant, nx, ny]
         array of n_resultant images giving each resultant
+    dq : np.ndarray[n_resultant, nx, ny]
+        dq array marking CR hits in resultants
     """
     if not np.all(counts == np.round(counts)):
         raise ValueError('apportion_counts_to_resultants expects the counts '
                          'to be integers!')
 
     if rng is None and seed is None:
         seed = 46
@@ -255,14 +256,15 @@
     # two separate generators so that if you turn off CRs / persistence
     # you don't change the image
 
     pij = tij_to_pij(tij, remaining=True)
     resultants = np.zeros((len(tij),) + counts.shape, dtype='f4')
     counts_so_far = np.zeros(counts.shape, dtype='f4')
     resultant_counts = np.zeros(counts.shape, dtype='f4')
+    dq = np.zeros(resultants.shape, dtype='i4')
 
     efficiency = 1
     if linearity is not None:
         pij_per_read = tij_to_pij(tij)
         ki_numerator = np.cumsum(pij_per_read)
         ki_denominator = np.zeros(counts_so_far.shape, dtype='f4')
 
@@ -305,16 +307,19 @@
                 m = (efficiency < 0) | (efficiency > 1)
                 nlflag[m] = True
                 efficiency = np.clip(efficiency, 0, 1)
             read = rng_numpy.binomial((counts - counts_so_far).astype('i4'),
                                       p * efficiency * ki)
             counts_so_far += read
             if crparam is not None:
+                old_instrumental_so_far = instrumental_so_far.copy()
                 cr.simulate_crs(instrumental_so_far, parameters.read_time,
                                 **crparam, rng=rng_numpy_cr)
+                crhits = instrumental_so_far != old_instrumental_so_far
+                dq[i, crhits] |= parameters.dqbits['jump_det']
             if persistence is not None:
                 tnow = tstart + tij[i][j] / (24 * 60 * 60)
                 persistence.add_to_read(
                     instrumental_so_far, tnow, rng=rng_numpy_ps)
             resultant_counts += counts_so_far + instrumental_so_far
             if linearity is not None:
                 ki_denominator += efficiency * pij_per_read[i][j]
@@ -329,15 +334,15 @@
 
     nweirdpixfrac = np.sum(nlflag) / np.product(nlflag.shape)
     if nweirdpixfrac > 0:
         log.warning(f'{nweirdpixfrac:5.1e} fraction of pixels have '
                     'observed(corrected) nonlinearity slopes of >1 or <0.  '
                     'The CRDS reference values are likely problematic for '
                     'these pixels.')
-    return resultants
+    return resultants, dq
 
 
 def add_read_noise_to_resultants(resultants, tij, read_noise=None, rng=None,
                                  seed=None):
     """Adds read noise to resultants.
 
     The resultants get Gaussian read noise with sigma = sigma_read/sqrt(N).
@@ -378,27 +383,29 @@
         read_noise = parameters.read_noise
     noise = noise * read_noise / np.array(
         [len(x)**0.5 for x in tij]).reshape(-1, 1, 1)
     resultants += noise
     return resultants
 
 
-def make_asdf(resultants, filepath=None, metadata=None, persistence=None):
+def make_asdf(resultants, dq=None, filepath=None, metadata=None, persistence=None):
     """Package and optionally write out an L1 frame.
 
     This routine packages an L1 data file with the appropriate Roman data
     model.  It currently does not do anything with the necessary metadata,
     and leaves that information as filler values.
 
     Parameters
     ----------
     resultants : np.ndarray[n_resultant, nx, ny] (float)
         resultants array, giving each of n_resultant resultant images
     filepath : str
         if not None, path of asdf file to L1 image into
+    dq : np.ndarray[n_resultant, nx, ny] (int)
+        dq array flagging saturated / CR hit pixels
 
     Returns
     -------
     roman_datamodels.datamodels.ScienceRawModel
         L1 image
     """
 
@@ -407,19 +414,19 @@
     except ImportError:
         import roman_datamodels.maker_utils as maker_utils
     nborder = parameters.nborder
     npix = galsim.roman.n_pix + 2 * nborder
     out = maker_utils.mk_level1_science_raw(
         shape=(len(resultants), npix, npix))
     if metadata is not None:
-        tmpmeta = util.flatten_dictionary(out['meta'])
-        tmpmeta.update(util.flatten_dictionary(
-            util.unflatten_dictionary(metadata)['roman']['meta']))
-        out['meta'].update(util.unflatten_dictionary(tmpmeta))
+        out['meta'].update(metadata)
     out['data'][:, nborder:-nborder, nborder:-nborder] = resultants
+    if dq is not None:
+        out['dq'] = np.zeros(out['data'].shape, dtype='i4')
+        out['dq'][:, nborder:-nborder, nborder:-nborder] = dq
     if persistence is not None:
         out['meta']['persistence'] = persistence.to_dict()
     if filepath:
         af = asdf.AsdfFile()
         af.tree = {'roman': out}
         af.write_to(filepath)
     return out
@@ -478,15 +485,15 @@
                            mode='constant', cval=0)
     return out
 
 
 def make_l1(counts, ma_table_number,
             read_noise=None, rng=None, seed=None,
             gain=None, linearity=None, crparam=None,
-            persistence=None, tstart=None):
+            persistence=None, tstart=None, saturation=None):
     """Make an L1 image from a counts image.
 
     This apportions the total counts among the different resultants and adds
     some instrumental effects.  The current instrumental effects aren't quite
     right: nonlinearity and reciprocity failure are applied to the resultants
     rather than to the reads (which aren't really available to this function).
 
@@ -513,51 +520,64 @@
     persistence : romanisim.persistence.Persistence
         Persistence instance describing persistence-affected pixels
     tstart : astropy.time.Time
         time of exposure start
 
     Returns
     -------
-    np.ndarray[n_resultant, nx, ny]
+    l1, dq
+    l1: np.ndarray[n_resultant, nx, ny]
         resultants image array including systematic effects
+    dq: np.ndarray[n_resultant, nx, ny]
+        DQ array marking saturated pixels and cosmic rays
     """
 
     tij = ma_table_to_tij(ma_table_number)
     log.info('Apportioning counts to resultants...')
-    resultants = apportion_counts_to_resultants(
+    resultants, dq = apportion_counts_to_resultants(
         counts.array, tij, linearity=linearity, crparam=crparam,
         persistence=persistence, tstart=tstart,
         rng=rng, seed=seed)
 
     # roman.addReciprocityFailure(resultants_object)
 
     add_ipc(resultants)
 
     if not isinstance(resultants, u.Quantity):
-        resultants *= ru.electron
+        resultants *= u.electron
 
     if gain is None:
         gain = parameters.gain
     if gain is not None and not isinstance(gain, u.Quantity):
-        gain = gain * ru.electron / ru.DN
+        gain = gain * u.electron / u.DN
         log.warning('Making up units for gain.')
 
     resultants /= gain
 
     if read_noise is not None and not isinstance(read_noise, u.Quantity):
-        read_noise = read_noise * ru.DN
+        read_noise = read_noise * u.DN
         log.warning('Making up units for read noise.')
 
     # resultants are now in counts.
     # read noise is in counts.
     log.info('Adding read noise...')
     resultants = add_read_noise_to_resultants(
         resultants, tij, rng=rng, seed=seed,
         read_noise=read_noise)
 
     # quantize
     resultants = np.round(resultants)
 
-    # garbage "saturation" implementation
-    resultants = np.clip(resultants, 0 * ru.DN, (2**16 - 1) * ru.DN)
+    # add pedestal
+    resultants += parameters.pedestal
 
-    return resultants
+    if saturation is None:
+        saturation = parameters.saturation
+
+    # this maybe should be better applied at read time?
+    # it's not actually clear to me what the right thing to do
+    # is in detail.
+    resultants = np.clip(resultants, 0 * u.DN, saturation)
+    m = resultants >= saturation
+    dq[m] |= parameters.dqbits['saturated']
+
+    return resultants, dq
```

### Comparing `romanisim-0.2.0/romanisim/nonlinearity.py` & `romanisim-0.2.2/romanisim/nonlinearity.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/romanisim/persistence.py` & `romanisim-0.2.2/romanisim/persistence.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/romanisim/psf.py` & `romanisim-0.2.2/romanisim/psf.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/romanisim/ramp.py` & `romanisim-0.2.2/romanisim/ramp.py`

 * *Files 21% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 So the routines in these packages construct these different matrices, store
 them, and interpolate between them for different different fluxes and ratios.
 """
 
 import numpy as np
 from . import parameters
+import romanisim.ramp_fit_casertano
 from scipy import interpolate
 from astropy import units as u
 
 
 def ma_table_to_tbar(ma_table):
     """Construct the mean times for each resultant from an ma_table.
 
@@ -358,14 +359,16 @@
             read_noise.shape + (1,) * (len(var.shape) - len(read_noise.shape)))
         var *= read_noise**2
         return var
 
     def fit_ramps(self, resultants, read_noise, fluxest=None):
         """Fit ramps for a set of resultants and their read noise.
 
+        Does not handle partial ramps (i.e., broken due to CRs).
+
         Parameters
         ----------
         resultants : np.ndarray[n_resultants, nx, ny] (numeric)
             Resultants to fit
         read_noise : float or array_like like resultants
             read noise in array
         fluxest : float or array_like like resultants
@@ -453,11 +456,203 @@
     from . import l1
 
     if ma_table is None:
         ma_table = [[1, 4], [5, 1], [6, 3], [9, 10], [19, 3], [22, 15]]
     nread = np.array([x[1] for x in ma_table])
     tij = l1.ma_table_to_tij(ma_table)
     totcounts = np.random.poisson(flux * np.max(np.concatenate(tij)), ntrial)
-    resultants = l1.apportion_counts_to_resultants(totcounts, tij)
+    resultants, dq = l1.apportion_counts_to_resultants(totcounts, tij)
     resultants += np.random.randn(len(ma_table), ntrial) * (
         readnoise / np.sqrt(nread)).reshape(len(ma_table), 1)
     return (ma_table, flux, readnoise, resultants)
+
+
+def fit_ramps_casertano(resultants, dq, read_noise, ma_table):
+    """Fit ramps following Casertano+2022, including averaging partial ramps.
+
+    Ramps are broken where dq != 0, and fits are performed on each sub-ramp.
+    Resultants containing multiple ramps have their ramp fits averaged using
+    inverse variance weights based on the variance in the individual slope fits
+    due to read noise.
+
+    Parameters
+    ----------
+    resultants : np.ndarry[nresultants, ...]
+        the resultants in electrons
+    dq : np.ndarry[nresultants, ...]
+        the dq array.  dq != 0 implies bad pixel / CR.
+    read noise: float
+        the read noise in electrons
+    ma_table : list[list[int]]
+        the ma table prescription
+
+    Returns
+    -------
+    par : np.ndarray[..., 2] (float)
+        the best fit pedestal and slope for each pixel
+    var : np.ndarray[..., 3, 2, 2] (float)
+        the covariance matrix of par, for each of three noise terms:
+        the read noise, Poisson source noise, and total noise.
+    """
+
+    resultants_unit = getattr(resultants, 'unit', None)
+    if resultants_unit is not None:
+        resultants = resultants.to(u.electron).value
+
+    resultants = np.array(resultants).astype('f4')
+
+    dq = np.array(dq).astype('i4')
+
+    if np.ndim(read_noise) <= 1:
+        read_noise = read_noise * np.ones(resultants.shape[1:])
+    read_noise = np.array(read_noise).astype('f4')
+
+    origshape = resultants.shape
+    if len(resultants.shape) == 1:
+        # single ramp.
+        resultants = resultants.reshape(origshape + (1,))
+        dq = dq.reshape(origshape + (1,))
+        read_noise = read_noise.reshape(origshape[1:] + (1,))
+
+    rampfitdict = romanisim.ramp_fit_casertano.fit_ramps(
+        resultants.reshape(resultants.shape[0], -1),
+        dq.reshape(resultants.shape[0], -1),
+        read_noise.reshape(-1),
+        ma_table)
+
+    par = np.zeros(resultants.shape[1:] + (2,), dtype='f4')
+    var = np.zeros(resultants.shape[1:] + (3, 2, 2), dtype='f4')
+
+    npix = resultants.reshape(resultants.shape[0], -1).shape[1]
+    # we need to do some averaging to merge the results in each ramp.
+    # inverse variance weights based on slopereadvar
+    weight = ((rampfitdict['slopepoissonvar'] != 0) / (
+        rampfitdict['slopereadvar'] + (rampfitdict['slopereadvar'] == 0)))
+    weight = np.clip(weight, 0, 10**10)  # gracefully? handle read noise = 0 case.
+    totweight = np.bincount(rampfitdict['pix'], weights=weight, minlength=npix)
+    totval = np.bincount(rampfitdict['pix'],
+                         weights=weight * rampfitdict['slope'],
+                         minlength=npix)
+    # fill in the averaged slopes
+    par.reshape(npix, 2)[:, 1] = (
+        totval / (totweight + (totweight == 0)))
+
+    # read noise variances
+    totval = np.bincount(
+        rampfitdict['pix'], weights=weight ** 2 * rampfitdict['slopereadvar'],
+        minlength=npix)
+    var.reshape(npix, 3, 2, 2)[:, 0, 1, 1] = (
+        totval / (totweight ** 2 + (totweight == 0)))
+    # poisson noise variances
+    totval = np.bincount(
+        rampfitdict['pix'],
+        weights=weight ** 2 * rampfitdict['slopepoissonvar'], minlength=npix)
+    var.reshape(npix, 3, 2, 2)[..., 1, 1, 1] = (
+        totval / (totweight ** 2 + (totweight == 0)))
+
+    var[..., 1, 1, 1] *= par[..., 1]  # multiply Poisson term by flux
+    var[..., 2, 1, 1] = var[..., 0, 1, 1] + var[..., 1, 1, 1]
+
+    if resultants.shape != origshape:
+        par = par[0]
+        var = var[0]
+
+    if resultants_unit is not None:
+        par = par * resultants_unit
+
+    return par, var
+
+
+def fit_ramps_casertano_no_dq(resultants, read_noise, ma_table):
+    """Fit ramps following Casertano+2022, only using full ramps.
+
+    This is a simpler implementation of fit_ramps_casertano, which doesn't
+    address the case of partial ramps broken by CRs.  This case is easier
+    and can be done reasonably efficiently in pure python; results can be
+    compared with fit_ramps_casertano in for the case of unbroken ramps.
+
+    Parameters
+    ----------
+    resultants : np.ndarry[nresultants, npixel]
+        the resultants in electrons
+    read noise: float
+        the read noise in electrons
+    ma_table : list[list[int]]
+        the ma table prescription
+
+    Returns
+    -------
+    par : np.ndarray[nx, ny, 2] (float)
+        the best fit pedestal and slope for each pixel
+    var : np.ndarray[nx, ny, 3, 2, 2] (float)
+        the covariance matrix of par, for each of three noise terms:
+        the read noise, Poisson source noise, and total noise.
+    """
+    nadd = len(resultants.shape) - 1
+    if np.ndim(read_noise) <= 1:
+        read_noise = np.array(read_noise).reshape((1,) * nadd)
+    smax = resultants[-1]
+    s = smax / np.sqrt(read_noise**2 + smax)  # Casertano+2022 Eq. 44
+    ptable = np.array([  # Casertano+2022, Table 2
+        [-np.inf, 0], [5, 0.4], [10, 1], [20, 3], [50, 6], [100, 10]])
+    pp = ptable[np.searchsorted(ptable[:, 0], s) - 1, 1]
+    nn = np.array([x[1] for x in ma_table])  # number of reads in each resultant
+    tbar = ma_table_to_tbar(ma_table)
+    tau = ma_table_to_tau(ma_table)
+    tbarmid = (tbar[0] + tbar[-1]) / 2
+    if nadd > 0:
+        newshape = ((-1,) + (1,) * nadd)
+        nn = nn.reshape(*newshape)
+        tbar = tbar.reshape(*newshape)
+        tau = tau.reshape(*newshape)
+        tbarmid = tbarmid.reshape(*newshape)
+    ww = (  # Casertano+22, Eq. 45
+        (1 + pp)[None, ...] * nn
+        / (1 + pp[None, ...] * nn)
+        * np.abs(tbar - tbarmid) ** pp[None, ...])
+
+    # Casertano+22 Eq. 35
+    f0 = np.sum(ww, axis=0)
+    f1 = np.sum(ww * tbar, axis=0)
+    f2 = np.sum(ww * tbar**2, axis=0)
+    # Casertano+22 Eq. 36
+    dd = f2 * f0 - f1 ** 2
+    bad = dd == 0
+    dd[bad] = 1
+    # Casertano+22 Eq. 37
+    kk = (f0[None, ...] * tbar - f1[None, ...]) * ww / (
+        dd[None, ...])
+    # shape: [n_resultant, ny, nx]
+    ff = np.sum(kk * resultants, axis=0)  # Casertano+22 Eq. 38
+    # Casertano+22 Eq. 39
+    vr = np.sum(kk**2 / nn, axis=0) * read_noise**2
+    # Casertano+22 Eq. 40
+    vs1 = np.sum(kk**2 * tau, axis=0)
+    vs2inner = np.cumsum(kk * tbar, axis=0)
+    vs2inner = np.concatenate([0 * vs2inner[0][None, ...], vs2inner[:-1, ...]], axis=0)
+    vs2 = 2 * np.sum(vs2inner * kk, axis=0)
+    # sum_{i=1}^{j-1} K_i \bar{t}_i
+    # this is the inner of the two sums in the 2nd term of Eq. 40
+    # Casertano+22 has some discussion of whether it's more efficient to do
+    # this as an explicit double sum or to construct the inner sum separately.
+    # We've made a lot of other quantities that are [nr, ny, nx] in size,
+    # so I don't feel bad about making another.  Clearly a memory optimized
+    # code would work a lot harder to reuse a lot of variables above!
+
+    vs = (vs1 + vs2) * ff
+    vs = np.clip(vs, 0, np.inf)
+    # we can estimate negative flux, but we really shouldn't add variance for
+    # that case!
+
+    # match return values from RampFitInterpolator.fit_ramps
+    # we haven't explicitly calculated here the pedestal, its
+    # uncertainty, or covariance terms.  We just fill
+    # with zeros.
+
+    par = np.zeros(ff.shape + (2,), dtype='f4')
+    var = np.zeros(ff.shape + (3, 2, 2), dtype='f4')
+    par[..., 1] = ff
+    var[..., 0, 1, 1] = vr
+    var[..., 1, 1, 1] = vs
+    var[..., 2, 1, 1] = vr + vs
+
+    return par, var
```

### Comparing `romanisim-0.2.0/romanisim/tests/test_bandpass.py` & `romanisim-0.2.2/romanisim/tests/test_bandpass.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/romanisim/tests/test_catalog.py` & `romanisim-0.2.2/romanisim/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/romanisim/tests/test_cr.py` & `romanisim-0.2.2/romanisim/tests/test_cr.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     ii, jj, lengths = cr.traverse([53.6, 77.1], [54.8, 76.1])
     # set of pixels is unique
     assert len(set(zip(ii, jj))) == len(ii)
     i1, j1 = np.random.random((2, 100)) * 100
     i2, j2 = np.random.random((2, 100)) * 100
     for i in range(len(i1)):
         ii, jj, lengths = cr.traverse((i1[i], j1[i]), (i2[i], j2[i]), 100, 100)
+        totlen = np.hypot(i1[i] - i2[i], j1[i] - j2[i])
         assert len(set(zip(ii, jj))) == len(ii)
         assert np.all(lengths > 0)
-        assert np.all(lengths < np.hypot(i1[i] - i2[i], j1[i] - j2[i]))
-
+        assert np.all((lengths < totlen) | np.isclose(lengths, totlen))
 
 def test_create_sampler():
     xx = np.linspace(0, 1, 1000)
     sampler = cr.create_sampler(lambda x: np.ones_like(x), xx)
     assert np.allclose(sampler(xx), xx)
```

### Comparing `romanisim-0.2.0/romanisim/tests/test_gaia.py` & `romanisim-0.2.2/romanisim/tests/test_gaia.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/romanisim/tests/test_image.py` & `romanisim-0.2.2/romanisim/tests/test_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,28 +10,29 @@
 - simulate: reads in Roman calibration files.  Sends to simulate_counts, and
   further passes that to L1 and L2 routines.
 - make_test_catalog_and_images: routine which kicks the tires on everything.
 - make_asdf: Makes an l2 asdf file.
 """
 
 import os
+import copy
 import numpy as np
 import galsim
 from galsim import roman
 from romanisim import image, parameters, catalog, psf, util, wcs, persistence
 from astropy.coordinates import SkyCoord
 from astropy import units as u
 from astropy.time import Time
 from astropy import table
 import asdf
 import webbpsf
 from astropy.modeling.functional_models import Sersic2D
 import pytest
 from romanisim import log
-from roman_datamodels import units as ru
+from roman_datamodels.stnode import WfiScienceRaw, WfiImage
 
 
 def test_in_bounds():
     bounds = galsim.BoundsI(0, 1000, 0, 1000)
     xx = np.random.rand(1000) * 1000
     yy = np.random.rand(1000) * 1000
     assert np.all(image.in_bounds(xx, yy, bounds, 0))
@@ -68,18 +69,19 @@
 def test_make_l2():
     resultants = np.ones((4, 50, 50), dtype='i4')
     ma_table = [[0, 4], [4, 4], [8, 4], [12, 4]]
     slopes, readvar, poissonvar = image.make_l2(
         resultants, ma_table, gain=1, flat=1, dark=0)
     assert np.allclose(slopes, 0)
     resultants[:, :, :] = np.arange(4)[:, None, None]
-    resultants *= ru.DN
+    resultants *= u.DN
+    gain = 1 * u.electron / u.DN
     slopes, readvar, poissonvar = image.make_l2(
         resultants, ma_table,
-        gain=1 * ru.electron / ru.DN, flat=1, dark=0)
+        gain=gain, flat=1, dark=0)
     assert np.allclose(slopes, 1 / parameters.read_time / 4 * u.electron / u.s)
     assert np.all(np.array(slopes.shape) == np.array(readvar.shape))
     assert np.all(np.array(slopes.shape) == np.array(poissonvar.shape))
     assert np.all(readvar >= 0)
     assert np.all(poissonvar >= 0)
     slopes1, readvar1, poissonvar1 = image.make_l2(
         resultants, ma_table, read_noise=1, dark=0)
@@ -92,15 +94,15 @@
     assert np.all(np.abs(readvar2 / (readvar1 * 4) - 1) < 0.1)
     slopes2, readvar2, poissonvar2 = image.make_l2(
         resultants, ma_table, read_noise=1, flat=0.5)
     assert np.allclose(slopes2, slopes1 / 0.5)
     assert np.allclose(readvar2, readvar1 / 0.5**2)
     assert np.allclose(poissonvar2, poissonvar1 / 0.5**2)
     slopes, readvar, poissonvar = image.make_l2(
-        resultants, ma_table, read_noise=1, gain=1, flat=1,
+        resultants, ma_table, read_noise=1, gain=gain, flat=1,
         dark=resultants)
     assert np.allclose(slopes, 0)
 
 
 def set_up_image_rendering_things():
     im = galsim.Image(100, 100, scale=0.1, xmin=0, ymin=0)
     filter_name = 'F158'
@@ -361,23 +363,29 @@
     for o in graycat:
         o.sky_pos = coord
     # these are all dumb coordinates; the coord sent to simulate_counts
     # is the coordinate of the boresight, but that doesn't need to be on SCA 1.
     # But at least they'll exercise some machinery if the ignore_distant_sources
     # argument is high enough!
     roman.n_pix = 100
-    metadata = {'roman.meta.exposure.start_time': '2020-01-01T00:00:00',
-                'roman.meta.instrument.detector': 'WFI01',
-                'roman.meta.instrument.optical_element': 'F158',
-                'roman.meta.exposure.ma_table_number': 1,
-                }
-    wcs.fill_in_parameters(metadata, coord)
-    im1 = image.simulate_counts(metadata, chromcat, usecrds=False,
+
+    meta = {
+        'exposure': {
+            'start_time': Time('2020-01-01T00:00:00'),
+            'ma_table_number' : 1,
+        },
+        'instrument': {
+            'detector': 'WFI01',
+            'optical_element': 'F158',
+        },
+    }
+    wcs.fill_in_parameters(meta, coord)
+    im1 = image.simulate_counts(meta, chromcat, usecrds=False,
                                 webbpsf=False, ignore_distant_sources=100)
-    im2 = image.simulate_counts(metadata, graycat,
+    im2 = image.simulate_counts(meta, graycat,
                                 usecrds=False, webbpsf=True,
                                 ignore_distant_sources=100)
     im1 = im1[0].array
     im2 = im2[0].array
     maxim = np.where(im1 > im2, im1, im2)
     m = np.abs(im1 - im2) <= 20 * np.sqrt(maxim)
     assert np.all(m)
@@ -388,23 +396,32 @@
     """Test convolved image generation and L2 simulation framework.
     Demonstrates DMS216: convolved image generation - Level 2
     Demonstrates DMS224: persistence.
     """
     imdict = set_up_image_rendering_things()
     # simulate gray, chromatic, level0, level1, level2 images
     roman.n_pix = 100
-    meta = dict()
     coord = SkyCoord(270 * u.deg, 66 * u.deg)
     time = Time('2020-01-01T00:00:00')
-    meta['roman.meta.exposure.start_time'] = time
-    meta['roman.meta.pointing.ra_v1'] = coord.ra.to(u.deg).value
-    meta['roman.meta.pointing.dec_v1'] = coord.dec.to(u.deg).value
-    meta['roman.meta.exposure.ma_table_number'] = 1
-    meta['roman.meta.instrument.optical_element'] = 'F158'
-    meta['roman.meta.instrument.detector'] = 'WFI01'
+
+    meta = {
+        'exposure' : {
+            'start_time' : time,
+            'ma_table_number' : 1,
+        },
+        'instrument' : {
+            'optical_element' : 'F158',
+            'detector' : 'WFI01'
+        },
+        'pointing' : {
+            'ra_v1' : coord.ra.to(u.deg).value,
+            'dec_v1' : coord.dec.to(u.deg).value,
+        },
+    }
+
     chromcat = imdict['chromcatalog']
     graycat = imdict['graycatalog']
     for o in chromcat:
         o.sky_pos = coord
     for o in graycat:
         o.sky_pos = coord
     l0 = image.simulate(meta, graycat, webbpsf=True, level=0,
@@ -424,15 +441,15 @@
     rng = galsim.BaseDeviate(1)
     l1_nocr = image.simulate(meta, graycat, webbpsf=True, level=1,
                              usecrds=False, crparam=None, rng=rng)
     assert np.all(l1[0].data >= l1_nocr[0].data)
     log.info('DMS221: Successfully added cosmic rays to an L1 image.')
     l2 = image.simulate(meta, graycat, webbpsf=True, level=2,
                         usecrds=False, crparam=dict())
-    # through in some CRs for fun
+    # throw in some CRs for fun
     l2c = image.simulate(meta, chromcat, webbpsf=False, level=2,
                          usecrds=False)
     persist = persistence.Persistence()
     fluence = 30000
     persist.update(l0[0]['data'] * 0 + fluence, time.mjd - 100 / 60 / 60 / 24)
     # zap the whole frame, 100 seconds ago.
     rng = galsim.BaseDeviate(1)
@@ -484,7 +501,48 @@
     roman.n_pix = 100
     fn = os.environ.get('GALSIM_CAT_PATH', None)
     if fn is not None:
         fn = str(fn)
     res = image.make_test_catalog_and_images(usecrds=False,
                                              galaxy_sample_file_name=fn)
     assert len(res) > 0
+
+@pytest.mark.parametrize(
+    "level",
+    [
+        1, 2,
+    ],
+)
+@pytest.mark.skipif(
+    os.environ.get("CI") == "true",
+    reason=(
+        "Roman CRDS servers are not currently available outside the internal network"
+    ),
+)
+def test_reference_file_crds_match(level):
+    # Set up parameters for simulation run
+    galsim.roman.n_pix = 4088
+    metadata = copy.deepcopy(parameters.default_parameters_dictionary)
+    metadata['instrument']['detector'] = 'WFI07'
+    metadata['instrument']['optical_element'] = 'F158'
+    metadata['exposure']['ma_table_number'] = 1
+
+    twcs = wcs.get_wcs(metadata, usecrds=True)
+    rd_sca = twcs.toWorld(galsim.PositionD(
+        galsim.roman.n_pix / 2, galsim.roman.n_pix / 2))
+
+    cat = catalog.make_dummy_table_catalog(
+        rd_sca, bandpasses=[metadata['instrument']['optical_element']], nobj=1000)
+
+    rng = galsim.UniformDeviate(None)
+    im, simcatobj = image.simulate(
+        metadata, cat, usecrds=True,
+        webbpsf=True, level=level,
+        rng=rng)
+
+    # Confirm that CRDS keyword was updated
+    assert im.meta.ref_file.crds.sw_version != '12.3.1'
+
+    if (level==1):
+        assert (type(im) == WfiScienceRaw)
+    else: #level = 2
+        assert (type(im) == WfiImage)
```

### Comparing `romanisim-0.2.0/romanisim/tests/test_l1.py` & `romanisim-0.2.2/romanisim/tests/test_l1.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 - make_asdf
 - ma_table_to_tij
 - make_l1
 """
 
 import pytest
 import numpy as np
-from romanisim import l1, log
+from romanisim import l1, log, parameters
 import galsim
 import galsim.roman
 import asdf
-from roman_datamodels import units as ru
+from astropy import units as u
 
 
 tijlist = [
     [[1], [2, 3], [4, 5], [6, 7]],
     [[100], [101, 102, 103], [110]],
     [[1], [2], [3, 4, 5, 100]],
 ]
@@ -61,42 +61,43 @@
     read noise to those resultants, fulfilling DMS220.
     """
     # we'll skip the linearity tests until new linearity files with
     # inverse coefficients are available in CRDS.
     counts = np.random.poisson(100, size=(100, 100))
     read_noise = 10
     for tij in tijlist:
-        resultants = l1.apportion_counts_to_resultants(counts, tij)
+        resultants, dq = l1.apportion_counts_to_resultants(counts, tij)
         assert np.all(np.diff(resultants, axis=0) >= 0)
         assert np.all(resultants >= 0)
         assert np.all(resultants <= counts[None, :, :])
-        res2 = l1.add_read_noise_to_resultants(resultants.copy() * ru.DN,
+        res2 = l1.add_read_noise_to_resultants(resultants.copy() * u.DN,
                                                tij)
         res3 = l1.add_read_noise_to_resultants(resultants.copy(), tij,
                                                read_noise=read_noise)
         assert np.all(res2 != resultants)
         assert np.all(res3 != resultants)
         for restij, plane_index in zip(tij, np.arange(res3.shape[0])):
             sdev = np.std(res3[plane_index] - resultants[plane_index])
-            assert (sdev - read_noise / np.sqrt(len(restij))
+            assert (np.abs(sdev - read_noise / np.sqrt(len(restij)))
                     < 20 * sdev / np.sqrt(2 * len(counts.ravel())))
-        log.info('DMS220: successfully added read noise to resultants.')
+    log.info('DMS220: successfully added read noise to resultants.')
 
 
 @pytest.mark.soctests
 def test_inject_source_into_ramp():
     """Inject a source into a ramp.
     Demonstrates DMS225.
     """
     ramp = np.zeros((6, 100, 100), dtype='f4')
     sourcecounts = np.zeros((100, 100), dtype='f4')
     flux = 10000
     sourcecounts[49, 49] = flux  # delta function source with 100 counts.
     tij = np.arange(1, 6 * 3 + 1).reshape(6, 3)
-    newramp = ramp + l1.apportion_counts_to_resultants(sourcecounts, tij)
+    resultants, dq = l1.apportion_counts_to_resultants(sourcecounts, tij)
+    newramp = ramp + resultants
     assert np.all(newramp >= ramp)
     # only added photons
     assert np.sum(newramp == ramp) == (100 * 100 - 1) * 6
     # only added to the one pixel
     injectedsource = (newramp - ramp)[:, 49, 49]
     assert (np.abs(injectedsource[-1] - flux * np.mean(tij[-1]) / tij[-1][-1])
             < 10 * np.sqrt(flux))
@@ -137,30 +138,40 @@
     Demonstrates DMS227.
     """
     # these two functions basically just wrap the above and we'll really
     # just test for sanity.
     counts = np.random.poisson(100, size=(100, 100))
     galsim.roman.n_pix = 100
     for ma_table in ma_table_list:
-        resultants = l1.make_l1(galsim.Image(counts), ma_table,
-                                gain=1 * ru.electron / ru.DN)
+        resultants, dq = l1.make_l1(galsim.Image(counts), ma_table,
+                                    gain=1 * u.electron / u.DN)
         assert resultants.shape[0] == len(ma_table)
         assert resultants.shape[1] == counts.shape[0]
         assert resultants.shape[2] == counts.shape[1]
         # these contain read noise and shot noise, so it's not
         # clear what else to do with them?
         assert np.all(resultants == resultants.astype('i4'))
         # we could look for non-zero correlations from the IPC to
         # check that that is working?  But that is slightly annoying.
-        resultants = l1.make_l1(galsim.Image(counts), ma_table,
-                                read_noise=0 * ru.DN,
-                                gain=1 * ru.electron / ru.DN)
-        assert np.all(resultants <= np.max(counts[None, ...] * ru.DN))
+        resultants, dq = l1.make_l1(galsim.Image(counts), ma_table,
+                                    read_noise=0 * u.DN,
+                                    gain=1 * u.electron / u.DN)
+        assert np.all(resultants - parameters.pedestal
+                      <= np.max(counts[None, ...] * u.DN))
         # because of IPC, one can't require that each pixel is smaller
         # than the number of counts
-        assert np.all(resultants >= 0 * ru.DN)
-        assert np.all(np.diff(resultants, axis=0) >= 0 * ru.DN)
+        assert np.all(resultants >= 0 * u.DN)
+        assert np.all(np.diff(resultants, axis=0) >= 0 * u.DN)
         res_forasdf = l1.make_asdf(resultants, filepath=tmp_path / 'tmp.asdf')
         af = asdf.AsdfFile()
         af.tree = {'roman': res_forasdf}
         af.validate()
+        resultants, dq = l1.make_l1(galsim.Image(np.full((100, 100), 10**7)),
+                                    ma_table, gain=1 * u.electron / u.DN,
+                                    saturation=10**6 * u.DN)
+        assert np.all((dq[-1] & parameters.dqbits['saturated']) != 0)
+        resultants, dq = l1.make_l1(galsim.Image(np.zeros((100, 100))),
+                                    ma_table, gain=1 * u.electron / u.DN,
+                                    read_noise=0 * u.DN, crparam=dict())
+        assert np.all((resultants[0] - parameters.pedestal == 0)
+                      | ((dq[0] & parameters.dqbits['jump_det']) != 0))
     log.info('DMS227: successfully made an L1 file that validates.')
```

### Comparing `romanisim-0.2.0/romanisim/tests/test_persistence.py` & `romanisim-0.2.2/romanisim/tests/test_persistence.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/romanisim/tests/test_psf.py` & `romanisim-0.2.2/romanisim/tests/test_psf.py`

 * *Files identical despite different names*

### Comparing `romanisim-0.2.0/romanisim/tests/test_ramp.py` & `romanisim-0.2.2/romanisim/tests/test_ramp.py`

 * *Files 12% similar despite different names*

```diff
@@ -90,17 +90,34 @@
     fitter = ramp.RampFitInterpolator(test_table, flux_on_readvar_pts)
     ki = fitter.ki(flux, read_noise)
     var = fitter.variances(flux, read_noise)
     fluxes = np.array([10, 100, 1000, 1, 2, 3, 0])
     pedestals = np.array([-10, 0, 10, -1, 0, 1, 2])
     resultants = (fluxes.reshape(1, -1) * tbar.reshape(-1, 1)
                   + pedestals.reshape(1, -1))
-    par, var = fitter.fit_ramps(resultants, read_noise)
-    assert np.allclose(par[:, 1], fluxes, atol=1e-6)
-    assert np.allclose(par[:, 0], pedestals, atol=1e-2)
+    from functools import partial
+    rampfitters = [
+        fitter.fit_ramps,
+        partial(ramp.fit_ramps_casertano_no_dq, ma_table=test_table),
+        partial(ramp.fit_ramps_casertano, ma_table=test_table,
+                dq=resultants * 0)
+    ]
+    for fitfun in rampfitters:
+        par, var = fitfun(resultants=resultants, read_noise=read_noise)
+        assert np.allclose(par[:, 1], fluxes, atol=1e-6)
+        if not np.all(par[:, 0]) == 0:
+            assert np.allclose(par[:, 0], pedestals, atol=1e-2)
+
+    # compare single ramp and multi-ramp versions
+    p1, v1 = ramp.fit_ramps_casertano(resultants, resultants * 0, read_noise,
+                                      test_table)
+    p2, v2 = ramp.fit_ramps_casertano(resultants[:, 0], resultants[:, 0] * 0,
+                                      read_noise, test_table)
+    assert np.all(np.isclose(p1[0], p2))
+    assert np.all(np.isclose(v1[0], v2))
 
 
 def test_hard_ramps():
     ma_tables = list()
     ma_tables.append([[0, 1], [1, 1]])  # simple ramp
     ma_tables.append([[0, 100], [100, 100]])
     ma_tables.append([[x, 1] for x in np.arange(100)])  # big ramp
@@ -118,29 +135,48 @@
     par2, var2 = fitter.fit_ramps(resultants, read_noise, fluxest=flux)
     # in the simulation, the true flux was flux, so we expect this
     # to be ~Gaussian distributed about 0 with variance var.
     # the offset was 0.
     for p, v in [[par, var], [par2, var2]]:
         chi2dof_slope = np.sum((p[:, 1] - flux)**2 / v[:, 2, 1, 1]) / ntrial
         chi2dof_pedestal = np.sum((p[:, 0] - 0)**2 / v[:, 2, 0, 0]) / ntrial
-    assert np.abs(chi2dof_slope - 1) < 0.03
-    assert np.abs(chi2dof_pedestal - 1) < 0.03
+        assert np.abs(chi2dof_slope - 1) < 0.03
+        assert np.abs(chi2dof_pedestal - 1) < 0.03
     # It's not clear what level of precision to demand here.  This should
     # not actually give a value consistent with a normal chi^2 distribution
-    # because the Poisson noise is Poisson distribution, but we are treating
+    # because the Poisson noise is Poisson distributed, but we are treating
     # it as Gaussian distributed in the ramp fitting.  So we kind of just want
     # good rather than perfect.  The above requires that the sigmas be right
     # at the 5% level, which isn't terrible.  Presumably the accuracy
     # of the simulation is best for very high and very low count rates,
     # as in those two limits either the Poisson counts can be very closely
     # approximated as Gaussians, or the Poisson counts are not important.
     # Still, the default settings do give something very close to chi^2/dof
     # = 1.  Running 10**6 samples, we get chi^2/dof ~ 1 +/- 0.001 or so.
     # This test depends on random numbers and may eventually fail, but
     # the 0.03 margin is enough that it should very (_very_) rarely fail
     # absent code changes.
 
+    par, var = ramp.fit_ramps_casertano(
+        resultants, resultants * 0, read_noise, ma_table)
+    chi2dof_slope = np.sum((par[:, 1] - flux)**2 / var[:, 2, 1, 1]) / ntrial
+    assert np.abs(chi2dof_slope - 1) < 0.03
+
+    # now let's mark a bunch of the ramps as compromised.
+    bad = np.random.uniform(size=resultants.shape) > 0.7
+    dq = resultants * 0 + bad
+    par, var = ramp.fit_ramps_casertano(
+        resultants, dq, read_noise, ma_table)
+    # only use okay ramps
+    # ramps passing the below criterion have at least two adjacent valid reads
+    # i.e., we can make a measurement from them.
+    m = np.sum((dq[1:, :] == 0) & (dq[:-1, :] == 0), axis=0) != 0
+    chi2dof_slope = np.sum((par[m, 1] - flux)**2 / var[m, 2, 1, 1]) / np.sum(m)
+    assert np.abs(chi2dof_slope - 1) < 0.03
+    assert np.all(par[~m, 1] == 0)
+    assert np.all(var[~m, 1] == 0)
+
 
 def test_resultants_to_differences():
     resultants = np.array([[10, 11, 12, 13, 14, 15]], dtype='f4').T
     differences = ramp.resultants_to_differences(resultants)
     assert np.allclose(differences, np.array([[10, 1, 1, 1, 1, 1]]).T)
```

### Comparing `romanisim-0.2.0/romanisim/tests/test_util.py` & `romanisim-0.2.2/romanisim/tests/test_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Unit tests for utility functions.
 """
 
 import pytest
 import numpy as np
 from astropy import units as u
+from astropy.time import Time
 import galsim
 from romanisim import util
 from astropy.coordinates import SkyCoord
 from galsim import CelestialCoord
 
 
 def test_dummy():
@@ -81,20 +82,26 @@
     assert np.max(seps) < 5
     fracininnerhalf = np.sum(seps < 5 / np.sqrt(2)) / npts
     # should be distributed with stdev ~ sqrt(0.5*npts)/npts = sqrt(0.5/npts)
     assert np.abs(fracininnerhalf - 0.5) < 10 * np.sqrt(0.5 / npts)
 
 
 def test_add_more_metadata():
-    metadata = {'roman.meta.exposure.start_time': '2026-01-01T00:00:00',
-                'roman.meta.instrument.detector': 'WFI01',
-                'roman.meta.exposure.ma_table_number': 1,
+    metadata = {'exposure' :
+                    {
+                        'start_time': Time('2026-01-01T00:00:00'),
+                        'ma_table_number': 1,
+                    },
+                'instrument' :
+                    {
+                        'detector': 'WFI01',
+                    },
                 }
     util.add_more_metadata(metadata)
-    assert len(metadata) > 3  # some metadata got added.
+    assert len(metadata['exposure']) > 2  # some metadata got added.
 
 
 def test_king_profile():
     """Test King (1962) profile routines."""
     # king_profile, sample_king_distances, random_points_in_king
 
     # truncation radius
```

### Comparing `romanisim-0.2.0/romanisim/wcs.py` & `romanisim-0.2.2/romanisim/wcs.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,106 +16,139 @@
 more investigation.
 """
 
 import warnings
 import numpy as np
 import astropy.coordinates
 from astropy import units as u
+from astropy.modeling import models
 import astropy.time
+import roman_datamodels
 import crds
-import asdf
 import gwcs.geometry
 from gwcs import coordinate_frames as cf
 import gwcs.wcs
 import galsim.wcs
 from galsim import roman
 from . import util
 
 
+# Needed until RCAL release unfreezing link to RDM/RAD versions 0.14.1
+try:
+    import roman_datamodels.maker_utils as maker_utils
+except ImportError:
+    import roman_datamodels.testing.utils as maker_utils
+
+
+
 def fill_in_parameters(parameters, coord, roll_ref=0, boresight=True):
     """Add WCS info to parameters dictionary.
 
     Parameters
     ----------
     parameters : dict
         CRDS parameters dictionary
-        keys like roman.meta.pointing.* and roman.meta.wcsinfo.* may be modified
+        keys like pointing.* and wcsinfo.* may be modified
 
     coord : astropy.coordinates.SkyCoord or galsim.CelestialCoord
         world coordinates at V2 / V3 ref (boresight or center of WFI CCDs)
 
     roll_ref : float
         roll of the V3 axis from north
 
     boresight : bool
         whether coord is the telescope boresight (V2 = V3 = 0) or the center of
         the WFI CCD array
     """
     coord = util.skycoord(coord)
 
-    parameters['roman.meta.pointing.ra_v1'] = coord.ra.to(u.deg).value
-    parameters['roman.meta.wcsinfo.ra_ref'] = (
-        parameters['roman.meta.pointing.ra_v1'])
-
-    parameters['roman.meta.pointing.dec_v1'] = coord.dec.to(u.deg).value
-    parameters['roman.meta.wcsinfo.dec_ref'] = (
-        parameters['roman.meta.pointing.dec_v1'])
+    if 'pointing' not in parameters.keys():
+        parameters['pointing'] = {}
+
+    parameters['pointing']['ra_v1'] = coord.ra.to(u.deg).value
+
+    if 'wcsinfo' not in parameters.keys():
+        parameters['wcsinfo'] = {}
+
+    parameters['wcsinfo']['ra_ref'] = (
+        parameters['pointing']['ra_v1'])
+
+    parameters['pointing']['dec_v1'] = coord.dec.to(u.deg).value
+    parameters['wcsinfo']['dec_ref'] = (
+        parameters['pointing']['dec_v1'])
 
-    parameters['roman.meta.wcsinfo.roll_ref'] = roll_ref
+    parameters['wcsinfo']['roll_ref'] = roll_ref
 
     if boresight:
-        parameters['roman.meta.wcsinfo.v2_ref'] = 0
-        parameters['roman.meta.wcsinfo.v3_ref'] = 0
+        parameters['wcsinfo']['v2_ref'] = 0
+        parameters['wcsinfo']['v3_ref'] = 0
     else:
         from .parameters import v2v3_wficen
         v2_ref = v2v3_wficen[0] / 3600
         v3_ref = v2v3_wficen[1] / 3600
-        parameters['roman.meta.wcsinfo.v2_ref'] = v2_ref
-        parameters['roman.meta.wcsinfo.v3_ref'] = v3_ref
-        parameters['roman.meta.wcsinfo.roll_ref'] = (
-            parameters.get('roman.meta.wcsinfo.roll_ref', 0) + 60)
+        parameters['wcsinfo']['v2_ref'] = v2_ref
+        parameters['wcsinfo']['v3_ref'] = v3_ref
+        parameters['wcsinfo']['roll_ref'] = (
+            parameters['wcsinfo'].get('roll_ref', 0) + 60)
 
-
-def get_wcs(metadata, usecrds=True, distortion=None):
+def get_wcs(image, usecrds=True, distortion=None):
     """Get a WCS object for a given sca or set of CRDS parameters.
 
     Parameters
     ----------
-    metadata : dict
-        CRDS parameters dictionary specifying appropriate reference distortion
+    image : roman_datamodels.datamodels.ImageModel or dict
+        Image model or dictionary containing CRDS parameters
+        specifying appropriate reference distortion
         map to load.
     usecrds : bool
         If True, use crds reference distortions rather than galsim.roman
         distortion model.
     boresight : bool
         If True, world_pos specifies the location of the telescope boresight;
         otherwise the location of the science aperture.
 
     Returns
     -------
     galsim.CelestialWCS for an SCA
     """
 
-    metadata = util.flatten_dictionary(metadata)
-    sca = int(metadata['roman.meta.instrument.detector'][3:])
-    date = astropy.time.Time(metadata['roman.meta.exposure.start_time'])
+    # If sent a dictionary, create a temporary model for CRDS interface
+    if(type(image) != roman_datamodels.datamodels.ImageModel):
+        image_node = maker_utils.mk_level2_image()
+        for key in image.keys():
+            if isinstance(image[key], dict):
+                image_node['meta'][key].update(image[key])
+            else:
+                image_node['meta'][key] = image[key]
+        image_mod = roman_datamodels.datamodels.ImageModel(image_node)
+    else:
+        image_mod = image
+
+    sca = int(image_mod.meta.instrument.detector[3:])
+    date = astropy.time.Time(image_mod.meta.exposure.start_time)
+
     world_pos = astropy.coordinates.SkyCoord(
-        metadata['roman.meta.wcsinfo.ra_ref'] * u.deg,
-        metadata['roman.meta.wcsinfo.dec_ref'] * u.deg)
+        image_mod.meta.wcsinfo.ra_ref * u.deg,
+        image_mod.meta.wcsinfo.dec_ref * u.deg)
 
     if (distortion is None) and usecrds:
-        fn = crds.getreferences(metadata, reftypes=['distortion'],
-                                observatory='roman')
-        distortion = asdf.open(fn['distortion'])
-        distortion = distortion['roman']['coordinate_distortion_transform']
+        dist_name = crds.getreferences(
+            image_mod.get_crds_parameters(),
+            reftypes=['distortion'],
+            observatory='roman',
+        )['distortion']
+
+        dist_model = roman_datamodels.datamodels.DistortionRefModel(dist_name)
+        distortion = dist_model.coordinate_distortion_transform
+
     if distortion is not None:
         wcs = make_wcs(util.skycoord(world_pos), distortion,
-                       v2_ref=metadata['roman.meta.wcsinfo.v2_ref'],
-                       v3_ref=metadata['roman.meta.wcsinfo.v3_ref'],
-                       roll_ref=metadata['roman.meta.wcsinfo.roll_ref'])
+                       v2_ref=image_mod.meta.wcsinfo.v2_ref,
+                       v3_ref=image_mod.meta.wcsinfo.v3_ref,
+                       roll_ref=image_mod.meta.wcsinfo.roll_ref)
         wcs = GWCS(wcs)
     else:
         # use galsim.roman
         # galsim.roman does something smarter with choosing the roll
         # angle to optimize the solar panels given the target, and
         # therefore requires a date.
         wcs_dict = roman.getWCS(world_pos=util.celestialcoord(world_pos),
@@ -167,21 +200,20 @@
     ra_ref = targ_pos.ra.to(u.deg).value
     dec_ref = targ_pos.dec.to(u.deg).value
 
     # full transformation from romancal.assign_wcs.pointing
     # angles = np.array([v2_ref, -v3_ref, roll_ref, dec_ref, -ra_ref])
     # axes = "zyxyz"
     # rot = RotationSequence3D(angles, axes_order=axes)
-    from astropy.modeling.models import RotationSequence3D, Scale
-    rot = RotationSequence3D(
+    rot = models.RotationSequence3D(
         [v2_ref, -v3_ref, roll_ref, dec_ref, -ra_ref], 'zyxyz')
 
     # distortion takes pixels to V2V3
     # V2V3 are in arcseconds, while SphericalToCartesian expects degrees.
-    model = (distortion | (Scale(1 / 3600) & Scale(1 / 3600))
+    model = (distortion | (models.Scale(1 / 3600) & models.Scale(1 / 3600))
              | gwcs.geometry.SphericalToCartesian(wrap_lon_at=wrap_v2_at)
              | rot
              | gwcs.geometry.CartesianToSpherical(wrap_lon_at=wrap_lon_at))
     model.name = 'pixeltosky'
     detector = cf.Frame2D(name='detector', axes_order=(0, 1),
                           unit=(u.pix, u.pix))
     world = cf.CelestialFrame(reference_frame=astropy.coordinates.ICRS(),
```

### Comparing `romanisim-0.2.0/romanisim.egg-info/PKG-INFO` & `romanisim-0.2.2/romanisim.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romanisim
-Version: 0.2.0
+Version: 0.2.2
 Summary: Nancy Grace Roman Space Telescope WFI Simulator
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2022 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -38,17 +38,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 [![CI](https://github.com/spacetelescope/romanisim/actions/workflows/ci.yml/badge.svg)](https://github.com/spacetelescope/romanisim/actions/workflows/ci.yml) [![codecov](https://codecov.io/gh/spacetelescope/romanisim/branch/main/graph/badge.svg?token=pkoLtQOa2v)](https://codecov.io/gh/spacetelescope/romanisim)
```

### Comparing `romanisim-0.2.0/romanisim.egg-info/SOURCES.txt` & `romanisim-0.2.2/romanisim.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,67 @@
 .flake8
 .gitignore
 .readthedocs.yaml
 CHANGES.rst
 CODE_OF_CONDUCT.md
+JenkinsfileRT_dev
 LICENSE
 README.md
 pyproject.toml
 requirements-dev.txt
 setup.py
 tox.ini
 .github/CODEOWNERS
-.github/workflows/cancel_workflows.yml
 .github/workflows/ci.yml
 .github/workflows/ci_cron.yml
 .github/workflows/publish-to-pypi.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
+docs/rtd_environment.yaml
 docs/romanisim/apt.rst
 docs/romanisim/bandpass.rst
 docs/romanisim/catalog.rst
 docs/romanisim/image.rst
 docs/romanisim/install.rst
 docs/romanisim/l1.rst
 docs/romanisim/l2.rst
 docs/romanisim/overview.rst
 docs/romanisim/parameters.rst
 docs/romanisim/psf.rst
 docs/romanisim/refs.rst
 docs/romanisim/running.rst
 docs/romanisim/util.rst
 docs/romanisim/wcs.rst
-regtest/__init__.py
-regtest/test_l1.py
 romanisim/__init__.py
 romanisim/apt.py
 romanisim/bandpass.py
 romanisim/catalog.py
 romanisim/cr.py
 romanisim/gaia.py
 romanisim/image.py
 romanisim/l1.py
 romanisim/nonlinearity.py
 romanisim/parameters.py
 romanisim/persistence.py
 romanisim/psf.py
 romanisim/ramp.py
+romanisim/ramp_fit_casertano.c
+romanisim/ramp_fit_casertano.pyx
 romanisim/util.py
 romanisim/wcs.py
 romanisim.egg-info/PKG-INFO
 romanisim.egg-info/SOURCES.txt
 romanisim.egg-info/dependency_links.txt
 romanisim.egg-info/not-zip-safe
 romanisim.egg-info/requires.txt
 romanisim.egg-info/top_level.txt
 romanisim/data/Roman_effarea_20201130.csv
+romanisim/regtest/__init__.py
+romanisim/regtest/test_l1.py
 romanisim/tests/__init__.py
 romanisim/tests/test_bandpass.py
 romanisim/tests/test_catalog.py
 romanisim/tests/test_cr.py
 romanisim/tests/test_gaia.py
 romanisim/tests/test_image.py
 romanisim/tests/test_l1.py
```

### Comparing `romanisim-0.2.0/scripts/romanisim-make-image` & `romanisim-0.2.2/scripts/romanisim-make-image`

 * *Files 5% similar despite different names*

```diff
@@ -46,42 +46,42 @@
     parser.add_argument('--previous', default=None, type=str,
                         help=('previous simulated file in chronological order '
                               'used for persistence modeling.'))
 
     args = parser.parse_args()
 
     log.info('Starting simulation...')
-    log.warning("romanisim is under active developement.  Its output has "
+    log.warning("romanisim is under active development.  Its output has "
                 "not been formally validated; only limited testing has been "
                 "performed.  For this reason, use of romanisim for "
                 "preparation of ROSES proposals is not advised.  Other "
                 "packages like galsim's roman package or STIPS may better "
                 "serve such purposes.")
 
     metadata = deepcopy(default_parameters_dictionary)
 
     if args.radec is not None:
         coord = SkyCoord(ra=args.radec[0] * u.deg, dec=args.radec[1] * u.deg,
                          frame='icrs')
         wcs.fill_in_parameters(metadata, coord, boresight=args.boresight)
 
     if args.date is not None:
-        metadata['roman.meta.exposure.start_time'] = Time(
+        metadata['exposure']['start_time'] = Time(
             datetime.datetime(*args.date)).isot
-    date = Time(metadata['roman.meta.exposure.start_time'], format='isot')
 
-    metadata['roman.meta.instrument.detector'] = f'WFI{args.sca:02d}'
-    metadata['roman.meta.instrument.optical_element'] = args.bandpass
-    metadata['roman.meta.exposure.ma_table_number'] = args.ma_table_number
-
-    twcs = wcs.get_wcs(metadata, usecrds=args.usecrds)
-    rd_sca = twcs.toWorld(galsim.PositionD(
-        galsim.roman.n_pix/2, galsim.roman.n_pix/2))
+    date = Time(metadata['exposure']['start_time'], format='isot')
+
+    metadata['instrument']['detector'] = f'WFI{args.sca:02d}'
+    metadata['instrument']['optical_element'] = args.bandpass
+    metadata['exposure']['ma_table_number'] = args.ma_table_number
 
     if args.catalog is None:
+        twcs = wcs.get_wcs(metadata, usecrds=args.usecrds)
+        rd_sca = twcs.toWorld(galsim.PositionD(
+            galsim.roman.n_pix / 2, galsim.roman.n_pix / 2))
         cat = catalog.make_dummy_table_catalog(
             rd_sca, bandpasses=[args.bandpass], nobj=args.nobj)
     else:
         log.warning('Catalog input will probably not work unless the catalog '
                     'covers a lot of area or you have thought carefully about '
                     'the relation between the boresight and the SCA locations.')
         cat = Table.read(args.catalog)
```

### Comparing `romanisim-0.2.0/tox.ini` & `romanisim-0.2.2/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -34,32 +34,35 @@
     devdeps: with the latest developer version of key dependencies
     oldestdeps: with the oldest supported version of key dependencies
     pyargs: with --pyargs on installed package
     warnings: treating warnings as errors
     regtests: with --bigdata and --slow flags
     cov: with coverage
     xdist: using parallel processing
+use_develop = true
 pass_env =
     HOME
     CI
     TOXENV
     CRDS_*
     TEST_BIGDATA
     CODECOV_*
     WEBBPSF_PATH
     GALSIM_CAT_PATH
+set_env =
+    devdeps: PIP_EXTRA_INDEX_URL = https://pypi.anaconda.org/scipy-wheels-nightly/simple
 extras =
     test
 deps =
     xdist: pytest-xdist
-    devdeps: -rrequirements-dev.txt
     oldestdeps: minimum_dependencies
 commands_pre =
     oldestdeps: minimum_dependencies romanisim --filename requirements-min.txt
     oldestdeps: pip install -r requirements-min.txt
+    devdeps: pip install -r requirements-dev.txt -U --upgrade-strategy eager
     pip freeze
 commands =
     pip freeze
     pytest \
     cov: --cov=romanisim --cov-config=pyproject.toml --cov-report=term-missing --cov-report=xml \
     warnings: -W error \
     regtests: --bigdata --slow --basetemp={homedir}/test_outputs \
```

