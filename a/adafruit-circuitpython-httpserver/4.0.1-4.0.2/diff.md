# Comparing `tmp/adafruit-circuitpython-httpserver-4.0.1.tar.gz` & `tmp/adafruit-circuitpython-httpserver-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-httpserver-4.0.1.tar", last modified: Fri May 26 16:16:18 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-httpserver-4.0.2.tar", last modified: Tue May 30 00:58:11 2023, max compression
```

## Comparing `adafruit-circuitpython-httpserver-4.0.1.tar` & `adafruit-circuitpython-httpserver-4.0.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:18.685745 adafruit-circuitpython-httpserver-4.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:18.669744 adafruit-circuitpython-httpserver-4.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:18.673745 adafruit-circuitpython-httpserver-4.0.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:18.673745 adafruit-circuitpython-httpserver-4.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:18.677744 adafruit-circuitpython-httpserver-4.0.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-26 16:16:18.685745 adafruit-circuitpython-httpserver-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:18.677744 adafruit-circuitpython-httpserver-4.0.1/adafruit_circuitpython_httpserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-26 16:16:18.000000 adafruit-circuitpython-httpserver-4.0.1/adafruit_circuitpython_httpserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-26 16:16:18.000000 adafruit-circuitpython-httpserver-4.0.1/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:16:18.000000 adafruit-circuitpython-httpserver-4.0.1/adafruit_circuitpython_httpserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 16:16:18.000000 adafruit-circuitpython-httpserver-4.0.1/adafruit_circuitpython_httpserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 16:16:18.000000 adafruit-circuitpython-httpserver-4.0.1/adafruit_circuitpython_httpserver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:18.677744 adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/mime_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/route.py
--rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:18.681745 adafruit-circuitpython-httpserver-4.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:18.681745 adafruit-circuitpython-httpserver-4.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:18.681745 adafruit-circuitpython-httpserver-4.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/examples/home.html
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_authentication_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_authentication_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_chunked.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_cpu_information.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_handler_serves_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_mdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_multiple_servers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_neopixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_redirects.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_simpletest_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_simpletest_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_start_and_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_static_files_serving.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_url_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/examples/settings.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-26 16:16:10.000000 adafruit-circuitpython-httpserver-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 16:15:59.000000 adafruit-circuitpython-httpserver-4.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:16:18.685745 adafruit-circuitpython-httpserver-4.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.050245 adafruit-circuitpython-httpserver-4.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.038245 adafruit-circuitpython-httpserver-4.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.042245 adafruit-circuitpython-httpserver-4.0.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.042245 adafruit-circuitpython-httpserver-4.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.042245 adafruit-circuitpython-httpserver-4.0.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-30 00:58:11.050245 adafruit-circuitpython-httpserver-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.042245 adafruit-circuitpython-httpserver-4.0.2/adafruit_circuitpython_httpserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-30 00:58:11.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_circuitpython_httpserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-30 00:58:11.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:58:11.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_circuitpython_httpserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-30 00:58:11.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_circuitpython_httpserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 00:58:11.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_circuitpython_httpserver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.042245 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/mime_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.046245 adafruit-circuitpython-httpserver-4.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.046245 adafruit-circuitpython-httpserver-4.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.050245 adafruit-circuitpython-httpserver-4.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/examples/home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_authentication_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_authentication_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_chunked.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_cpu_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_handler_serves_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_mdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_multiple_servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_neopixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_redirects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_simpletest_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_simpletest_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_start_and_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_static_files_serving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_url_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/settings.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 00:58:11.054245 adafruit-circuitpython-httpserver-4.0.2/setup.cfg
```

### Comparing `adafruit-circuitpython-httpserver-4.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-httpserver-4.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/.gitignore` & `adafruit-circuitpython-httpserver-4.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/.pre-commit-config.yaml` & `adafruit-circuitpython-httpserver-4.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/.pylintrc` & `adafruit-circuitpython-httpserver-4.0.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-httpserver-4.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/LICENSE` & `adafruit-circuitpython-httpserver-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-httpserver-4.0.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/LICENSES/MIT.txt` & `adafruit-circuitpython-httpserver-4.0.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-httpserver-4.0.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/PKG-INFO` & `adafruit-circuitpython-httpserver-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-httpserver
-Version: 4.0.1
+Version: 4.0.2
 Summary: Simple HTTP Server for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git
 Keywords: adafruit,blinka,circuitpython,micropython,httpserver,web,server,webserver,http
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-httpserver-4.0.1/README.rst` & `adafruit-circuitpython-httpserver-4.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/adafruit_circuitpython_httpserver.egg-info/PKG-INFO` & `adafruit-circuitpython-httpserver-4.0.2/adafruit_circuitpython_httpserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-httpserver
-Version: 4.0.1
+Version: 4.0.2
 Summary: Simple HTTP Server for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git
 Keywords: adafruit,blinka,circuitpython,micropython,httpserver,web,server,webserver,http
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-httpserver-4.0.1/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt` & `adafruit-circuitpython-httpserver-4.0.2/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/__init__.py` & `adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 """
 
-__version__ = "4.0.1"
+__version__ = "4.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git"
 
 
 from .authentication import (
     Basic,
     Bearer,
     check_authentication,
```

### Comparing `adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/authentication.py` & `adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/authentication.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/exceptions.py` & `adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/exceptions.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/headers.py` & `adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/headers.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/mime_types.py` & `adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/mime_types.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/request.py` & `adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/request.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/response.py` & `adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/response.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/route.py` & `adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/route.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/server.py` & `adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/server.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/adafruit_httpserver/status.py` & `adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/status.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/docs/_static/favicon.ico` & `adafruit-circuitpython-httpserver-4.0.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/docs/api.rst` & `adafruit-circuitpython-httpserver-4.0.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/docs/conf.py` & `adafruit-circuitpython-httpserver-4.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/docs/examples.rst` & `adafruit-circuitpython-httpserver-4.0.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/docs/index.rst` & `adafruit-circuitpython-httpserver-4.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_authentication_handlers.py` & `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_authentication_handlers.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_authentication_server.py` & `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_authentication_server.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_chunked.py` & `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_chunked.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_cpu_information.py` & `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_cpu_information.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_mdns.py` & `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_mdns.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_methods.py` & `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_methods.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_multiple_servers.py` & `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_multiple_servers.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_neopixel.py` & `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_neopixel.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_redirects.py` & `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_redirects.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_simpletest_auto.py` & `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_simpletest_auto.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_simpletest_manual.py` & `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_simpletest_manual.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_start_and_poll.py` & `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_start_and_poll.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_static_files_serving.py` & `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_static_files_serving.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/examples/httpserver_url_parameters.py` & `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_url_parameters.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.1/pyproject.toml` & `adafruit-circuitpython-httpserver-4.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-httpserver"
 description = "Simple HTTP Server for CircuitPython"
-version = "4.0.1"
+version = "4.0.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git"}
 keywords = [
     "adafruit",
@@ -37,12 +37,12 @@
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["adafruit_httpserver"]
+packages = ["adafruit_httpserver"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 optional-dependencies = {optional = {file = ["optional_requirements.txt"]}}
```

