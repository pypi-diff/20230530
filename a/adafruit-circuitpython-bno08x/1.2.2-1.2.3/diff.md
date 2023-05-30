# Comparing `tmp/adafruit-circuitpython-bno08x-1.2.2.tar.gz` & `tmp/adafruit-circuitpython-bno08x-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bno08x-1.2.2.tar", last modified: Fri May 26 16:08:48 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-bno08x-1.2.3.tar", last modified: Tue May 30 14:47:41 2023, max compression
```

## Comparing `adafruit-circuitpython-bno08x-1.2.2.tar` & `adafruit-circuitpython-bno08x-1.2.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.829193 adafruit-circuitpython-bno08x-1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.821193 adafruit-circuitpython-bno08x-1.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.821193 adafruit-circuitpython-bno08x-1.2.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.825193 adafruit-circuitpython-bno08x-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.825193 adafruit-circuitpython-bno08x-1.2.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-26 16:08:48.825193 adafruit-circuitpython-bno08x-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.825193 adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/
--rw-r--r--   0 runner    (1001) docker     (123)    38910 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/uart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.825193 adafruit-circuitpython-bno08x-1.2.2/adafruit_circuitpython_bno08x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-26 16:08:48.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_circuitpython_bno08x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-26 16:08:48.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:08:48.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_circuitpython_bno08x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 16:08:48.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_circuitpython_bno08x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 16:08:48.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_circuitpython_bno08x.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.825193 adafruit-circuitpython-bno08x-1.2.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.825193 adafruit-circuitpython-bno08x-1.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.825193 adafruit-circuitpython-bno08x-1.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_find_heading.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_more_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_quaternion_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_simpletest_spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_simpletest_uart.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:08:48.829193 adafruit-circuitpython-bno08x-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:47:41.870470 adafruit-circuitpython-bno08x-1.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:47:41.858470 adafruit-circuitpython-bno08x-1.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:47:41.862470 adafruit-circuitpython-bno08x-1.2.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:47:41.862470 adafruit-circuitpython-bno08x-1.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:47:41.862470 adafruit-circuitpython-bno08x-1.2.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-30 14:47:41.870470 adafruit-circuitpython-bno08x-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:47:41.866470 adafruit-circuitpython-bno08x-1.2.3/adafruit_bno08x/
+-rw-r--r--   0 runner    (1001) docker     (123)    40573 2023-05-30 14:47:34.000000 adafruit-circuitpython-bno08x-1.2.3/adafruit_bno08x/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-30 14:47:34.000000 adafruit-circuitpython-bno08x-1.2.3/adafruit_bno08x/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-30 14:47:34.000000 adafruit-circuitpython-bno08x-1.2.3/adafruit_bno08x/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-05-30 14:47:34.000000 adafruit-circuitpython-bno08x-1.2.3/adafruit_bno08x/spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-30 14:47:34.000000 adafruit-circuitpython-bno08x-1.2.3/adafruit_bno08x/uart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:47:41.866470 adafruit-circuitpython-bno08x-1.2.3/adafruit_circuitpython_bno08x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-30 14:47:41.000000 adafruit-circuitpython-bno08x-1.2.3/adafruit_circuitpython_bno08x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-30 14:47:41.000000 adafruit-circuitpython-bno08x-1.2.3/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:47:41.000000 adafruit-circuitpython-bno08x-1.2.3/adafruit_circuitpython_bno08x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 14:47:41.000000 adafruit-circuitpython-bno08x-1.2.3/adafruit_circuitpython_bno08x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 14:47:41.000000 adafruit-circuitpython-bno08x-1.2.3/adafruit_circuitpython_bno08x.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:47:41.866470 adafruit-circuitpython-bno08x-1.2.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:47:41.866470 adafruit-circuitpython-bno08x-1.2.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:47:41.870470 adafruit-circuitpython-bno08x-1.2.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-30 14:47:34.000000 adafruit-circuitpython-bno08x-1.2.3/examples/bno08x_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-30 14:47:34.000000 adafruit-circuitpython-bno08x-1.2.3/examples/bno08x_find_heading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-30 14:47:34.000000 adafruit-circuitpython-bno08x-1.2.3/examples/bno08x_more_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-30 14:47:34.000000 adafruit-circuitpython-bno08x-1.2.3/examples/bno08x_quaternion_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-30 14:47:34.000000 adafruit-circuitpython-bno08x-1.2.3/examples/bno08x_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-30 14:47:34.000000 adafruit-circuitpython-bno08x-1.2.3/examples/bno08x_simpletest_spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-30 14:47:34.000000 adafruit-circuitpython-bno08x-1.2.3/examples/bno08x_simpletest_uart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-30 14:47:34.000000 adafruit-circuitpython-bno08x-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-30 14:47:22.000000 adafruit-circuitpython-bno08x-1.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:47:41.870470 adafruit-circuitpython-bno08x-1.2.3/setup.cfg
```

### Comparing `adafruit-circuitpython-bno08x-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-bno08x-1.2.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/.gitignore` & `adafruit-circuitpython-bno08x-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/.pre-commit-config.yaml` & `adafruit-circuitpython-bno08x-1.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/.pylintrc` & `adafruit-circuitpython-bno08x-1.2.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-bno08x-1.2.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/LICENSE` & `adafruit-circuitpython-bno08x-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-bno08x-1.2.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/LICENSES/MIT.txt` & `adafruit-circuitpython-bno08x-1.2.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-bno08x-1.2.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/PKG-INFO` & `adafruit-circuitpython-bno08x-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bno08x
-Version: 1.2.2
+Version: 1.2.3
 Summary: Helper library for the Hillcrest Laboratories BNO08x IMUs
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BNO08x
 Keywords: adafruit,blinka,circuitpython,micropython,bno080,IMU,BNO055,SENSOR,FUSION,VR,MOTION,TRACK,BNO085
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bno08x-1.2.2/README.rst` & `adafruit-circuitpython-bno08x-1.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/__init__.py` & `adafruit-circuitpython-bno08x-1.2.3/adafruit_bno08x/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,25 +21,34 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https:# github.com/adafruit/circuitpython/releases
 
 * `Adafruit's Bus Device library <https:# github.com/adafruit/Adafruit_CircuitPython_BusDevice>`_
 """
-__version__ = "1.2.2"
+from __future__ import annotations
+
+__version__ = "1.2.3"
 __repo__ = "https:# github.com/adafruit/Adafruit_CircuitPython_BNO08x.git"
 
 from struct import unpack_from, pack_into
 from collections import namedtuple
 import time
 from micropython import const
 
 # TODO: Remove on release
 from .debug import channels, reports
 
+# For IDE type recognition
+try:
+    from typing import Any, Dict, List, Optional, Tuple, Union
+    from digitalio import DigitalInOut
+except ImportError:
+    pass
+
 # TODO: shorten names
 # Channel 0: the SHTP command channel
 BNO_CHANNEL_SHTP_COMMAND = const(0)
 BNO_CHANNEL_EXE = const(1)
 _BNO_CHANNEL_CONTROL = const(2)
 _BNO_CHANNEL_INPUT_SENSOR_REPORTS = const(3)
 _BNO_CHANNEL_WAKE_INPUT_SENSOR_REPORTS = const(4)
@@ -202,20 +211,20 @@
 
 class PacketError(Exception):
     """Raised when the packet couldnt be parsed"""
 
     pass  # pylint:disable=unnecessary-pass
 
 
-def _elapsed(start_time):
+def _elapsed(start_time: float) -> float:
     return time.monotonic() - start_time
 
 
 ############ PACKET PARSING ###########################
-def _parse_sensor_report_data(report_bytes):
+def _parse_sensor_report_data(report_bytes: bytearray) -> Tuple[Tuple, int]:
     """Parses reports with only 16-bit fields"""
     data_offset = 4  # this may not always be true
     report_id = report_bytes[0]
     scalar, count, _report_length = _AVAIL_SENSOR_REPORTS[report_id]
     if report_id in _RAW_REPORTS:
         # raw reports are unsigned
         format_str = "<H"
@@ -231,44 +240,44 @@
         scaled_data = raw_data * scalar
         results.append(scaled_data)
     results_tuple = tuple(results)
 
     return (results_tuple, accuracy)
 
 
-def _parse_step_couter_report(report_bytes):
+def _parse_step_couter_report(report_bytes: bytearray) -> int:
     return unpack_from("<H", report_bytes, offset=8)[0]
 
 
-def _parse_stability_classifier_report(report_bytes):
+def _parse_stability_classifier_report(report_bytes: bytearray) -> str:
     classification_bitfield = unpack_from("<B", report_bytes, offset=4)[0]
     return ["Unknown", "On Table", "Stationary", "Stable", "In motion"][
         classification_bitfield
     ]
 
 
 # report_id
 # feature_report_id
 # feature_flags
 # change_sensitivity
 # report_interval
 # batch_interval_word
 # sensor_specific_configuration_word
-def _parse_get_feature_response_report(report_bytes):
+def _parse_get_feature_response_report(report_bytes: bytearray) -> Tuple[Any, ...]:
     return unpack_from("<BBBHIII", report_bytes)
 
 
 # 0 Report ID = 0x1E
 # 1 Sequence number
 # 2 Status
 # 3 Delay
 # 4 Page Number + EOS
 # 5 Most likely state
 # 6-15 Classification (10 x Page Number) + confidence
-def _parse_activity_classifier_report(report_bytes):
+def _parse_activity_classifier_report(report_bytes: bytearray) -> Dict[str, str]:
     activities = [
         "Unknown",
         "In-Vehicle",  # look
         "On-Bicycle",  # at
         "On-Foot",  # all
         "Still",  # this
         "Tilting",  # room
@@ -288,50 +297,53 @@
     for idx, raw_confidence in enumerate(confidences):
         confidence = (10 * page_number) + raw_confidence
         activity_string = activities[idx]
         classification[activity_string] = confidence
     return classification
 
 
-def _parse_shake_report(report_bytes):
+def _parse_shake_report(report_bytes: bytearray) -> bool:
     shake_bitfield = unpack_from("<H", report_bytes, offset=4)[0]
     return (shake_bitfield & 0x111) > 0
 
 
-def parse_sensor_id(buffer):
+def parse_sensor_id(buffer: bytearray) -> Tuple[int, ...]:
     """Parse the fields of a product id report"""
     if not buffer[0] == _SHTP_REPORT_PRODUCT_ID_RESPONSE:
         raise AttributeError("Wrong report id for sensor id: %s" % hex(buffer[0]))
 
     sw_major = unpack_from("<B", buffer, offset=2)[0]
     sw_minor = unpack_from("<B", buffer, offset=3)[0]
     sw_patch = unpack_from("<H", buffer, offset=12)[0]
     sw_part_number = unpack_from("<I", buffer, offset=4)[0]
     sw_build_number = unpack_from("<I", buffer, offset=8)[0]
 
     return (sw_part_number, sw_major, sw_minor, sw_patch, sw_build_number)
 
 
-def _parse_command_response(report_bytes):
+def _parse_command_response(report_bytes: bytearray) -> Tuple[Any, Any]:
     # CMD response report:
     # 0 Report ID = 0xF1
     # 1 Sequence number
     # 2 Command
     # 3 Command sequence number
     # 4 Response sequence number
     # 5 R0-10 A set of response values. The interpretation of these values is specific
     # to the response for each command.
     report_body = unpack_from("<BBBBB", report_bytes)
     response_values = unpack_from("<BBBBBBBBBBB", report_bytes, offset=5)
     return (report_body, response_values)
 
 
 def _insert_command_request_report(
-    command, buffer, next_sequence_number, command_params=None
-):
+    command: int,
+    buffer: bytearray,
+    next_sequence_number: int,
+    command_params: Optional[List[int]] = None,
+) -> None:
     if command_params and len(command_params) > 9:
         raise AttributeError(
             "Command request reports can only have up to 9 arguments but %d were given"
             % len(command_params)
         )
     for _i in range(12):
         buffer[_i] = 0
@@ -341,22 +353,22 @@
     if command_params is None:
         return
 
     for idx, param in enumerate(command_params):
         buffer[3 + idx] = param
 
 
-def _report_length(report_id):
+def _report_length(report_id: int) -> int:
     if report_id < 0xF0:  # it's a sensor report
         return _AVAIL_SENSOR_REPORTS[report_id][2]
 
     return _REPORT_LENGTHS[report_id]
 
 
-def _separate_batch(packet, report_slices):
+def _separate_batch(packet: Packet, report_slices: List[Any]) -> None:
     # get first report id, loop up its report length
     # read that many bytes, parse them
     next_byte_index = 0
     while next_byte_index < packet.header.data_length:
         report_id = packet.data[next_byte_index]
         required_bytes = _report_length(report_id)
 
@@ -372,20 +384,20 @@
         report_slices.append([report_slice[0], report_slice])
         next_byte_index = next_byte_index + required_bytes
 
 
 class Packet:
     """A class representing a Hillcrest LaboratorySensor Hub Transport packet"""
 
-    def __init__(self, packet_bytes):
+    def __init__(self, packet_bytes: bytearray) -> None:
         self.header = self.header_from_buffer(packet_bytes)
         data_end_index = self.header.data_length + _BNO_HEADER_LEN
         self.data = packet_bytes[_BNO_HEADER_LEN:data_end_index]
 
-    def __str__(self):
+    def __str__(self) -> str:
         length = self.header.packet_byte_count
         outstr = "\n\t\t********** Packet *************\n"
         outstr += "DBG::\t\t HEADER:\n"
 
         outstr += "DBG::\t\t Data Len: %d\n" % (self.header.data_length)
         outstr += "DBG::\t\t Channel: %s (%d)\n" % (
             channels[self.channel_number],
@@ -435,39 +447,39 @@
             outstr += "0x{:02X} ".format(packet_byte)
         outstr += "\n"
         outstr += "\t\t*******************************\n"
 
         return outstr
 
     @property
-    def report_id(self):
+    def report_id(self) -> int:
         """The Packet's Report ID"""
         return self.data[0]
 
     @property
