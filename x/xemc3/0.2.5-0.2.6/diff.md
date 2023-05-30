# Comparing `tmp/xemc3-0.2.5.tar.gz` & `tmp/xemc3-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xemc3-0.2.5.tar", last modified: Fri May 26 13:00:01 2023, max compression
+gzip compressed data, was "xemc3-0.2.6.tar", last modified: Tue May 30 11:21:58 2023, max compression
```

## Comparing `xemc3-0.2.5.tar` & `xemc3-0.2.6.tar`

### file list

```diff
@@ -1,100 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.296853 xemc3-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 12:59:40.000000 xemc3-0.2.5/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.288853 xemc3-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.288853 xemc3-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-26 12:59:40.000000 xemc3-0.2.5/.github/workflows/black-fix.yml
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-26 12:59:40.000000 xemc3-0.2.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-26 12:59:40.000000 xemc3-0.2.5/.github/workflows/python_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-26 12:59:40.000000 xemc3-0.2.5/.github/workflows/test-python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-26 12:59:40.000000 xemc3-0.2.5/.github/workflows/version-yaml.yml
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-26 12:59:40.000000 xemc3-0.2.5/.github/workflows/zenodo.yml
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-26 12:59:40.000000 xemc3-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 12:59:40.000000 xemc3-0.2.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-26 12:59:40.000000 xemc3-0.2.5/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 12:59:40.000000 xemc3-0.2.5/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-26 12:59:40.000000 xemc3-0.2.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-26 13:00:01.296853 xemc3-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-26 12:59:40.000000 xemc3-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.288853 xemc3-0.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/citing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/cli.rst.in.py
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/config.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.292853 xemc3-0.2.5/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/examples/evaluate_at.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/examples/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/examples/heatflux.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/examples/info.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/examples/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/examples/load1.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/examples/load2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/examples/setup_plt.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.292853 xemc3-0.2.5/docs/exercises/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/exercises/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/exercises/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/filenames.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/xarray.rst
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-26 12:59:40.000000 xemc3-0.2.5/docs/xemc3.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-26 12:59:40.000000 xemc3-0.2.5/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-26 12:59:40.000000 xemc3-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-26 12:59:40.000000 xemc3-0.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-26 13:00:01.296853 xemc3-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-26 12:59:40.000000 xemc3-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.292853 xemc3-0.2.5/xemc3/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 13:00:00.000000 xemc3-0.2.5/xemc3/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.292853 xemc3-0.2.5/xemc3/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/cli/_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1465 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/cli/append_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/cli/to_archive.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      887 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/cli/to_netcdf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3698 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/cli/xdivertor.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.292853 xemc3-0.2.5/xemc3/core/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21282 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/core/depo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/core/evaluate_at.py
--rw-r--r--   0 runner    (1001) docker     (123)    56312 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/core/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/core/plot_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/core/plot_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.292853 xemc3-0.2.5/xemc3/data/
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/data/default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/data/v0.2.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/data/v0.2.1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/data/v0.2.2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/data/v0.2.3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/data/v0.2.4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/data/v0.2.5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.292853 xemc3-0.2.5/xemc3/load/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/load/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.296853 xemc3-0.2.5/xemc3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/test/gen_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/test/test_average.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/test/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/test/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/test/test_load_real.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/test/test_write_load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.296853 xemc3-0.2.5/xemc3/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/tools/run_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.296853 xemc3-0.2.5/xemc3/write/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/write/fortran.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:59:40.000000 xemc3-0.2.5/xemc3/write/nc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:00:01.292853 xemc3-0.2.5/xemc3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-26 13:00:01.000000 xemc3-0.2.5/xemc3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-26 13:00:01.000000 xemc3-0.2.5/xemc3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:00:01.000000 xemc3-0.2.5/xemc3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-26 13:00:01.000000 xemc3-0.2.5/xemc3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-26 13:00:01.000000 xemc3-0.2.5/xemc3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 13:00:01.000000 xemc3-0.2.5/xemc3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:21:58.166062 xemc3-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-30 11:21:42.000000 xemc3-0.2.6/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:21:58.154062 xemc3-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:21:58.158062 xemc3-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-30 11:21:42.000000 xemc3-0.2.6/.github/workflows/black-fix.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-30 11:21:42.000000 xemc3-0.2.6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-30 11:21:42.000000 xemc3-0.2.6/.github/workflows/python_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-30 11:21:42.000000 xemc3-0.2.6/.github/workflows/test-python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-30 11:21:42.000000 xemc3-0.2.6/.github/workflows/version-yaml.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-30 11:21:42.000000 xemc3-0.2.6/.github/workflows/zenodo.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-30 11:21:42.000000 xemc3-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-30 11:21:42.000000 xemc3-0.2.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-30 11:21:42.000000 xemc3-0.2.6/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-30 11:21:42.000000 xemc3-0.2.6/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-30 11:21:42.000000 xemc3-0.2.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-30 11:21:58.166062 xemc3-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-30 11:21:42.000000 xemc3-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:21:58.158062 xemc3-0.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/citing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/cli.rst.in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/config.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:21:58.158062 xemc3-0.2.6/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/examples/evaluate_at.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/examples/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/examples/heatflux.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/examples/info.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/examples/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/examples/load1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/examples/load2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/examples/setup_plt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:21:58.158062 xemc3-0.2.6/docs/exercises/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/exercises/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/exercises/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/filenames.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/xarray.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-30 11:21:42.000000 xemc3-0.2.6/docs/xemc3.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-30 11:21:42.000000 xemc3-0.2.6/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-30 11:21:42.000000 xemc3-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-30 11:21:42.000000 xemc3-0.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-30 11:21:58.166062 xemc3-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-30 11:21:42.000000 xemc3-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:21:58.162062 xemc3-0.2.6/xemc3/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 11:21:57.000000 xemc3-0.2.6/xemc3/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:21:58.162062 xemc3-0.2.6/xemc3/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/cli/_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1465 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/cli/append_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/cli/to_archive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      887 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/cli/to_netcdf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3698 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/cli/xdivertor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:21:58.162062 xemc3-0.2.6/xemc3/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21282 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/core/depo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/core/evaluate_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56914 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/core/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/core/plot_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/core/plot_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:21:58.162062 xemc3-0.2.6/xemc3/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/data/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/data/v0.2.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/data/v0.2.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/data/v0.2.2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/data/v0.2.3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/data/v0.2.4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/data/v0.2.5.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/data/v0.2.6.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:21:58.162062 xemc3-0.2.6/xemc3/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/load/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:21:58.166062 xemc3-0.2.6/xemc3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/test/gen_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/test/test_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/test/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/test/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/test/test_load_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/test/test_write_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:21:58.166062 xemc3-0.2.6/xemc3/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/tools/run_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:21:58.166062 xemc3-0.2.6/xemc3/write/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/write/fortran.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:21:42.000000 xemc3-0.2.6/xemc3/write/nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:21:58.162062 xemc3-0.2.6/xemc3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-30 11:21:58.000000 xemc3-0.2.6/xemc3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-30 11:21:58.000000 xemc3-0.2.6/xemc3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:21:58.000000 xemc3-0.2.6/xemc3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-30 11:21:58.000000 xemc3-0.2.6/xemc3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-30 11:21:58.000000 xemc3-0.2.6/xemc3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 11:21:58.000000 xemc3-0.2.6/xemc3.egg-info/top_level.txt
```

### Comparing `xemc3-0.2.5/.github/workflows/black-fix.yml` & `xemc3-0.2.6/.github/workflows/black-fix.yml`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/.github/workflows/python_publish.yml` & `xemc3-0.2.6/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/.github/workflows/test-python-package.yml` & `xemc3-0.2.6/.github/workflows/test-python-package.yml`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/.github/workflows/version-yaml.yml` & `xemc3-0.2.6/.github/workflows/version-yaml.yml`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/COPYING` & `xemc3-0.2.6/COPYING`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/Makefile` & `xemc3-0.2.6/Makefile`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/PKG-INFO` & `xemc3-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xemc3
-Version: 0.2.5
+Version: 0.2.6
 Summary: Collect data from EMC3 runs in python using xarray
 Home-page: https://github.com/dschwoerer/xemc3
 Author: David Bold
 Author-email: dave@ipp.mpg.de
 License: GPL
 Project-URL: Tracker, https://github.com/dschwoerer/xemc3/issues
 Project-URL: Documentation, https://xemc3.rtfd.io
```

