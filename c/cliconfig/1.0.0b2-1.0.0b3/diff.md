# Comparing `tmp/cliconfig-1.0.0b2.tar.gz` & `tmp/cliconfig-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliconfig-1.0.0b2.tar", last modified: Tue May 30 11:29:26 2023, max compression
+gzip compressed data, was "cliconfig-1.0.0b3.tar", last modified: Tue May 30 14:52:42 2023, max compression
```

## Comparing `cliconfig-1.0.0b2.tar` & `cliconfig-1.0.0b3.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.094412 cliconfig-1.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.070412 cliconfig-1.0.0b2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.074412 cliconfig-1.0.0b2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.markdownlint.json
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-30 11:29:26.094412 cliconfig-1.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.074412 cliconfig-1.0.0b2/cliconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-30 11:29:25.000000 cliconfig-1.0.0b2/cliconfig/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/config_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    15588 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/process_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.078412 cliconfig-1.0.0b2/cliconfig/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/processing/_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/processing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    26940 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/processing/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/processing/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/tag_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.078412 cliconfig-1.0.0b2/cliconfig/yaml_tags/
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/yaml_tags/_yaml_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.078412 cliconfig-1.0.0b2/cliconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-30 11:29:26.000000 cliconfig-1.0.0b2/cliconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-30 11:29:26.000000 cliconfig-1.0.0b2/cliconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:29:26.000000 cliconfig-1.0.0b2/cliconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 11:29:26.000000 cliconfig-1.0.0b2/cliconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 11:29:26.000000 cliconfig-1.0.0b2/cliconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.082412 cliconfig-1.0.0b2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/README_pypi.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.082412 cliconfig-1.0.0b2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/_static/logo_extend.png
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/cliconfig.processing_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/cliconfig_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/edge_cases.md
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    16436 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/processing.md
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.082412 cliconfig-1.0.0b2/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.082412 cliconfig-1.0.0b2/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/licenses_tier/FLATTEN_DICT_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:29:26.098412 cliconfig-1.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.082412 cliconfig-1.0.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.086412 cliconfig-1.0.0b2/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/configtag1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/configtag2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/default2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.086412 cliconfig-1.0.0b2/tests/configs/delete/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/delete/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/delete/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/fallback.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.070412 cliconfig-1.0.0b2/tests/configs/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.086412 cliconfig-1.0.0b2/tests/configs/integration/test1/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test1/main.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test1/sub1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test1/sub2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.090412 cliconfig-1.0.0b2/tests/configs/integration/test2/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test2/data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test2/default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test2/exp1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test2/exp2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test2/exp3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.090412 cliconfig-1.0.0b2/tests/configs/integration/test2/models/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test2/models/resnet100.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test2/models/resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test2/models/vit_b16.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.094412 cliconfig-1.0.0b2/tests/configs/merge/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/merge/additional1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/merge/additional2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/merge/additional3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/merge/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/merge/default2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/merge/default3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/multi_files_with_tags.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.094412 cliconfig-1.0.0b2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/integration/test_inte_multiple_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.094412 cliconfig-1.0.0b2/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.094412 cliconfig-1.0.0b2/tests/unit/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/processing/test_base_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/processing/test_builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/processing/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/processing/test_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/test_base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/test_cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/test_config_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/test_dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/test_ex_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/test_process_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/test_tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.669768 cliconfig-1.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.645768 cliconfig-1.0.0b3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.653768 cliconfig-1.0.0b3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.markdownlint.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-30 14:52:42.669768 cliconfig-1.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.653768 cliconfig-1.0.0b3/cliconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-30 14:52:42.000000 cliconfig-1.0.0b3/cliconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/config_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15588 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/process_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.657768 cliconfig-1.0.0b3/cliconfig/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/processing/_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26940 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/processing/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/processing/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.657768 cliconfig-1.0.0b3/cliconfig/yaml_tags/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/cliconfig/yaml_tags/_yaml_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.653768 cliconfig-1.0.0b3/cliconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-30 14:52:42.000000 cliconfig-1.0.0b3/cliconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-30 14:52:42.000000 cliconfig-1.0.0b3/cliconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:52:42.000000 cliconfig-1.0.0b3/cliconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 14:52:42.000000 cliconfig-1.0.0b3/cliconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 14:52:42.000000 cliconfig-1.0.0b3/cliconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.657768 cliconfig-1.0.0b3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/README_pypi.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.657768 cliconfig-1.0.0b3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/_static/logo_extend.png
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/cliconfig.processing_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/cliconfig_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/edge_cases.md
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    16436 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/processing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.657768 cliconfig-1.0.0b3/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.657768 cliconfig-1.0.0b3/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/licenses_tier/FLATTEN_DICT_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:52:42.669768 cliconfig-1.0.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.657768 cliconfig-1.0.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.661768 cliconfig-1.0.0b3/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/configtag1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/configtag2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/default2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.661768 cliconfig-1.0.0b3/tests/configs/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/delete/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/delete/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/fallback.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.645768 cliconfig-1.0.0b3/tests/configs/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.661768 cliconfig-1.0.0b3/tests/configs/integration/test1/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test1/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test1/sub1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test1/sub2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.661768 cliconfig-1.0.0b3/tests/configs/integration/test2/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test2/data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test2/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test2/exp1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test2/exp2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test2/exp3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.661768 cliconfig-1.0.0b3/tests/configs/integration/test2/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test2/models/resnet100.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test2/models/resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/integration/test2/models/vit_b16.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.665768 cliconfig-1.0.0b3/tests/configs/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/merge/additional1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/merge/additional2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/merge/additional3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/merge/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/merge/default2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/merge/default3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/configs/multi_files_with_tags.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.665768 cliconfig-1.0.0b3/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/integration/test_inte_multiple_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.665768 cliconfig-1.0.0b3/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:52:42.665768 cliconfig-1.0.0b3/tests/unit/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/processing/test_base_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/processing/test_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/processing/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/processing/test_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/test_base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/test_cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/test_config_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/test_dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/test_ex_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/test_process_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-30 14:52:22.000000 cliconfig-1.0.0b3/tests/unit/test_tag_routines.py
```

### Comparing `cliconfig-1.0.0b2/.github/workflows/pipy_deployment.yaml` & `cliconfig-1.0.0b3/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/.github/workflows/pydocstyle.yaml` & `cliconfig-1.0.0b3/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/.github/workflows/pylint.yaml` & `cliconfig-1.0.0b3/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/.github/workflows/tests.yaml` & `cliconfig-1.0.0b3/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/.pylintrc` & `cliconfig-1.0.0b3/.pylintrc`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/CONTRIBUTING.md` & `cliconfig-1.0.0b3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/LICENSE` & `cliconfig-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/PKG-INFO` & `cliconfig-1.0.0b3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: cli,config,cliconfig,python,yaml,merge
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -37,38 +37,49 @@
 
 |Ruff_logo| |Black_logo|
 
 |Ruff| |Flake8| |Pydocstyle| |MyPy| |PyLint|
 
 |Tests| |Coverage| |Documentation Status|
 
-Make default config file(s) in your project (configs are merged from left to right):
+Make default config yaml file(s) in your project (configs are merged from left to right):
 
 .. code:: python
 
    # main.py
    from cliconfig import make_config
 
    config = make_config('default1.yaml', 'default2.yaml')
-   config_dict = config.dict  # native python dict
 
 Then launch your script with additional config(s) file(s) and parameters by command line.
 The additional configs are merge on the default ones then the parameters are set.
 
 .. code:: bash
 
    python main.py --config first.yaml,second.yaml --param1=1 --subconfig.param2='foo'
 
 **By default, these additional configs cannot add new parameters to the default config
 (for security and retro-compatibility reasons).**
 
+Now you can get your configuration parameters in your script:
+
+.. code:: python
+
+   # Nested config dict as a native python dict
+   config.dict
+   # Get a parameter value (you can also set it or delete it)
+   config.foo1.foo2.bar
+
+You can also load and save configs with `cliconfig.save_config` and `cliconfig.load_config`.
+
+
 With processing
 ---------------
 
-The library provide powerfull tools to modify the configuration called "processings".
+The library provide powerful tools to modify the configuration called "processings".
 One of the possibility they add is to merge multiple configurations,
 copy a parameter on another, enforce type and more. To do so, simply adding the
 corresponding tags to your parameter names (on config files or CLI parameters).
 
 For instance with these config files:
 
 .. code:: yaml
```