-    def channel_number(self):
+    def channel_number(self) -> int:
         """The packet channel"""
         return self.header.channel_number
 
     @classmethod
-    def header_from_buffer(cls, packet_bytes):
+    def header_from_buffer(cls, packet_bytes: bytearray) -> PacketHeader:
         """Creates a `PacketHeader` object from a given buffer"""
         packet_byte_count = unpack_from("<H", packet_bytes)[0]
         packet_byte_count &= ~0x8000
         channel_number = unpack_from("<B", packet_bytes, offset=2)[0]
         sequence_number = unpack_from("<B", packet_bytes, offset=3)[0]
         data_length = max(0, packet_byte_count - 4)
 
         header = PacketHeader(
             channel_number, sequence_number, data_length, packet_byte_count
         )
         return header
 
     @classmethod
-    def is_error(cls, header):
+    def is_error(cls, header: PacketHeader) -> bool:
         """Returns True if the header is an error condition"""
 
         if header.channel_number > 5:
             return True
         if header.packet_byte_count == 0xFFFF and header.sequence_number == 0xFF:
             return True
         return False
@@ -476,146 +488,145 @@
 class BNO08X:  # pylint: disable=too-many-instance-attributes, too-many-public-methods
     """Library for the BNO08x IMUs from Hillcrest Laboratories
 
     :param ~busio.I2C i2c_bus: The I2C bus the BNO08x is connected to.
 
     """
 