### Comparing `xemc3-0.2.5/README.md` & `xemc3-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/docs/cli.rst.in.py` & `xemc3-0.2.6/docs/cli.rst.in.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/docs/conf.py` & `xemc3-0.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/docs/config.ipynb` & `xemc3-0.2.6/docs/config.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/docs/examples/evaluate_at.ipynb` & `xemc3-0.2.6/docs/examples/evaluate_at.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/docs/examples/get_data.py` & `xemc3-0.2.6/docs/examples/get_data.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/docs/examples/heatflux.ipynb` & `xemc3-0.2.6/docs/examples/heatflux.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/docs/examples/info.ipynb` & `xemc3-0.2.6/docs/examples/info.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/docs/examples/introduction.ipynb` & `xemc3-0.2.6/docs/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/docs/examples/load1.ipynb` & `xemc3-0.2.6/docs/examples/load1.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/docs/examples/load2.ipynb` & `xemc3-0.2.6/docs/examples/load2.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/docs/exercises/get_data.py` & `xemc3-0.2.6/docs/exercises/get_data.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/docs/exercises/introduction.ipynb` & `xemc3-0.2.6/docs/exercises/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/docs/filenames.ipynb` & `xemc3-0.2.6/docs/filenames.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/docs/index.rst` & `xemc3-0.2.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/docs/introduction.rst` & `xemc3-0.2.6/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/docs/xarray.rst` & `xemc3-0.2.6/docs/xarray.rst`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/docs/xemc3.rst` & `xemc3-0.2.6/docs/xemc3.rst`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/requirements.txt` & `xemc3-0.2.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/setup.cfg` & `xemc3-0.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/__init__.py` & `xemc3-0.2.6/xemc3/__init__.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/cli/_common.py` & `xemc3-0.2.6/xemc3/cli/_common.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/cli/append_time.py` & `xemc3-0.2.6/xemc3/cli/append_time.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/cli/to_archive.py` & `xemc3-0.2.6/xemc3/cli/to_archive.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/cli/to_netcdf.py` & `xemc3-0.2.6/xemc3/cli/to_netcdf.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/cli/xdivertor.py` & `xemc3-0.2.6/xemc3/cli/xdivertor.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/core/config.py` & `xemc3-0.2.6/xemc3/core/config.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/core/dataset.py` & `xemc3-0.2.6/xemc3/core/dataset.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/core/depo.py` & `xemc3-0.2.6/xemc3/core/depo.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/core/evaluate_at.py` & `xemc3-0.2.6/xemc3/core/evaluate_at.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/core/load.py` & `xemc3-0.2.6/xemc3/core/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,19 +325,35 @@
         t = t.reshape(dims, order="F")
         _assert_eof(f, fn)
     da = xr.DataArray(dims=("r", "theta", "phi"), data=t)
     da.attrs = dict(numcells=infos[0], plasmacells=infos[1], other=infos[2])
     return da
 
 
