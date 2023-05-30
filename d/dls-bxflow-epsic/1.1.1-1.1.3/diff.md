# Comparing `tmp/dls-bxflow-epsic-1.1.1.tar.gz` & `tmp/dls-bxflow-epsic-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-bxflow-epsic-1.1.1.tar", last modified: Mon May 29 17:00:59 2023, max compression
+gzip compressed data, was "dls-bxflow-epsic-1.1.3.tar", last modified: Tue May 30 04:46:05 2023, max compression
```

## Comparing `dls-bxflow-epsic-1.1.1.tar` & `dls-bxflow-epsic-1.1.3.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.195572 dls-bxflow-epsic-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.187572 dls-bxflow-epsic-1.1.1/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.187572 dls-bxflow-epsic-1.1.1/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/docs/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.187572 dls-bxflow-epsic-1.1.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.187572 dls-bxflow-epsic-1.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.183571 dls-bxflow-epsic-1.1.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.187572 dls-bxflow-epsic-1.1.1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/Makefile-conda
--rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-05-29 17:00:59.195572 dls-bxflow-epsic-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.187572 dls-bxflow-epsic-1.1.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/docs/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/explanations/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/explanations/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/explanations/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/explanations/todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/how-to/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/how-to/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/how-to/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/how-to/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/how-to/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/how-to/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/reference/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/reference/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/reference/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:00:59.195572 dls-bxflow-epsic-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.187572 dls-bxflow-epsic-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.195572 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 17:00:59.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.195572 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/algorithms/mib_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.195572 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/collectors/mib_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/epsic_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/epsic_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.195572 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-05-29 17:00:59.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-29 17:00:59.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:00:59.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-29 17:00:59.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-29 17:00:59.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-29 17:00:59.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.195572 dls-bxflow-epsic-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/tests/base_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/tests/test_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.810609 dls-bxflow-epsic-1.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.798609 dls-bxflow-epsic-1.1.3/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/Makefile-conda
+-rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.798609 dls-bxflow-epsic-1.1.3/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.802609 dls-bxflow-epsic-1.1.3/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 04:46:05.810609 dls-bxflow-epsic-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.798609 dls-bxflow-epsic-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 04:46:05.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/algorithms/mib_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/collectors/mib_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/epsic_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/epsic_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-05-30 04:46:05.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-30 04:46:05.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 04:46:05.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-30 04:46:05.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-30 04:46:05.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 04:46:05.000000 dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:46:05.806609 dls-bxflow-epsic-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/tests/base_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-30 04:45:56.000000 dls-bxflow-epsic-1.1.3/tests/test_stub.py
```

### Comparing `dls-bxflow-epsic-1.1.1/.dae-devops/Makefile` & `dls-bxflow-epsic-1.1.3/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/.dae-devops/docs/conventions.rst` & `dls-bxflow-epsic-1.1.3/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/.dae-devops/docs/developing.rst` & `dls-bxflow-epsic-1.1.3/.dae-devops/docs/developing.rst`

 * *Files 15% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 Clone the repository::
 
     $ cd <your development area>
     $ git clone https://github.com/DiamondLightSource/dls-bxflow-epsic.git
 
 It is recommended that you install into a virtual environment so this
 installation will not interfere with any existing Python software.
-Make sure to have at least python version 3.9 then::
+Make sure to have at least python version >=3.10 then::
 
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 Install the package in edit mode which will also install all its dependencies::
 
     $ cd dls-bxflow-epsic
     $ pip install -e .[dev,docs]
 
 Now you may begin modifying the code.
 
 
-.. # dae_devops_fingerprint 7826bc083f17254f3dd7ee314d804d35
+.. # dae_devops_fingerprint 541a732e9b67fb4322c7d4286330894f
```

### Comparing `dls-bxflow-epsic-1.1.1/.dae-devops/docs/devops.rst` & `dls-bxflow-epsic-1.1.3/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/.dae-devops/docs/docs_structure.rst` & `dls-bxflow-epsic-1.1.3/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/.dae-devops/docs/documenting.rst` & `dls-bxflow-epsic-1.1.3/.dae-devops/docs/documenting.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/.dae-devops/docs/installing.rst` & `dls-bxflow-epsic-1.1.3/.dae-devops/docs/installing.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 .. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-bxflow-epsic
 
 Installing
 =======================================================================
 
 
-You will need python 3.9 or later. 
+You will need python >=3.10 or later. 
 