-    def __init__(self, reset=None, debug=False):
-        self._debug = debug
-        self._reset = reset
+    def __init__(
+        self, reset: Optional[DigitalInOut] = None, debug: bool = False
+    ) -> None:
+        self._debug: bool = debug
+        self._reset: Optional[DigitalInOut] = reset
         self._dbg("********** __init__ *************")
-        self._data_buffer = bytearray(DATA_BUFFER_SIZE)
-        self._command_buffer = bytearray(12)
-        self._packet_slices = []
+        self._data_buffer: bytearray = bytearray(DATA_BUFFER_SIZE)
+        self._command_buffer: bytearray = bytearray(12)
+        self._packet_slices: List[Any] = []
 
         # TODO: this is wrong there should be one per channel per direction
-        self._sequence_number = [0, 0, 0, 0, 0, 0]
-        self._two_ended_sequence_numbers = {
-            "send": {},  # holds the next seq number to send with the report id as a key
-            "receive": {},
-        }
-        self._dcd_saved_at = -1
-        self._me_calibration_started_at = -1
+        self._sequence_number: List[int] = [0, 0, 0, 0, 0, 0]
+        self._two_ended_sequence_numbers: Dict[int, int] = {}
+        self._dcd_saved_at: float = -1
+        self._me_calibration_started_at: float = -1.0
         self._calibration_complete = False
         self._magnetometer_accuracy = 0
         self._wait_for_initialize = True
         self._init_complete = False
         self._id_read = False
         # for saving the most recent reading when decoding several packets
