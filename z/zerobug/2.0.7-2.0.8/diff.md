# Comparing `tmp/zerobug-2.0.7.tar.gz` & `tmp/zerobug-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zerobug-2.0.7.tar", last modified: Thu May 25 08:52:48 2023, max compression
+gzip compressed data, was "dist/zerobug-2.0.8.tar", last modified: Tue May 30 10:38:41 2023, max compression
```

## Comparing `zerobug-2.0.7.tar` & `zerobug-2.0.8.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:52:48.000000 zerobug-2.0.7/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/__main__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    23977 2023-05-20 08:38:13.000000 zerobug-2.0.7/zerobug/z0testrc
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug/dummy/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      121 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/dummy/dummylib.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)       47 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/dummy/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug/scripts/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     4138 2023-05-21 12:33:18.000000 zerobug-2.0.7/zerobug/scripts/setup.info
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6806 2023-05-20 08:38:13.000000 zerobug-2.0.7/zerobug/scripts/main.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/scripts/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug/_travis/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1852 2023-04-14 14:02:41.000000 zerobug-2.0.7/zerobug/_travis/travis_after_tests_success
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    17892 2023-05-20 08:38:13.000000 zerobug-2.0.7/zerobug/_travis/travis_run_pypi_tests
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug/_travis/cfg/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      668 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2005 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_pr.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      534 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_70.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      593 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1126 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/coveragerc
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      744 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      716 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      122 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_shellcheck.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      703 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1022 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      690 2023-01-30 07:04:22.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8__init__AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      132 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_shellcheck_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      629 2023-01-30 06:58:04.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8__init__.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      152 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_shellcheck_MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2575 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2823 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      533 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_61.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      704 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8__init__NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2526 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_beta.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      814 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8_MINIMAL.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    24224 2023-05-20 08:38:13.000000 zerobug-2.0.7/zerobug/_travis/travis_install_env
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1361 2023-01-27 07:10:19.000000 zerobug-2.0.7/zerobug/_travis/build_cmd
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       24 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/_travis/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    60073 2023-05-20 08:38:13.000000 zerobug-2.0.7/zerobug/z0testlib.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      574 2023-05-20 08:38:13.000000 zerobug-2.0.7/zerobug/zerobug.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      157 2022-12-09 05:08:44.000000 zerobug-2.0.7/zerobug/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        8 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-09 06:43:26.000000 zerobug-2.0.7/zerobug.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       91 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1946 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       70 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    15053 2023-05-25 08:52:48.000000 zerobug-2.0.7/zerobug.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-25 08:52:48.000000 zerobug-2.0.7/setup.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2877 2023-05-22 09:12:28.000000 zerobug-2.0.7/setup.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    15053 2023-05-25 08:52:48.000000 zerobug-2.0.7/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    10937 2023-05-25 08:52:42.000000 zerobug-2.0.7/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:38:41.000000 zerobug-2.0.8/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/__main__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    23977 2023-05-30 10:36:08.000000 zerobug-2.0.8/zerobug/z0testrc
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug/dummy/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      121 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/dummy/dummylib.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)       47 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/dummy/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2877 2023-05-30 10:36:16.000000 zerobug-2.0.8/zerobug/scripts/setup.info
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6806 2023-05-30 10:36:08.000000 zerobug-2.0.8/zerobug/scripts/main.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/scripts/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug/_travis/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1852 2023-04-14 14:02:41.000000 zerobug-2.0.8/zerobug/_travis/travis_after_tests_success
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    17892 2023-05-30 10:36:08.000000 zerobug-2.0.8/zerobug/_travis/travis_run_pypi_tests
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug/_travis/cfg/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      668 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2005 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_pr.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      534 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_70.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      593 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1126 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/coveragerc
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      744 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      716 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      122 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_shellcheck.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      703 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1022 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      690 2023-01-30 07:04:22.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8__init__AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      132 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_shellcheck_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      629 2023-01-30 06:58:04.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8__init__.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      152 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_shellcheck_MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2575 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2823 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      533 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_61.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      704 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8__init__NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2526 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_beta.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      814 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8_MINIMAL.cfg
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    24224 2023-05-30 10:36:08.000000 zerobug-2.0.8/zerobug/_travis/travis_install_env
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1361 2023-01-27 07:10:19.000000 zerobug-2.0.8/zerobug/_travis/build_cmd
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       24 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    60073 2023-05-30 10:36:08.000000 zerobug-2.0.8/zerobug/z0testlib.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      574 2023-05-30 10:36:08.000000 zerobug-2.0.8/zerobug/zerobug.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      157 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        8 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-09 06:43:26.000000 zerobug-2.0.8/zerobug.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       91 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1946 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       70 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    15072 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-30 10:38:41.000000 zerobug-2.0.8/setup.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2877 2023-05-30 10:36:08.000000 zerobug-2.0.8/setup.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    15072 2023-05-30 10:38:41.000000 zerobug-2.0.8/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    10940 2023-05-30 10:38:35.000000 zerobug-2.0.8/README.rst
```

### Comparing `zerobug-2.0.7/zerobug/z0testrc` & `zerobug-2.0.8/zerobug/z0testrc`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 # WLOGCMD:        oveerride opt_echo; may be None, 'echo', 'echo-1' or 'echo-0'
 #
 # This free software is released under GNU Affero GPL3
 # author: Antonio M. Vigliotti - antoniomaria.vigliotti@gmail.com
 # (C) 2015-2023 by SHS-AV s.r.l. - http://www.shs-av.com - info@shs-av.com
 #
 
-__version__=2.0.7
+__version__=2.0.8
 
 export opt_dry_run
 export ctr
 export opt_verbose
 export max_test
 export min_test
 export opt_noctr
```