-On a Diamond Light Source internal computer, you can achieve Python 3.9 by::
+On a Diamond Light Source internal computer, you can achieve Python >=3.10 by::
 
-    $ module load python/3.9
+    $ module load python/>=3.10
 
 You can check your version of python by typing into a terminal::
 
     $ python3 --version
 
 It is recommended that you install into a virtual environment so this
 installation will not interfere with any existing Python software::
@@ -35,8 +35,8 @@
 
 The package should now be installed and the command line should be available.
 You can check the version that has been installed by typing::
 
     $ dls-bxflow-epsic --version
     $ dls-bxflow-epsic --version-json
 
-.. # dae_devops_fingerprint 48af32ed4de39d505677bee06a605da4
+.. # dae_devops_fingerprint 2536adcdc877e553821264097f0af330
```

### Comparing `dls-bxflow-epsic-1.1.1/.dae-devops/docs/testing.rst` & `dls-bxflow-epsic-1.1.3/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/.devcontainer/Dockerfile` & `dls-bxflow-epsic-1.1.3/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/.devcontainer/devcontainer.json` & `dls-bxflow-epsic-1.1.3/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/.github/CONTRIBUTING.rst` & `dls-bxflow-epsic-1.1.3/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/.github/actions/install_requirements/action.yml` & `dls-bxflow-epsic-1.1.3/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/.github/dependabot.yml` & `dls-bxflow-epsic-1.1.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/.github/pages/index.html` & `dls-bxflow-epsic-1.1.3/.github/pages/index.html`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/.github/pages/make_switcher.py` & `dls-bxflow-epsic-1.1.3/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/.github/workflows/code.yml` & `dls-bxflow-epsic-1.1.3/.github/workflows/code.yml`

 * *Files 2% similar despite different names*

```diff
@@ -37,19 +37,14 @@
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest"] # can add windows-latest, macos-latest
         python: ["3.10"]
         install: ["-e .[dev,docs]"]
-        # Make one version be non-editable to test both paths of version code
-        include:
-          - os: "ubuntu-latest"
-            python: "3.9"
-            install: ".[dev,docs]"
 
     runs-on: ${{ matrix.os }}
     env:
       # https://github.com/pytest-dev/pytest/issues/2042
       PY_IGNORE_IMPORTMISMATCH: "1"
 
     steps:
@@ -212,8 +207,8 @@
 
       - name: Publish to PyPI
         if: ${{ env.HAS_PYPI_TOKEN }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_TOKEN }}
 
-# dae_devops_fingerprint 10ebf277e974272f2bc4b2ee40a5f388
+# dae_devops_fingerprint 89e4c11d17b951574201c67b84c67efd
```

### Comparing `dls-bxflow-epsic-1.1.1/.github/workflows/docs.yml` & `dls-bxflow-epsic-1.1.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/.github/workflows/docs_clean.yml` & `dls-bxflow-epsic-1.1.3/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/.github/workflows/linkcheck.yml` & `dls-bxflow-epsic-1.1.3/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/.gitignore` & `dls-bxflow-epsic-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/.gitlab-ci.yml` & `dls-bxflow-epsic-1.1.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/.vscode/launch.json` & `dls-bxflow-epsic-1.1.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/LICENSE` & `dls-bxflow-epsic-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/Makefile` & `dls-bxflow-epsic-1.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/Makefile-conda` & `dls-bxflow-epsic-1.1.3/Makefile-conda`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/PKG-INFO` & `dls-bxflow-epsic-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-bxflow-epsic
-Version: 1.1.1
+Version: 1.1.3
 Summary: Bxflow beamline code for ePSIC.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,28 +204,25 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: github, https://github.com/DiamondLightSource/dls-bxflow-epsic
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 dls-bxflow-epsic
 =======================================================================
 
-Bxflow beamline library for B24.
+Bxflow beamline library for ePSIC.
 
 Wraps core science algorithms as runnable tasks for workflow execution.
 
 Also implements the filesystem naming conventions at the beamline.
 