### Comparing `cliconfig-1.0.0b2/README.md` & `cliconfig-1.0.0b3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,28 +62,35 @@
 ```
 
 Now you can write these following lines in your python program to use this config
 with `make_config`:
 
 ```python
 # main.py
-from cliconfig import make_config, show_config
+from cliconfig import load_config, make_config, show_config, save_config
 
 config = make_config('default1.yaml', 'default2.yaml')
 show_config(config)  # print the config to check it
-config.dict  # the configuration as a dict
+
+config.dict  # the configuration as a native python dict
+print('letter 1:', config.letters.letter1)  # access a parameter (you can also set it or delete it)
+
+# Save the config as a yaml file
+save_config(config, 'myconfig.yaml')
+# Load the config and merge with the default configs if any (useful if default configs were updated)
+config = load_config('myconfig.yaml', default_config_paths=['default1.yaml', 'default2.yaml'])
 ```
 
 Then you can add one or multiple additional config files that will be passed on
 command line and that will override the default values.
 
 ```yaml
 # first.yaml
 letters:
-  letter3: C  # equivalent to "letters.letter3: "C"
+  letter3: C  # equivalent to "letters.letter3: 'C'"
 
 # second.yaml
 param1: -1
 letters.letter1: A
 ```
 
 **Please note that the additional config files must not introduce new parameters that
@@ -114,17 +121,22 @@
 Config:
     param1: -1
     param2: -2
     letters:
         letter1: A
         letter2: B
         letter3: C
+letter 1: A
 ```
 
 Note that the configurations is stored as native python dict at each step of the process.
