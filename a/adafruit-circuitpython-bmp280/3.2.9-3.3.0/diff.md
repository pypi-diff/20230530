# Comparing `tmp/adafruit-circuitpython-bmp280-3.2.9.tar.gz` & `tmp/adafruit-circuitpython-bmp280-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bmp280-3.2.9.tar", last modified: Mon Nov 15 17:35:17 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-bmp280-3.3.0.tar", last modified: Tue May 30 14:28:00 2023, max compression
```

## Comparing `adafruit-circuitpython-bmp280-3.2.9.tar` & `adafruit-circuitpython-bmp280-3.3.0.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:35:17.072060 adafruit-circuitpython-bmp280-3.2.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:35:17.064060 adafruit-circuitpython-bmp280-3.2.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:35:17.068060 adafruit-circuitpython-bmp280-3.2.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:35:17.068060 adafruit-circuitpython-bmp280-3.2.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:35:17.068060 adafruit-circuitpython-bmp280-3.2.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4170 2021-11-15 17:35:17.072060 adafruit-circuitpython-bmp280-3.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3338 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)    17947 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/adafruit_bmp280.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:35:17.068060 adafruit-circuitpython-bmp280-3.2.9/adafruit_circuitpython_bmp280.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4170 2021-11-15 17:35:16.000000 adafruit-circuitpython-bmp280-3.2.9/adafruit_circuitpython_bmp280.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      918 2021-11-15 17:35:16.000000 adafruit-circuitpython-bmp280-3.2.9/adafruit_circuitpython_bmp280.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 17:35:16.000000 adafruit-circuitpython-bmp280-3.2.9/adafruit_circuitpython_bmp280.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-11-15 17:35:16.000000 adafruit-circuitpython-bmp280-3.2.9/adafruit_circuitpython_bmp280.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-11-15 17:35:16.000000 adafruit-circuitpython-bmp280-3.2.9/adafruit_circuitpython_bmp280.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:35:17.068060 adafruit-circuitpython-bmp280-3.2.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:35:17.068060 adafruit-circuitpython-bmp280-3.2.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5374 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:35:17.072060 adafruit-circuitpython-bmp280-3.2.9/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/examples/bmp280_normal_mode.py
--rw-r--r--   0 runner    (1001) docker     (121)      960 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/examples/bmp280_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-15 17:35:17.072060 adafruit-circuitpython-bmp280-3.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1947 2021-11-15 17:35:03.000000 adafruit-circuitpython-bmp280-3.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:28:00.243821 adafruit-circuitpython-bmp280-3.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:28:00.239821 adafruit-circuitpython-bmp280-3.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:28:00.239821 adafruit-circuitpython-bmp280-3.3.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:28:00.239821 adafruit-circuitpython-bmp280-3.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:28:00.239821 adafruit-circuitpython-bmp280-3.3.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-05-30 14:28:00.243821 adafruit-circuitpython-bmp280-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)    18781 2023-05-30 14:27:52.000000 adafruit-circuitpython-bmp280-3.3.0/adafruit_bmp280.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:28:00.239821 adafruit-circuitpython-bmp280-3.3.0/adafruit_circuitpython_bmp280.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-05-30 14:28:00.000000 adafruit-circuitpython-bmp280-3.3.0/adafruit_circuitpython_bmp280.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-30 14:28:00.000000 adafruit-circuitpython-bmp280-3.3.0/adafruit_circuitpython_bmp280.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:28:00.000000 adafruit-circuitpython-bmp280-3.3.0/adafruit_circuitpython_bmp280.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-30 14:28:00.000000 adafruit-circuitpython-bmp280-3.3.0/adafruit_circuitpython_bmp280.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 14:28:00.000000 adafruit-circuitpython-bmp280-3.3.0/adafruit_circuitpython_bmp280.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:28:00.243821 adafruit-circuitpython-bmp280-3.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:28:00.243821 adafruit-circuitpython-bmp280-3.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:28:00.243821 adafruit-circuitpython-bmp280-3.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-30 14:27:52.000000 adafruit-circuitpython-bmp280-3.3.0/examples/bmp280_normal_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-30 14:27:52.000000 adafruit-circuitpython-bmp280-3.3.0/examples/bmp280_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-30 14:27:52.000000 adafruit-circuitpython-bmp280-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-30 14:27:43.000000 adafruit-circuitpython-bmp280-3.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:28:00.243821 adafruit-circuitpython-bmp280-3.3.0/setup.cfg
```

### Comparing `adafruit-circuitpython-bmp280-3.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-bmp280-3.3.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2021 Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 Thank you for contributing! Before you submit a pull request, please read the following.
 