### Comparing `zerobug-2.0.7/zerobug/scripts/main.py` & `zerobug-2.0.8/zerobug/scripts/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
```

### Comparing `zerobug-2.0.7/zerobug/_travis/travis_after_tests_success` & `zerobug-2.0.8/zerobug/_travis/travis_after_tests_success`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/travis_run_pypi_tests` & `zerobug-2.0.8/zerobug/_travis/travis_run_pypi_tests`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.7
+__version__=2.0.8
 
 
 travis_test_bash() {
     echo "======== Testing test_bash   ========"
     local s sts
     sts=0
     if [ ${opt_dry_run:-0} -eq 0 ]; then
```

### Comparing `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg` & `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_pr.cfg` & `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_pr.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_70.cfg` & `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_70.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg` & `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/cfg/coveragerc` & `zerobug-2.0.8/zerobug/_travis/cfg/coveragerc`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg` & `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg` & `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg` & `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg` & `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg` & `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg` & `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8.cfg` & `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8__init__.cfg` & `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8__init__.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint.cfg` & `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg` & `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_61.cfg` & `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_61.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg` & `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_pylint_beta.cfg` & `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_beta.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/cfg/travis_run_flake8_MINIMAL.cfg` & `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8_MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/_travis/travis_install_env` & `zerobug-2.0.8/zerobug/_travis/travis_install_env`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.7
+__version__=2.0.8
 
 
 run_traced() {
   [[ :$SHELLOPTS: =~ :xtrace: ]] && set +x
   [[ -z ${Z0_STACK:+_} ]] && export Z0_STACK=0
   ((Z0_STACK=Z0_STACK+2))
   local xcmd="$1" lm="                    "
```

### Comparing `zerobug-2.0.7/zerobug/_travis/build_cmd` & `zerobug-2.0.8/zerobug/_travis/build_cmd`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug/z0testlib.py` & `zerobug-2.0.8/zerobug/z0testlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from subprocess import PIPE, Popen
 
 import magic
 
 from os0 import os0
 from python_plus import _c
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 # return code
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 if os.name == "posix":
     RED = "\033[1;31m"
     GREEN = "\033[1;32m"
```

### Comparing `zerobug-2.0.7/zerobug/zerobug.py` & `zerobug-2.0.8/zerobug/zerobug.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 """
     Zeroincombenze® unit test library for python programs Regression Test Suite
 """
 import sys
 from . import z0test
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 
 def version():
     return __version__
 
 
 def main(cli_args=None):
```

### Comparing `zerobug-2.0.7/zerobug.egg-info/SOURCES.txt` & `zerobug-2.0.8/zerobug.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.7/zerobug.egg-info/PKG-INFO` & `zerobug-2.0.8/zerobug.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: zerobug
-Version: 2.0.7
+Version: 2.0.8
 Summary: Zeroincombenze continuous testing framework and tools for python and bash programs
 Home-page: https://github.com/zeroincombenze/tools
 Author: Antonio Maria Vigliotti
 Author-email: <info@shs-av.com>
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools/tree/master/zerobug
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io/en/latest/zerobug
@@ -303,23 +303,25 @@
         
         
         Contributors
         ------------
         
         * Antonio Maria Vigliotti <antoniomaria.vigliotti@gmail.com>
         
+        
+        
         |
         
         This module is part of tools project.
         
         Last Update / Ultimo aggiornamento: 2023-05-21
         
         .. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
             :target: https://odoo-community.org/page/development-status
-            :alt:
+            :alt: 
         .. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
             :target: https://travis-ci.com/zeroincombenze/tools
             :alt: github.com
         .. |license gpl| image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
             :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
             :alt: License: AGPL-3
         .. |license opl| image:: https://img.shields.io/badge/licence-OPL-7379c3.svg
```

### Comparing `zerobug-2.0.7/setup.py` & `zerobug-2.0.8/zerobug/scripts/setup.info`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             'os0',
             'z0lib',
         ],
     )
 
 setup(
     name='zerobug',
-    version='2.0.7',
+    version='2.0.8',
     description='Zeroincombenze continuous testing framework'
     ' and tools for python and bash programs',
     long_description=open("README.rst").read(),
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: POSIX',
```

### Comparing `zerobug-2.0.7/PKG-INFO` & `zerobug-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: zerobug
-Version: 2.0.7
+Version: 2.0.8
 Summary: Zeroincombenze continuous testing framework and tools for python and bash programs
 Home-page: https://github.com/zeroincombenze/tools
 Author: Antonio Maria Vigliotti
 Author-email: <info@shs-av.com>
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools/tree/master/zerobug
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io/en/latest/zerobug
@@ -303,23 +303,25 @@
         
         
         Contributors
         ------------
         
         * Antonio Maria Vigliotti <antoniomaria.vigliotti@gmail.com>
         
+        
+        
         |
         
         This module is part of tools project.
         
         Last Update / Ultimo aggiornamento: 2023-05-21
         
         .. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
             :target: https://odoo-community.org/page/development-status
-            :alt:
+            :alt: 
         .. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
             :target: https://travis-ci.com/zeroincombenze/tools
             :alt: github.com
         .. |license gpl| image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
             :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
             :alt: License: AGPL-3
         .. |license opl| image:: https://img.shields.io/badge/licence-OPL-7379c3.svg
```

### Comparing `zerobug-2.0.7/README.rst` & `zerobug-2.0.8/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -292,23 +292,25 @@
 
 
 Contributors
 ------------
 
 * Antonio Maria Vigliotti <antoniomaria.vigliotti@gmail.com>
 
+
+
 |
 
 This module is part of tools project.
 
 Last Update / Ultimo aggiornamento: 2023-05-21
 
 .. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
-    :alt:
+    :alt: 
 .. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
     :target: https://travis-ci.com/zeroincombenze/tools
     :alt: github.com
 .. |license gpl| image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. |license opl| image:: https://img.shields.io/badge/licence-OPL-7379c3.svg
```

