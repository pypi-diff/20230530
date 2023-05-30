# Comparing `tmp/adafruit-circuitpython-wiznet5k-2.5.2.tar.gz` & `tmp/adafruit-circuitpython-wiznet5k-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-wiznet5k-2.5.2.tar", last modified: Fri May 26 16:15:48 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-wiznet5k-2.5.3.tar", last modified: Tue May 30 13:27:10 2023, max compression
```

## Comparing `adafruit-circuitpython-wiznet5k-2.5.2.tar` & `adafruit-circuitpython-wiznet5k-2.5.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:48.807623 adafruit-circuitpython-wiznet5k-2.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:48.799623 adafruit-circuitpython-wiznet5k-2.5.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:48.799623 adafruit-circuitpython-wiznet5k-2.5.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:48.799623 adafruit-circuitpython-wiznet5k-2.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:48.799623 adafruit-circuitpython-wiznet5k-2.5.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-26 16:15:48.807623 adafruit-circuitpython-wiznet5k-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:48.803623 adafruit-circuitpython-wiznet5k-2.5.2/adafruit_circuitpython_wiznet5k.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-26 16:15:48.000000 adafruit-circuitpython-wiznet5k-2.5.2/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-26 16:15:48.000000 adafruit-circuitpython-wiznet5k-2.5.2/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:15:48.000000 adafruit-circuitpython-wiznet5k-2.5.2/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 16:15:48.000000 adafruit-circuitpython-wiznet5k-2.5.2/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 16:15:48.000000 adafruit-circuitpython-wiznet5k-2.5.2/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:48.803623 adafruit-circuitpython-wiznet5k-2.5.2/adafruit_wiznet5k/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/adafruit_wiznet5k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50486 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/adafruit_wiznet5k/adafruit_wiznet5k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    27777 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py
--rw-r--r--   0 runner    (1001) docker     (123)    27027 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/adafruit_wiznet5k/adafruit_wiznet5k_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:48.803623 adafruit-circuitpython-wiznet5k-2.5.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:48.803623 adafruit-circuitpython-wiznet5k-2.5.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:48.803623 adafruit-circuitpython-wiznet5k-2.5.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/examples/wiznet5k_aio_post.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/examples/wiznet5k_cheerlights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/examples/wiznet5k_cpython_client_for_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/examples/wiznet5k_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/examples/wiznet5k_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/examples/wiznet5k_simpletest_manual_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/examples/wiznet5k_wsgiserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 16:15:31.000000 adafruit-circuitpython-wiznet5k-2.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:15:48.807623 adafruit-circuitpython-wiznet5k-2.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:48.807623 adafruit-circuitpython-wiznet5k-2.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/tests/dhcp_dummy_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/tests/extract_unique_dns_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)    31513 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/tests/test_dhcp_helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/tests/test_dns_server_nonbreaking_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-26 16:15:41.000000 adafruit-circuitpython-wiznet5k-2.5.2/tests/test_parse_dns_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.681176 adafruit-circuitpython-wiznet5k-2.5.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.673175 adafruit-circuitpython-wiznet5k-2.5.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.673175 adafruit-circuitpython-wiznet5k-2.5.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.673175 adafruit-circuitpython-wiznet5k-2.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.673175 adafruit-circuitpython-wiznet5k-2.5.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-30 13:27:10.681176 adafruit-circuitpython-wiznet5k-2.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.677176 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_circuitpython_wiznet5k.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-30 13:27:10.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-30 13:27:10.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:27:10.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-30 13:27:10.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 13:27:10.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.677176 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50486 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27777 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27027 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.677176 adafruit-circuitpython-wiznet5k-2.5.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.677176 adafruit-circuitpython-wiznet5k-2.5.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.677176 adafruit-circuitpython-wiznet5k-2.5.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_aio_post.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_cheerlights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_cpython_client_for_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_simpletest_manual_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_wsgiserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-30 13:26:55.000000 adafruit-circuitpython-wiznet5k-2.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:27:10.681176 adafruit-circuitpython-wiznet5k-2.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:27:10.681176 adafruit-circuitpython-wiznet5k-2.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/tests/dhcp_dummy_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/tests/extract_unique_dns_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31513 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/tests/test_dhcp_helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/tests/test_dns_server_nonbreaking_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-30 13:27:03.000000 adafruit-circuitpython-wiznet5k-2.5.3/tests/test_parse_dns_function.py
```

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-wiznet5k-2.5.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/.gitignore` & `adafruit-circuitpython-wiznet5k-2.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/.pre-commit-config.yaml` & `adafruit-circuitpython-wiznet5k-2.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/.pylintrc` & `adafruit-circuitpython-wiznet5k-2.5.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-wiznet5k-2.5.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/LICENSE` & `adafruit-circuitpython-wiznet5k-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-wiznet5k-2.5.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/LICENSES/MIT.txt` & `adafruit-circuitpython-wiznet5k-2.5.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-wiznet5k-2.5.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/PKG-INFO` & `adafruit-circuitpython-wiznet5k-2.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wiznet5k
-Version: 2.5.2
+Version: 2.5.3
 Summary: Pure-Python interface for WIZNET 5k ethernet modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
 Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/README.rst` & `adafruit-circuitpython-wiznet5k-2.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO` & `adafruit-circuitpython-wiznet5k-2.5.3/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wiznet5k
-Version: 2.5.2
+Version: 2.5.3
 Summary: Pure-Python interface for WIZNET 5k ethernet modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
 Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt` & `adafruit-circuitpython-wiznet5k-2.5.3/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/adafruit_wiznet5k/adafruit_wiznet5k.py` & `adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     if TYPE_CHECKING:
         from circuitpython_typing import WriteableBuffer
         import busio
         import digitalio
 except ImportError:
     pass
 
-__version__ = "2.5.2"
+__version__ = "2.5.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k.git"
 
 from random import randint
 import time
 import gc
 from micropython import const
```

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/adafruit_wiznet5k/adafruit_wiznet5k_debug.py` & `adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_debug.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py` & `adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/adafruit_wiznet5k/adafruit_wiznet5k_dns.py` & `adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_dns.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py` & `adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     if TYPE_CHECKING:
         from adafruit_wiznet5k.adafruit_wiznet5k import WIZNET5K
 except ImportError:
     pass
 import time
 import adafruit_wiznet5k.adafruit_wiznet5k_socket as socket
 