-        self._readings = {}
+        self._readings: Dict[int, Any] = {}
         self.initialize()
 
-    def initialize(self):
+    def initialize(self) -> None:
         """Initialize the sensor"""
         for _ in range(3):
             self.hard_reset()
             self.soft_reset()
             try:
                 if self._check_id():
                     break
             except:  # pylint:disable=bare-except
                 time.sleep(0.5)
         else:
             raise RuntimeError("Could not read ID")
 
     @property
-    def magnetic(self):
+    def magnetic(self) -> Optional[Tuple[float, float, float]]:
         """A tuple of the current magnetic field measurements on the X, Y, and Z axes"""
         self._process_available_packets()  # decorator?
         try:
             return self._readings[BNO_REPORT_MAGNETOMETER]
         except KeyError:
             raise RuntimeError("No magfield report found, is it enabled?") from None
 
     @property
-    def quaternion(self):
+    def quaternion(self) -> Optional[Tuple[float, float, float, float]]:
         """A quaternion representing the current rotation vector"""
         self._process_available_packets()
         try:
             return self._readings[BNO_REPORT_ROTATION_VECTOR]
         except KeyError:
             raise RuntimeError("No quaternion report found, is it enabled?") from None
 
     @property
-    def geomagnetic_quaternion(self):
+    def geomagnetic_quaternion(self) -> Optional[Tuple[float, float, float, float]]:
         """A quaternion representing the current geomagnetic rotation vector"""
         self._process_available_packets()
         try:
             return self._readings[BNO_REPORT_GEOMAGNETIC_ROTATION_VECTOR]
         except KeyError:
             raise RuntimeError(
                 "No geomag quaternion report found, is it enabled?"
             ) from None
 
     @property
-    def game_quaternion(self):
+    def game_quaternion(self) -> Optional[Tuple[float, float, float, float]]:
         """A quaternion representing the current rotation vector expressed as a quaternion with no
         specific reference for heading, while roll and pitch are referenced against gravity. To
         prevent sudden jumps in heading due to corrections, the `game_quaternion` property is not
         corrected using the magnetometer. Some drift is expected"""
         self._process_available_packets()
         try:
             return self._readings[BNO_REPORT_GAME_ROTATION_VECTOR]
         except KeyError:
             raise RuntimeError(
                 "No game quaternion report found, is it enabled?"
             ) from None
 
     @property