+The config object is just a wrapper around this dict that allows to access the parameters
+via dots (and containing the list of processings, see
+[*Processing*](https://cliconfig.readthedocs.io/en/stable/processing.html)
+section of the documentation for details.)
 
 You can also use multiple documents in a single YAML file with the `---` separator. In
 this case, the documents are merged in sequence and the file is interpreted as a single
 additional config file containing this merged configuration.
 
 ## Use tags
 
@@ -220,15 +232,20 @@
 **Please note that YAML does not support tuples and sets**, and therefore they
 cannot be used in YAML files. If possible, consider using lists instead.
 
 Moreover, YAML does not recognize "None" as a None object, but interprets it as a
 string. If you wish to set a None object, you can use "null" or "Null" instead.
 
 "@" is a special character used by the package to identify tags. You can't use it
-in your parameters names (but you can use it in your values).
+in your parameters names (but you can use it in your values). It will raise an error
+if you try to do so.
+
+"dict" and "process_list" are reserved names of attributes and should not be used
+as sub-config or parameter names. It can raise an error if you try to access them
+as config attributes.
 
 In the context of this package, dictionaries are treated as sub-configurations,
 which means that modifying or adding keys directly in the additional configs may
 not be possible (because only the merge of default configuration allow adding new keys).
 If you need to modify or add keys within a dictionary, consider enclosing it in a list.
 
 For instance:
```

### Comparing `cliconfig-1.0.0b2/cliconfig/__init__.py` & `cliconfig-1.0.0b3/cliconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/cliconfig/cli_parser.py` & `cliconfig-1.0.0b3/cliconfig/cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/cliconfig/config_routines.py` & `cliconfig-1.0.0b3/cliconfig/config_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/cliconfig/dict_routines.py` & `cliconfig-1.0.0b3/cliconfig/dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/cliconfig/process_routines.py` & `cliconfig-1.0.0b3/cliconfig/process_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/cliconfig/processing/_type_parser.py` & `cliconfig-1.0.0b3/cliconfig/processing/_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/cliconfig/processing/base.py` & `cliconfig-1.0.0b3/cliconfig/processing/base.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/cliconfig/processing/builtin.py` & `cliconfig-1.0.0b3/cliconfig/processing/builtin.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/cliconfig/processing/create.py` & `cliconfig-1.0.0b3/cliconfig/processing/create.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/cliconfig/tag_routines.py` & `cliconfig-1.0.0b3/cliconfig/tag_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/cliconfig/yaml_tags/_yaml_tags.py` & `cliconfig-1.0.0b3/cliconfig/yaml_tags/_yaml_tags.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/cliconfig.egg-info/PKG-INFO` & `cliconfig-1.0.0b3/cliconfig.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: cli,config,cliconfig,python,yaml,merge
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -37,38 +37,49 @@
 
 |Ruff_logo| |Black_logo|
 
 |Ruff| |Flake8| |Pydocstyle| |MyPy| |PyLint|
 
 |Tests| |Coverage| |Documentation Status|
 
-Make default config file(s) in your project (configs are merged from left to right):
+Make default config yaml file(s) in your project (configs are merged from left to right):
 
 .. code:: python
 
    # main.py
    from cliconfig import make_config
 
    config = make_config('default1.yaml', 'default2.yaml')
-   config_dict = config.dict  # native python dict
 
 Then launch your script with additional config(s) file(s) and parameters by command line.
 The additional configs are merge on the default ones then the parameters are set.
 
 .. code:: bash
 
    python main.py --config first.yaml,second.yaml --param1=1 --subconfig.param2='foo'
 
 **By default, these additional configs cannot add new parameters to the default config
 (for security and retro-compatibility reasons).**
 
+Now you can get your configuration parameters in your script:
+
+.. code:: python
+
+   # Nested config dict as a native python dict
+   config.dict
+   # Get a parameter value (you can also set it or delete it)
+   config.foo1.foo2.bar
+
+You can also load and save configs with `cliconfig.save_config` and `cliconfig.load_config`.
+
+
 With processing
 ---------------
 
-The library provide powerfull tools to modify the configuration called "processings".
+The library provide powerful tools to modify the configuration called "processings".
 One of the possibility they add is to merge multiple configurations,
 copy a parameter on another, enforce type and more. To do so, simply adding the
 corresponding tags to your parameter names (on config files or CLI parameters).
 
 For instance with these config files:
 
 .. code:: yaml
```

### Comparing `cliconfig-1.0.0b2/cliconfig.egg-info/SOURCES.txt` & `cliconfig-1.0.0b3/cliconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/docs/Makefile` & `cliconfig-1.0.0b3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/docs/README_pypi.rst` & `cliconfig-1.0.0b3/docs/README_pypi.rst`

 * *Files 4% similar despite different names*

```diff
@@ -25,38 +25,49 @@
 
 |Ruff_logo| |Black_logo|
 
 |Ruff| |Flake8| |Pydocstyle| |MyPy| |PyLint|
 
 |Tests| |Coverage| |Documentation Status|
 
-Make default config file(s) in your project (configs are merged from left to right):
+Make default config yaml file(s) in your project (configs are merged from left to right):
 
 .. code:: python
 
    # main.py
    from cliconfig import make_config
 
    config = make_config('default1.yaml', 'default2.yaml')
-   config_dict = config.dict  # native python dict
 
 Then launch your script with additional config(s) file(s) and parameters by command line.
 The additional configs are merge on the default ones then the parameters are set.
 
 .. code:: bash
 
    python main.py --config first.yaml,second.yaml --param1=1 --subconfig.param2='foo'
 
 **By default, these additional configs cannot add new parameters to the default config
 (for security and retro-compatibility reasons).**
 
+Now you can get your configuration parameters in your script:
+
+.. code:: python
+
+   # Nested config dict as a native python dict
+   config.dict
+   # Get a parameter value (you can also set it or delete it)
+   config.foo1.foo2.bar
+
+You can also load and save configs with `cliconfig.save_config` and `cliconfig.load_config`.
+
+
 With processing
 ---------------
 
-The library provide powerfull tools to modify the configuration called "processings".
+The library provide powerful tools to modify the configuration called "processings".
 One of the possibility they add is to merge multiple configurations,
 copy a parameter on another, enforce type and more. To do so, simply adding the
 corresponding tags to your parameter names (on config files or CLI parameters).
 
 For instance with these config files:
 
 .. code:: yaml
```

### Comparing `cliconfig-1.0.0b2/docs/_static/logo.png` & `cliconfig-1.0.0b3/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/docs/_static/logo_extend.png` & `cliconfig-1.0.0b3/docs/_static/logo_extend.png`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/docs/cliconfig_api.rst` & `cliconfig-1.0.0b3/docs/cliconfig_api.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/docs/conf.py` & `cliconfig-1.0.0b3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/docs/edge_cases.md` & `cliconfig-1.0.0b3/docs/edge_cases.md`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 Moreover, YAML does not recognize "None" as a None object, but interprets it as a
 string. If you wish to set a None object, you can use "null" or "Null" instead.
 
 "@" is a special character used by the package to identify tags. You can't use it
 in your parameters names (but you can use it in your values).
 
+"dict" and "process_list" are reserved names of attributes and should not be used
+as sub-config or parameter names. It can raise an error if you try to access them
+as config attributes.
+
 In the context of this package, dictionaries are treated as sub-configurations,
 which means that modifying or adding keys directly in the additional configs may
 not be possible (because only the merge of default configuration allow adding new keys).
 If you need to modify or add keys within a dictionary, consider enclosing it in a list.
 
 For instance:
```

### Comparing `cliconfig-1.0.0b2/docs/license.md` & `cliconfig-1.0.0b3/docs/license.md`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/docs/make.bat` & `cliconfig-1.0.0b3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/docs/processing.md` & `cliconfig-1.0.0b3/docs/processing.md`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/docs/quickstart.md` & `cliconfig-1.0.0b3/docs/quickstart.md`

 * *Files 8% similar despite different names*

```diff
@@ -19,27 +19,35 @@
 ```
 
 Now you can write these following lines in your python program to use this config
 with `make_config`:
 
 ```python
 # main.py
-from cliconfig import make_config, show_config
+from cliconfig import load_config, make_config, show_config, save_config
 
 config = make_config('default1.yaml', 'default2.yaml')
 show_config(config)  # print the config to check it
+
+config.dict  # the configuration as a native python dict
+print('letter 1:', config.letters.letter1)  # access a parameter (you can also set it or delete it)
+
+# Save the config as a yaml file
+save_config(config, 'myconfig.yaml')
+# Load the config and merge with the default configs if any (useful if default configs were updated)
+config = load_config('myconfig.yaml', default_config_paths=['default1.yaml', 'default2.yaml'])
 ```
 
 Then you can add one or multiple additional config files that will be passed on
 command line and that will override the default values.
 
 ```yaml
 # first.yaml
 letters:
-  letter3: C
+  letter3: C  # equivalent to "letters.letter3: 'C'"
 
 # second.yaml
 param1: -1
 letters.letter1: A
 ```
 
 **Please note that the additional config files must not introduce new parameters that
@@ -70,21 +78,26 @@
 Config:
     param1: -1
     param2: -2
     letters:
         letter1: A
         letter2: B
         letter3: C
+letter 1: A
 ```
 
 Note that the configurations is stored as native python dict at each step of the process.
+The config object is just a wrapper around this dict that allows to access the parameters
+via dots (and containing the list of processings, see
+[*Processing*](https://cliconfig.readthedocs.io/en/stable/processing.html)
+section of the documentation for details.)
 
 You can also use multiple documents in a single YAML file with the `---` separator. In
-this case, the configs of the documents are merged in sequence and the file is interpreted
-as a single additional config file containing this merged configuration.
+this case, the documents are merged in sequence and the file is interpreted as a single
+additional config file containing this merged configuration.
 
 ## Use tags
 
 By default, the package provides some "tags" represented as strings that start with
 '@' and are placed at the end of a key containing a parameter. These tags change
 the way the configuration is processed.
```

### Comparing `cliconfig-1.0.0b2/github_actions_utils/pydocstyle_manager.py` & `cliconfig-1.0.0b3/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/github_actions_utils/pylint_manager.py` & `cliconfig-1.0.0b3/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/github_actions_utils/pytest_manager.py` & `cliconfig-1.0.0b3/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/licenses_tier/FLATTEN_DICT_LICENSE` & `cliconfig-1.0.0b3/licenses_tier/FLATTEN_DICT_LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/pre-commit-checks.sh` & `cliconfig-1.0.0b3/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/pyproject.toml` & `cliconfig-1.0.0b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/tests/configs/integration/test2/default.yaml` & `cliconfig-1.0.0b3/tests/configs/integration/test2/default.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/tests/conftest.py` & `cliconfig-1.0.0b3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/tests/integration/test_inte_multiple_tags.py` & `cliconfig-1.0.0b3/tests/integration/test_inte_multiple_tags.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/tests/unit/processing/test_base_processing.py` & `cliconfig-1.0.0b3/tests/unit/processing/test_base_processing.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/tests/unit/processing/test_builtin.py` & `cliconfig-1.0.0b3/tests/unit/processing/test_builtin.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/tests/unit/processing/test_create.py` & `cliconfig-1.0.0b3/tests/unit/processing/test_create.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/tests/unit/processing/test_type_parser.py` & `cliconfig-1.0.0b3/tests/unit/processing/test_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/tests/unit/test_base_config.py` & `cliconfig-1.0.0b3/tests/unit/test_base_config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,44 @@
 """Test base class of configuration."""
 
 import pytest_check as check
 
 from cliconfig.base import Config
+from cliconfig.dict_routines import unflatten
 from cliconfig.processing.base import Processing
 
 
 def test_config(process_add1: Processing) -> None:
     """Test base class of configuration."""
     config_dict = {"a.b": 1, "b": 2, "c.d.e": 3, "c.d.f": [2, 3]}
+    config_dict = unflatten(config_dict)
     config = Config(config_dict, [process_add1])
     check.equal(config.dict, config_dict)
     check.equal(config.process_list, [process_add1])
     check.equal(repr(config), f"Config({config_dict}, ['ProcessAdd1'])")
     config_dict2 = {"c.d.e": 3, "a.b": 1, "b": 2, "c.d.f": [2, 3]}
+    config_dict2 = unflatten(config_dict2)
     config2 = Config(config_dict2, [process_add1])
     check.equal(config, config2)
     config3 = Config(config_dict2, [process_add1, process_add1])
     check.not_equal(config, config3)
     config4 = Config(config_dict2, [])
     check.not_equal(config, config4)
+    # Test get/set attribute
+    config = Config(config_dict, [process_add1])
+    check.equal(config.a.b, 1)
+    check.equal(config.c.d.f, [2, 3])
+    check.equal(config.c.d, Config({"e": 3, "f": [2, 3]}, [process_add1]))
+    config.a.b = 2
+    check.equal(config.a.b, 2)
+    config.c.d.f = [3, 4]
+    check.equal(config.c.d.f, [3, 4])
+    config.c.d.f.append(5)
+    check.equal(config.c.d.f, [3, 4, 5])
+    # Test delete attribute
+    del config.a.b
+    check.equal(config.dict, {"a": {}, "b": 2, "c": {"d": {"e": 3, "f": [3, 4, 5]}}})
+    del config.c.d
+    check.equal(config.dict, {"a": {}, "b": 2, "c": {}})
+    # Should no raise error
+    del config.dict
+    del config.process_list
```

### Comparing `cliconfig-1.0.0b2/tests/unit/test_cli_parser.py` & `cliconfig-1.0.0b3/tests/unit/test_cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/tests/unit/test_config_routines.py` & `cliconfig-1.0.0b3/tests/unit/test_config_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/tests/unit/test_dict_routines.py` & `cliconfig-1.0.0b3/tests/unit/test_dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/tests/unit/test_ex_docs.py` & `cliconfig-1.0.0b3/tests/unit/test_ex_docs.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/tests/unit/test_process_routines.py` & `cliconfig-1.0.0b3/tests/unit/test_process_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b2/tests/unit/test_tag_routines.py` & `cliconfig-1.0.0b3/tests/unit/test_tag_routines.py`

 * *Files identical despite different names*