-Make sure any changes you're submitting are in line with the CircuitPython Design Guide, available here: https://circuitpython.readthedocs.io/en/latest/docs/design_guide.html
+Make sure any changes you're submitting are in line with the CircuitPython Design Guide, available here: https://docs.circuitpython.org/en/latest/docs/design_guide.html
 
 If your changes are to documentation, please verify that the documentation builds locally by following the steps found here: https://adafru.it/build-docs
 
 Before submitting the pull request, make sure you've run Pylint and Black locally on your code. You can do this manually or using pre-commit. Instructions are available here: https://adafru.it/check-your-code
 
 Please remove all of this text before submitting. Include an explanation or list of changes included in your PR, as well as, if applicable, a link to any related issues.
```

### Comparing `adafruit-circuitpython-bmp280-3.2.9/.pre-commit-config.yaml` & `adafruit-circuitpython-bmp280-3.3.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
--   repo: https://github.com/python/black
-    rev: 20.8b1
+  - repo: https://github.com/python/black
+    rev: 23.3.0
     hooks:
-    - id: black
--   repo: https://github.com/fsfe/reuse-tool
-    rev: v0.12.1
+      - id: black
+  - repo: https://github.com/fsfe/reuse-tool
+    rev: v1.1.2
     hooks:
-    - id: reuse
--   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v2.3.0
+      - id: reuse
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.4.0
     hooks:
-    -   id: check-yaml
-    -   id: end-of-file-fixer
-    -   id: trailing-whitespace
--   repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+      - id: check-yaml
+      - id: end-of-file-fixer
+      - id: trailing-whitespace
+  - repo: https://github.com/pycqa/pylint
+    rev: v2.17.4
     hooks:
-    -   id: pylint
+      - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
-    -   id: pylint
+      - id: pylint
         name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
         types: [python]
         files: "^examples/"
         args:
-        - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
-    -   id: pylint
+          - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
+      - id: pylint
         name: pylint (test code)
         description: Run pylint rules on "tests/*.py" files
         types: [python]
         files: "^tests/"
         args:
-        - --disable=missing-docstring,consider-using-f-string,duplicate-code
+          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `adafruit-circuitpython-bmp280-3.2.9/.pylintrc` & `adafruit-circuitpython-bmp280-3.3.0/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
+# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code
 extension-pkg-whitelist=
 
-# Add files or directories to the blacklist. They should be base names, not
+# Add files or directories to the ignore-list. They should be base names, not
 # paths.
 ignore=CVS
 
-# Add files or directories matching the regex patterns to the blacklist. The
+# Add files or directories matching the regex patterns to the ignore-list. The
 # regex matches against base names, not paths.
 ignore-patterns=
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -248,86 +242,58 @@
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
 ignore-imports=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=4
+min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
@@ -429,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-bmp280-3.2.9/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-bmp280-3.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bmp280-3.2.9/LICENSE` & `adafruit-circuitpython-bmp280-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bmp280-3.2.9/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-bmp280-3.3.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bmp280-3.2.9/LICENSES/MIT.txt` & `adafruit-circuitpython-bmp280-3.3.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bmp280-3.2.9/LICENSES/Unlicense.txt` & `adafruit-circuitpython-bmp280-3.3.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bmp280-3.2.9/PKG-INFO` & `adafruit-circuitpython-bmp280-3.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bmp280
-Version: 3.2.9
+Version: 3.3.0
 Summary: CircuitPython driver for the BMP280.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BMP280
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit bmp280 barometric pressure temperature hardware sensor micropython circuitpython
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BMP280
+Keywords: adafruit,bmp280,barometric,pressure,temperature,hardware,sensor,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-bmp280/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/bmp280/en/latest/
+    :target: https://docs.circuitpython.org/projects/bmp280/en/latest/
     :alt: Documentation Status
 
-.. image :: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BMP280/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_BMP280/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 CircuitPython driver from BMP280 Temperature and Barometic Pressure sensor
 
 Installation and Dependencies
 =============================
 
 This driver depends on:
 
@@ -66,16 +67,16 @@
     sudo pip3 install adafruit-circuitpython-bmp280
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-bmp280
 
 Usage Example
 =============
 
 .. code-block:: python
 
@@ -101,23 +102,17 @@
         print("Pressure: %0.1f hPa" % bmp280.pressure)
         print("Altitude = %0.2f meters" % bmp280.altitude)
         time.sleep(2)
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/bmp280/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/bmp280/en/latest/>`_.
+
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_bmp280/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.Travis will. This is a good way to
-locally verify it will pass.
-
-
```

### Comparing `adafruit-circuitpython-bmp280-3.2.9/README.rst` & `adafruit-circuitpython-bmp280-3.3.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-bmp280/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/bmp280/en/latest/
+    :target: https://docs.circuitpython.org/projects/bmp280/en/latest/
     :alt: Documentation Status
 