-    def steps(self):
+    def steps(self) -> Optional[int]:
         """The number of steps detected since the sensor was initialized"""
         self._process_available_packets()
         try:
             return self._readings[BNO_REPORT_STEP_COUNTER]
         except KeyError:
             raise RuntimeError("No steps report found, is it enabled?") from None
 
     @property
-    def linear_acceleration(self):
+    def linear_acceleration(self) -> Optional[Tuple[float, float, float]]:
         """A tuple representing the current linear acceleration values on the X, Y, and Z
         axes in meters per second squared"""
         self._process_available_packets()
         try:
             return self._readings[BNO_REPORT_LINEAR_ACCELERATION]
         except KeyError:
             raise RuntimeError("No lin. accel report found, is it enabled?") from None
 
     @property
-    def acceleration(self):
+    def acceleration(self) -> Optional[Tuple[float, float, float]]:
         """A tuple representing the acceleration measurements on the X, Y, and Z
         axes in meters per second squared"""
         self._process_available_packets()
         try:
             return self._readings[BNO_REPORT_ACCELEROMETER]
         except KeyError:
             raise RuntimeError("No accel report found, is it enabled?") from None
 
     @property
-    def gravity(self):
+    def gravity(self) -> Optional[Tuple[float, float, float]]:
         """A tuple representing the gravity vector in the X, Y, and Z components
         axes in meters per second squared"""
         self._process_available_packets()
         try:
             return self._readings[BNO_REPORT_GRAVITY]
         except KeyError:
             raise RuntimeError("No gravity report found, is it enabled?") from None
 
     @property
-    def gyro(self):
+    def gyro(self) -> Optional[Tuple[float, float, float]]:
         """A tuple representing Gyro's rotation measurements on the X, Y, and Z
         axes in radians per second"""
         self._process_available_packets()
         try:
             return self._readings[BNO_REPORT_GYROSCOPE]
         except KeyError:
             raise RuntimeError("No gyro report found, is it enabled?") from None
 
     @property
-    def shake(self):
+    def shake(self) -> Optional[bool]:
         """True if a shake was detected on any axis since the last time it was checked
 
         This property has a "latching" behavior where once a shake is detected, it will stay in a
         "shaken" state until the value is read. This prevents missing shake events but means that
         this property is not guaranteed to reflect the shake state at the moment it is read
         """
         self._process_available_packets()
@@ -625,15 +636,15 @@
             if shake_detected:
                 self._readings[BNO_REPORT_SHAKE_DETECTOR] = False
             return shake_detected
         except KeyError:
             raise RuntimeError("No shake report found, is it enabled?") from None
 
     @property
-    def stability_classification(self):
+    def stability_classification(self) -> Optional[str]:
         """Returns the sensor's assessment of it's current stability, one of:
 
         * "Unknown" - The sensor is unable to classify the current stability
         * "On Table" - The sensor is at rest on a stable surface with very little vibration
         * "Stationary" -  The sensor’s motion is below the stable threshold but\
         the stable duration requirement has not been met. This output is only available when\
         gyro calibration is enabled
@@ -647,15 +658,15 @@
             return stability_classification
         except KeyError:
             raise RuntimeError(
                 "No stability classification report found, is it enabled?"
             ) from None
 
     @property
-    def activity_classification(self):
+    def activity_classification(self) -> Optional[dict]:
         """Returns the sensor's assessment of the activity that is creating the motions\
         that it is sensing, one of:
 
         * "Unknown"
         * "In-Vehicle"
         * "On-Bicycle"
         * "On-Foot"
@@ -672,46 +683,46 @@
             return activity_classification
         except KeyError:
             raise RuntimeError(
                 "No activity classification report found, is it enabled?"
             ) from None
 
     @property
-    def raw_acceleration(self):
+    def raw_acceleration(self) -> Optional[Tuple[int, int, int]]:
         """Returns the sensor's raw, unscaled value from the accelerometer registers"""
         self._process_available_packets()
         try:
             raw_acceleration = self._readings[BNO_REPORT_RAW_ACCELEROMETER]
             return raw_acceleration
         except KeyError:
             raise RuntimeError(
                 "No raw acceleration report found, is it enabled?"
             ) from None
 
     @property
-    def raw_gyro(self):
+    def raw_gyro(self) -> Optional[Tuple[int, int, int]]:
         """Returns the sensor's raw, unscaled value from the gyro registers"""
         self._process_available_packets()
         try:
             raw_gyro = self._readings[BNO_REPORT_RAW_GYROSCOPE]
             return raw_gyro
         except KeyError:
             raise RuntimeError("No raw gyro report found, is it enabled?") from None
 
     @property