-def add_metadata(ds: xr.Dataset):
+def ensure_metadata(ds: xr.Dataset) -> xr.Dataset:
+    if not ds:
+        return ds
+    meta = get_default_metadata()
+    for k in meta:
+        if k not in ds.attrs:
+            ds.attrs.update(meta)
+            return ds
+    return ds
+
+
+def add_metadata(ds: xr.Dataset) -> xr.Dataset:
+    ds.attrs.update(get_default_metadata())
+    return ds
+
+
+def get_default_metadata() -> dict:
     # Delay import to avoid circular dependency
     from .. import __version__
 
-    ds.attrs.update(
+    return dict(
         title="EMC3-EIRENE Simulation data",
         software_name="xemc3",
         software_version=__version__,
         date_created=datetime.datetime.utcnow().isoformat(),
         id=str(uuid.uuid1()),
         references="https://doi.org/10.5281/zenodo.5562265",
     )
@@ -397,16 +413,15 @@
     )
     for x in ds.coords:
         ds[x].attrs["xemc3_type"] = "geom"
     ds.emc3.unit("R_bounds", "m")
     ds.emc3.unit("z_bounds", "m")
     ds.emc3.unit("phi_bounds", "radian")
     assert isinstance(ds, xr.Dataset)
-    add_metadata(ds)
-    return ds
+    return add_metadata(ds)
 
 
 def scrape(f: typing.TextIO, *, ignore="!", verbose=False) -> str:
     """read next data line from configuration file (skip lines with
     leading *)
 
     Parameters
@@ -630,15 +645,17 @@
         plates = []
         for plate in range(num_plates):
             s = scrape(f).split()
             assert len(s) == 2, (
                 f"Unexpected string `{s}` while reading {plate}." + raise_issue
             )
             _, geom = s
-            r, z, phi = read_plate(cwd + geom)
+            if not geom.startswith("/"):
+                geom = cwd + geom
+            r, z, phi = read_plate(geom)
             nx, ny = r.shape
             nx -= 1
             ny -= 1
             s = scrape(f).split()
             total = np.array([float(i) for i in s])
             s = scrape(f).split()
             if len(s) == 3:
@@ -721,18 +738,20 @@
                                 (1.0, b, a, a * b)
                                 for a, b in [(a0, b0), (a0, b1), (a1, b0), (a1, b1)]
                             ]
                         ).T
                         newpos[ix::xref, iy::yref, :] = pos @ A
 
                     corrs[i] = newpos
+                dims = [plate_prefix + x for x in ("phi", "x")]
+                dims += ["delta_" + x for x in dims]
                 corrs_da = [
                     xr.DataArray(
                         data=a.reshape(nxr, nyr, 2, 2),
-                        dims=("phi", "x", "delta_phi", "delta_x"),
+                        dims=dims,
                     )
                     for a in corrs
                 ]
             else:
                 assert mode == 1
                 corrs_da = [
                     to_interval((plate_prefix + "phi", plate_prefix + "x"), a)
@@ -1431,15 +1450,18 @@
     defaults = files[filename].copy()
     defaults.update(opts)
     type = defaults.get("type", "mapped")
     if type == "info":
         if not isinstance(ds, xr.Dataset):
             ds = xr.Dataset()
         return read_fort_file(ds, fn, **defaults)
-    ds = ensure_mapping("/".join(fn.split("/")[:-1]), ds, type == "mapped", fn=fn)
+    if type == "target_flux":
+        ds = ds or xr.Dataset()
+    else:
+        ds = ensure_mapping("/".join(fn.split("/")[:-1]), ds, type == "mapped", fn=fn)
     assert isinstance(ds, xr.Dataset)
     return read_fort_file(ds, fn, **defaults)
 
 
 def read_fort_file(ds: xr.Dataset, fn: str, type: str = "mapped", **opts) -> xr.Dataset:
     """
     Read an EMC3 simulation file and add to a dataset.