-.. image :: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BMP280/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_BMP280/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 CircuitPython driver from BMP280 Temperature and Barometic Pressure sensor
 
 Installation and Dependencies
 =============================
 
 This driver depends on:
 
@@ -45,16 +49,16 @@
     sudo pip3 install adafruit-circuitpython-bmp280
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-bmp280
 
 Usage Example
 =============
 
 .. code-block:: python
 
@@ -80,21 +84,17 @@
         print("Pressure: %0.1f hPa" % bmp280.pressure)
         print("Altitude = %0.2f meters" % bmp280.altitude)
         time.sleep(2)
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/bmp280/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/bmp280/en/latest/>`_.
+
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_bmp280/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.Travis will. This is a good way to
-locally verify it will pass.
```

### Comparing `adafruit-circuitpython-bmp280-3.2.9/adafruit_bmp280.py` & `adafruit-circuitpython-bmp280-3.3.0/adafruit_bmp280.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # SPDX-FileCopyrightText: 2017 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
+# SPDX-FileCopyrightText: 2022 Bill Van Leeuwen for Adafruit Industries
+#
+# SPDX-License-Identifier: MIT
+
 """
 `adafruit_bmp280`
 ===============================================================================
 
 CircuitPython driver from BMP280 Temperature and Barometric Pressure sensor
 
 * Author(s): ladyada
@@ -21,23 +25,31 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 """
 import math
+import struct
 from time import sleep
 
+from micropython import const
+
+
 try:
-    import struct
+    from typing import Optional
+
+    # Used only for type annotations.
+    from busio import SPI, I2C
+    from digitalio import DigitalInOut
+
 except ImportError:
-    import ustruct as struct
-from micropython import const
+    pass
 
-__version__ = "0.0.0-auto.0"
+__version__ = "3.3.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BMP280.git"
 
 #    I2C ADDRESS/BITS/SETTINGS
 #    -----------------------------------------------------------------------
 _CHIP_ID = const(0x58)
 
 _REGISTER_CHIPID = const(0xD0)
@@ -120,15 +132,15 @@
 
     .. note::
         The operational range of the BMP280 is 300-1100 hPa.
         Pressure measurements outside this range may not be as accurate.
 
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         # Check device ID.
         chip_id = self._read_byte(_REGISTER_CHIPID)
         if _CHIP_ID != chip_id:
             raise RuntimeError("Failed to find BMP280! Chip ID 0x%x" % chip_id)
         # Set some reasonable defaults.
         self._iir_filter = IIR_FILTER_DISABLE
         self._overscan_temperature = OVERSCAN_X2
@@ -139,15 +151,15 @@
         self._read_coefficients()
         self._write_ctrl_meas()
         self._write_config()
         self.sea_level_pressure = 1013.25
         """Pressure in hectoPascals at sea level. Used to calibrate `altitude`."""
         self._t_fine = None
 
-    def _read_temperature(self):
+    def _read_temperature(self) -> None:
         # perform one measurement
         if self.mode != MODE_NORMAL:
             self.mode = MODE_FORCE
             # Wait for conversion to complete
             while self._get_status() & 0x08:
                 sleep(0.002)
         raw_temperature = (
@@ -163,168 +175,168 @@
             * (raw_temperature / 131072.0 - self._temp_calib[0] / 8192.0)
         ) * self._temp_calib[2]
         # print(var2)
 
         self._t_fine = int(var1 + var2)
         # print("t_fine: ", self.t_fine)
 
