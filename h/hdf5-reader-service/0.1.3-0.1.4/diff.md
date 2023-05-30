# Comparing `tmp/hdf5-reader-service-0.1.3.tar.gz` & `tmp/hdf5-reader-service-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdf5-reader-service-0.1.3.tar", last modified: Tue May 30 10:49:04 2023, max compression
+gzip compressed data, was "hdf5-reader-service-0.1.4.tar", last modified: Tue May 30 12:10:03 2023, max compression
```

## Comparing `hdf5-reader-service-0.1.3.tar` & `hdf5-reader-service-0.1.4.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.568940 hdf5-reader-service-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.548939 hdf5-reader-service-0.1.3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.548939 hdf5-reader-service-0.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.544939 hdf5-reader-service-0.1.3/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.548939 hdf5-reader-service-0.1.3/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.548939 hdf5-reader-service-0.1.3/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.548939 hdf5-reader-service-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.548939 hdf5-reader-service-0.1.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15608 2023-05-30 10:49:04.568940 hdf5-reader-service-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.548939 hdf5-reader-service-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.548939 hdf5-reader-service-0.1.3/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.548939 hdf5-reader-service-0.1.3/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.548939 hdf5-reader-service-0.1.3/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/developer/explanations/decisions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.552940 hdf5-reader-service-0.1.3/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.552940 hdf5-reader-service-0.1.3/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.552940 hdf5-reader-service-0.1.3/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.552940 hdf5-reader-service-0.1.3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.552940 hdf5-reader-service-0.1.3/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.552940 hdf5-reader-service-0.1.3/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/user/explanations/docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.552940 hdf5-reader-service-0.1.3/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.552940 hdf5-reader-service-0.1.3/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.552940 hdf5-reader-service-0.1.3/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/docs/user/tutorials/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:49:04.568940 hdf5-reader-service-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.548939 hdf5-reader-service-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.556940 hdf5-reader-service-0.1.3/src/hdf5_reader_service/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service/__init__ copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 10:49:04.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service/_version_git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service/fork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.556940 hdf5-reader-service-0.1.3/src/hdf5_reader_service/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service/tasks/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service/tasks/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service/tasks/shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service/tasks/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service/tasks/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.556940 hdf5-reader-service-0.1.3/src/hdf5_reader_service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15608 2023-05-30 10:49:04.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-30 10:49:04.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:49:04.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-30 10:49:04.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-30 10:49:04.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 10:49:04.000000 hdf5-reader-service-0.1.3/src/hdf5_reader_service.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.560940 hdf5-reader-service-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.560940 hdf5-reader-service-0.1.3/tests/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/tests/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/tests/tasks/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/tests/tasks/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/tests/tasks/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/tests/tasks/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/tests/tasks/test_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.560940 hdf5-reader-service-0.1.3/tests/test-data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:49:04.560940 hdf5-reader-service-0.1.3/tests/test-data/p45-104/
--rw-r--r--   0 runner    (1001) docker     (123)  7704118 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/tests/test-data/p45-104/p45-104-DIFFRACTION.h5
--rw-r--r--   0 runner    (1001) docker     (123)    55178 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/tests/test-data/p45-104.nxs
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/tests/test_boilerplate_removed copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/tests/test_boilerplate_removed.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-05-30 10:48:54.000000 hdf5-reader-service-0.1.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.145065 hdf5-reader-service-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.113065 hdf5-reader-service-0.1.4/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.113065 hdf5-reader-service-0.1.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.105065 hdf5-reader-service-0.1.4/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.113065 hdf5-reader-service-0.1.4/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.113065 hdf5-reader-service-0.1.4/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.117065 hdf5-reader-service-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.117065 hdf5-reader-service-0.1.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15608 2023-05-30 12:10:03.145065 hdf5-reader-service-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.117065 hdf5-reader-service-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.117065 hdf5-reader-service-0.1.4/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.121065 hdf5-reader-service-0.1.4/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.121065 hdf5-reader-service-0.1.4/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/developer/explanations/decisions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.121065 hdf5-reader-service-0.1.4/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.125065 hdf5-reader-service-0.1.4/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.125065 hdf5-reader-service-0.1.4/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.125065 hdf5-reader-service-0.1.4/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.125065 hdf5-reader-service-0.1.4/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.125065 hdf5-reader-service-0.1.4/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/user/explanations/docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.125065 hdf5-reader-service-0.1.4/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.125065 hdf5-reader-service-0.1.4/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.125065 hdf5-reader-service-0.1.4/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/docs/user/tutorials/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 12:10:03.145065 hdf5-reader-service-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.109065 hdf5-reader-service-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.129065 hdf5-reader-service-0.1.4/src/hdf5_reader_service/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service/__init__ copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 12:10:02.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service/_version_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service/fork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.133065 hdf5-reader-service-0.1.4/src/hdf5_reader_service/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service/tasks/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service/tasks/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service/tasks/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service/tasks/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service/tasks/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.133065 hdf5-reader-service-0.1.4/src/hdf5_reader_service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15608 2023-05-30 12:10:03.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-30 12:10:03.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:10:03.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-30 12:10:03.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-30 12:10:03.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 12:10:03.000000 hdf5-reader-service-0.1.4/src/hdf5_reader_service.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.137065 hdf5-reader-service-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.137065 hdf5-reader-service-0.1.4/tests/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/tests/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/tests/tasks/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/tests/tasks/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/tests/tasks/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/tests/tasks/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/tests/tasks/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.137065 hdf5-reader-service-0.1.4/tests/test-data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:10:03.137065 hdf5-reader-service-0.1.4/tests/test-data/p45-104/
+-rw-r--r--   0 runner    (1001) docker     (123)  7704118 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/tests/test-data/p45-104/p45-104-DIFFRACTION.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    55178 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/tests/test-data/p45-104.nxs
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/tests/test_boilerplate_removed copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/tests/test_boilerplate_removed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-05-30 12:09:53.000000 hdf5-reader-service-0.1.4/tests/test_utils.py
```

### Comparing `hdf5-reader-service-0.1.3/.devcontainer/devcontainer.json` & `hdf5-reader-service-0.1.4/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/.github/CONTRIBUTING.rst` & `hdf5-reader-service-0.1.4/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/.github/actions/install_requirements/action.yml` & `hdf5-reader-service-0.1.4/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/.github/dependabot.yml` & `hdf5-reader-service-0.1.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/.github/pages/make_switcher.py` & `hdf5-reader-service-0.1.4/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/.github/workflows/code.yml` & `hdf5-reader-service-0.1.4/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/.github/workflows/docs.yml` & `hdf5-reader-service-0.1.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/.github/workflows/docs_clean.yml` & `hdf5-reader-service-0.1.4/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/.github/workflows/linkcheck.yml` & `hdf5-reader-service-0.1.4/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/.gitignore` & `hdf5-reader-service-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/.vscode/launch.json` & `hdf5-reader-service-0.1.4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/Dockerfile` & `hdf5-reader-service-0.1.4/Dockerfile`

 * *Files 11% similar despite different names*

```diff
@@ -30,8 +30,7 @@
 
 # copy the virtual environment from the build stage and put it in PATH
 COPY --from=build /venv/ /venv/
 ENV PATH=/venv/bin:$PATH
 
 # change this entrypoint if it is not the same as the repo
 ENTRYPOINT ["hdf5-reader-service"]