-# __version__ = "2.5.2"
+# __version__ = "2.5.3"
 # __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_NTP.git"
 
 
 class NTP:
     """Wiznet5k NTP Client."""
 
     def __init__(
```

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/adafruit_wiznet5k/adafruit_wiznet5k_socket.py` & `adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_socket.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py` & `adafruit-circuitpython-wiznet5k-2.5.3/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/docs/_static/favicon.ico` & `adafruit-circuitpython-wiznet5k-2.5.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/docs/api.rst` & `adafruit-circuitpython-wiznet5k-2.5.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/docs/conf.py` & `adafruit-circuitpython-wiznet5k-2.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/docs/index.rst` & `adafruit-circuitpython-wiznet5k-2.5.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/examples/wiznet5k_aio_post.py` & `adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/examples/wiznet5k_cheerlights.py` & `adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/examples/wiznet5k_cpython_client_for_simpleserver.py` & `adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_cpython_client_for_simpleserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/examples/wiznet5k_simpleserver.py` & `adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_simpleserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/examples/wiznet5k_simpletest.py` & `adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/examples/wiznet5k_simpletest_manual_network.py` & `adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_simpletest_manual_network.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/examples/wiznet5k_wsgiserver.py` & `adafruit-circuitpython-wiznet5k-2.5.3/examples/wiznet5k_wsgiserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/pyproject.toml` & `adafruit-circuitpython-wiznet5k-2.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-wiznet5k"
 description = "Pure-Python interface for WIZNET 5k ethernet modules."
-version = "2.5.2"
+version = "2.5.3"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k"}
 keywords = [
     "adafruit",
@@ -39,12 +39,12 @@
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["adafruit_wiznet5k"]
+packages = ["adafruit_wiznet5k"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 optional-dependencies = {optional = {file = ["optional_requirements.txt"]}}
```

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/tests/dhcp_dummy_data.py` & `adafruit-circuitpython-wiznet5k-2.5.3/tests/dhcp_dummy_data.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/tests/extract_unique_dns_responses.py` & `adafruit-circuitpython-wiznet5k-2.5.3/tests/extract_unique_dns_responses.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/tests/test_dhcp_helper_functions.py` & `adafruit-circuitpython-wiznet5k-2.5.3/tests/test_dhcp_helper_functions.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/tests/test_dns_server_nonbreaking_changes.py` & `adafruit-circuitpython-wiznet5k-2.5.3/tests/test_dns_server_nonbreaking_changes.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.5.2/tests/test_parse_dns_function.py` & `adafruit-circuitpython-wiznet5k-2.5.3/tests/test_parse_dns_function.py`

 * *Files identical despite different names*