-    def _reset(self):
+    def _reset(self) -> None:
         """Soft reset the sensor"""
         self._write_register_byte(_REGISTER_SOFTRESET, 0xB6)
         sleep(0.004)  # Datasheet says 2ms.  Using 4ms just to be safe
 
-    def _write_ctrl_meas(self):
+    def _write_ctrl_meas(self) -> None:
         """
         Write the values to the ctrl_meas register in the device
         ctrl_meas sets the pressure and temperature data acquisition options
         """
         self._write_register_byte(_REGISTER_CTRL_MEAS, self._ctrl_meas)
 
-    def _get_status(self):
-        """Get the value from the status register in the device """
+    def _get_status(self) -> int:
+        """Get the value from the status register in the device"""
         return self._read_byte(_REGISTER_STATUS)
 
-    def _read_config(self):
-        """Read the value from the config register in the device """
+    def _read_config(self) -> int:
+        """Read the value from the config register in the device"""
         return self._read_byte(_REGISTER_CONFIG)
 
-    def _write_config(self):
-        """Write the value to the config register in the device """
+    def _write_config(self) -> None:
+        """Write the value to the config register in the device"""
         normal_flag = False
         if self._mode == MODE_NORMAL:
             # Writes to the config register may be ignored while in Normal mode
             normal_flag = True
             self.mode = MODE_SLEEP  # So we switch to Sleep mode first
         self._write_register_byte(_REGISTER_CONFIG, self._config)
         if normal_flag:
             self.mode = MODE_NORMAL
 
     @property
-    def mode(self):
+    def mode(self) -> int:
         """
         Operation mode
         Allowed values are set in the MODE enum class
         """
         return self._mode
 
     @mode.setter
-    def mode(self, value):
+    def mode(self, value: int) -> None:
         if not value in _BMP280_MODES:
             raise ValueError("Mode '%s' not supported" % (value))
         self._mode = value
         self._write_ctrl_meas()
 
     @property
-    def standby_period(self):
+    def standby_period(self) -> int:
         """
         Control the inactive period when in Normal mode
         Allowed standby periods are set the STANDBY enum class
         """
         return self._t_standby
 
     @standby_period.setter
-    def standby_period(self, value):
+    def standby_period(self, value: int) -> None:
         if not value in _BMP280_STANDBY_TCS:
             raise ValueError("Standby Period '%s' not supported" % (value))
         if self._t_standby == value:
             return
         self._t_standby = value
         self._write_config()
 
     @property
-    def overscan_temperature(self):
+    def overscan_temperature(self) -> int:
         """
         Temperature Oversampling
         Allowed values are set in the OVERSCAN enum class
         """
         return self._overscan_temperature
 
     @overscan_temperature.setter
-    def overscan_temperature(self, value):
+    def overscan_temperature(self, value: int) -> None:
         if not value in _BMP280_OVERSCANS:
             raise ValueError("Overscan value '%s' not supported" % (value))
         self._overscan_temperature = value
         self._write_ctrl_meas()
 
     @property
-    def overscan_pressure(self):
+    def overscan_pressure(self) -> int:
         """
         Pressure Oversampling
         Allowed values are set in the OVERSCAN enum class
         """
         return self._overscan_pressure
 
     @overscan_pressure.setter
-    def overscan_pressure(self, value):
+    def overscan_pressure(self, value: int) -> None:
         if not value in _BMP280_OVERSCANS:
             raise ValueError("Overscan value '%s' not supported" % (value))
         self._overscan_pressure = value
         self._write_ctrl_meas()
 
     @property
-    def iir_filter(self):
+    def iir_filter(self) -> int:
         """
         Controls the time constant of the IIR filter
         Allowed values are set in the IIR_FILTER enum class
         """
         return self._iir_filter
 
     @iir_filter.setter
-    def iir_filter(self, value):
+    def iir_filter(self, value: int) -> None:
         if not value in _BMP280_IIR_FILTERS:
             raise ValueError("IIR Filter '%s' not supported" % (value))
         self._iir_filter = value
         self._write_config()
 
     @property
-    def _config(self):
-        """Value to be written to the device's config register """
+    def _config(self) -> int:
+        """Value to be written to the device's config register"""
         config = 0
         if self.mode == MODE_NORMAL:
             config += self._t_standby << 5
         if self._iir_filter:
             config += self._iir_filter << 2
         return config
 
     @property