-    def raw_magnetic(self):
+    def raw_magnetic(self) -> Optional[Tuple[int, int, int]]:
         """Returns the sensor's raw, unscaled value from the magnetometer registers"""
         self._process_available_packets()
         try:
             raw_magnetic = self._readings[BNO_REPORT_RAW_MAGNETOMETER]
             return raw_magnetic
         except KeyError:
             raise RuntimeError("No raw magnetic report found, is it enabled?") from None
 
-    def begin_calibration(self):
+    def begin_calibration(self) -> None:
         """Begin the sensor's self-calibration routine"""
         # start calibration for accel, gyro, and mag
         self._send_me_command(
             [
                 1,  # calibrate accel
                 1,  # calibrate gyro
                 1,  # calibrate mag
@@ -722,15 +733,15 @@
                 0,  # reserved
                 0,  # reserved
             ]
         )
         self._calibration_complete = False
 
     @property
-    def calibration_status(self):
+    def calibration_status(self) -> int:
         """Get the status of the self-calibration"""
         self._send_me_command(
             [
                 0,  # calibrate accel
                 0,  # calibrate gyro
                 0,  # calibrate mag
                 _ME_GET_CAL,
@@ -739,15 +750,15 @@
                 0,  # reserved
                 0,  # reserved
                 0,  # reserved
             ]
         )
         return self._magnetometer_accuracy
 