-CMD ["--version"]
```

### Comparing `hdf5-reader-service-0.1.3/LICENSE` & `hdf5-reader-service-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/PKG-INFO` & `hdf5-reader-service-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdf5-reader-service
-Version: 0.1.3
+Version: 0.1.4
 Summary: Microservice for reading HDF5 data and serving it via REST, aimed at performance and concurrency
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `hdf5-reader-service-0.1.3/README.rst` & `hdf5-reader-service-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/docs/conf.py` & `hdf5-reader-service-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst` & `hdf5-reader-service-0.1.4/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/docs/developer/explanations/decisions.rst` & `hdf5-reader-service-0.1.4/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/docs/developer/how-to/build-docs.rst` & `hdf5-reader-service-0.1.4/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/docs/developer/how-to/lint.rst` & `hdf5-reader-service-0.1.4/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/docs/developer/how-to/make-release.rst` & `hdf5-reader-service-0.1.4/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/docs/developer/how-to/pin-requirements.rst` & `hdf5-reader-service-0.1.4/docs/developer/how-to/pin-requirements.rst`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/docs/developer/how-to/test-container.rst` & `hdf5-reader-service-0.1.4/docs/developer/how-to/test-container.rst`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/docs/developer/how-to/update-tools.rst` & `hdf5-reader-service-0.1.4/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/docs/developer/index.rst` & `hdf5-reader-service-0.1.4/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/docs/developer/reference/standards.rst` & `hdf5-reader-service-0.1.4/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/docs/developer/tutorials/dev-install.rst` & `hdf5-reader-service-0.1.4/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/docs/images/dls-favicon.ico` & `hdf5-reader-service-0.1.4/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/docs/images/dls-logo.svg` & `hdf5-reader-service-0.1.4/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/docs/index.rst` & `hdf5-reader-service-0.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/docs/user/explanations/docs-structure.rst` & `hdf5-reader-service-0.1.4/docs/user/explanations/docs-structure.rst`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/docs/user/index.rst` & `hdf5-reader-service-0.1.4/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/docs/user/tutorials/installation.rst` & `hdf5-reader-service-0.1.4/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/pyproject.toml` & `hdf5-reader-service-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/src/hdf5_reader_service/__main__.py` & `hdf5-reader-service-0.1.4/src/hdf5_reader_service/__main__.py`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/src/hdf5_reader_service/_version_git.py` & `hdf5-reader-service-0.1.4/src/hdf5_reader_service/_version_git.py`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/src/hdf5_reader_service/api.py` & `hdf5-reader-service-0.1.4/src/hdf5_reader_service/api.py`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/src/hdf5_reader_service/fork.py` & `hdf5-reader-service-0.1.4/src/hdf5_reader_service/fork.py`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/src/hdf5_reader_service/model.py` & `hdf5-reader-service-0.1.4/src/hdf5_reader_service/model.py`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/src/hdf5_reader_service/tasks/metadata.py` & `hdf5-reader-service-0.1.4/src/hdf5_reader_service/tasks/metadata.py`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/src/hdf5_reader_service/tasks/shapes.py` & `hdf5-reader-service-0.1.4/src/hdf5_reader_service/tasks/shapes.py`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/src/hdf5_reader_service/tasks/slice.py` & `hdf5-reader-service-0.1.4/src/hdf5_reader_service/tasks/slice.py`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/src/hdf5_reader_service/utils.py` & `hdf5-reader-service-0.1.4/src/hdf5_reader_service/utils.py`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/src/hdf5_reader_service.egg-info/PKG-INFO` & `hdf5-reader-service-0.1.4/src/hdf5_reader_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdf5-reader-service
-Version: 0.1.3
+Version: 0.1.4
 Summary: Microservice for reading HDF5 data and serving it via REST, aimed at performance and concurrency
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `hdf5-reader-service-0.1.3/src/hdf5_reader_service.egg-info/SOURCES.txt` & `hdf5-reader-service-0.1.4/src/hdf5_reader_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/tests/tasks/test_metadata.py` & `hdf5-reader-service-0.1.4/tests/tasks/test_metadata.py`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/tests/tasks/test_search.py` & `hdf5-reader-service-0.1.4/tests/tasks/test_search.py`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/tests/tasks/test_shapes.py` & `hdf5-reader-service-0.1.4/tests/tasks/test_shapes.py`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/tests/tasks/test_slice.py` & `hdf5-reader-service-0.1.4/tests/tasks/test_slice.py`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/tests/tasks/test_tree.py` & `hdf5-reader-service-0.1.4/tests/tasks/test_tree.py`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/tests/test-data/p45-104/p45-104-DIFFRACTION.h5` & `hdf5-reader-service-0.1.4/tests/test-data/p45-104/p45-104-DIFFRACTION.h5`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/tests/test-data/p45-104.nxs` & `hdf5-reader-service-0.1.4/tests/test-data/p45-104.nxs`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/tests/test_boilerplate_removed copy.py` & `hdf5-reader-service-0.1.4/tests/test_boilerplate_removed copy.py`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/tests/test_boilerplate_removed.py` & `hdf5-reader-service-0.1.4/tests/test_boilerplate_removed.py`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/tests/test_system.py` & `hdf5-reader-service-0.1.4/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `hdf5-reader-service-0.1.3/tests/test_utils.py` & `hdf5-reader-service-0.1.4/tests/test_utils.py`

 * *Files identical despite different names*