-    def _ctrl_meas(self):
-        """Value to be written to the device's ctrl_meas register """
+    def _ctrl_meas(self) -> int:
+        """Value to be written to the device's ctrl_meas register"""
         ctrl_meas = self.overscan_temperature << 5
         ctrl_meas += self.overscan_pressure << 2
         ctrl_meas += self.mode
         return ctrl_meas
 
     @property
-    def measurement_time_typical(self):
+    def measurement_time_typical(self) -> float:
         """Typical time in milliseconds required to complete a measurement in normal mode"""
         meas_time_ms = 1
         if self.overscan_temperature != OVERSCAN_DISABLE:
             meas_time_ms += 2 * _BMP280_OVERSCANS.get(self.overscan_temperature)
         if self.overscan_pressure != OVERSCAN_DISABLE:
             meas_time_ms += 2 * _BMP280_OVERSCANS.get(self.overscan_pressure) + 0.5
         return meas_time_ms
 
     @property
-    def measurement_time_max(self):
+    def measurement_time_max(self) -> float:
         """Maximum time in milliseconds required to complete a measurement in normal mode"""
         meas_time_ms = 1.25
         if self.overscan_temperature != OVERSCAN_DISABLE:
             meas_time_ms += 2.3 * _BMP280_OVERSCANS.get(self.overscan_temperature)
         if self.overscan_pressure != OVERSCAN_DISABLE:
             meas_time_ms += 2.3 * _BMP280_OVERSCANS.get(self.overscan_pressure) + 0.575
         return meas_time_ms
 
     @property
-    def temperature(self):
+    def temperature(self) -> float:
         """The compensated temperature in degrees Celsius."""
         self._read_temperature()
         return self._t_fine / 5120.0
 
     @property
-    def pressure(self):
+    def pressure(self) -> Optional[float]:
         """
         The compensated pressure in hectoPascals.
         returns `None` if pressure measurement is disabled
         """
         self._read_temperature()
 
         # Algorithm from the BMP280 driver
@@ -347,22 +359,27 @@
         var2 = pressure * self._pressure_calib[7] / 32768.0
         pressure = pressure + (var1 + var2 + self._pressure_calib[6]) / 16.0
         pressure /= 100
 
         return pressure
 
     @property
-    def altitude(self):
+    def altitude(self) -> float:
         """The altitude based on the sea level pressure (:attr:`sea_level_pressure`)
         - which you must enter ahead of time)"""
         p = self.pressure  # in Si units for hPascal
         return 44330 * (1.0 - math.pow(p / self.sea_level_pressure, 0.1903))
 
+    @altitude.setter
+    def altitude(self, value: float) -> None:
+        p = self.pressure  # in Si units for hPascal
+        self.sea_level_pressure = p / math.pow(1.0 - value / 44330.0, 5.255)
+
     ####################### Internal helpers ################################
-    def _read_coefficients(self):
+    def _read_coefficients(self) -> None:
         """Read & save the calibration coefficients"""
         coeff = self._read_register(_REGISTER_DIG_T1, 24)
         coeff = list(struct.unpack("<HhhHhhhhhhhh", bytes(coeff)))
         coeff = [float(i) for i in coeff]
         # The temp_calib lines up with DIG_T# registers.
         self._temp_calib = coeff[:3]
         self._pressure_calib = coeff[3:]
@@ -370,31 +387,31 @@
         # print("%d %d %d" % (self._pressure_calib[0], self._pressure_calib[1],
         #                     self._pressure_calib[2]))
         # print("%d %d %d" % (self._pressure_calib[3], self._pressure_calib[4],
         #                     self._pressure_calib[5]))
         # print("%d %d %d" % (self._pressure_calib[6], self._pressure_calib[7],
         #                     self._pressure_calib[8]))
 
-    def _read_byte(self, register):
+    def _read_byte(self, register: int) -> int:
         """Read a byte register value and return it"""
         return self._read_register(register, 1)[0]
 
-    def _read24(self, register):
+    def _read24(self, register: int) -> float:
         """Read an unsigned 24-bit value as a floating point and return it."""
         ret = 0.0
         for b in self._read_register(register, 3):
             ret *= 256.0
             ret += float(b & 0xFF)
         return ret
 
-    def _read_register(self, register, length):
+    def _read_register(self, register: int, length: int) -> None:
         """Low level register reading, not implemented in base class"""
         raise NotImplementedError()
 