-..
-    Anything below this line is used when viewing README.rst and will be replaced
-    when included in index.rst
+For documentation see: https://diamondlightsource.github.io/dls-bxflow-epsic
```

### Comparing `dls-bxflow-epsic-1.1.1/docs/conf.py` & `dls-bxflow-epsic-1.1.3/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,17 +184,17 @@
 
 # I got this from https://github.com/sphinx-doc/sphinx/issues/4054.
 # It will allow the ${token} replacement in the rst documents.
 ultimate_replacements = {
     "$" + "{repository_name}": "dls-bxflow-epsic",
     "$" + "{package_name}": "dls_bxflow_epsic",
     "$" + "{git_url}": "https://github.com/DiamondLightSource",
-    "$" + "{python_version_at_least}": "3.9",
+    "$" + "{python_version_at_least}": ">=3.10",
 }
 
 
 def setup(app):
     app.add_config_value("ultimate_replacements", {}, True)
     app.connect("source-read", ultimateReplace)
 
 
-# dae_devops_fingerprint 771750311240a1d0e5a5ff2021d97ae7
+# dae_devops_fingerprint 3f4594f6f175a8e6f58718c177489f82
```

### Comparing `dls-bxflow-epsic-1.1.1/docs/images/dls-favicon.ico` & `dls-bxflow-epsic-1.1.3/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/docs/images/dls-logo.svg` & `dls-bxflow-epsic-1.1.3/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/docs/reference/classes.rst` & `dls-bxflow-epsic-1.1.3/docs/reference/classes.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/pyproject.toml` & `dls-bxflow-epsic-1.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,24 +7,23 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dls-bxflow-epsic"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 description = "Bxflow beamline code for ePSIC."
 dependencies = ["dls-bxflow"]
 dynamic = ["version"]
 license.file = "LICENSE"
-readme = "README.rst"
-requires-python = ">=3.9"
+readme = "README.md"
+requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = [
     "black==22.12.0",
     "mypy",
     "flake8-isort",
     "Flake8-pyproject",
@@ -98,8 +97,8 @@
 source = ["src", "**/site-packages/"]
 
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = "[tox]\nskipsdist=True\n\n[testenv:{pre-commit,mypy,pytest,docs}]\n# Don't create a virtualenv for the command, requires tox-direct plugin\ndirect = True\npassenv = *\nallowlist_externals = \n    pytest \n    pre-commit\n    mypy\n    sphinx-build\n    sphinx-autobuild\ncommands =\n    pytest: pytest {posargs}\n    mypy: mypy src tests {posargs}\n    pre-commit: pre-commit run --all-files {posargs}\n    docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html\n"
 
-# dae_devops_fingerprint 672bc5399adbec5a8ff773c50f9fcffd
+# dae_devops_fingerprint eac5c6537034a1e55824d3b38d41e7e3
```

### Comparing `dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/__main__.py` & `dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/algorithms/mib_converter.py` & `dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/algorithms/mib_converter.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/collectors/mib_scraper.py` & `dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/collectors/mib_scraper.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/epsic_main.py` & `dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/epsic_main.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/epsic_workflow.py` & `dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/epsic_workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/utilities.py` & `dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/utilities.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/version.py` & `dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic/version.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic.egg-info/PKG-INFO` & `dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-bxflow-epsic
-Version: 1.1.1
+Version: 1.1.3
 Summary: Bxflow beamline code for ePSIC.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,28 +204,25 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: github, https://github.com/DiamondLightSource/dls-bxflow-epsic
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 dls-bxflow-epsic
 =======================================================================
 
-Bxflow beamline library for B24.
+Bxflow beamline library for ePSIC.
 
 Wraps core science algorithms as runnable tasks for workflow execution.
 
 Also implements the filesystem naming conventions at the beamline.
 
-..
-    Anything below this line is used when viewing README.rst and will be replaced
-    when included in index.rst
+For documentation see: https://diamondlightsource.github.io/dls-bxflow-epsic
```

### Comparing `dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic.egg-info/SOURCES.txt` & `dls-bxflow-epsic-1.1.3/src/dls_bxflow_epsic.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .gitignore
 .gitlab-ci.yml
 .pre-commit-config.yaml
 LICENSE
 Makefile
 Makefile-conda
-README.rst
+README.md
 pyproject.toml
 .dae-devops/Makefile
 .dae-devops/prepare_git_dependencies.sh
 .dae-devops/project.yaml
 .dae-devops/docs/conventions.rst
 .dae-devops/docs/developing.rst
 .dae-devops/docs/devops.rst
```

### Comparing `dls-bxflow-epsic-1.1.1/tests/base_tester.py` & `dls-bxflow-epsic-1.1.3/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/tests/conftest.py` & `dls-bxflow-epsic-1.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.1/tests/test_stub.py` & `dls-bxflow-epsic-1.1.3/tests/test_stub.py`

 * *Files identical despite different names*