@@ -1493,15 +1515,15 @@
         datas = read_depo_raw(ds, fn)
     else:
         raise RuntimeError(f"Unexpected type {type}")
     assert opts == {}, "Unexpected arguments: " + ", ".join(
         [f"{k}={v}" for k, v in opts.items()]
     )
     if datas is None:
-        return ds
+        return ensure_metadata(ds)
     vars = vars.copy()
     assert opts == {}
     keys = [k for k in vars]
     if "%" in keys[-1]:
         key = keys[-1]
         flexi = vars.pop(key)
         for i in range(len(vars), len(datas)):
@@ -1522,15 +1544,15 @@
             if k in varopts:
                 attrs[k] = varopts.pop(k)
 
         ds[var].attrs.update(attrs)
         assert (
             varopts == {}
         ), f"variable {var} has options {varopts} but didn't expect anything"
-    return ds
+    return ensure_metadata(ds)
 
 
 def guess_type(ds: xr.Dataset, key: typing.Hashable) -> str:
     data = ds[key]
     assert isinstance(key, str)
     try:
         ret = data.attrs["xemc3_type"]
```

### Comparing `xemc3-0.2.5/xemc3/core/plot_2d.py` & `xemc3-0.2.6/xemc3/core/plot_2d.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/core/plot_3d.py` & `xemc3-0.2.6/xemc3/core/plot_3d.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/core/utils.py` & `xemc3-0.2.6/xemc3/core/utils.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/data/default.yaml` & `xemc3-0.2.6/xemc3/data/default.yaml`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/data/v0.2.0.yaml` & `xemc3-0.2.6/xemc3/data/v0.2.0.yaml`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/data/v0.2.1.yaml` & `xemc3-0.2.6/xemc3/data/v0.2.1.yaml`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/data/v0.2.2.yaml` & `xemc3-0.2.6/xemc3/data/v0.2.2.yaml`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/data/v0.2.3.yaml` & `xemc3-0.2.6/xemc3/data/v0.2.3.yaml`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/data/v0.2.4.yaml` & `xemc3-0.2.6/xemc3/data/v0.2.4.yaml`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/data/v0.2.5.yaml` & `xemc3-0.2.6/xemc3/data/v0.2.5.yaml`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/load/__init__.py` & `xemc3-0.2.6/xemc3/load/__init__.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/test/gen_ds.py` & `xemc3-0.2.6/xemc3/test/gen_ds.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/test/test_average.py` & `xemc3-0.2.6/xemc3/test/test_average.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/test/test_cli.py` & `xemc3-0.2.6/xemc3/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/test/test_dataset.py` & `xemc3-0.2.6/xemc3/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/test/test_load_real.py` & `xemc3-0.2.6/xemc3/test/test_load_real.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/test/test_utils.py` & `xemc3-0.2.6/xemc3/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/test/test_write_load.py` & `xemc3-0.2.6/xemc3/test/test_write_load.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/tools/run_wrapper.py` & `xemc3-0.2.6/xemc3/tools/run_wrapper.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3/write/fortran.py` & `xemc3-0.2.6/xemc3/write/fortran.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.5/xemc3.egg-info/PKG-INFO` & `xemc3-0.2.6/xemc3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xemc3
-Version: 0.2.5
+Version: 0.2.6
 Summary: Collect data from EMC3 runs in python using xarray
 Home-page: https://github.com/dschwoerer/xemc3
 Author: David Bold
 Author-email: dave@ipp.mpg.de
 License: GPL
 Project-URL: Tracker, https://github.com/dschwoerer/xemc3/issues
 Project-URL: Documentation, https://xemc3.rtfd.io
```

### Comparing `xemc3-0.2.5/xemc3.egg-info/SOURCES.txt` & `xemc3-0.2.6/xemc3.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 xemc3/data/default.yaml
 xemc3/data/v0.2.0.yaml
 xemc3/data/v0.2.1.yaml
 xemc3/data/v0.2.2.yaml
 xemc3/data/v0.2.3.yaml
 xemc3/data/v0.2.4.yaml
 xemc3/data/v0.2.5.yaml
+xemc3/data/v0.2.6.yaml
 xemc3/load/__init__.py
 xemc3/test/__init__.py
 xemc3/test/gen_ds.py
 xemc3/test/test_average.py
 xemc3/test/test_basic.py
 xemc3/test/test_cli.py
 xemc3/test/test_dataset.py
```