-    def _write_register_byte(self, register, value):
+    def _write_register_byte(self, register: int, value: int) -> None:
         """Low level register writing, not implemented in base class"""
         raise NotImplementedError()
 
 
 class Adafruit_BMP280_I2C(Adafruit_BMP280):  # pylint: disable=invalid-name
     """Driver for I2C connected BMP280.
 
@@ -432,32 +449,32 @@
 
             temperature = bmp280.temperature
             pressure = bmp280.pressure
             altitude = bmp280.altitude
 
     """
 
-    def __init__(self, i2c, address=0x77):
+    def __init__(self, i2c: I2C, address: int = 0x77) -> None:
         from adafruit_bus_device import (  # pylint: disable=import-outside-toplevel
             i2c_device,
         )
 
         self._i2c = i2c_device.I2CDevice(i2c, address)
         super().__init__()
 
-    def _read_register(self, register, length):
+    def _read_register(self, register: int, length: int) -> bytearray:
         """Low level register reading over I2C, returns a list of values"""
         with self._i2c as i2c:
             i2c.write(bytes([register & 0xFF]))
             result = bytearray(length)
             i2c.readinto(result)
             # print("$%02X => %s" % (register, [hex(i) for i in result]))
             return result
 
-    def _write_register_byte(self, register, value):
+    def _write_register_byte(self, register: int, value: int) -> None:
         """Low level register writing over I2C, writes one 8-bit value"""
         with self._i2c as i2c:
             i2c.write(bytes([register & 0xFF, value & 0xFF]))
             # print("$%02X <= 0x%02X" % (register, value))
 
 
 class Adafruit_BMP280_SPI(Adafruit_BMP280):