-    def _send_me_command(self, subcommand_params):
+    def _send_me_command(self, subcommand_params: Optional[List[int]]) -> None:
         start_time = time.monotonic()
         local_buffer = self._command_buffer
         _insert_command_request_report(
             _ME_CALIBRATE,
             self._command_buffer,  # should use self._data_buffer :\ but send_packet don't
             self._get_report_seq_id(_COMMAND_REQUEST),
             subcommand_params,
@@ -755,15 +766,15 @@
         self._send_packet(_BNO_CHANNEL_CONTROL, local_buffer)
         self._increment_report_seq(_COMMAND_REQUEST)
         while _elapsed(start_time) < _DEFAULT_TIMEOUT:
             self._process_available_packets()
             if self._me_calibration_started_at > start_time:
                 break
 
-    def save_calibration_data(self):
+    def save_calibration_data(self) -> None:
         """Save the self-calibration data"""
         # send a DCD save command
         start_time = time.monotonic()
         local_buffer = bytearray(12)
         _insert_command_request_report(
             _SAVE_DCD,
             local_buffer,  # should use self._data_buffer :\ but send_packet don't
@@ -775,15 +786,15 @@
             self._process_available_packets()
             if self._dcd_saved_at > start_time:
                 return
         raise RuntimeError("Could not save calibration data")
 
     ############### private/helper methods ###############
     # # decorator?
-    def _process_available_packets(self, max_packets=None):
+    def _process_available_packets(self, max_packets: Optional[int] = None) -> None:
         processed_count = 0
         while self._data_ready:
             if max_packets and processed_count > max_packets:
                 return
             # print("reading a packet")
             try:
                 new_packet = self._read_packet()
@@ -793,15 +804,17 @@
             processed_count += 1
             self._dbg("")
             # print("Processed", processed_count, "packets")
             self._dbg("")
         self._dbg("")
         self._dbg(" ** DONE! **")
 
-    def _wait_for_packet_type(self, channel_number, report_id=None, timeout=5.0):
+    def _wait_for_packet_type(
+        self, channel_number: int, report_id: Optional[int] = None, timeout: float = 5.0
+    ) -> Packet:
         if report_id:
             report_id_str = " with report id %s" % hex(report_id)
         else:
             report_id_str = ""
         self._dbg("** Waiting for packet on channel", channel_number, report_id_str)
         start_time = time.monotonic()
         while _elapsed(start_time) < timeout:
@@ -818,42 +831,42 @@
                 BNO_CHANNEL_SHTP_COMMAND,
             ):
                 self._dbg("passing packet to handler for de-slicing")
                 self._handle_packet(new_packet)
 
         raise RuntimeError("Timed out waiting for a packet on channel", channel_number)
 
-    def _wait_for_packet(self, timeout=_PACKET_READ_TIMEOUT):
+    def _wait_for_packet(self, timeout: float = _PACKET_READ_TIMEOUT) -> Packet:
         start_time = time.monotonic()
         while _elapsed(start_time) < timeout:
             if not self._data_ready:
                 continue
             new_packet = self._read_packet()
             return new_packet
         raise RuntimeError("Timed out waiting for a packet")
 
     # update the cached sequence number so we know what to increment from
     # TODO: this is wrong there should be one per channel per direction
     # and apparently per report as well
-    def _update_sequence_number(self, new_packet):
+    def _update_sequence_number(self, new_packet: Packet) -> None:
         channel = new_packet.channel_number
         seq = new_packet.header.sequence_number
         self._sequence_number[channel] = seq
 
-    def _handle_packet(self, packet):
+    def _handle_packet(self, packet: Packet) -> None:
         # split out reports first
         try:
             _separate_batch(packet, self._packet_slices)
             while len(self._packet_slices) > 0:
                 self._process_report(*self._packet_slices.pop())
         except Exception as error:
             print(packet)
             raise error
 
-    def _handle_control_report(self, report_id, report_bytes):
+    def _handle_control_report(self, report_id: int, report_bytes: bytearray) -> None:
         if report_id == _SHTP_REPORT_PRODUCT_ID_RESPONSE:
             (
                 sw_part_number,
                 sw_major,
                 sw_minor,
                 sw_patch,
                 sw_build_number,
@@ -869,15 +882,15 @@
             _report_id, feature_report_id, *_remainder = get_feature_report
             self._readings[feature_report_id] = _INITIAL_REPORTS.get(
                 feature_report_id, (0.0, 0.0, 0.0)
             )
         if report_id == _COMMAND_RESPONSE:
             self._handle_command_response(report_bytes)
 
-    def _handle_command_response(self, report_bytes):
+    def _handle_command_response(self, report_bytes: bytearray) -> None:
         (report_body, response_values) = _parse_command_response(report_bytes)
 
         (
             _report_id,
             _seq_number,
             command,
             _command_seq_number,
@@ -892,15 +905,15 @@
 
         if command == _SAVE_DCD:
             if command_status == 0:
                 self._dcd_saved_at = time.monotonic()
             else:
                 raise RuntimeError("Unable to save calibration data")
 
-    def _process_report(self, report_id, report_bytes):
+    def _process_report(self, report_id: int, report_bytes: bytearray) -> None:
         if report_id >= 0xF0:
             self._handle_control_report(report_id, report_bytes)
             return
         self._dbg("\tProcessing report:", reports[report_id])
         if self._debug:
             outstr = ""
             for idx, packet_byte in enumerate(report_bytes):
@@ -941,28 +954,30 @@
         # for the same type will end with the oldest/last being kept and the other
         # newer reports thrown away
         self._readings[report_id] = sensor_data
 
     # TODO: Make this a Packet creation
     @staticmethod
     def _get_feature_enable_report(
-        feature_id, report_interval=_DEFAULT_REPORT_INTERVAL, sensor_specific_config=0
-    ):
+        feature_id: int,
+        report_interval: int = _DEFAULT_REPORT_INTERVAL,
+        sensor_specific_config: int = 0,
+    ) -> bytearray:
         set_feature_report = bytearray(17)
         set_feature_report[0] = _SET_FEATURE_COMMAND
         set_feature_report[1] = feature_id
         pack_into("<I", set_feature_report, 5, report_interval)
         pack_into("<I", set_feature_report, 13, sensor_specific_config)
 
         return set_feature_report
 
     # TODO: add docs for available features
     # TODO2: I think this should call an fn that imports all the bits for the given feature
     # so we're not carrying around  stuff for extra features
-    def enable_feature(self, feature_id):
+    def enable_feature(self, feature_id: int) -> None:
         """Used to enable a given feature of the BNO08x"""
         self._dbg("\n********** Enabling feature id:", feature_id, "**********")
 
         if feature_id == BNO_REPORT_ACTIVITY_CLASSIFIER:
             set_feature_report = self._get_feature_enable_report(
                 feature_id, sensor_specific_config=_ENABLED_ACTIVITIES
             )
@@ -982,15 +997,15 @@
 
         while _elapsed(start_time) < _FEATURE_ENABLE_TIMEOUT:
             self._process_available_packets(max_packets=10)
             if feature_id in self._readings:
                 return
         raise RuntimeError("Was not able to enable feature", feature_id)
 
-    def _check_id(self):
+    def _check_id(self) -> bool:
         self._dbg("\n********** READ ID **********")
         if self._id_read:
             return True
         data = bytearray(2)
         data[0] = _SHTP_REPORT_PRODUCT_ID_REQUEST
         data[1] = 0  # padding
         self._dbg("\n** Sending ID Request Report **")
@@ -1005,15 +1020,15 @@
             if sensor_id:
                 self._id_read = True
                 return True
             self._dbg("Packet didn't have sensor ID report, trying again")
 
         return False
 
-    def _parse_sensor_id(self):
+    def _parse_sensor_id(self) -> Optional[int]:
         if not self._data_buffer[4] == _SHTP_REPORT_PRODUCT_ID_RESPONSE:
             return None
 
         sw_major = self._get_data(2, "<B")
         sw_minor = self._get_data(3, "<B")
         sw_patch = self._get_data(12, "<H")
         sw_part_number = self._get_data(4, "<I")
@@ -1023,43 +1038,43 @@
         self._dbg("*** Part Number: %d" % sw_part_number)
         self._dbg("*** Software Version: %d.%d.%d" % (sw_major, sw_minor, sw_patch))
         self._dbg(" Build: %d" % (sw_build_number))
         self._dbg("")
         # TODO: this is only one of the numbers!
         return sw_part_number
 
-    def _dbg(self, *args, **kwargs):
+    def _dbg(self, *args: Any, **kwargs: Any) -> None:
         if self._debug:
             print("DBG::\t\t", *args, **kwargs)
 
-    def _get_data(self, index, fmt_string):
+    def _get_data(self, index: int, fmt_string: str) -> Any:
         # index arg is not including header, so add 4 into data buffer
         data_index = index + 4
         return unpack_from(fmt_string, self._data_buffer, offset=data_index)[0]
 
     # pylint:disable=no-self-use
     @property
-    def _data_ready(self):
+    def _data_ready(self) -> None:
         raise RuntimeError("Not implemented")
 
-    def hard_reset(self):
+    def hard_reset(self) -> None:
         """Hardware reset the sensor to an initial unconfigured state"""
         if not self._reset:
             return
         import digitalio  # pylint:disable=import-outside-toplevel
 
         self._reset.direction = digitalio.Direction.OUTPUT
         self._reset.value = True
         time.sleep(0.01)
         self._reset.value = False
         time.sleep(0.01)
         self._reset.value = True
         time.sleep(0.01)
 
-    def soft_reset(self):
+    def soft_reset(self) -> None:
         """Reset the sensor to an initial unconfigured state"""
         self._dbg("Soft resetting...", end="")
         data = bytearray(1)
         data[0] = 1
         _seq = self._send_packet(BNO_CHANNEL_EXE, data)
         time.sleep(0.5)
         _seq = self._send_packet(BNO_CHANNEL_EXE, data)
@@ -1070,19 +1085,19 @@
                 _packet = self._read_packet()
             except PacketError:
                 time.sleep(0.5)
 
         self._dbg("OK!")
         # all is good!
 
-    def _send_packet(self, channel, data):
+    def _send_packet(self, channel: int, data: bytearray) -> Optional[int]:
         raise RuntimeError("Not implemented")
 
-    def _read_packet(self):
+    def _read_packet(self) -> Optional[Packet]:
         raise RuntimeError("Not implemented")
 
-    def _increment_report_seq(self, report_id):
+    def _increment_report_seq(self, report_id: int) -> None:
         current = self._two_ended_sequence_numbers.get(report_id, 0)
         self._two_ended_sequence_numbers[report_id] = (current + 1) % 256
 
-    def _get_report_seq_id(self, report_id):
+    def _get_report_seq_id(self, report_id: int) -> int:
         return self._two_ended_sequence_numbers.get(report_id, 0)
```

### Comparing `adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/debug.py` & `adafruit-circuitpython-bno08x-1.2.3/adafruit_bno08x/debug.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/i2c.py` & `adafruit-circuitpython-bno08x-1.2.3/adafruit_bno08x/i2c.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/spi.py` & `adafruit-circuitpython-bno08x-1.2.3/adafruit_bno08x/spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/uart.py` & `adafruit-circuitpython-bno08x-1.2.3/adafruit_bno08x/uart.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/adafruit_circuitpython_bno08x.egg-info/PKG-INFO` & `adafruit-circuitpython-bno08x-1.2.3/adafruit_circuitpython_bno08x.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bno08x
-Version: 1.2.2
+Version: 1.2.3
 Summary: Helper library for the Hillcrest Laboratories BNO08x IMUs
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BNO08x
 Keywords: adafruit,blinka,circuitpython,micropython,bno080,IMU,BNO055,SENSOR,FUSION,VR,MOTION,TRACK,BNO085
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bno08x-1.2.2/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt` & `adafruit-circuitpython-bno08x-1.2.3/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/docs/_static/favicon.ico` & `adafruit-circuitpython-bno08x-1.2.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/docs/conf.py` & `adafruit-circuitpython-bno08x-1.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/docs/index.rst` & `adafruit-circuitpython-bno08x-1.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_calibration.py` & `adafruit-circuitpython-bno08x-1.2.3/examples/bno08x_calibration.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_find_heading.py` & `adafruit-circuitpython-bno08x-1.2.3/examples/bno08x_find_heading.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_more_reports.py` & `adafruit-circuitpython-bno08x-1.2.3/examples/bno08x_more_reports.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_quaternion_service.py` & `adafruit-circuitpython-bno08x-1.2.3/examples/bno08x_quaternion_service.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_simpletest.py` & `adafruit-circuitpython-bno08x-1.2.3/examples/bno08x_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_simpletest_spi.py` & `adafruit-circuitpython-bno08x-1.2.3/examples/bno08x_simpletest_spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_simpletest_uart.py` & `adafruit-circuitpython-bno08x-1.2.3/examples/bno08x_simpletest_uart.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.2/pyproject.toml` & `adafruit-circuitpython-bno08x-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-bno08x"
 description = "Helper library for the Hillcrest Laboratories BNO08x IMUs"
-version = "1.2.2"
+version = "1.2.3"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BNO08x"}
 keywords = [
     "adafruit",
```