@@ -501,32 +518,32 @@
 
             temperature = bmp280.temperature
             pressure = bmp280.pressure
             altitude = bmp280.altitude
 
     """
 
-    def __init__(self, spi, cs, baudrate=100000):
+    def __init__(self, spi: SPI, cs: DigitalInOut, baudrate=100000) -> None:
         from adafruit_bus_device import (  # pylint: disable=import-outside-toplevel
             spi_device,
         )
 
         self._spi = spi_device.SPIDevice(spi, cs, baudrate=baudrate)
         super().__init__()
 
-    def _read_register(self, register, length):
+    def _read_register(self, register: int, length: int) -> bytearray:
         """Low level register reading over SPI, returns a list of values"""
         register = (register | 0x80) & 0xFF  # Read single, bit 7 high.
         with self._spi as spi:
             # pylint: disable=no-member
             spi.write(bytearray([register]))
             result = bytearray(length)
             spi.readinto(result)
             # print("$%02X => %s" % (register, [hex(i) for i in result]))
             return result
 
-    def _write_register_byte(self, register, value):
+    def _write_register_byte(self, register: int, value: int) -> None:
         """Low level register writing over SPI, writes one 8-bit value"""
         register &= 0x7F  # Write, bit 7 low.
         with self._spi as spi:
             # pylint: disable=no-member
             spi.write(bytes([register, value & 0xFF]))
```

### Comparing `adafruit-circuitpython-bmp280-3.2.9/adafruit_circuitpython_bmp280.egg-info/PKG-INFO` & `adafruit-circuitpython-bmp280-3.3.0/adafruit_circuitpython_bmp280.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bmp280
-Version: 3.2.9
+Version: 3.3.0
 Summary: CircuitPython driver for the BMP280.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BMP280
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit bmp280 barometric pressure temperature hardware sensor micropython circuitpython
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BMP280
+Keywords: adafruit,bmp280,barometric,pressure,temperature,hardware,sensor,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-bmp280/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/bmp280/en/latest/
+    :target: https://docs.circuitpython.org/projects/bmp280/en/latest/
     :alt: Documentation Status
 
-.. image :: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BMP280/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_BMP280/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 CircuitPython driver from BMP280 Temperature and Barometic Pressure sensor
 
 Installation and Dependencies
 =============================
 
 This driver depends on:
 
@@ -66,16 +67,16 @@
     sudo pip3 install adafruit-circuitpython-bmp280
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-bmp280
 
 Usage Example
 =============
 
 .. code-block:: python
 
@@ -101,23 +102,17 @@
         print("Pressure: %0.1f hPa" % bmp280.pressure)
         print("Altitude = %0.2f meters" % bmp280.altitude)
         time.sleep(2)
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/bmp280/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/bmp280/en/latest/>`_.
+
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_bmp280/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.Travis will. This is a good way to
-locally verify it will pass.
-
-
```

### Comparing `adafruit-circuitpython-bmp280-3.2.9/adafruit_circuitpython_bmp280.egg-info/SOURCES.txt` & `adafruit-circuitpython-bmp280-3.3.0/adafruit_circuitpython_bmp280.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 adafruit_bmp280.py
+optional_requirements.txt
+pyproject.toml
 requirements.txt
-setup.py
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_bmp280.egg-info/PKG-INFO
 adafruit_circuitpython_bmp280.egg-info/SOURCES.txt
 adafruit_circuitpython_bmp280.egg-info/dependency_links.txt
 adafruit_circuitpython_bmp280.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-bmp280-3.2.9/docs/_static/favicon.ico` & `adafruit-circuitpython-bmp280-3.3.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bmp280-3.2.9/docs/conf.py` & `adafruit-circuitpython-bmp280-3.3.0/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,52 +2,61 @@
 
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
 ]
 
 intersphinx_mapping = {
-    "python": ("https://docs.python.org/3.4", None),
+    "python": ("https://docs.python.org/3", None),
     "BusDevice": (
-        "https://circuitpython.readthedocs.io/projects/busdevice/en/latest/",
+        "https://docs.circuitpython.org/projects/busdevice/en/latest/",
         None,
     ),
     "Register": (
-        "https://circuitpython.readthedocs.io/projects/register/en/latest/",
+        "https://docs.circuitpython.org/projects/register/en/latest/",
         None,
     ),
-    "CircuitPython": ("https://circuitpython.readthedocs.io/en/latest/", None),
+    "CircuitPython": ("https://docs.circuitpython.org/en/latest/", None),
 }
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit BMP280 Library"
-copyright = "2017 ladyada"
+creation_year = "2017"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " ladyada"
 author = "ladyada"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
@@ -56,15 +65,15 @@
 release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".env", "CODE_OF_CONDUCT.md"]
 
 # The reST default role (used for this markup: `text`) to use for all
```

### Comparing `adafruit-circuitpython-bmp280-3.2.9/docs/index.rst` & `adafruit-circuitpython-bmp280-3.3.0/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,17 @@
     :caption: Related Products
 
     Adafruit BMP280 I2C or SPI Barometric Pressure & Altitude Sensor  <https://www.adafruit.com/product/2651>
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/Adafruit_CircuitPython_BMP280/releases/latest>
-    CircuitPython Reference Documentation <https://circuitpython.readthedocs.io>
+    Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_BMP280/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
+    CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
 
 Indices and tables
```

### Comparing `adafruit-circuitpython-bmp280-3.2.9/examples/bmp280_normal_mode.py` & `adafruit-circuitpython-bmp280-3.3.0/examples/bmp280_normal_mode.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 """
 import time
 import board
 import adafruit_bmp280
 
 # Create sensor object, communicating over the board's default I2C bus
 i2c = board.I2C()  # uses board.SCL and board.SDA
+# i2c = board.STEMMA_I2C()  # For using the built-in STEMMA QT connector on a microcontroller
 bmp280 = adafruit_bmp280.Adafruit_BMP280_I2C(i2c)
 
 # OR Create sensor object, communicating over the board's default SPI bus
 # spi = busio.SPI()
 # bmp_cs = digitalio.DigitalInOut(board.D10)
 # bmp280 = adafruit_bmp280.Adafruit_BMP280_SPI(spi, bmp_cs)
```

### Comparing `adafruit-circuitpython-bmp280-3.2.9/examples/bmp280_simpletest.py` & `adafruit-circuitpython-bmp280-3.3.0/examples/bmp280_simpletest.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import board
 
 # import digitalio # For use with SPI
 import adafruit_bmp280
 
 # Create sensor object, communicating over the board's default I2C bus
 i2c = board.I2C()  # uses board.SCL and board.SDA
+# i2c = board.STEMMA_I2C()  # For using the built-in STEMMA QT connector on a microcontroller
 bmp280 = adafruit_bmp280.Adafruit_BMP280_I2C(i2c)
 
 # OR Create sensor object, communicating over the board's default SPI bus
 # spi = board.SPI()
 # bmp_cs = digitalio.DigitalInOut(board.D10)
 # bmp280 = adafruit_bmp280.Adafruit_BMP280_SPI(spi, bmp_cs)
```

